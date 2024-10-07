# Imagen base de Node.js
FROM node:18

# Establecer el directorio de trabajo
WORKDIR /app

# Copiar los archivos package.json y package-lock.json
COPY package*.json ./

# Instalar las dependencias
RUN npm install

# Copiar el resto de la aplicación
# COPY . .

# Exponer el puerto que Vue.js utilizará (8080 por defecto)
EXPOSE 8080

# Comando por defecto para ejecutar Vue.js
CMD ["npm", "run", "serve"]
