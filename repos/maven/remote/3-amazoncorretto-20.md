## `maven:3-amazoncorretto-20`

```console
$ docker pull maven@sha256:b23cead0cf2d6a929848b7a5d0d36cce0fba4587220d0a01d8dc2cfef18d95b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-20` - linux; amd64

```console
$ docker pull maven@sha256:8ca4ff6e2f22cb298693de1fa4af2e6d7fe742885e7e29519d6f03590ec3c20d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.6 MB (386629331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0dec079acef81af7fe4bbd853a2e606d9fcb52888319bd0c03b59d24711cf1b`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 20 Jun 2023 22:20:15 GMT
COPY dir:129c77392b447afbaa234a34f434bed5ec790278efd165e1d59d4425216de49b in / 
# Tue, 20 Jun 2023 22:20:16 GMT
CMD ["/bin/bash"]
# Tue, 20 Jun 2023 22:57:14 GMT
ARG version=20.0.1.9-1
# Tue, 20 Jun 2023 22:57:37 GMT
# ARGS: version=20.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Jun 2023 22:57:38 GMT
ENV LANG=C.UTF-8
# Tue, 20 Jun 2023 22:57:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
# Mon, 26 Jun 2023 13:48:06 GMT
RUN yum install -y tar which gzip # TODO remove # buildkit
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
	-	`sha256:0086aac11276884f299f6c13a98f93369cc50f7c0518989c2d4a29dd999feb70`  
		Last Modified: Fri, 16 Jun 2023 00:07:41 GMT  
		Size: 62.5 MB (62487611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a67431843d9e5854a588042bb3ab1dea757eb095a929ea60bef489fc4f13e9`  
		Last Modified: Tue, 20 Jun 2023 23:03:25 GMT  
		Size: 160.8 MB (160763226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b564b4dd7dc6d7da9b62aa718be45e90bde32c37bc24131b7dd89148629d40c`  
		Last Modified: Tue, 20 Jun 2023 23:40:43 GMT  
		Size: 154.0 MB (154049544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb17807de1b89c3f855d163ffbb960b0eece2ad7e327ef1356d615cfacbac623`  
		Last Modified: Tue, 27 Jun 2023 01:18:41 GMT  
		Size: 9.3 MB (9327576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f604dc58e450290de42beb98b62d6999db751baa877f0396c1161e90bddbf3`  
		Last Modified: Tue, 27 Jun 2023 01:18:41 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0847b3c4a0d0feecea867f43d6cc25c6e6b2405a3b38ff8010c08759b95cb5af`  
		Last Modified: Tue, 27 Jun 2023 01:18:41 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d3e65f8cc15fb80f2da180fb49f8c8a79f0655c619dcfcaf8e2bb1cf92bf1a`  
		Last Modified: Tue, 27 Jun 2023 01:18:41 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-20` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:0811b6f3ee46115c0d20c45e51cfc27a459a9ab4ac98f4dc3041856bb21ca730
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.2 MB (353248665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95f8c53d6250e8fa6d508833e5462510121858701cc54b035de525f3a45ab5a6`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 13 Jul 2023 00:40:00 GMT
COPY dir:a284fdf4a484ebc9131c665fc151094ec73265d07d353476272944e301722064 in / 
# Thu, 13 Jul 2023 00:40:01 GMT
CMD ["/bin/bash"]
# Thu, 13 Jul 2023 01:11:08 GMT
ARG version=20.0.1.9-1
# Thu, 13 Jul 2023 01:11:27 GMT
# ARGS: version=20.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 13 Jul 2023 01:11:29 GMT
ENV LANG=C.UTF-8
# Thu, 13 Jul 2023 01:11:29 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
# Mon, 26 Jun 2023 13:48:06 GMT
RUN yum install -y tar which gzip # TODO remove # buildkit
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
	-	`sha256:20c8bca6ae5daad56b485a4b6f1f395a51727d69eb6a7566c53b00a366e46576`  
		Last Modified: Fri, 30 Jun 2023 17:38:06 GMT  
		Size: 64.1 MB (64128925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2fe269925b1fc2448bd27586fd47ded5d1d6a0ab53705a653dbe68cde80b7b`  
		Last Modified: Thu, 13 Jul 2023 01:18:38 GMT  
		Size: 158.8 MB (158799437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aedd55124d279d4fcc596f14af8051b3315e879419a0310ac85a8bc552b71cb`  
		Last Modified: Thu, 13 Jul 2023 01:37:09 GMT  
		Size: 121.0 MB (120991321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd4198e5eb8594d97541a7522c4376d020ae33dbe0e12a6832923a60d5bcedd`  
		Last Modified: Thu, 13 Jul 2023 01:37:01 GMT  
		Size: 9.3 MB (9327599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc2d58f07cd986ba5545e3774af95741779e79da3c185e923ac6684feb607a5`  
		Last Modified: Thu, 13 Jul 2023 01:37:00 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18812365a1b56cf87fe608e895f1cf19325ae15001b3001398f232272528d0b`  
		Last Modified: Thu, 13 Jul 2023 01:37:00 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2924adf9d870a0835ab1fdf02ead30993691975959d993e56d771df3d7438ba3`  
		Last Modified: Thu, 13 Jul 2023 01:37:00 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
