## `maven:3-amazoncorretto-11-debian-bookworm`

```console
$ docker pull maven@sha256:ca6f15d8498b3df7177fafb940df22698f0e2e5a8b6a720424b56d5ae92f064e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-11-debian-bookworm` - linux; amd64

```console
$ docker pull maven@sha256:4df1bdd49619f6e0f3e61d74f3b45b1806ad56972fb8091b647af5e4e870c9fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.6 MB (237555305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae0219c0c166b84cfb33f356607132c3e70d4864acc3d2d470bd393725ca50b`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Sat, 17 Jun 2023 08:38:16 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-11-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 17 Jun 2023 08:38:16 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 17 Jun 2023 08:38:16 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Sat, 17 Jun 2023 08:38:16 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Sat, 17 Jun 2023 08:38:16 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Sat, 17 Jun 2023 08:38:16 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Sat, 17 Jun 2023 08:38:16 GMT
ARG MAVEN_VERSION=3.9.2
# Sat, 17 Jun 2023 08:38:16 GMT
ARG USER_HOME_DIR=/root
# Sat, 17 Jun 2023 08:38:16 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 17 Jun 2023 08:38:16 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 17 Jun 2023 08:38:16 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a62d46d36a9938499e4df7f77961d2180d9b3f842a3fcd6b46b88f7b546c83`  
		Last Modified: Tue, 20 Jun 2023 22:45:19 GMT  
		Size: 199.1 MB (199114754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2df41adf18d71ce7b6bc4f2e6d782df52245a61116dfff9a24f2881b41b0fa5`  
		Last Modified: Tue, 20 Jun 2023 22:45:06 GMT  
		Size: 9.3 MB (9314432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b82aad631d4791d334289810610f71d13e6e752412134190a73764cb300669`  
		Last Modified: Tue, 20 Jun 2023 22:45:06 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a6acdc173f4dd2185cb82326733fcdc69e692aec9e3ee42a486c5bd7d3ea6f`  
		Last Modified: Tue, 20 Jun 2023 22:45:06 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3784182bb86e72ece204c11bc24549ce486f95c3765842d30683e35d69d4c6c6`  
		Last Modified: Tue, 20 Jun 2023 22:45:06 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-11-debian-bookworm` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:8da417ad115f63edfe314958c260d5de8b75f73b2e3a24c4536b3dead13be241
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.5 MB (234524812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d2c129d167d886a52b92eafe2826ac5e249db1a39078f113afcee4f6f5517d7`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Sat, 17 Jun 2023 08:38:16 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-11-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 17 Jun 2023 08:38:16 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 17 Jun 2023 08:38:16 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Sat, 17 Jun 2023 08:38:16 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Sat, 17 Jun 2023 08:38:16 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Sat, 17 Jun 2023 08:38:16 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Sat, 17 Jun 2023 08:38:16 GMT
ARG MAVEN_VERSION=3.9.2
# Sat, 17 Jun 2023 08:38:16 GMT
ARG USER_HOME_DIR=/root
# Sat, 17 Jun 2023 08:38:16 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 17 Jun 2023 08:38:16 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 17 Jun 2023 08:38:16 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61e45ff6193b3dd6f485a930dfd689329509eab85d6f879be6a102635f20116`  
		Last Modified: Tue, 20 Jun 2023 23:02:15 GMT  
		Size: 196.1 MB (196056487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2dd13ac6286d2cf559383f94ffe075ae567fba26c77eb529b9783f1fc0328f1`  
		Last Modified: Tue, 20 Jun 2023 23:02:04 GMT  
		Size: 9.3 MB (9314418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfaaae31255ac24752735d0253f1c4debffab3db142ae9fe69a8f97dc9a2cf60`  
		Last Modified: Tue, 20 Jun 2023 23:02:03 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b799e80ae3a940d396472c3d9e41ef20c0242ad7cb76f9ce711c483c6a4727`  
		Last Modified: Tue, 20 Jun 2023 23:02:04 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912dcb58c7b6efb8066623ce6d3901b291ac5c1ea32636dd933287965cee273b`  
		Last Modified: Tue, 20 Jun 2023 23:02:04 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
