FROM node:20-alpine
WORKDIR /app
COPY .output ./.output
COPY package.json package-lock.json* ./
RUN npm ci --omit=dev || npm install --omit=dev
EXPOSE 3000
CMD ["node", ".output/server/index.mjs"]