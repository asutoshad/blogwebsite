FROM node:18-alpine

WORKDIR /app

COPY package.json yarn.lock ./
RUN yarn install --frozen-lockfile


COPY . .


EXPOSE 4004
CMD ["sh", "-c", "yarn migrate && yarn start"]
