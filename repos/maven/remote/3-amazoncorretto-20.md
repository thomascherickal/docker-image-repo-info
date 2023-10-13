## `maven:3-amazoncorretto-20`

```console
$ docker pull maven@sha256:bbf769add52a0e6c8787fcb19c61a76bbf8b7407a8bd63847ecda5c7e242119e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-20` - linux; amd64

```console
$ docker pull maven@sha256:27430f9660c791c1dde37e63bad54a01bf6b9c8d0756c9327e94cc860ee3ae67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **372.8 MB (372796776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f88789eb1cccf69628e39ab4fe051a76a2e6f9f8249218e72cdd83683f5b230`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 12 Oct 2023 22:38:11 GMT
COPY dir:bba3c324992ed0e5d34f0f5796fe9c0e46ced00dc01939b98cad3bc355594b38 in / 
# Thu, 12 Oct 2023 22:38:11 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 23:14:45 GMT
ARG version=20.0.2.10-1
# Thu, 12 Oct 2023 23:15:22 GMT
# ARGS: version=20.0.2.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 12 Oct 2023 23:15:22 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 23:15:22 GMT
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
	-	`sha256:2b92a4a464539d6c28ffd6b40875226086ace1e24d6598d771d8a65a6938acb1`  
		Last Modified: Fri, 29 Sep 2023 04:44:19 GMT  
		Size: 62.5 MB (62469645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e2ae33200141fd4607751bb457b645086a1410c32e8ed27a2e8817f64ecf5d`  
		Last Modified: Thu, 12 Oct 2023 23:26:59 GMT  
		Size: 160.9 MB (160908704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908e98521dfe2b6751da52212b97eb0733ddb5591b2d44ea0423df4218c6c0e4`  
		Last Modified: Fri, 13 Oct 2023 01:19:58 GMT  
		Size: 140.0 MB (140010617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a534b9fcd778d2b2c317d4eb6b8d7ff4f438eae14ee6eba19e8a486754fec5`  
		Last Modified: Fri, 13 Oct 2023 01:19:40 GMT  
		Size: 9.4 MB (9406423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e9d6c41850a7355b858f670b2c36d35b8bc1a42723cad9129e67ff68c109bd`  
		Last Modified: Fri, 13 Oct 2023 01:19:39 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0ab1664011a80f803a8efc5bd852e854c587df022389600f68e8c37c86a9c3`  
		Last Modified: Fri, 13 Oct 2023 01:19:39 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9219bc61d1db610ca713d87b0f88ee05476a5557f64bc8db3cd33871e54808e6`  
		Last Modified: Fri, 13 Oct 2023 01:19:39 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-20` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:dc11c08965c16db7babf76a58ae3acdda7e9b4909e33ca891adae26d518cbdf1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.8 MB (343756717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e357100af1bb7720bd5165cde682d1687e320f9e82daceff728fb2e6d8ae16f7`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 12 Oct 2023 22:24:12 GMT
COPY dir:826b274d38ec470bf9beb46977486da92a3347aff5fcb970deb82f445fd7f20e in / 
# Thu, 12 Oct 2023 22:24:13 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 23:20:21 GMT
ARG version=20.0.2.10-1
# Thu, 12 Oct 2023 23:20:49 GMT
# ARGS: version=20.0.2.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 12 Oct 2023 23:20:50 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 23:20:50 GMT
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
	-	`sha256:d503fbdb054df5fe68cd13e3abb40a519885fcda4fbaf301b0667ae8c1285f4f`  
		Last Modified: Tue, 03 Oct 2023 00:59:41 GMT  
		Size: 64.2 MB (64163711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c3acd8096f64e92105487b02b17b7295b82a30af65af6990439ef7043cea12`  
		Last Modified: Thu, 12 Oct 2023 23:31:07 GMT  
		Size: 159.0 MB (158967578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee07ff9a8fd80018bf4c6be8ba5fd1409ed7171876df74da2121a84b7d27907`  
		Last Modified: Fri, 13 Oct 2023 00:09:58 GMT  
		Size: 111.2 MB (111217624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d487aefa3649f07d45de316e3fa5ae5ba136a786344fade879a9cbfbbef372`  
		Last Modified: Fri, 13 Oct 2023 00:09:47 GMT  
		Size: 9.4 MB (9406420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bedce1d8dac1d3a830e130648143d97e3b3d83a7371dd3bc2d7485faeb54b9`  
		Last Modified: Fri, 13 Oct 2023 00:09:46 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef74eb99f5b85b0e88a23a2f5b803088f54a307dba1328db23ed28a8e5b08777`  
		Last Modified: Fri, 13 Oct 2023 00:09:46 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f1aaaa1f42b41acc1d6216ce7a78d8577224a8d071ca7c1a54dfd6ff3383a0`  
		Last Modified: Fri, 13 Oct 2023 00:09:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
