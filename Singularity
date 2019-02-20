BootStrap: docker
From: biocorecrg/debian-perlbrew-pyenv:stretch

%runscript
    echo "Welcome to BiocoreCRG SANSPANZ Image"

%post

    DOWNLOAD_URL=http://ekhidna2.biocenter.helsinki.fi/sanspanz/SANSPANZ.3.tar.gz
    PROG_DIR=SANSPANZ.3
	PYTHON_VERSION=2.7.13

    # Install dependencies
    /usr/local/perl/bin/cpanm Switch
	/usr/local/python/bin/pyenv rehash
    /usr/local/python/versions/${PYTHON_VERSION}/bin/pip install requests scipy numpy fastcluster

    cd /usr/local; curl --fail --silent --show-error --location --remote-name ${DOWNLOAD_URL}; tar zxf ${PROG_DIR}.tar.gz; rm ${PROG_DIR}.tar.gz

%labels
	Maintainer Biocorecrg
	Version 0.1.0

