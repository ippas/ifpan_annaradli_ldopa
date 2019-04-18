# ifpan-annaradli-ldopa

## Rat model of Parkinson - Medial Forebrain Bundle RNAseq (tissue collected from both hemispheres, n = 5 group)

### Experimental scheme:

* Experimental group: Rats with 6-OHDA-induced Parkinson symptoms (left hemisphere) treated with L-DOPA
* Control group: Rats with 6-OHDA-induced Parkinson symptoms (left hemisphere)

### Animal list
exp: L1star, L2star, L4star, L5star, L6star
ctrl: L10star, L11star, L23, L32, L39

### Sample list (sample stored in /home/ifpan/projects/ifpan-annaradli-ldopa/data/fq)
 | file_name | number_of_reads | 
 | -------- | ------- |
 | L10starL_1.fq.gz | 1880504 | 
 | L10starL_2.fq.gz | 1971877 | 
 | L10starP_1.fq.gz | 2221950 | 
 | L10starP_2.fq.gz | 2290032 | 
 | L11starL_1.fq.gz | 2012511 | 
 | L11starL_2.fq.gz | 2117865 | 
 | L11starP_1.fq.gz | 2089387 | 
 | L11starP_2.fq.gz | 2221945 | 
 | L1starL_1.fq.gz | 2009261 | 
 | L1starL_2.fq.gz | 2044706 | 
 | L1starP_1.fq.gz | 1726636 | 
 | L1starP_2.fq.gz | 1759766 | 
 | L23L_1.fq.gz | 1815865 | 
 | L23L_2.fq.gz | 1855456 | 
 | L23P_1.fq.gz | 1658417 | 
 | L23P_2.fq.gz | 1699851 | 
 | L2starL_1.fq.gz | 2000326 | 
 | L2starL_2.fq.gz | 2047582 | 
 | L2starP_1.fq.gz | 1971617 | 
 | L2starP_2.fq.gz | 2021615 | 
 | L32L_1.fq.gz | 2382900 | 
 | L32L_2.fq.gz | 2519685 | 
 | L32P_1.fq.gz | 2325242 | 
 | L32P_2.fq.gz | 2394761 | 
 | L39L_1.fq.gz | 2263788 | 
 | L39L_2.fq.gz | 2439760 | 
 | L39P_1.fq.gz | 1803855 | 
 | L39P_2.fq.gz | 1859031 | 
 | L4starL_1.fq.gz | 1821616 | 
 | L4starL_2.fq.gz | 1894408 | 
 | L4starP_1.fq.gz | 2604298 | 
 | L4starP_2.fq.gz | 2682332 | 
 | L5starL_1.fq.gz | 1993071 | 
 | L5starL_2.fq.gz | 2074781 | 
 | L5starP_1.fq.gz | 1793386 | 
 | L5starP_2.fq.gz | 1821850 | 
 | L6starL_1.fq.gz | 1619904 | 
 | L6starL_2.fq.gz | 1648328 | 
 | L6starP_1.fq.gz | 1800201 | 
 | L6starP_2.fq.gz | 1837372 | 

### sample quality control
1. Running qc using the pulled docker image: [detailed instructions here](https://hub.docker.com/r/pegi3s/fastqc), see atached script `run-fastqc.sh`

### software + versions + installations
1. [docker installation](https://gist.github.com/gosborcz/f1f3dbd7aa256e26ae1e8ce33fd30509)
2. [pulling docker image with fastqc](https://gist.github.com/gosborcz/1735c2533061354756b05154519972bf), fastqc version=0.11.8


### attached files
1. files-and-reads.md - list of all the samples, with read numbers
2. list-and-count-reads.sh - simple script that lists files, counts reads and makes a .md table
3. run-fastqc.sh - run fastqc on .fq.gz samples in current directory using pegi3/fastqc image
4. fastqc-dockerfile - dockerfiles of the pegi3/fastqc image
