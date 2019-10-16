
# Table of Contents

1.  [First time setting](#orgefdcab8)
2.  [Accessing data on `/project` or `/scratch/pgfs`](#orgeb6ddfe)
3.  [Uploading Files](#orge3c6ab4)
4.  [Downloading Files](#org8bf41cf)


<a id="orgefdcab8"></a>

# First time setting

-   Go to 
    <https://jupyter.rc.princeton.edu>
-   You will need authenticate with your Princeton `netid` and password.
    ![img](./figures/PU_authenticate.png)
-   In `Spawner options` select `Anaconda3 2019.07 in home directory -
      Climate Modeling`.  Note that the building the image the first time
    will take about 3 min. Afterthe first build it will be faster.
    ![img](./figures/spawn-image-raw-video.gif)


<a id="orgeb6ddfe"></a>

# Accessing data on `/project` or `/scratch/pgfs`

-   The server `jupyter.rc` is independent from the cluster `tiger` but
    has access to both `/tigress` and `/scratch/gpfs` on tiger. For
    convenience, create some symbolic links in your home directory.
    
    You can do this by opening a terminal by clicking on `New` then `Terminal`.
    
        $ ln -s /projects/GEOCLIM projects
        $ ln -s /tiger/scratch/gpfs gpfs
    
    ![img](./figures/symlinks.gif)
-   After this, the directories `projects` and `gpfs` will be in your
    home directory. You may need to refresh your browser to see them
    ![img](./figures/symlinks-in-browser.png)


<a id="orge3c6ab4"></a>

# Uploading Files

To upload a file click `Upload`
  ![img](./figures/upload.gif)


<a id="org8bf41cf"></a>

# Downloading Files

To download a file click the file and `Download`. The file will be
  downloaded where your browser downloads files.
  ![img](./figures/download.gif)
