# rust-bedtools-pangenome
 - rust-bedtools but from the pangenome point of view. 
 - rust ancestral state estimation from genome arthemtic intervals from bed alignment. 
 - searches for the longest alignment match according to the specified length filter.
 - infers the ancestrals states using the prank. 
 - writes the ancestral states in a separate fasta file. 
 - please see the last commit message and if it says compiled binary then it is completed or else still in development version.

  ```
  cargo build
  ```
 
 - to run the binary 
 
 ```
 ➜ gauravsablok  rust-ancestral-state git:(main) ✗
  ./target/debug/rust-pangenome-ancestral-state -h
 Usage: rust-pangenome-ancestral-state <ALIGNMENT> <THRESHOLD> <FASTAFILE>

  Arguments:
  <ALIGNMENT>  please provide the path to the first alignment file
  <THRESHOLD>  please provide the alignment length to be used as a threshold
  <FASTAFILE>  please provide the reference fasta file

 Options:
  -h, --help     Print help
  -V, --version  Print version
 ```
 
 ```
 ./target/debug/rust-pangenome-ancestral-state
./sample-file/sample.bed
./sample-file/sample.fasta 7 ./prank

-rw-r--r--. 1 gauravsablok gauravsablok  72 Jan  6 22:10 ancestral-aligned.fasta.best.anc.dnd 
-rw-r--r--. 1 gauravsablok gauravsablok 104 Jan  6 22:10 ancestral-aligned.fasta.best.anc.fas
-rw-r--r--. 1 gauravsablok gauravsablok  66 Jan  6 22:10 ancestral-aligned.fasta.best.fas
 
```
 Gaurav Sablok
