
# Bioinformatics Format Specimens

[![Join the chat at https://gitter.im/BioJulia/BioFmtSpecimens](https://badges.gitter.im/BioJulia/BioFmtSpecimens.svg)](https://gitter.im/BioJulia/BioFmtSpecimens?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Bioinformatics is rife with formats and parsers for those formats. These parsers
don't always agree on the definitions of these formats, since many lack any sort
of formal standard.

This repository aims to consolidate a collection of format specimens to create a
unified set of data with which to test software against. Testing against the
same cases is a first step towards agreeing on the details and edge cases of a
format.


# Organization

This repository consists of a directory for every major format. Directories
contain format specimens along with a file `index.yml`. This is a
[YAML](http://www.yaml.org/) document containing an entry for every specimen in
the directory. Each entry has the following fields:

  * **filename** Specimen filename.
  * **valid** True or false, annotating whether the example is considered to
    conform to the format.
  * **origin** The contributor or source from which a specimen was taken.
  * **tags** Zero or more words used to group specimens by shared features.
  * **comments** (Optional) Any additional information that might be of
    interest.

