# Build the React Application

FROM node:20-alpine 
WORKDIR /app
COPY package.json package-lock.json ./
RUN npm install
COPY . .
EXPOSE 3000
CMD ["npm", "start"]

# We can specify - COPY package.json* ./ [it means - include both the files, i.e. package.json and package-lock.json ]

# Serve the Static Assets using Nginx

# RUN npm run build
# FROM nginx:alpine
# COPY --from=builder /app/build /usr/share/nginx/html
# EXPOSE 80
# CMD ["nginx", "-g", "daemon off;"]
