
# build stage
FROM node:16-alpine as builder 
WORKDIR '/app'
COPY package.json .
RUN npm install
COPY . .
RUN npm run build

# run stage, just copy the build folder from the previous step.
FROM nginx:1.23.3
EXPOSE 80
COPY --from=builder /app/build /usr/share/nginx/html