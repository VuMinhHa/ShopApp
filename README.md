## ShopApp
__FrontEnd__: Dùng Angular 17.0.6

Cài đặt: 
1. 'npm install -g yarn'
2. 'yarn install'
3. 'yarn start' để chạy dự án

__BackEnd__: Dùng Java Spring boot 3.1.2

__Docker__: Dùng các câu lệnh theo thứ tự:
1. docker-compose -f ./deployment.yaml rm -s -f mysql8-container
2. docker-compose -f ./deployment.yaml rm -s -f phpmyadmin8-container
3. docker-compose -f ./deployment.yaml rm -s -f shopapp-spring-container
4. docker-compose -f ./deployment.yaml rm -s -f redis-container
5. docker-compose -f ./kafka-deployment.yaml up -d zookeeper-01
6. docker-compose -f ./kafka-deployment.yaml up -d zookeeper-02
7. docker-compose -f ./kafka-deployment.yaml up -d zookeeper-03
8. docker-compose -f ./kafka-deployment.yaml up -d kafka-broker-01



