# Dockerfile para Frontend (Next.js)
FROM node:18

# Definir o diretório de trabalho no container
WORKDIR /app

# Copiar os arquivos de package.json e package-lock.json para o container
COPY package*.json ./

# Instalar as dependências do Next.js
RUN npm install

# Copiar o código do projeto para dentro do container
COPY . .

# Construir o projeto Next.js
RUN npm run build

# Expor a porta 3000 para o frontend Next.js
EXPOSE 3000

# Iniciar o servidor Next.js
CMD ["npm", "start"]
