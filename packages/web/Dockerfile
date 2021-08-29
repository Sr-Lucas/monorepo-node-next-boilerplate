FROM node:lts

ENV PORT 3000

# Create app directory
RUN mkdir -p /usr/app
WORKDIR /usr/app

# Installing dependencies
COPY package*.json .
RUN yarn

# Copying source files
COPY . .

# Running the app
CMD ["yarn", "dev"]
