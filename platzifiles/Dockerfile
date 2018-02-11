FROM jeanblanchard/busybox-java:/
MAINTAINER Noel Vaca, noel.vm.2501@gmail.com
RUN wget -O http://dynamodb-local.s3-website-us-west-2.amazonas.com/dynamodb_local_latest | gunzip | tar x
ENTRYPOINT ["/opt/jdk/bin/java", "-Djava.library.path=./DynamoDBLocal_lib", "-jar", "DynamoDBLocal.jar"]
CMD ["-help"]

