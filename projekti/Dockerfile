FROM ubuntu:16.04 

WORKDIR /mydir 
RUN touch hello.txt 
COPY hello.txt . 
RUN wget http://example.com/index.html 
CMD ["/bin/bash"]