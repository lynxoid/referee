## Referee

##### Rapid Separable Compression for Sequence Alignments 

Alignment files may exceed the size of the original sequence by an order of magnitude, however, Referee is able to compress it down to 1/10 of the original SAM file size and is twice as efficient as SAM’s binary BAM variant. Referee is fast, highly parallelizable, and outperformes state of the art tools by an average of 8.1%. It enables a variety of sequence-related tasks that require only a partial decompression. Computations like depth of sequencing that involve seeking through all alignments take from 8 to 44 seconds as opposed to tens of minutes with `samtools`. Referee uses a lightweight streaming clustering algorithm to improve quality values compression and encodes sequence information very efficiently, with compression rates as low as 0.03 bits per base. Its modular structure allows one to omit extraneous alignment information from the download reducing the total data size from many gigabytes to under a hundred megabytes.

Main version of this tool is hosted at [Kingsford-group/referee](https://github.com/Kingsford-Group/referee).
