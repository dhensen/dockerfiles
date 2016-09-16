FROM ubuntu

RUN apt-get update
RUN apt-get install -y wget unpaper exactimage imagemagick poppler-utils ghostscript
RUN apt-get install -y tesseract-ocr
RUN wget https://sourceforge.net/projects/pdfsandwich/files/pdfsandwich%200.1.5/pdfsandwich_0.1.5_amd64.deb
RUN dpkg -i pdfsandwich_0.1.5_amd64.deb

ENTRYPOINT ["/usr/bin/pdfsandwich"]

CMD ["--help"]

