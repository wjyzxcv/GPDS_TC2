(lesson_2_4)=
# Job submission
Most of the commands that we use to submit, alter, and delete jobs in the queue start with the letter q. Let's try to perform some basic tasks related to job submission.

## Practice 9 
Check the available cluster nodes and who is currently using them.
````{admonition} Checking status
- `qstat -u "*"`:  request the status of the jobs currently running.
````

````{admonition} Expected output
```{figure} ../pictures/lesson_2_4/P9.png
```
````

## Practice 10
Delete the `combined_files.csv` from your folder. Then, download the Jupyter Notebook in [**Practice 7**](Practice_7) as `combining_files.py` and put it in your script folder. Submit this file to the cluster machine and execute it using the python installed in your virtual environment.

```{admonition} Submitting job
<style>
td, th {
   border: none!important;
}
</style>

|qsub| -l s_vmem=1G| -cwd| -S *pythonpath*| *filename*|
|-|-|-|-|-|
|Submit job| Reserve memory slot| Send output to current directory| Declare which python to use| Declare which file to submit|
```

````{admonition} Steps
1. Delete the `combined_files.csv`.
   ```{figure} ../pictures/lesson_2_4/P10_1.png
   ```
2. Download `combining_files.ipynb` as `.py` then put it in the same folder.
   ```{figure} ../pictures/lesson_2_4/P10_2.png
   ```
3. Get inside your folder in terminal using `cd`.
   ```{figure} ../pictures/lesson_2_4/P10_3.png
   ```
4. Write down the job submission command. Reserve 2 GB memory then use the python in your virtual environment. The path should be like
`/home/*yourgroupfolder*/*yourfolder*/local/anaconda3/envs/*yourenvname*/bin/python`
   ```{figure} ../pictures/lesson_2_4/P10_4.png
   ```
````

## Practice 11
Show the output files and error files.
````{admonition} Check job status
- `qstat`: check your own submission status.
If `qstat gives no output, that means everything runs well.
```{figure} ../pictures/lesson_2_4/P11_1.png
```
If qstat gives output like this, that means it is still waiting.
Wait for few seconds and run qstat again.
```{figure} ../pictures/lesson_2_4/P11_2.png
```
````
Go back to Jupyter Notebook and if you do everything correctly, you will see the error file (`.e####`) and the output file (`.o####`). 

Since we don't have any errors and haven't printed any output (only writing `combined_files.csv`), both files are empty. If the job failed, you can always delete them and you will get a new one.

````{admonition} Expected output
```{figure} ../pictures/lesson_2_4/P11_3.png
```
````

## Practice 12
TTry to put in the wrong path for your virtual environment. Submit the `combining_files.py` again, check its status, then delete the job.

````{admonition} delete job
- `qdel *jobnumber*`: Delete the job from the queue.
````

````{admonition} Expected output
```{figure} ../pictures/lesson_2_4/P12.png
```
````
