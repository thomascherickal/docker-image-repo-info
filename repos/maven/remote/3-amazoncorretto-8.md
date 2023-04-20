## `maven:3-amazoncorretto-8`

```console
$ docker pull maven@sha256:295e3349ad44bbef687842e3a8fc45647151e2eb8a854d618b329d2430fa1a71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-8` - linux; amd64

```console
$ docker pull maven@sha256:dd2fa03e55648ac08b37fbdfe23d70f4c52a4785121075ba74e4d552236e5aaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.9 MB (296856275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ed69d280604f4c1df92a6176203a43485a24b0edf22450edd8b505118001592`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 28 Mar 2023 18:20:51 GMT
COPY dir:d74df4759bcd6e2619baa3ec354d8703c77c836345c6a887554df76aaf1d9965 in / 
# Tue, 28 Mar 2023 18:20:52 GMT
CMD ["/bin/bash"]
# Thu, 20 Apr 2023 18:19:26 GMT
ARG version=1.8.0_372.b07-1
# Thu, 20 Apr 2023 18:19:47 GMT
# ARGS: version=1.8.0_372.b07-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 20 Apr 2023 18:19:48 GMT
ENV LANG=C.UTF-8
# Thu, 20 Apr 2023 18:19:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Thu, 20 Apr 2023 18:19:48 GMT
RUN yum install -y tar which gzip # TODO remove # buildkit
# Thu, 20 Apr 2023 18:19:48 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 20 Apr 2023 18:19:48 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Thu, 20 Apr 2023 18:19:48 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Thu, 20 Apr 2023 18:19:48 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Thu, 20 Apr 2023 18:19:48 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Thu, 20 Apr 2023 18:19:48 GMT
ARG MAVEN_VERSION=3.9.1
# Thu, 20 Apr 2023 18:19:48 GMT
ARG USER_HOME_DIR=/root
# Thu, 20 Apr 2023 18:19:48 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 20 Apr 2023 18:19:48 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 20 Apr 2023 18:19:48 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:128d54f2c9b134270b406c5f3a41296da7c1111d3a6927f0b4451131d636151e`  
		Last Modified: Thu, 23 Mar 2023 21:24:22 GMT  
		Size: 62.5 MB (62483466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6563691f44a1cfe5035253e7444c30366ce8d028d246929660d109373967461`  
		Last Modified: Thu, 20 Apr 2023 18:27:49 GMT  
		Size: 75.5 MB (75534467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479e22fcd867c51a0f670a84bf2f14f0c5037f936d52e0c1a4e21f7d7063c81b`  
		Last Modified: Thu, 20 Apr 2023 19:10:41 GMT  
		Size: 149.7 MB (149730798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe9965d96229c1a5bdef714afa7701dfcebe4260a6f9d24bb06944e4c816ecc`  
		Last Modified: Thu, 20 Apr 2023 19:10:30 GMT  
		Size: 9.1 MB (9106157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e901cc046697d2006534aaa3eed8ec21f4321b2054fb37e25707a497839cc452`  
		Last Modified: Thu, 20 Apr 2023 19:10:29 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893afd4a35982c550991e09d57d3429583cea65ebe23068f71e6090523d4a021`  
		Last Modified: Thu, 20 Apr 2023 19:10:29 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7a13b8cba11e0d7946e2e1fd2d567a81f54f342a343a19236a1ac0eeaaed6c`  
		Last Modified: Thu, 20 Apr 2023 19:10:29 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-8` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:bdba5c6a9e266c1a04198ed1de7313687d772ebb60790a152c20a7581ff47b7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.6 MB (247638918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48dd5e766aee3c957011c888880e03a07f324fd1544d3e6595bbc561c486d554`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 28 Mar 2023 18:40:10 GMT
COPY dir:1d0df99dbb2a961dca382ec30c27f40e06635a9186a0715c0d2a629262a04288 in / 
# Tue, 28 Mar 2023 18:40:10 GMT
CMD ["/bin/bash"]
# Thu, 20 Apr 2023 17:39:19 GMT
ARG version=1.8.0_372.b07-1
# Thu, 20 Apr 2023 17:39:36 GMT
# ARGS: version=1.8.0_372.b07-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 20 Apr 2023 17:39:37 GMT
ENV LANG=C.UTF-8
# Thu, 20 Apr 2023 17:39:37 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Thu, 20 Apr 2023 17:39:37 GMT
RUN yum install -y tar which gzip # TODO remove # buildkit
# Thu, 20 Apr 2023 17:39:37 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 20 Apr 2023 17:39:37 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Thu, 20 Apr 2023 17:39:37 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Thu, 20 Apr 2023 17:39:37 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Thu, 20 Apr 2023 17:39:37 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Thu, 20 Apr 2023 17:39:37 GMT
ARG MAVEN_VERSION=3.9.1
# Thu, 20 Apr 2023 17:39:37 GMT
ARG USER_HOME_DIR=/root
# Thu, 20 Apr 2023 17:39:37 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 20 Apr 2023 17:39:37 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 20 Apr 2023 17:39:37 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:949542da27c3c0ab979766d37f455344960f838d9f661b9db50bec634ca7149e`  
		Last Modified: Thu, 23 Mar 2023 21:25:53 GMT  
		Size: 64.1 MB (64126936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bda22e97c92633e6535dcd517c99f22c531f8084065805a3176f201f73bcd5`  
		Last Modified: Thu, 20 Apr 2023 17:47:00 GMT  
		Size: 59.6 MB (59578131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052782fedc4ad82ecacaf24e99adad64542efe702c8c1af9c097b438254ff796`  
		Last Modified: Thu, 20 Apr 2023 18:21:56 GMT  
		Size: 114.8 MB (114826325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86eb64bd84ae581006700245bad5189e9b517f391f2a51b36829dce51ec9567f`  
		Last Modified: Thu, 20 Apr 2023 18:21:48 GMT  
		Size: 9.1 MB (9106144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f549517263c056f26094dbf767fe6b6f324ebf677d694a8ab46b3c25055055`  
		Last Modified: Thu, 20 Apr 2023 18:21:48 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86de062c157904c42901d6265769bd8ded00e1c101219eb4d094a48fd72d534`  
		Last Modified: Thu, 20 Apr 2023 18:21:48 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d789ae5595ac58c59b7aa968ea86d044f636be2ef908043c977a2f45ac977a75`  
		Last Modified: Thu, 20 Apr 2023 18:21:48 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
