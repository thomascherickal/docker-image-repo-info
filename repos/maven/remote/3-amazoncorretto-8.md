## `maven:3-amazoncorretto-8`

```console
$ docker pull maven@sha256:c94a2ff041094c57ba73b17cdf6a2cbb5b87a65515afc8a332322cb665c7d45e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-8` - linux; amd64

```console
$ docker pull maven@sha256:970e77de7222a573e2db77f4e377edbc75b1922022b52e0e099d087d651bf921
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.4 MB (287449004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50f64ce179655593765b031a8d3d75e709d862fcc50e7e1d917eaf89e1b79b3`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 12 Oct 2023 22:38:11 GMT
COPY dir:bba3c324992ed0e5d34f0f5796fe9c0e46ced00dc01939b98cad3bc355594b38 in / 
# Thu, 12 Oct 2023 22:38:11 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 23:02:00 GMT
ARG version=1.8.0_382.b05-1
# Thu, 12 Oct 2023 23:02:34 GMT
# ARGS: version=1.8.0_382.b05-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 12 Oct 2023 23:02:35 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 23:02:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
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
	-	`sha256:2b92a4a464539d6c28ffd6b40875226086ace1e24d6598d771d8a65a6938acb1`  
		Last Modified: Fri, 29 Sep 2023 04:44:19 GMT  
		Size: 62.5 MB (62469645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24257d040582222853d6094dcc978441cf1520d7ac27c3d36abe44c7cb3fe33`  
		Last Modified: Thu, 12 Oct 2023 23:19:44 GMT  
		Size: 75.5 MB (75546949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d4632868435e07b5189dc3433041d228c4197524eba40724bb2c2c21d21bdd`  
		Last Modified: Fri, 13 Oct 2023 01:21:30 GMT  
		Size: 140.0 MB (140024604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05723eaff7008915e92db6fefe86950a5d67e2f3496f68bbd68cc821ed6ad846`  
		Last Modified: Fri, 13 Oct 2023 01:21:15 GMT  
		Size: 9.4 MB (9406423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac9c163157c7ec28d081bf3cf1424a502b0e92cbb323ea215e93870f3c7919c`  
		Last Modified: Fri, 13 Oct 2023 01:21:14 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cb14007eaf6d17a67e8078e22a650bac311f5ced6a64cb6441c0af70642a49`  
		Last Modified: Fri, 13 Oct 2023 01:21:14 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0225a14995050338a8dc01d07ea9e17674f1bf4fa4ed33140639e2d1c085f2a0`  
		Last Modified: Fri, 13 Oct 2023 01:21:14 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-8` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:9ee7f6150330bcaeaa86cfb72855306a5cd07a04f48ebb6ce423d12d24f2ad8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.4 MB (244391835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cd660e798fb5a17293d6a975df171e8ee8d2db7db28f056367564b8748699a1`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 12 Oct 2023 22:24:12 GMT
COPY dir:826b274d38ec470bf9beb46977486da92a3347aff5fcb970deb82f445fd7f20e in / 
# Thu, 12 Oct 2023 22:24:13 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 23:11:40 GMT
ARG version=1.8.0_382.b05-1
# Thu, 12 Oct 2023 23:12:05 GMT
# ARGS: version=1.8.0_382.b05-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 12 Oct 2023 23:12:06 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 23:12:06 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
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
	-	`sha256:d503fbdb054df5fe68cd13e3abb40a519885fcda4fbaf301b0667ae8c1285f4f`  
		Last Modified: Tue, 03 Oct 2023 00:59:41 GMT  
		Size: 64.2 MB (64163711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d7437ea8e14492f712a44b7637d4795d32ad72c614516e9556ac0a7a25379b`  
		Last Modified: Thu, 12 Oct 2023 23:24:55 GMT  
		Size: 59.6 MB (59602737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b64767dde38f48e99f3991b0cacdb1d878ad499e0e06f216d5b39d52af5ac9`  
		Last Modified: Fri, 13 Oct 2023 00:11:19 GMT  
		Size: 111.2 MB (111217584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58621512e1383149bd80c8e60d19998cb1393580ec90e5ceabd2e3f1ffa316a6`  
		Last Modified: Fri, 13 Oct 2023 00:11:09 GMT  
		Size: 9.4 MB (9406419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7ddd6286b4f9143d1499329812098dfc4c374347a1ed04f89a0ce6aa2bcfc4`  
		Last Modified: Fri, 13 Oct 2023 00:11:08 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab3b250b327c341c2510110f7409d148e3fb2681a6fbc6cc35b8e99241d65f1`  
		Last Modified: Fri, 13 Oct 2023 00:11:08 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe5f85c432609bcca2f0514764697697726b4ea67657f79aec57e8e7f68225e`  
		Last Modified: Fri, 13 Oct 2023 00:11:08 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
