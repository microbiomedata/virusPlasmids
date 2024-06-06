# $ docker build . -t microbiomedata/genomad:latest --build-arg http_proxy=http://proxyout.lanl.gov:8080 --build-arg https_proxy=http://proxyout.lanl.gov:8080
# $ docker login
# $ docker push microbiomedata/genomad:latest

From continuumio/miniconda3:4.11.0

LABEL maintainer="Antonio Camargo (antoniop.camargo@lbl.gov)"
LABEL version="1.7.1"

RUN conda install -y -n base -c conda-forge -c bioconda genomad==1.7.1 && \
    conda clean --all --yes

CMD ["/bin/bash"]