# nist-ehandbook-datasets

[![Static Badge](https://img.shields.io/badge/doi-10.18434%2FM32189-blue?label=doi&color=blue)](https://doi.org/10.18434/M32189)

This repository is a simple mirror of the datasets referenced from **NIST/SEMATECH e-Handbook of Statistical Methods**. [^nist-datasets] Every file is in the `.DAT` file format, and specifically formatted for the Dataplot software also created by NIST. [^dataplot-file-format]

For licensing information concerning the datasets, please read NIST's policy. [^nist-license]

## Example dataset

An example dataset ([`ANSCOMBE.DAT`](./ANSCOMBE.DAT)) is shown below. Some files may contain I/O commands for Dataplot, which are specified in the Dataplot Reference Manual. [^dataplot-manual]

```dat
ANSCOMBE'S   GRAPHICS VERSUS STATISTICS    DATA
(WITH THANKS TO KEITH EBERHARDT AT NIST)
NUMBER OF OBSERVATIONS = 11
NUMBER OF VARIABLES = 8
ORDER OF VARIABLES ON A LINE IMAGE--
   X1 Y1   X2 Y2   X3 Y3   X4 Y4
NOTE--THESE 4 DATA SETS ARE DIFFERENT IN GRAPHICAL STRUCTURE
      BUT HAVE THE FOLLOWING IDENTICAL STATISTICS--
         SAMPLE SIZE        = 11
         MEAN OF X'S        = 9.0
         MEAN OF Y'S        = 7.5
         INTERCEPT          = 3.0
         SLOPE              = 0.5
         RESID. STAND. DEV. = 1.125
         CORR. COEFFICIENT  = 81.7%
SOURCE--ANSCOMBE, FRANK J. (1973). "GRAPHS IN STATISTICAL ANALYSIS"
        AMERICAN STATISTICIAN, VOL. 27, FEBRUARY 1973.
TO READ THIS FILE INTO DATAPLOT (& ANALYZE)--
   SKIP 25
   READ ANSCOMBE.DAT X1 Y1 X2 Y2 X3 Y3 X4 Y4
   CHARACTERS X; LINES BLANK
   MULTIPLOT 2 2
   PLOT Y1 X1; PLOT Y2 X2; PLOT Y3 X3; PLOT Y4 X4
  X1     Y1       X2     Y2       X3     Y3       X4     Y4
-------------------------------------------------------------------
10.00   8.04    10.00   9.14    10.00   7.46     8.00   6.58
 8.00   6.95     8.00   8.14     8.00   6.77     8.00   5.76
13.00   7.58    13.00   8.74    13.00  12.74     8.00   7.71
 9.00   8.81     9.00   8.77     9.00   7.11     8.00   8.84
11.00   8.33    11.00   9.26    11.00   7.81     8.00   8.47
14.00   9.96    14.00   8.10    14.00   8.84     8.00   7.04
 6.00   7.24     6.00   6.13     6.00   6.08     8.00   5.25
 4.00   4.26     4.00   3.10     4.00   5.39    19.00  12.50
12.00  10.84    12.00   9.13    12.00   8.15     8.00   5.56
 7.00   4.82     7.00   7.26     7.00   6.42     8.00   7.91
 5.00   5.68     5.00   4.74     5.00   5.73     8.00   6.89

```

[^dataplot-manual]: Heckert, A. (2001, June 5). Dataplot Reference Manual: Volume 1. NIST Electrical Engineering Division. <https://www.itl.nist.gov/div898/software/dataplot/refman1/homepage.htm>
[^dataplot-file-format]: Heckert, A. (2001, June 5). Dataplot frequently asked questions (FAQS). NIST Electrical Engineering Division. <https://www.itl.nist.gov/div898/software/dataplot/faqs.htm#datafaq2>
[^nist-datasets]: NIST/SEMATECH e-Handbook of Statistical Methods, <https://www.itl.nist.gov/div898/handbook/datasets.htm>, July 11, 2023.
[^nist-license]: Copyright, fair use, and licensing statements for SRD, data, software, and Technical Series Publications. NIST. (2023, June 1). <https://www.nist.gov/open/copyright-fair-use-and-licensing-statements-srd-data-software-and-technical-series-publications>
