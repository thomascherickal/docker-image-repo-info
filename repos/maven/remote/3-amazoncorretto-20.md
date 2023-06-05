## `maven:3-amazoncorretto-20`

```console
$ docker pull maven@sha256:f1051587148b3a6e64e3e9ac65b89c42cb9c62601e554dc6ea810baa29337992
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-20` - linux; amd64

```console
$ docker pull maven@sha256:227b782b4145d4375c1891497fd69cb083d6e9317f63bdcb6ff62e94bb2100a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.3 MB (386257921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21de0d8210ba42c065f8df1987f0cc96752fcb89b6140516255940570bcace6f`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 05 Jun 2023 19:20:11 GMT
COPY dir:1ad47ba01d0d349e7e7d7ca6f7f5a60739b61c1a0bb68b6f66605d9af77bb0d5 in / 
# Mon, 05 Jun 2023 19:20:12 GMT
CMD ["/bin/bash"]
# Mon, 05 Jun 2023 19:41:56 GMT
ARG version=20.0.1.9-1
# Mon, 05 Jun 2023 19:42:19 GMT
# ARGS: version=20.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 05 Jun 2023 19:42:20 GMT
ENV LANG=C.UTF-8
# Mon, 05 Jun 2023 19:42:20 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
# Tue, 16 May 2023 11:35:55 GMT
RUN yum install -y tar which gzip # TODO remove # buildkit
# Tue, 16 May 2023 11:35:55 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 16 May 2023 11:35:55 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Tue, 16 May 2023 11:35:55 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Tue, 16 May 2023 11:35:55 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Tue, 16 May 2023 11:35:55 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Tue, 16 May 2023 11:35:55 GMT
ARG MAVEN_VERSION=3.9.2
# Tue, 16 May 2023 11:35:55 GMT
ARG USER_HOME_DIR=/root
# Tue, 16 May 2023 11:35:55 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 16 May 2023 11:35:55 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 16 May 2023 11:35:55 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:a168ccb1c126cd9267eedd2686bc6d0e5415b7fe1009cd832c78ba00655a34d9`  
		Last Modified: Wed, 24 May 2023 21:22:43 GMT  
		Size: 62.5 MB (62493087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f50472d35bcaf1dac70c662dbd806d8ddd2cd1ce134dfcef4c0139613607e13`  
		Last Modified: Mon, 05 Jun 2023 19:47:37 GMT  
		Size: 160.8 MB (160763489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbcf6289222c0ffe4d7a238f777f53854d5d0a75e424953dd73d9403fa70074c`  
		Last Modified: Mon, 05 Jun 2023 20:23:31 GMT  
		Size: 153.7 MB (153685544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1deb9fdb851370cc1b7651c53aebe6b2bfd5cb764c336e01fb0a79b836865ca`  
		Last Modified: Mon, 05 Jun 2023 20:23:20 GMT  
		Size: 9.3 MB (9314416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454ce54e8fee779ef879d4b23201880002010624a508b5dbfe0ede6fd0c7915d`  
		Last Modified: Mon, 05 Jun 2023 20:23:19 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea47225ccc3ce599e9167647306ececd22141fcb158eed2b09daabfab4ba09d`  
		Last Modified: Mon, 05 Jun 2023 20:23:19 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fabdd6cee5a032bd67f065404bc4ba71640dfefd24d827f2d293def47828cea`  
		Last Modified: Mon, 05 Jun 2023 20:23:19 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-20` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:9992b389def5fac2a58ef3e2c67da0ccecbd8bf391cdd17850111113a30260f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.9 MB (350851829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b98f1381ba34878d530285266e3abeb96afb1a28bfae019fc1361132e6f9d7`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 05 Jun 2023 19:39:49 GMT
COPY dir:dfd59a801cb05cf6d9b2d75085c49494763e9b18842c146030985cf41b66d3ca in / 
# Mon, 05 Jun 2023 19:39:50 GMT
CMD ["/bin/bash"]
# Mon, 05 Jun 2023 19:59:09 GMT
ARG version=20.0.1.9-1
# Mon, 05 Jun 2023 19:59:29 GMT
# ARGS: version=20.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 05 Jun 2023 19:59:31 GMT
ENV LANG=C.UTF-8
# Mon, 05 Jun 2023 19:59:31 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
# Tue, 16 May 2023 11:35:55 GMT
RUN yum install -y tar which gzip # TODO remove # buildkit
# Tue, 16 May 2023 11:35:55 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 16 May 2023 11:35:55 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Tue, 16 May 2023 11:35:55 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Tue, 16 May 2023 11:35:55 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Tue, 16 May 2023 11:35:55 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Tue, 16 May 2023 11:35:55 GMT
ARG MAVEN_VERSION=3.9.2
# Tue, 16 May 2023 11:35:55 GMT
ARG USER_HOME_DIR=/root
# Tue, 16 May 2023 11:35:55 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 16 May 2023 11:35:55 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 16 May 2023 11:35:55 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:d916dc829437e3254e7c7e665dd90678298358e7fb563161caa849ca46390827`  
		Last Modified: Wed, 24 May 2023 23:14:13 GMT  
		Size: 64.1 MB (64136791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba14e8e7588270a2605d46eb72f5f563cb7ad6f124b2183030b978070a57b6b`  
		Last Modified: Mon, 05 Jun 2023 20:04:20 GMT  
		Size: 158.8 MB (158779965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d23d2cf44f57a1e08b52c2bd50ca4f3c27612ab5e8d3ddf27465914efc9728`  
		Last Modified: Mon, 05 Jun 2023 20:28:12 GMT  
		Size: 118.6 MB (118619286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0e6beb81b67fc423a6c25e51893d6aa62f5b84ed66427daf8c6939cfe03d0`  
		Last Modified: Mon, 05 Jun 2023 20:28:04 GMT  
		Size: 9.3 MB (9314401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7da23be8e40545e0a24cbbce3e43121f41e378c9f0725adb61ca05da0296988`  
		Last Modified: Mon, 05 Jun 2023 20:28:03 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2202ce7bae41361442fdc1e03584f75b8a498337dd191392b2a62a3b004551`  
		Last Modified: Mon, 05 Jun 2023 20:28:03 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c401b34722c8406f3ae4d26aa9a0b698012ad4338a40806885dd8f7bd1d49059`  
		Last Modified: Mon, 05 Jun 2023 20:28:03 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
