FROM ubuntu:18.04

WORKDIR /jup

RUN apt update && \
    apt install python3 python3-pip curl -y

RUN curl -sL https://deb.nodesource.com/setup_10.x | bash

RUN apt install -y nodejs

RUN pip3 install --upgrade pip

RUN pip3 install jupyterlab

RUN pip3 install plotly pandas numpy seaborn pyldavis beautifulsoup4 nltk

RUN jupyter labextension install @jupyterlab/plotly-extension

EXPOSE 8888

ENTRYPOINT ["jupyter", "lab","--ip=0.0.0.0","--allow-root", "--NotebookApp.token=''"]
