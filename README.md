## 0.simple-web: 

-  docker build -t yourName/simpleweb .
-  docker run -p 8080:8080 yourNameAccount/simpleweb

## 1.visits-counter:

- docker-compose up

## 2.production-grade-workflow

![production-grade-workflow](./img/3.png)

## 3.fibonacci-sequence

![fibonacci architecture](./img/0-fibonacci.png)

![fibonacci deployment](./img/1-fibonacci.png)

### 4. K8S deployment of Project 3 

To run you need to add the secrets in an imperative way (commands typing from terminal):

```kubectl create secret generic pgpassword --from-literal POSTGRES_PASSWORD=password ```

![fibonacci deployment to prod](./img/deployment-to-prod-fibonacci.png)