# r4wrds-data-intro

Datasets used in the introductory R4WRDS class.

Best practice is to create a new RStudio project, and run the following code to download and use these data.

```
# create a data directory in your project
dir.create("data") # warning is ok if already exists!

# downloads the data.zip file to the data directory
download.file("https://github.com/r4wrds/r4wrds-data-intro/raw/main/data.zip", destfile = "data/data.zip")

# unzip the data:
unzip(zipfile = "data/data.zip")

```

