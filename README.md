### WHAM-BAM

Structural variants (SVs) have largely been ignored in Genome Wide Association Studies.  SVs are difficult to call from NGS data.  Often the same SV allele is assigned different breakpoints across individuals.  WHAM-BAM takes a different approach and directly apply association tests on the BAM files.  WHAM-BAM does not call SVs, but rather examines the patterns of mate pair mapping across cases and controls.  If there is an enrichment of unmapped mates in the cases or controls is performs an association test.


### INSTALLING WHAM-BAM

The first step is installing BamTools which is shipped with WHAM-BAM.

```
git clone --recusive git@github.com:jewmanchue/wham.git wham
cd wham/src/bamtools
mkdir build
cd build
cmake ..
make
```

The second step is to build WHAM-BAM.  From "wham" directory simply make.

``` 
make
```
