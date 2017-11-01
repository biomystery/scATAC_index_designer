scATAC-seq index designer
============================================================
Time-stamp: "2017-11-01 11:34:20"

# Two round barcoding multiplex
![Barcode usage](./barcode_multiplex.png) From [An Introduction to Next-Generation Sequencing Technology](https://www.illumina.com/content/dam/illumina-marketing/documents/products/illumina_sequencing_introduction.pdf) by Illumina

# Requirements for a barcodes design

* `-d`: Hamming distance between every two barcodes >=4(of 8bp): for possible sequencing error 
* `-gmax` and `gmin`: GC content 37.5-62.5% : for sequencer 
* `-n`: max number of repeat bps [3]

# Algorithm 


# Usage

``` Shell
chmod u+x scATAC_index_designer
scATAC_index_designer -l 8 -d 4 -o i7.4mm.txt -gmax 0.625 -gmin 0.375  -n 3
```
