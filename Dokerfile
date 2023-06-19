FROM registry.redhat.io/openshift4/ose-jenkins-agent-maven
COPY vulnerability_scan.sh /vulnerability_scan.sh
RUN mkdir /home/jenkins/docker
COPY --chown=1000780000:1000780000 config.json /home/jenkins/docker/config.json
USER root
RUN yum -y install skopeo curl jq grep sed bash --disableplugin=subscription-manager && \
chmod 755 /vulnerability_scan.sh && \
chmod 777 /home/jenkins/docker/config.json
