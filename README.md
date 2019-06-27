# Calculate Internal PageRank From Crawler CSV Export
Calculate Internal PageRank using R script

Please note that the script featured here filters the dataset before parsing, only taking into account link from page to page (links to images, CSS and JavaScript resources are ignored).

Credit: [Paul Shapiro from Search Engine Land](https://searchengineland.com/improve-internal-linking-calculate-internal-pagerank-r-246883)

## Files included
- internal_pagerank.R is the actual script
- all_outlinks.csv is a Screaming Frog export I got from crawling https://www.catalystdigital.com/
- output-pagerank.csv is the output of the script, showing computed URLs and their respective internal PageRank

## How to use it
First, import this project by:
  - using Git: `git clone https://github.com/nabillemen/r-internal-pagerank`
  - downloading it as a .zip file

After installing R, editing the script to fit your needs (how to edit it is fully explained in the script comments), open your terminal, set current working directory to this project, and run:
  - `install.packages("igraph", lib="[path to your R packages foler]")` if igraph package isn't installed yet
  - `Rscript internal_pagerank.R` (don't forget to add R executables folder to your PATH environment variable)
