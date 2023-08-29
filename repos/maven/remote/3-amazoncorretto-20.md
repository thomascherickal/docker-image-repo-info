## `maven:3-amazoncorretto-20`

```console
$ docker pull maven@sha256:2414455006f101515c59af2c7d2a7c3c099ed0ec170961652e357458729bfdf7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-20` - linux; amd64

```console
$ docker pull maven@sha256:ad4fd9bfc00c6cac789fb885b7b5fc68fb36c3e0685f99a40e2250cf1fb6ce04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.6 MB (393642141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d13bc99fa512b5a4f927ff6ab4239a740d50f99c7515febea3dd1717756cf06`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 29 Aug 2023 18:29:22 GMT
COPY dir:591ada5c2fb65633b614a3ff732e6d83dcd91fe9ae925844fe9ba3323311bf74 in / 
# Tue, 29 Aug 2023 18:29:23 GMT
CMD ["/bin/bash"]
# Tue, 29 Aug 2023 19:49:37 GMT
ARG version=20.0.2.9-1
# Tue, 29 Aug 2023 19:50:04 GMT
# ARGS: version=20.0.2.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 29 Aug 2023 19:50:04 GMT
ENV LANG=C.UTF-8
# Tue, 29 Aug 2023 19:50:05 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
# Fri, 18 Aug 2023 15:26:34 GMT
RUN yum install -y tar which gzip # TODO remove # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 18 Aug 2023 15:26:34 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
ARG MAVEN_VERSION=3.9.4
# Fri, 18 Aug 2023 15:26:34 GMT
ARG USER_HOME_DIR=/root
# Fri, 18 Aug 2023 15:26:34 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 18 Aug 2023 15:26:34 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 18 Aug 2023 15:26:34 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:8be3d01330d7e2e197495d440aa60d14ac366aad5e8d105d86e384876aefec18`  
		Last Modified: Fri, 25 Aug 2023 08:53:43 GMT  
		Size: 62.5 MB (62477278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d57871a336f39c390c3c2ef46bc2038b3c822042220a4cd2ba8d403d199410`  
		Last Modified: Tue, 29 Aug 2023 19:59:05 GMT  
		Size: 160.9 MB (160938758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f1ab354c15728a20e721944d85abfb6390387f316d0534b91cda544e6a88c7`  
		Last Modified: Tue, 29 Aug 2023 20:20:39 GMT  
		Size: 160.8 MB (160818286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c496088e26b0611bdf4dbb112fe9718434c3482545844fc6088ee7e25b14d4`  
		Last Modified: Tue, 29 Aug 2023 20:20:25 GMT  
		Size: 9.4 MB (9406438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a071433df43608aae443d01083f1ecb01dde2e2eb7d6b8d3a5084f84ddbc36d`  
		Last Modified: Tue, 29 Aug 2023 20:20:24 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8bcfbbba3d6094ff9bd49d7cecb4906a9da4e412a37e402748350299215d3b`  
		Last Modified: Tue, 29 Aug 2023 20:20:24 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57205b17731dd0c9c2e0cc8fc3411d7c7ceb6e44fd079b78b3a9f74fa70e55b9`  
		Last Modified: Tue, 29 Aug 2023 20:20:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-20` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:4c74e4311d81742756ef7232c8965b84d9da17d4e5ee35deea47bf998d887af6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.9 MB (357855845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa71814e86a35beeff41224a672b46bd6ba2854e2f4cfb79c1baff715dfd75e9`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 29 Aug 2023 18:41:03 GMT
COPY dir:6fcca547a5a58ffe09e9507247c1ba371889e20efec9c9e016fb6276715fb958 in / 
# Tue, 29 Aug 2023 18:41:04 GMT
CMD ["/bin/bash"]
# Tue, 29 Aug 2023 19:14:14 GMT
ARG version=20.0.2.9-1
# Tue, 29 Aug 2023 19:14:37 GMT
# ARGS: version=20.0.2.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 29 Aug 2023 19:14:39 GMT
ENV LANG=C.UTF-8
# Tue, 29 Aug 2023 19:14:39 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
# Fri, 18 Aug 2023 15:26:34 GMT
RUN yum install -y tar which gzip # TODO remove # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 18 Aug 2023 15:26:34 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
ARG MAVEN_VERSION=3.9.4
# Fri, 18 Aug 2023 15:26:34 GMT
ARG USER_HOME_DIR=/root
# Fri, 18 Aug 2023 15:26:34 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 18 Aug 2023 15:26:34 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 18 Aug 2023 15:26:34 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:aa4ff431ef8289088d3cf576f166a7c73e7a5dabe3fae46528dbdd9d7194e9e4`  
		Last Modified: Fri, 25 Aug 2023 18:25:09 GMT  
		Size: 64.1 MB (64129994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9f27765d71e08c53697fe290b73d787771c0c362584869885a2f8a3af13e49`  
		Last Modified: Tue, 29 Aug 2023 19:22:22 GMT  
		Size: 159.0 MB (158968137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b246f9376d8f5baccc947080c86cd9389b747aaabd8dcf0ef3ef1f4407afdde`  
		Last Modified: Tue, 29 Aug 2023 19:52:11 GMT  
		Size: 125.3 MB (125349908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629c2c4f72fe039655b8bafb4183934055058e6225e714795c6219c2f4f90ff3`  
		Last Modified: Tue, 29 Aug 2023 19:52:02 GMT  
		Size: 9.4 MB (9406425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0f11c4d4ea9ab572f24fe39c23e3cf124e84636ac375302ceb189c49b81d70`  
		Last Modified: Tue, 29 Aug 2023 19:52:01 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ef568a57b90811225f9e46da99bedd626e3273799c3543dddde648e415f462`  
		Last Modified: Tue, 29 Aug 2023 19:52:01 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82664f2fd882f2a26b316c8d5e4a9cf8436945714bf8b0de0d9942321a42f41`  
		Last Modified: Tue, 29 Aug 2023 19:52:01 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
