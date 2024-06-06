# $ docker build . -t microbiomedata/checkv:latest --build-arg http_proxy=http://proxyout.lanl.gov:8080 --build-arg https_proxy=http://proxyout.lanl.gov:8080
# $ docker login
# $ docker push microbiomedata/checkv:latest

From continuumio/miniconda3:4.10.0

LABEL maintainer="Michal Babinski"
LABEL version="1.0.1"

RUN conda install -c conda-forge -c bioconda checkv

CMD ["/bin/bash"]

# FROM quay.io/biocontainers/checkv:0.8.1--pyhdfd78af_0
# LABEL maintainer="Antonio Camargo (antoniop.camargo@lbl.gov), Stephen Nayfach (snayfach@lbl.gov)"
# LABEL version="0.8.1"
# CMD ['/bin/bash']
