FROM 100.125.0.198:20202/hwcpe-cn-north-1/dockerhub-java:8-jre-alpine

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && \
    echo "Asia/Shanghai" > /etc/timezone

WORKDIR /home/apps/
ADD target/demo-operation-1.2.0.jar .


ENTRYPOINT ["java","-jar", "demo-operation-1.2.0.jar"]
