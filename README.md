# PiDiv
PiDiv is a tool for profiling nucleotide diversity using the π (pi) metric.
## Install
The following dependencies are required to run PiDiv:
* PySam
* Picard Tools
* SAMTools
* NumPy
* Minimap2
* HTStream
* Python gffutils
* Python colorama
* Biopython

These can be installed with a properly configured Bioconda into a Conda environment like so:

    mamba create -y -n pidiv pysam samtools picard numpy minimap2 htstream gffutils colorama biopython

Place the three PiDiv Python scripts somewhere in your path to use them, e.g.

    git clone https://github.com/marade/PiDiv.git
    sudo install -m 0755 PiDiv/AlignReads /usr/local/bin/
    sudo install -m 0755 PiDiv/PiDiv /usr/local/bin/
    sudo install -m 0755 PiDiv/PiDiv /usr/local/bin/
    
## Run

First run the AlingReads script to create initial alignments. Then run PiDiv to do the downsampling and pi calculations.
