## `maven:3-amazoncorretto-21`

```console
$ docker pull maven@sha256:02f2c8d1d68d5a4bc45dee0778c06cf82faf345bd96f084f7b1b417b9578700e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-21` - linux; amd64

```console
$ docker pull maven@sha256:e2c6854d4944eb0b97594a5a00191c61e92b859cd1080d8660ce205cb14287d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **376.2 MB (376214804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ce199e70ea86dbd20fa0dfb45dacd9a559e0da4174d56afaae7d0149f13a0f`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 29 Aug 2023 18:29:22 GMT
COPY dir:591ada5c2fb65633b614a3ff732e6d83dcd91fe9ae925844fe9ba3323311bf74 in / 
# Tue, 29 Aug 2023 18:29:23 GMT
CMD ["/bin/bash"]
# Fri, 22 Sep 2023 00:21:15 GMT
ARG version=21.0.0.35-1
# Fri, 22 Sep 2023 00:21:52 GMT
# ARGS: version=21.0.0.35-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-21-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-21-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 22 Sep 2023 00:21:53 GMT
ENV LANG=C.UTF-8
# Fri, 22 Sep 2023 00:21:53 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
# Fri, 22 Sep 2023 09:11:50 GMT
RUN yum install -y tar which gzip # TODO remove # buildkit
# Fri, 22 Sep 2023 09:11:50 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 22 Sep 2023 09:11:50 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Fri, 22 Sep 2023 09:11:50 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Fri, 22 Sep 2023 09:11:50 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Fri, 22 Sep 2023 09:11:50 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Fri, 22 Sep 2023 09:11:50 GMT
ARG MAVEN_VERSION=3.9.4
# Fri, 22 Sep 2023 09:11:50 GMT
ARG USER_HOME_DIR=/root
# Fri, 22 Sep 2023 09:11:50 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 22 Sep 2023 09:11:50 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 22 Sep 2023 09:11:50 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:8be3d01330d7e2e197495d440aa60d14ac366aad5e8d105d86e384876aefec18`  
		Last Modified: Fri, 25 Aug 2023 08:53:43 GMT  
		Size: 62.5 MB (62477278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431d68e139e72b927b43c4d934ed4d14137aead2ddddfb7a1e713391aa90a0cf`  
		Last Modified: Fri, 22 Sep 2023 00:26:52 GMT  
		Size: 165.4 MB (165433736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb119251e7ac3b5dfc69016d0d066425372b032b35001f7a130bffc2bcc72fef`  
		Last Modified: Fri, 22 Sep 2023 19:24:16 GMT  
		Size: 138.9 MB (138895992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3166abe53b87004d22dd6f6fde70526e30b181ec03ffc5a9331a631ace327086`  
		Last Modified: Fri, 22 Sep 2023 19:24:00 GMT  
		Size: 9.4 MB (9406411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41bb2c3dc2923871f0d8bc3bc2bb884466df1f81169040e57deca7e8e1a78b6`  
		Last Modified: Fri, 22 Sep 2023 19:23:59 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1382eda787f19158bbe7eaf890fd2539ec13b8cbedf89958531b0119fae922c1`  
		Last Modified: Fri, 22 Sep 2023 19:23:59 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0671b5b62ddcb44177a08a074eba625a240af5f84a21f091fa8e70f2c1cbb8a4`  
		Last Modified: Fri, 22 Sep 2023 19:23:59 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-21` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:4cdd1e6c19e8c00d7231263ac88ab8d264dfbccf3170bf5008a130e0855050f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.1 MB (347130335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9269c590b07b2d1af63ddb299aaf074b5ebfe0c11eab0c53240a6bf848ea93b9`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 29 Aug 2023 18:41:03 GMT
COPY dir:6fcca547a5a58ffe09e9507247c1ba371889e20efec9c9e016fb6276715fb958 in / 
# Tue, 29 Aug 2023 18:41:04 GMT
CMD ["/bin/bash"]
# Fri, 22 Sep 2023 00:41:55 GMT
ARG version=21.0.0.35-1
# Fri, 22 Sep 2023 00:42:25 GMT
# ARGS: version=21.0.0.35-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-21-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-21-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 22 Sep 2023 00:42:26 GMT
ENV LANG=C.UTF-8
# Fri, 22 Sep 2023 00:42:26 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
# Fri, 22 Sep 2023 09:11:50 GMT
RUN yum install -y tar which gzip # TODO remove # buildkit
# Fri, 22 Sep 2023 09:11:50 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 22 Sep 2023 09:11:50 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Fri, 22 Sep 2023 09:11:50 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Fri, 22 Sep 2023 09:11:50 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Fri, 22 Sep 2023 09:11:50 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Fri, 22 Sep 2023 09:11:50 GMT
ARG MAVEN_VERSION=3.9.4
# Fri, 22 Sep 2023 09:11:50 GMT
ARG USER_HOME_DIR=/root
# Fri, 22 Sep 2023 09:11:50 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 22 Sep 2023 09:11:50 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 22 Sep 2023 09:11:50 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:aa4ff431ef8289088d3cf576f166a7c73e7a5dabe3fae46528dbdd9d7194e9e4`  
		Last Modified: Fri, 25 Aug 2023 18:25:09 GMT  
		Size: 64.1 MB (64129994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767eee88b4ae7a157734359dc319f9c169d69214a709f5a6f261e10541616792`  
		Last Modified: Fri, 22 Sep 2023 00:46:34 GMT  
		Size: 163.4 MB (163426396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c7c1de0893ce1d57d1a31fbbdc3e7ad390d6b31fbbacec49fbd7f32410a579`  
		Last Modified: Fri, 22 Sep 2023 19:42:36 GMT  
		Size: 110.2 MB (110166147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45caa157ad413ebba6a011c419ff61840314516f3ac49b7ed554dff69e9b5514`  
		Last Modified: Fri, 22 Sep 2023 19:42:25 GMT  
		Size: 9.4 MB (9406410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadbc9417391889d247a3f73c5c6b14ef502343e847ab588760a1538bfc1b96b`  
		Last Modified: Fri, 22 Sep 2023 19:42:25 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cc67d00c09e62ea9b4bba019cd0d7319eed53ff0219a7cb4a21ffcb6b570bb`  
		Last Modified: Fri, 22 Sep 2023 19:42:24 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af07d9bcdbd50b08ca11e6ef986a2ef1cb3352b005e5eee0d263b20266c156b`  
		Last Modified: Fri, 22 Sep 2023 19:42:25 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
