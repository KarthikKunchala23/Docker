FROM ubuntu:20.04
RUN apt update && apt install nginx wget curl vim -y
#RUN useradd test1
#LABEL user=karthik
#USER test1
#WORKDIR /home/test1
COPY useradd.sh .
EXPOSE 8080
#CMD ["bash", "useradd.sh"]
#ADD tmp.tar /home
#COPY tmp.tar .
ENTRYPOINT ["bash", "useradd.sh"]
