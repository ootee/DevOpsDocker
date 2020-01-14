FROM ubuntu:16.04 

WORKDIR /mydir 
RUN apt-get update && apt-get install -y wget 

RUN touch hello.txt 
RUN wget http://example.com/index.html 
CMD ["/bin/bash"]