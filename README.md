# r4wrds-data-intro

Datasets used in the introductory R4WRDS class.

## Download RStudio Project with Data

For a simple single download, we can use this zipped file which includes all the data, folders, and an RStudio project: 

 - [https://github.com/r4wrds/r4wrds-data-intro/raw/main/intro_proj.zip](https://github.com/r4wrds/r4wrds-data-intro/raw/main/intro_proj.zip)

Download and unzip into a folder where you want your RProjects to live, and double click the `intro_proj.Rproj` file.

## Create RStudio Project First, Then Download Data

Best practice is to create a new RStudio project, *then* run the following code inside your new project to download these data.

```
# create a data directory in your project
dir.create("data") # warning is ok if already exists!

# downloads the data.zip file to the data directory
download.file("https://github.com/r4wrds/r4wrds-data-intro/raw/main/data.zip", destfile = "data/data.zip")

# unzip the data:
unzip(zipfile = "data/data.zip")

# if get resulting __MACOSX folder (artifact of unzip), remove:
unlink("__MACOSX", recursive = TRUE)

```

