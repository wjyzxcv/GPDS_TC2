(lesson_1_2)=
# Introduction to Remote System
One of the challenges of working with big data is that you don't have the data on local storage. The data itself is located somewhere else, in our case, the data is on GSIS servers.

## What is Remote System?
A **remote system** is any type of computer that you don't have physical access to, and must be accessed remotely over the internet.

## Local Computer vs Remote Computer
A **local computer** is one that physically close and can be accessed using one's local network. Examples include computers in the same room or building.

**Remote computers** are far away and accessed via the internet. Examples include computing services provided by other universities, Amazon, or Google. 

In order to access remote computers, the first condition to be satisfied is accessing the organization's network. In our case, you are already part of this network if you are on campus, but what if you are somewhere else?

## Virtual Private Network
A **Virtual Private Network**, or **VPN**, allows you to create a secure connection to another network over the Internet. VPNs can be used to access remote computers.

## Secure Sockets Layer Virtual Private Network
A **secure sockets layer VPN**, or **SSL VPN** enables individual users to access an organization's network, client-server applications, and internal network utilities and directories.

After being inside the university network, how can we access remote computers?

## Secure Shell Protocol
**Secure Shell Protocol**, or **SSH**, refers to the protocol by which network communications can take place safely and remotely via an unsecured network.

SSH connects to a particular computer while a VPN connects to a network.

## Things you can do with SSH
1. protected file transfer
2. command execution
3. remote access to private network system

We will see several ways of using SSH with a **Graphic User Interface (GUI)** and the **Command Line Interface(CUI)**.