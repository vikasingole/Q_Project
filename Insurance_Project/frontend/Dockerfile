# Note - NGINX Dockerfile for PRODUCTION (Recommended) :-

# ✔ Advantages :-
# 1] Very fast
# 2] Lightweight
# 3] Optimized for production
# 4] Industry standard
# 5] Works perfectly behind backend API

# Build stage
FROM node:20
WORKDIR /app
COPY . .
RUN npm install
RUN npm run build

# Run stage
FROM nginx:alpine
COPY build /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]

# Note - NGINX Dockerfile for DEVELOPEMENT :-

# FROM node:20
# WORKDIR /app
# COPY package*.json ./
# RUN npm install
# COPY . .
# RUN npm run build
# EXPOSE 80
# CMD ["npm", "start"]

