Reproducer for https://github.com/spring-projects/spring-boot/issues/42012

* Create a large file using `dd if=/dev/urandom of=lib/src/main/resources/big.dat bs=1g count=3`
* Run `./mvnw package`
* Run `java -jar app/target/bigzip-app-0.0.1-SNAPSHOT.jar`


