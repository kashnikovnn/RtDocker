#RT Test work
FROM eclipse/ubuntu_jdk8

RUN sudo apt-get update 
RUN git clone https://github.com/kashnikovnn/RtTestWork.git
WORKDIR /projects/RtTestWork/
RUN mvn -Dmaven.test.skip=true package 
WORKDIR /projects/RtTestWork/target/
CMD ["java","-jar","/projects/RtTestWork/target/testwork-0.0.1.jar"]

EXPOSE 8080

