FROM node:22-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install --omit=dev
COPY . .
EXPOSE 4000
# index.js crea tablas y roles y monta todas las rutas
CMD ["node", "index.js"]
