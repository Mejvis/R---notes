# R_notes

##2: Workspace and Files 

Basic R functions

getwd()

ls()

list.files()

dir()

args()

dir.create("")

setwd("")

file.create("")

file.exists("")

file.info("")

file.rename("", "")

file.copy("", "")   > file.copy("mytest2.R", "mytest3.R")

file.path("")

| You can use file.path to construct file and directory paths that are independent of the operating system your R code is running on. Pass 'folder1' and
| 'folder2' as arguments to file.path to make a platform-independent pathname.

> file.path("folder1", "folder2")

dir.create(file.path('testdir2', 'testdir3'), recursive = TRUE)

> unlink("testdir2", recursive = TRUE)

end.
