## `maven:3-amazoncorretto-17-debian`

```console
$ docker pull maven@sha256:bb63f0893af58d37b00cb377b10c99492fcf68dc05eea5705b58e520e4af9356
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-17-debian` - linux; amd64

```console
$ docker pull maven@sha256:6fe4c32b81474913605c8917d348aedebecfcdb3ee4e7db0806bcccbd2692a85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.2 MB (236168163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a97bcbf818091e142f2c23d0217e5a5ff2e4378f794747218416bbd5ca2742b`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Mon, 26 Jun 2023 13:48:06 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-17-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
ARG MAVEN_VERSION=3.9.3
# Mon, 26 Jun 2023 13:48:06 GMT
ARG USER_HOME_DIR=/root
# Mon, 26 Jun 2023 13:48:06 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 26 Jun 2023 13:48:06 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 26 Jun 2023 13:48:06 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd07e925feea0cd7dbc8de682b166a0a7082743eb250be17e72ba65ebf2235a5`  
		Last Modified: Tue, 04 Jul 2023 12:55:18 GMT  
		Size: 197.7 MB (197714397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49779127a536333fce971d1f8d04e5b7ed5696f0fff934860891964f6ccad998`  
		Last Modified: Tue, 04 Jul 2023 12:55:05 GMT  
		Size: 9.3 MB (9327560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29cd790dce322346faf86dd3cdbf00b399be62ce66987ea7b312be4cf2759f34`  
		Last Modified: Tue, 04 Jul 2023 12:55:04 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4635e41f42fe9fd57081f2f593f69073bdf6f879813e0fc6138c01dd89b92291`  
		Last Modified: Tue, 04 Jul 2023 12:55:04 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976cbc23a8ce653e623702608da6e4e6ad2d112edf7704e59c0340291babc81d`  
		Last Modified: Tue, 04 Jul 2023 12:55:04 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-17-debian` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:2f642b8b6cbcb91c1332e5829539b67cc9369ddc6989458e4c2dcfdc5477ea79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.5 MB (234504340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a53e7f49573da96ac5ab445edd27ea3944dabfffb8f6b273e88e240548547f`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Mon, 26 Jun 2023 13:48:06 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-17-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
ARG MAVEN_VERSION=3.9.3
# Mon, 26 Jun 2023 13:48:06 GMT
ARG USER_HOME_DIR=/root
# Mon, 26 Jun 2023 13:48:06 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 26 Jun 2023 13:48:06 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 26 Jun 2023 13:48:06 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658b0e0fd1fe14bc1508f73751253c6f4c150398b341712e09c880ef72427a2f`  
		Last Modified: Tue, 04 Jul 2023 06:33:06 GMT  
		Size: 196.0 MB (196022943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a87933b59dbc8c08fe16b101682f65586d45a73eda0d065cc671a96eb855177`  
		Last Modified: Tue, 04 Jul 2023 06:32:56 GMT  
		Size: 9.3 MB (9327565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a019072f387d931421fab5a2c92d13bd96533bb3dd4c263b979af7ad4e37666`  
		Last Modified: Tue, 04 Jul 2023 06:32:55 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f3ae5fd57ccc7d512674d420c8519e9da79b5dfc1b21ad268f6656349ad13f`  
		Last Modified: Tue, 04 Jul 2023 06:32:55 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d40505a1d046a33c09cda43559100ee1ea1ccaf8a050a1b9feb79bc71660a5a`  
		Last Modified: Tue, 04 Jul 2023 06:32:55 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
