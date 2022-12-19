FROM alpine:3.12

# Atualiza o gerenciador de pacotes apk e instala as dependências do Terraform
RUN apk update && apk add curl

# Baixa o script de instalação automática do Terraform
RUN curl -fsSL https://apt.releases.hashicorp.com/install.sh | sh

# Especifica o diretório de trabalho do contêiner
WORKDIR /app

# Especifica um processo para ser executado quando o contêiner for iniciado
CMD ["tail", "-f", "/dev/null"]
