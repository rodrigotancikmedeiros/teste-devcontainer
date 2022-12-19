FROM alpine:3.12

# Atualiza o gerenciador de pacotes apk e instala as dependências do Terraform
RUN apk update && apk add curl

# Baixa o Terraform
RUN curl -LO https://releases.hashicorp.com/terraform/1.3.6/terraform_1.3.6_linux_amd64.zip

# Descompacta o arquivo baixado
RUN unzip terraform_1.3.6_linux_amd64.zip

# Move o executável do Terraform para o diretório de binários do sistema
RUN mv terraform /usr/local/bin/

# Remove os arquivos temporários
RUN rm terraform_1.3.6_linux_amd64.zip

# Especifica o diretório de trabalho do contêiner
WORKDIR /app

# Especifica um processo para ser executado quando o contêiner for iniciado
CMD ["tail", "-f", "/dev/null"]
