FROM ubuntu:14.04
RUN apt-get update && apt-get install curl vim nginx -y
RUN useradd testuser
LABEL owner=devops-team
COPY contfile .
COPY useradd.sh .
COPY project.tar .
ADD project.tar /home
ENV app=prod
#USER testuser
#WORKDIR /home
#CMD ["bash", "useradd.sh"]
#ENTRYPOINT ["bash", "useradd.sh"]
CMD ["user1"]
ENTRYPOINT ["echo", "hi"]
