FROM node:14.17.0
WORKDIR /app
COPY ["package.json", "yarn.lock", "wait-for.sh", "startup.sh", "./"]
RUN apt-get update && apt-get install netcat -y && chmod +x ./wait-for.sh ./startup.sh && yarn install --production
COPY . .
EXPOSE 5000
CMD ["yarn", "start"]