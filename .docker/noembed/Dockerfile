FROM perl:5.14

COPY ./cpanfile /usr/src/myapp/cpanfile
COPY ./cpanfile.snapshot /usr/src/myapp/cpanfile.snapshot
WORKDIR /usr/src/myapp

RUN cpanm Carton Starman
RUN carton install

COPY ./ /usr/src/myapp

EXPOSE 8080

CMD ["carton", "exec", "starman", "--port",  "8080", "-I",  "lib", "bin/noembed.psgi"]
