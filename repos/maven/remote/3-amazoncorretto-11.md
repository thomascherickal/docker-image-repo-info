## `maven:3-amazoncorretto-11`

```console
$ docker pull maven@sha256:e57216b115d21e46051298ad099c7aec3d27afd522ae527004a28fdd19a52dc5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-11` - linux; amd64

```console
$ docker pull maven@sha256:d620ac440ee3eae38363904962ccea0fa62132e46568ee48802f586f83d4bccb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **373.3 MB (373275164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce4534679afa7381c1ac42e16fb8db84b98acb993728215f08dc77710df04061`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 05 Jun 2023 19:20:11 GMT
COPY dir:1ad47ba01d0d349e7e7d7ca6f7f5a60739b61c1a0bb68b6f66605d9af77bb0d5 in / 
# Mon, 05 Jun 2023 19:20:12 GMT
CMD ["/bin/bash"]
# Mon, 05 Jun 2023 19:38:45 GMT
ARG version=11.0.19.7-1
# Mon, 05 Jun 2023 19:39:09 GMT
# ARGS: version=11.0.19.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 05 Jun 2023 19:39:09 GMT
ENV LANG=C.UTF-8
# Mon, 05 Jun 2023 19:39:09 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
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
	-	`sha256:2c50f034a7615b7e455c5e96fb926a1fb1b617715a462b30026aefdaec47c1e2`  
		Last Modified: Mon, 05 Jun 2023 19:44:39 GMT  
		Size: 147.8 MB (147786516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913bbc6ab04717e8d4b7dec6668c40fbdb85ee362f1edfc1ef78086b1ec23315`  
		Last Modified: Mon, 05 Jun 2023 20:22:36 GMT  
		Size: 153.7 MB (153679762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06fcc9faac92d9c6fa379ffc0d6d3bdccffb81119a31354e7cd59bb01d224b6`  
		Last Modified: Mon, 05 Jun 2023 20:22:24 GMT  
		Size: 9.3 MB (9314416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89254532a186f16cae18140c0c21bde1e1df77ad58b36a62d809dbab996a7193`  
		Last Modified: Mon, 05 Jun 2023 20:22:23 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780eeaba6a66dd10c48b4bd2fa9d35320483cd3eb366b7515f40ace3d1fed928`  
		Last Modified: Mon, 05 Jun 2023 20:22:23 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6471b472514cb18e2cf2983bb2ae05e2d3f44d88c621eb06f8b1db50ff1c1fd3`  
		Last Modified: Mon, 05 Jun 2023 20:22:23 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-11` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:dbb0449000e064b76f467c3f84f1cb8c2dff3494d04f8fbb544815057a1c35ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.0 MB (337030024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfaf69d366a494a1201669f4bdc92f3d3e9b88aabfa5240f2f17da5a347613bf`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 05 Jun 2023 19:39:49 GMT
COPY dir:dfd59a801cb05cf6d9b2d75085c49494763e9b18842c146030985cf41b66d3ca in / 
# Mon, 05 Jun 2023 19:39:50 GMT
CMD ["/bin/bash"]
# Mon, 05 Jun 2023 19:56:24 GMT
ARG version=11.0.19.7-1
# Mon, 05 Jun 2023 19:56:41 GMT
# ARGS: version=11.0.19.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 05 Jun 2023 19:56:43 GMT
ENV LANG=C.UTF-8
# Mon, 05 Jun 2023 19:56:43 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
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
	-	`sha256:53682602592d23518d45524dc16934c20954cac375350ac17476144e2c789c0a`  
		Last Modified: Mon, 05 Jun 2023 20:01:28 GMT  
		Size: 144.9 MB (144939840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33ebd25cc415a256d1551fcba5468c81bd194e08a0b9dea37bb4ea64b2805a8`  
		Last Modified: Mon, 05 Jun 2023 20:27:23 GMT  
		Size: 118.6 MB (118637607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14d52f8d6f890d120ff375c4f1f2fdf487b1d482f8cc0ca1dc7c0d8b181df8c`  
		Last Modified: Mon, 05 Jun 2023 20:27:15 GMT  
		Size: 9.3 MB (9314401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a97b9647427b87a0f84e89e9593381357c572dcd51ccd615b4cf458e4dbc78`  
		Last Modified: Mon, 05 Jun 2023 20:27:15 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c32d85ed7791e863eeba992b32503b1ea93145cc7dd273d0532f8afef4ed75`  
		Last Modified: Mon, 05 Jun 2023 20:27:15 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba94b7ee3003b1de6caec8301e196f4b18557ddfe64708818aeae35c968c18d`  
		Last Modified: Mon, 05 Jun 2023 20:27:15 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
