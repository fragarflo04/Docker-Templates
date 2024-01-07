FROM node:14
WORKDIR /app
RUN git clone https://github.com/strapi/strapi-docker.git .
RUN yarn install
EXPOSE 1337
CMD ["yarn", "develop"]