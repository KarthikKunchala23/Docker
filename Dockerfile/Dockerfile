FROM ubuntu:20.04
RUN apt update && apt install nginx wget curl vim -y
#RUN useradd test1
#LABEL user=karthik
#USER test1
#WORKDIR /home/test1
ENV app=prod
ARG version=2
ONBUILD COPY useradd.sh .
EXPOSE 80
#CMD ["bash", "useradd.sh"]
#ADD tmp.tar /home
#COPY tmp.tar .
#ENTRYPOINT ["bash", "useradd.sh"]
#ENTRYPOINT ["nginx", "-g", "daemon off;"]
HEALTHCHECK --interval=5s CMD ping -c 5 172.17.0.2
ENTRYPOINT ["nginx", "-g", "daemon off;"]

