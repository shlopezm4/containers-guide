# Se usa imagen alpine porque son livianas
FROM node:10.16.3-alpine
# asignando un directorio de trabajo
WORKDIR usr/src/app
# copiando package.json & package-lock.json
COPY package*.json ./
# instalando dependencias
RUN npm install
# copiando todos los archivos - excepto node_modules (especificado en dockerignore) 
COPY . .
#exponiendo el puerto 8080
EXPOSE 8080
# corriendo el comando 'npm starts'
CMD ["npm","start"]