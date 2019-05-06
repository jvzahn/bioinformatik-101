setwd("~/Desktop/r")
# setzt das working directory fest
library(Biostrings)
# fügt die biostrings library hinzu
dnastring = DNAString("CGGAAGCGAGATTCGCGTGGCGTGATTCCGGCGGGCGTGGAGAAGCGAGATTCATTCAAGCCGGGAGGCGTGGCGTGGCGTGGCGTGCGGATTCAAGCCGGCGGGCGTGATTCGAGCGGCGGATTCGAGATTCCGGGCGTGCGGGCGTGAAGCGCGTGGAGGAGGCGTGGCGTGCGGGAGGAGAAGCGAGAAGCCGGATTCAAGCAAGCATTCCGGCGGGAGATTCGCGTGGAGGCGTGGAGGCGTGGAGGCGTGCGGCGGGAGATTCAAGCCGGATTCGCGTGGAGAAGCGAGAAGCGCGTGCGGAAGCGAGGAGGAGAAGCATTCGCGTGATTCCGGGAGATTCAAGCATTCGCGTGCGGCGGGAGATTCAAGCGAGGAGGCGTGAAGCAAGCAAGCAAGCGCGTGGCGTGCGGCGGGAGAAGCAAGCGCGTGATTCGAGCGGGCGTGCGGAAGCGAGCGG", start=1)
# formatiert einen DNA-String
f12 <- oligonucleotideFrequency(dnastring, width=12, step=1,
                         as.prob=FALSE, as.array=FALSE,
                         fast.moving.side="right", with.labels=TRUE)
# berechnet die Häufigkeit der k-mere (width), abhängig von der Schrittweite,
# berechnet auch die relativen Häufigkeiten
# http://www.bioconductor.org/packages/release/bioc/manuals/Biostrings/man/Biostrings.pdf
# Title Efficient manipulation of biological strings
# Author H. Pagès, P. Aboyoun, R. Gentleman, and S. DebRoy
f12[f12 == max(f12)] 
# stellt in der Tabelle nur die maximalen Werte dar.
#
# oligonucleotideFrequency(dnastring, width=3, step=1,
#                         as.prob=TRUE, as.array=FALSE,
#                        fast.moving.side="right", with.labels=TRUE)
