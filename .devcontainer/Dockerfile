FROM debian
RUN apt update 
RUN apt install wget -y
RUN apt install unzip -y
RUN apt install curl -y
RUN wget https://releases.hashicorp.com/terraform/1.3.6/terraform_1.3.6_linux_386.zip
RUN unzip terraform_1.3.6_linux_386.zip -d /usr/local/bin
RUN curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
ENTRYPOINT ["tail", "-f", "/dev/null"]