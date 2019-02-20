# SANSPANZ_docker
SANSZPAZ Docker image

Run in Docker

Run in Singularity:

    singularity exec -e sanspanz3.simg python /usr/local/SANSPANZ.3/runsanspanz.py -R -o ",DE.out,GO.out,anno.out" -s "Macaca mulatta" < /path/to/testdata/querysequences.fasta

## TODO

* Fix python definition in Singularity

