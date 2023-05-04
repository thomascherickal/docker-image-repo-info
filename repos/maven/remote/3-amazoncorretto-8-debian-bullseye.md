## `maven:3-amazoncorretto-8-debian-bullseye`

```console
$ docker pull maven@sha256:7ab3d55b03caa87cc035eee182ce040482fcad99aebca005c765727c1e7160a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-8-debian-bullseye` - linux; amd64

```console
$ docker pull maven@sha256:62de1a09950388f859877645063775c019807868fca4f36f0af78204bb8b09f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.0 MB (159995665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3bcd6fa8dec7d72df47080ba9764d0d1e73e9c989e3e5ea5814afdd56bd5d61`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Thu, 04 May 2023 07:27:26 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-1.8.0-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 04 May 2023 07:27:26 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 04 May 2023 07:27:26 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Thu, 04 May 2023 07:27:26 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Thu, 04 May 2023 07:27:26 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Thu, 04 May 2023 07:27:26 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Thu, 04 May 2023 07:27:26 GMT
ARG MAVEN_VERSION=3.9.1
# Thu, 04 May 2023 07:27:26 GMT
ARG USER_HOME_DIR=/root
# Thu, 04 May 2023 07:27:26 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 04 May 2023 07:27:26 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 04 May 2023 07:27:26 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51276179a664e5cd96a54d121baa8e69f0b9841c3686a9f410c3786a8b26c167`  
		Last Modified: Wed, 03 May 2023 20:58:50 GMT  
		Size: 119.5 MB (119484599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5f6ed66791ca60313cf00055299b2402e582a217f0464980e4903ce23fad46`  
		Last Modified: Wed, 03 May 2023 20:58:42 GMT  
		Size: 9.1 MB (9106174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab3d43bbde8cbd99a9630c53a1486f09ef4e71a5ecb028616a3822af43eacf0`  
		Last Modified: Wed, 03 May 2023 20:58:41 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c7aeb77bfa998d7c4dfe61c3eb12a74947117476f168f7409455fcfedc9030`  
		Last Modified: Wed, 03 May 2023 20:58:41 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eeab87d880b9961990eeafc76e1cb997fd7a3679fe8ba6b119afa017443c7df`  
		Last Modified: Wed, 03 May 2023 20:58:41 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-8-debian-bullseye` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:b852b4e15b52349226c381f7875856bf969b4c38eaa0ca913d49d9cceccde134
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.6 MB (142620636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f79c9a70a60e74eaeadeda00d8668eecc51e01602662ffb5736ecd0d490c05a1`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Thu, 04 May 2023 03:25:59 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-1.8.0-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 04 May 2023 03:25:59 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 04 May 2023 03:25:59 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Thu, 04 May 2023 03:25:59 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Thu, 04 May 2023 03:25:59 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Thu, 04 May 2023 03:25:59 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Thu, 04 May 2023 03:25:59 GMT
ARG MAVEN_VERSION=3.9.1
# Thu, 04 May 2023 03:25:59 GMT
ARG USER_HOME_DIR=/root
# Thu, 04 May 2023 03:25:59 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 04 May 2023 03:25:59 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 04 May 2023 03:25:59 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb45b4d6424f642b0b69222bec2c002c21337d17bdd9115fb9d95ecf36984ee6`  
		Last Modified: Wed, 03 May 2023 19:46:54 GMT  
		Size: 103.5 MB (103460363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c63cba9d8a53f7f9c04d766313b8b4efc35bdd0c802b09ea9ec5c572831a4a`  
		Last Modified: Wed, 03 May 2023 19:46:48 GMT  
		Size: 9.1 MB (9106165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ea64d3c30a052654031fbdf2ca10df026953d30cae4fb09388699074c57cf1`  
		Last Modified: Wed, 03 May 2023 19:46:47 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867e8a10ec42c4a1964349f59595d99681f12436b6593318eab1f6f0cbc69cb3`  
		Last Modified: Wed, 03 May 2023 19:46:47 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0878c868d2c74e0249716bd64540135724b6c576a592bfc242ea71542280d5f4`  
		Last Modified: Wed, 03 May 2023 19:46:47 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
