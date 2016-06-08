FROM python:2

RUN apt -qq update \
 && apt -qq upgrade -y \
 && apt -qq install -y texlive-base texlive-latex-base texlive-fonts-recommended texlive-fonts-extra \
    texlive-latex-extra texlive-latex-recommended texlive-extra-utils texlive-font-utils \
 && rm -rf /var/lib/apt/lists/*

