FROM node:22-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install --omit=dev
COPY . .
EXPOSE 4000
# index.js es el servidor completo (crea tablas, roles y todas las rutas).
# server.js está incompleto: le falta /api/mantenimientos y no inicializa la BD.
CMD ["node", "index.js"]
