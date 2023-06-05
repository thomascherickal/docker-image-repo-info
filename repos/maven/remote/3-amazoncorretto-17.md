## `maven:3-amazoncorretto-17`

```console
$ docker pull maven@sha256:1f59ac0df136eefd9ecb9ba962cdd685b16fd36ae47dab4cf5132e25d716e3d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-17` - linux; amd64

```console
$ docker pull maven@sha256:95fabd3c139ba947295076158e5160ffad5e34721907dbf8a8a18ff711d9f4a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **377.5 MB (377464599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec8afd95274ab41011d2f3edc56cfa4fa4c0b38b68c898df1ab876f0768fd2a3`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 05 Jun 2023 19:20:11 GMT
COPY dir:1ad47ba01d0d349e7e7d7ca6f7f5a60739b61c1a0bb68b6f66605d9af77bb0d5 in / 
# Mon, 05 Jun 2023 19:20:12 GMT
CMD ["/bin/bash"]
# Mon, 05 Jun 2023 19:40:20 GMT
ARG version=17.0.7.7-1
# Mon, 05 Jun 2023 19:40:45 GMT
# ARGS: version=17.0.7.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 05 Jun 2023 19:40:45 GMT
ENV LANG=C.UTF-8
# Mon, 05 Jun 2023 19:40:45 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
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
	-	`sha256:96d6f06d8d0033f5280e4c0edc2be832e831c176dd379cdb9a0988241c40de54`  
		Last Modified: Mon, 05 Jun 2023 19:46:05 GMT  
		Size: 152.0 MB (151974028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f59c4646ab851c3896b431f5e0c21ff788e8e3ec7bd120ab80074888db06072`  
		Last Modified: Mon, 05 Jun 2023 20:23:08 GMT  
		Size: 153.7 MB (153681685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae0cea391656ed993891f4c2ca78c51b6d24070b249b3868e7f8277d9805e44`  
		Last Modified: Mon, 05 Jun 2023 20:22:56 GMT  
		Size: 9.3 MB (9314415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782eba97544732644be29db147d08c00d7ee1286c3898a5905d5742749647ba6`  
		Last Modified: Mon, 05 Jun 2023 20:22:55 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd243f343ac72ab6d7f319002b25b426721be563902f4ca54b2e3f60e9120e5`  
		Last Modified: Mon, 05 Jun 2023 20:22:55 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648ef9544ff0283f97034b7854416c8d5d68e8d086327ad34cd7119fe504398c`  
		Last Modified: Mon, 05 Jun 2023 20:22:55 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-17` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:6f8ffbc5cae5c2132dcc428a6319e9a8ff592037bc60130a17129337c1e5d908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.5 MB (342537752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0eb89222483b3bb0e5a67cedea1b6acaf2469c44e092789afaf1831fabfbdf9`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 05 Jun 2023 19:39:49 GMT
COPY dir:dfd59a801cb05cf6d9b2d75085c49494763e9b18842c146030985cf41b66d3ca in / 
# Mon, 05 Jun 2023 19:39:50 GMT
CMD ["/bin/bash"]
# Mon, 05 Jun 2023 19:57:48 GMT
ARG version=17.0.7.7-1
# Mon, 05 Jun 2023 19:58:07 GMT
# ARGS: version=17.0.7.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 05 Jun 2023 19:58:09 GMT
ENV LANG=C.UTF-8
# Mon, 05 Jun 2023 19:58:09 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
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
	-	`sha256:7407f2d277af63b35a8012844db0206282e31f3e01a5bb98c7ff87b82a5ae7f4`  
		Last Modified: Mon, 05 Jun 2023 20:02:51 GMT  
		Size: 150.5 MB (150466239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eacc6c9ae6d96870125fc5bba641faa7a706ffeb220a95f18ac4ed5d98609548`  
		Last Modified: Mon, 05 Jun 2023 20:27:51 GMT  
		Size: 118.6 MB (118618928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b55623f54d5dc9092dd56596287744e83481507cc14b93c5886e5159f82c51d`  
		Last Modified: Mon, 05 Jun 2023 20:27:44 GMT  
		Size: 9.3 MB (9314408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e7ba196e25784c36beab9914219b0c2439e4a4cdad5b765eba1cc2fe8064c7`  
		Last Modified: Mon, 05 Jun 2023 20:27:43 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d5fcc6e7913b0945a8572df9d7bb455b39a8bbc2a4c4cc6122adf744dd82e2`  
		Last Modified: Mon, 05 Jun 2023 20:27:43 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8356531efb8c9c714dc2188c4895fcf01816b8b0a5035e3e2f13e582db6b4a2`  
		Last Modified: Mon, 05 Jun 2023 20:27:43 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
