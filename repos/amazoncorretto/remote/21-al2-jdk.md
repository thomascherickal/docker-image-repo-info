## `amazoncorretto:21-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:c6a21d26970408b997e5e5cfb0ef3c14b70ab362c6ab097749c363de0f9df34c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:21-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4f1d3b478b0f1e0bea88d37a03c5c973aed4763e94291f0e9edcb48efb50c3b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.1 MB (228128472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3fee4b1572b93737c82c2934b75876b1d6e63df2d3771061f17fe696cad51d5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 15 Dec 2023 20:22:49 GMT
COPY dir:fd6bc3e61b31127123e1a8c57613d9baa7f5605d29d858f885c6a105709aa8fd in / 
# Fri, 15 Dec 2023 20:22:50 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 20:49:42 GMT
ARG version=21.0.1.12-1
# Fri, 15 Dec 2023 20:50:06 GMT
# ARGS: version=21.0.1.12-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-21-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-21-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 15 Dec 2023 20:50:07 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 20:50:07 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
```

-	Layers:
	-	`sha256:497f6fc6e5d7835e37c10dd6462da0d293dc146b7ead757dc61e580b47fd2578`  
		Last Modified: Tue, 12 Dec 2023 02:10:17 GMT  
		Size: 62.6 MB (62645650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6a10c4f7ceee0807d59ee5ccde088895b637676672dc6a17ecd82c02419c79`  
		Last Modified: Fri, 15 Dec 2023 20:59:45 GMT  
		Size: 165.5 MB (165482822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:21-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:9aaa33a604b178b412bb27617b37154438c49630bfed76eb600ac360370ac2c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.9 MB (227897922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194b846791c74385f0ab20adcb4212da143aab3834f83791ebf38f6ecc325ea9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 15 Dec 2023 20:44:39 GMT
COPY dir:10ec8ba603fc9dc4661d37af0490e95262fb40302640f3ade11c9c85291feebb in / 
# Fri, 15 Dec 2023 20:44:40 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 21:15:57 GMT
ARG version=21.0.1.12-1
# Fri, 15 Dec 2023 21:16:17 GMT
# ARGS: version=21.0.1.12-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-21-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-21-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 15 Dec 2023 21:16:19 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 21:16:19 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
```

-	Layers:
	-	`sha256:770064597beb3d761f91ecebb678371619bec21864a4248afd29b220625976f2`  
		Last Modified: Tue, 12 Dec 2023 08:31:57 GMT  
		Size: 64.4 MB (64444817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84a22ddf532a229c35b3bc1a6de42b3b347a9eca7be835dac1ca71fcb8cf22d`  
		Last Modified: Fri, 15 Dec 2023 21:24:10 GMT  
		Size: 163.5 MB (163453105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
