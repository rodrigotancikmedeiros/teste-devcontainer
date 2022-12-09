FROM debian
RUN apt update && apt install wget unzip -y
RUN wget https://releases.hashicorp.com/terraform/1.3.6/terraform_1.3.6_linux_386.zip -d /usr/local/bin 
ENTRYPOINT ["tail", "-f", "/dev/null"]