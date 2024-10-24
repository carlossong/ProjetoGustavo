# Dockerfile para Backend (AdonisJS)
FROM node:18

# Definir o diretório de trabalho no container
WORKDIR /app

# Copiar os arquivos de package.json e package-lock.json para o container
COPY package*.json ./

# Instalar as dependências do AdonisJS
RUN npm install

# Copiar o código do projeto para dentro do container
COPY . .

# Expor a porta 3333 para o backend AdonisJS
EXPOSE 3333

# Rodar as migrações e iniciar o servidor
CMD ["node", "ace", "serve", "--watch"]
