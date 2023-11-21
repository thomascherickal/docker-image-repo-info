## `maven:3-amazoncorretto-17`

```console
$ docker pull maven@sha256:71ed4a3650bf3fdb27fe24dea4e37bf33b02f683aa32a6ab255996827007a1eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-17` - linux; amd64

```console
$ docker pull maven@sha256:7700ba227569a8685dfacf72969b8af18b9168d9f99697e8283460c0c2a9b103
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.7 MB (367684655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f78a073a46cb594a37040b3115e68db8f1aaed4962ef99e68dba881989ee48bb`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 21 Nov 2023 03:21:54 GMT
COPY dir:ddf8ce4c235ebf92718d40c0041035b283a61cbd94b49610e57999ebc78d3ec6 in / 
# Tue, 21 Nov 2023 03:21:55 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 04:19:06 GMT
ARG version=17.0.9.8-1
# Tue, 21 Nov 2023 04:19:30 GMT
# ARGS: version=17.0.9.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 21 Nov 2023 04:19:31 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 04:19:31 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Thu, 19 Oct 2023 09:04:18 GMT
RUN yum install -y tar which gzip # TODO remove # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 19 Oct 2023 09:04:18 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
ARG MAVEN_VERSION=3.9.5
# Thu, 19 Oct 2023 09:04:18 GMT
ARG USER_HOME_DIR=/root
# Thu, 19 Oct 2023 09:04:18 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 19 Oct 2023 09:04:18 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 19 Oct 2023 09:04:18 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:0b4a6f011995244a95bff79a1298e83d230bc0aa22871a9c510745cafebec227`  
		Last Modified: Sun, 19 Nov 2023 03:18:53 GMT  
		Size: 62.6 MB (62641917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274aefe2866ac25d07f65db25903ae25536d5f231eeb28ddd6df3aaed855857c`  
		Last Modified: Tue, 21 Nov 2023 04:30:06 GMT  
		Size: 151.9 MB (151939996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71efc903c7b5986cfa793ca596db4f1415cd397b010f1753064bf478c8277340`  
		Last Modified: Tue, 21 Nov 2023 05:18:59 GMT  
		Size: 143.7 MB (143671858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ab0774fbfaff1d2289962b47976ce055c1e5113984b7b877d73bbe590754f9`  
		Last Modified: Tue, 21 Nov 2023 05:18:47 GMT  
		Size: 9.4 MB (9429503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06ff6118ec47d2bab0ddaa38044b7a972fb34478c1fcbd5fdba2497a8cc1cf7`  
		Last Modified: Tue, 21 Nov 2023 05:18:46 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ffb8fd6bbe7207a7aaeba4c89a25e25ea1188bd0c9b074e1c90476c1f18e26`  
		Last Modified: Tue, 21 Nov 2023 05:18:46 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ca04ac52bd83d65e971327c1a4b5fa070122e930f905ff8302f02c5885586e`  
		Last Modified: Tue, 21 Nov 2023 05:18:46 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-17` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:568b1ef7097daf1f0911ee8a1b855d5b1f8b3ae587d6a9535b077ee060ade0d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.2 MB (339209818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36c880478b9dc8ddb760f1df8d02c8b216fdbb1dd41b166c40a454e37c20bcb7`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 21 Nov 2023 03:39:49 GMT
COPY dir:21fc61c0ea1d6a14f556bdbd5029389644807e82a8de54f60438fc773e3e2465 in / 
# Tue, 21 Nov 2023 03:39:51 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 05:11:17 GMT
ARG version=17.0.9.8-1
# Tue, 21 Nov 2023 05:11:36 GMT
# ARGS: version=17.0.9.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 21 Nov 2023 05:11:37 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 05:11:37 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Thu, 19 Oct 2023 09:04:18 GMT
RUN yum install -y tar which gzip # TODO remove # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 19 Oct 2023 09:04:18 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
ARG MAVEN_VERSION=3.9.5
# Thu, 19 Oct 2023 09:04:18 GMT
ARG USER_HOME_DIR=/root
# Thu, 19 Oct 2023 09:04:18 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 19 Oct 2023 09:04:18 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 19 Oct 2023 09:04:18 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:ae50e077554aa1fe734206cc35e32dc0b0389a0ff7aa8d08626157b225100b42`  
		Last Modified: Mon, 20 Nov 2023 21:52:59 GMT  
		Size: 64.4 MB (64424056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cce207248d489b7100cfc209edcd8e95ff9abcb8746e2784278c9d8269fe87`  
		Last Modified: Tue, 21 Nov 2023 05:20:41 GMT  
		Size: 150.5 MB (150523972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772f6767e0d94d085c9ee021aa7e976340c12c19d1ab0cd85442c587667a3cb1`  
		Last Modified: Tue, 21 Nov 2023 06:01:06 GMT  
		Size: 114.8 MB (114830908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf1d4fa03bd84d54b30513c12edddb7d5c9928918aa2301cfef721a8444330a`  
		Last Modified: Tue, 21 Nov 2023 06:00:58 GMT  
		Size: 9.4 MB (9429503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d92d9a6cd678793289e3e94e141f0d132c647ea6c762f98ce16702d7b45c4a`  
		Last Modified: Tue, 21 Nov 2023 06:00:57 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36f54cc104db62a696e3705462176e4d67fc21eb554518ee14f0256fb03f16c`  
		Last Modified: Tue, 21 Nov 2023 06:00:57 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36993832f46e44e687764de130ff071cfd70028c92cf9f6a179da637e4b38696`  
		Last Modified: Tue, 21 Nov 2023 06:00:57 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
