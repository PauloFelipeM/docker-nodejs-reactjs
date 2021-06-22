FROM node:14.17.0
WORKDIR /app
COPY ["package.json", "yarn.lock", "./"]
RUN yarn install --production
COPY . .
EXPOSE 80
CMD ["yarn", "install", "--production"]