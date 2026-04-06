FROM node:20-alpine
WORKDIR /app
COPY  . .
RUN npm ci 
RUN npm run build
RUN npm run preview
EXPOSE 3000
