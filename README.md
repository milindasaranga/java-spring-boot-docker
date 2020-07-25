docker build -t springio/gs-spring-boot-docker .  
command builda an image and tag it as springio/gs-spring-boot-docker  
mkdir -p target/dependency && (cd target/dependency; jar -xf ../*.jar)  
docker run -p 8080:8080 -t springio/gs-spring-boot-docker  
docker run -e "SPRING_PROFILES_ACTIVE=prod" -p 8080:8080 -t springio/gs-spring-boot-docker. 

=================================================================  
build image using maven command. 
./mvnw spring-boot:build-image -Dspring-boot.build-image.imageName=springio/gs-spring-boot-docker. 
