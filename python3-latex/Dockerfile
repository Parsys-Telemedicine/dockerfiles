FROM python:3

RUN apt -qq update \
 && apt -qq upgrade -y \
 && apt -qq install -y latexmk texlive-base texlive-extra-utils texlive-fonts-extra \
    texlive-fonts-recommended texlive-font-utils texlive-generic-extra \
    texlive-latex-base texlive-latex-extra texlive-latex-recommended vim \
 && rm -rf /var/lib/apt/lists/*

