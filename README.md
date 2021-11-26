## Module of the R-featurecounts-deseq

* needs a working conda installation and conda in path

* install the RStudio and working environment using conda 

* sample_info.csv provides a example of the needed sampleseheet

* use the module like this:

```
$ cd R-featurecounts-deseq
```

the current working dirtectory needs to be the R-featurecounts-deseq folder 

```
"Rscript script/Rsubread_R.R $PathToSample_info.csv"                       
"Rscirpt script/DEseq2_R.R"
                      

```


* the pipeline creates a folder structure and writes all the output in the parent directory of the current working directory 

#Folder structure
```
        |_BAM file
        |_ R-featurecounts-deseq     
              |
              |_envs
              |   |_BiocManager::install("Rsamtools")
              |   |_BiocManager::install("Rsubread")
              |
              |_sample_info.csv
              |
              |
              |_script
              |   |_Rsubread_R.R
              |   |_DESeq2_R.R
              |
              |_Output folder structure		
                  |
                  |_ 01_featurescount
         	  	|_ counts.csv (results)
        	      02_deseq
                       |
                       |_DEseq_result.csv
                       |_normalized_counts.txt
                       |_mergedata.csv
                       |_Rplots
                            |_PCA Plot.pdf
                            |_Heatmap.pdf
                            |_Volcanoplot.pdf  
                    
 
```
# Author
Sakshi Singh ---> Sakshi.Singh@uniklinikum-dresden.de

