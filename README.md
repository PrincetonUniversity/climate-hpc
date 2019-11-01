
# Table of Contents

1.  [Getting an account](#org7e1b8b8)
2.  [Running Jupyter notebook](#org2ba4f6c)
2.  [Adding datasets](#add-data)

<a id="org7e1b8b8"></a>

# Getting an account

To get an account on the Tigress system have your faculty advisor
email David Luet with a request for a new account on `tiger`.  

An account on the `tigercpu` cluster gives you access to:

-   `tigercpu`: the cluster,
-   `tigressdata`: a visualization node,
-   `jupyter.rc`: a JupyterHub host.


<a id="org2ba4f6c"></a>

# Running Jupyter notebook

-   The easiest way to run Jupyter notebooks is to use [jupyter.rc](./jupyterhub.md).

<a id="add-data"></a>
# Adding datasets

Getting datasets onto the filesystem `tigress` (which can be accessed by all the machines above)
can be done in multiple ways:

1. [Download to local machine and transfer to remote](#down_ssh) (easy but only works for `smallish` datasets, which fit onto your local harddisk)

2. ... other methods are not documented yet

<a id="down_ssh"></a>
## Download to local machine and transfer to remote
Download your dataset to a location on your harddrive (e.g. `~/Downloads`).

From there you can copy the file to the remote filesystem by using
```
scp ~/Downloads/<yourfile> <username>@tigressdata.princeton.edu:/tigress/<username>/`
```
The words in `<...>` need to be replaced with specific filesnames and your princeton username.
If you have set up SSH keys (e.g. if you log into `tigressdata` with `ssh tigressdata`),
you can simplify the command above to:
```
scp ~/Downloads/<yourfile> tigressdata:/tigress/<username>/`
```
Now the file is in your folder on tigress and you can load it into your jupyter notebook,
by using the path `/tigress/<username>/<yourfile>`.

> Always make a `README_<yourfile>.txt` file that describes where you got the data (links)
and what is in the file. Copy that `.txt` file like you did the datafile.
