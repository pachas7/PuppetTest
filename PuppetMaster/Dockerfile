FROM centos

ENV PATH=$PATH:/opt/puppetlabs/puppet/bin/
ENV PUPPETSERVER_JAVA_ARGS="-Xms512m -Xmx512m"

RUN rpm -Uvh https://yum.puppet.com/puppet5/puppet5-release-el-7.noarch.rpm && \
    yum install -y puppetserver

CMD [ "puppet", "master" , "--no-daemonize" ]
