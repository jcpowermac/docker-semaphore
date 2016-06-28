FROM williamyeh/ansible:centos7

RUN mkdir -p /opt/semaphore/bin && \
    mkdir -p /opt/semaphore/playbooks

ADD https://github.com/ansible-semaphore/semaphore/releases/download/v2.0.4/semaphore_linux_amd64 /opt/semaphore/bin/semaphore
WORKDIR /opt/semaphore/bin
RUN chmod 755 semaphore
CMD ["/bin/bash"]
EXPOSE 3000