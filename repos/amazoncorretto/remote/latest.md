## `amazoncorretto:latest`

```console
$ docker pull amazoncorretto@sha256:b4852702fd7f91da54c9ab1ae0784ebfd3d20158e4ea7b7dc492a6bf84689aa1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:latest` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:d800cfa1208c70c3a1c81d6072b7b881b157620879aafef085235493599ef973
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (138041643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:401e277a9982b0d7caf3283be5eef964f87f16e004dababa3637a3faa8d47a2e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Mar 2023 18:20:51 GMT
COPY dir:d74df4759bcd6e2619baa3ec354d8703c77c836345c6a887554df76aaf1d9965 in / 
# Tue, 28 Mar 2023 18:20:52 GMT
CMD ["/bin/bash"]
# Tue, 28 Mar 2023 19:09:02 GMT
ARG version=1.8.0_362.b08-1
# Tue, 28 Mar 2023 19:09:23 GMT
# ARGS: version=1.8.0_362.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 28 Mar 2023 19:09:23 GMT
ENV LANG=C.UTF-8
# Tue, 28 Mar 2023 19:09:23 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:128d54f2c9b134270b406c5f3a41296da7c1111d3a6927f0b4451131d636151e`  
		Last Modified: Thu, 23 Mar 2023 21:24:22 GMT  
		Size: 62.5 MB (62483466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed02fb405f69d37280c5eff742126b7a2073052e009a5bfd05ad529fe1155471`  
		Last Modified: Tue, 28 Mar 2023 19:15:25 GMT  
		Size: 75.6 MB (75558177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:latest` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:2d644bee3d8682672820a2af01ba90e90c6da9dcf14b419f5f13aaa7e3edb8f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123705067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:465e874e0e70f85665dbdb01c7fcc2111083ac3cc0f6500a533d19786d6bd5e2`
-	Default Command: `["\/bin\/bash"]`

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
