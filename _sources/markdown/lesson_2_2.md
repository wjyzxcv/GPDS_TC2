(lesson_2_2)=
# Path in Python
One important task when dealing with batches of data is accessing and reading files in
folders. In Python, there are some libraries that can be used to handle filesystem paths such as `os` and `glob` but here we will focus on `pathlib` library.
Feel free to use `os` and `glob` library if you are already familiar with them.

## Benefits of **pathlib** library
1. No more cumbersome use of os and os.path functions.
2. Contains the semantics of different path types.
3. Well-defined semantics, eliminating any ambiguities

## Useful Methods
- `Path.cwd()`: Return a new path object representing the current directory.

````{admonition} Example
Let us try to see the folder we are currently in. (Using Jupyter Notebook, you can go to your folder and make a new Jupyter Notebook file.)
```{figure} ../pictures/lesson_2_2/cwd_1.png
```
```{figure} ../pictures/lesson_2_2/cwd_2.png
```
````



- `Path('/filepath').iterdir()`: When the path points to a directory, yield path objects of the directory contents.
````{admonition} Example
Let us check all the files in this directory: `/home/practice_data`.
```{figure} ../pictures/lesson_2_2/iterdir_1.png
```
```{figure} ../pictures/lesson_2_2/iterdir_2.png
```
````

- `Path('/filepath').exists()`: Whether the path points to an existing file or directory.
````{admonition} Example
Let us check a folder in /home/ directory called practice_data. This folder cannot be accessed directly from Jupyter Notebook.
```{figure} ../pictures/lesson_2_2/exists_1.png
```
```{figure} ../pictures/lesson_2_2/exists_2.png
```
````


- `Path('/filepath').glob(*pattern*)`: Glob the given relative pattern in the directory represented by this path, yielding all matching files.
````{admonition} Example
Let us get the path for all the .csv files in thisdirectory: `/home/practice_data`.
```{figure} ../pictures/lesson_2_2/glob_1.png
```
```{figure} ../pictures/lesson_2_2/glob_2.png
```
````

```{margin}
- The "**" pattern means “this directory and all subdirectories, recursively”.
```
(Practice_7)=
## Practice 7
Make a program called `combining_files` to combine all the files starting with "text" from `folder1` and `folder2` in `/home/practice_data`. Save the combined files as `combined_files.csv` in your folder.

::::{admonition} Steps
1. Make a new Notebook first. Rename the title to be `combining_files`.
2. Use `glob` with pattern `'**/text*'` to get the list of all files started with word “text". Save it in a variable `files_list`.
3. Import `pandas` and use a list comprehension to make a list of DataFrames containing all the files in `files_list`. For example: `df_list = [pd.read_csv(file) for file in files_list]`.
4. Use `pd.concat` to combine all the DataFrames in
`df_list`. Save the result in variable `df`.
5. Use `df.to_csv('combined_files.csv',index=False)` for writing the result of Step 3 into a .csv format.
::::

```{note}
Give screenshot of the code and the content of combined_files.csv (you can open it using Jupyter
Notebook).
```

## Practice 8
Save the first and second column of test_file.gz in folder2 as a DataFrame then save it as yourname_test_split.csv and put it in `/home/yourgroupfolder`.

:::{margin}
- You can experiment with formats other than `.csv`. For example, `.parquet` is a good choice if you have categorical data.
:::
::::{admonition} Steps
1. Make a new notebook.
2. Save the path for `test_file.gz` in a variable called `file_path`.
3. Import `pandas` and read the file using `pd.read_csv(file_path, compression='gzip', header=None, sep='\t')`. Save it in variable `df`.
4. Get the 1st and 2nd columns using `df.iloc`. Save it in a variable `new_df`.
5. Use `new_df.to_csv` for saving `new_df` into a .csv file. (Not in your folder but in your group folder!)
::::
