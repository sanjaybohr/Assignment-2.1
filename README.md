# Assignment-2.1


Assignment 2_1
1.	How to Import SAS XPORT files into R with the foreign package?
read.xport (foreign)
            read.xport(file)

2.	How to Import SAS Files into R with the Haven package?
install.packages("haven")
library(haven)
dat=read_sas("path to file", "path to formats catalog")
	Eg: path <-system.file("examples","iris.sas7bdat", package ="haven")
	read_sas(path)

3.	How to read Weka Attribute-Relation File Format (ARFF) files in R?
Library(foreign)

           read.arff(file)
           Eg: read.arff(system.file("arff","contact-lenses.arff",
                      package ="RWeka"))

4.	How to read a heavy csv/tsv file using readr package?
   # Read a txt file, named "mtcars.txt"
                      my_data<-read_tsv("mtcars.txt")
      # Read a csv file, named "mtcars.csv"
                     my_data<-read.csv("mtcars.csv")
