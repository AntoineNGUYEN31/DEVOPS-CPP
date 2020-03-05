FROM centos:7
LABEL maintainer="minh-quan.nguyen.external@airbus.com"
RUN curl -sL https://rpm.nodesource.com/setup_10.x | bash - &&\
yum -y update &&\
yum -y install java-1.8.0-openjdk &&\
yum -y install maven &&\
yum -y install nodejs &&\
yum -y install git &&\
yum -y install bzip2 &&\
yum -y install which &&\
curl -O https://repo.anaconda.com/archive/Anaconda3-5.3.1-Linux-x86_64.sh &&\
sh Anaconda3-5.3.1-Linux-x86_64.sh -b -p /opt/anaconda3 &&\
yum clean all &&\
rm -f Anaconda3-5.3.1-Linux-x86_64.sh
#COPY src des
#ADD src des/
#EXPOSE 80
ENV PATH /opt/anaconda3/bin/:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
#WORKDIR /tmp
#CMD[]
