FROM node:14

WORKDIR /app

COPY package*.json ./

# Nós instalamos as dependências antes de copiar o restante dos arquivos
# para aproveitar o cache do Docker.
RUN npm install

RUN npm install -g json-server

# Agora copiamos o restante dos arquivos.
COPY . .

# Nós mudamos para o diretório memoteca/backend.
WORKDIR /app/memoteca/backend

EXPOSE 3000

CMD ["npm", "start"]
