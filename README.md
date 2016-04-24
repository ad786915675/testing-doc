# Mastering maven 3

# Book
![1](https://dz13w8afd47il.cloudfront.net/sites/default/files/imagecache/ppv4_main_book_cover/3865OS%20(B02037)_mockupcover_normal_0.jpg)

# Commands
```
mvn clean install
# Remote debugging
mvn clean install -Dmaven.surefire.debug
# Enable debug level logging
mvn clean install –X
# Building dependency tree
mvn dependency:tree
# Viewing all environment variables and system properties
mvn help:system
# Viewing the dependency classpath
mvn dependency:build-classpath
# Analyze
mvn dependency:analyze
# Wagon system properties
# This enables or disables the HTTP connection pooling
mvn clean install -Dmaven.wagon.http.pool=true
# This speci es the maximum number of total HTTP connections that can be created against all the destinations/repositories
mvn clean install -Dmaven.wagon.httpconnectionManager.maxTotal=40
# Validates whether the server's TLS certi cate is signed by a trusted Certi cate Authority (CA)
mvn clean install -Dmaven.wagon.http.ssl.insecure=false
# Check whether the hostname of the endpoint matches the CN (Common Name) value of its certi cate
mvn clean install -Dmaven.wagon.http.ssl.allowall=false
# Use the mvn deploy command to deploy the artifacts into the con gured repository
mvn deploy
```

# Standard lifecycles in Maven
```
mvn help:describe -Dcmd=deploy
mvn help:describe -Dcmd=site
```

