FROM azul/zulu-openjdk-centos

ADD yum.repo /etc/yum.repos.d/portal-de-servicos.repo
RUN rpm --import https://raw.githubusercontent.com/servicosgovbr/portal-de-servicos/master/src/main/resources/static/GPG-KEY
RUN yum install -y portal-de-servicos

ADD run.sh /run.sh

EXPOSE 8080
CMD sh /run.sh
