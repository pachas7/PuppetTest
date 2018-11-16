FROM centos
ENV PATH=$PATH:/opt/puppetlabs/bin/

RUN rpm -Uvh https://yum.puppet.com/puppet5/puppet5-release-el-7.noarch.rpm && \
    yum install -y puppet && \

    
COPY test.pp /etc/puppetlabs/code/module
