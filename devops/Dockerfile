FROM teravisiontech/lampbase
MAINTAINER Teravision-Infraestructura <support@teravisiontech.com>
RUN yum -y update &&  yum -y install ansible git 
COPY ./ /tmp
RUN ansible-playbook -i "localhost," -c local --tags command /tmp/playbook.yml 
