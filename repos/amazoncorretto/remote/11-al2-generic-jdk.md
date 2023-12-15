## `amazoncorretto:11-al2-generic-jdk`

```console
$ docker pull amazoncorretto@sha256:3f1b24766eac661a87107c9cb473c16705f9a9799df5d6fd3b976cf02d187620
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-generic-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:d58aeb7004d6ecca1ed30819c7e5bddab6b27572e3f8ce5a426ffdaad72851e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.6 MB (210589602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce67435abe4bfd02ae6928a09984d226f60acd98405f2dbb0c8b895b2bc0b8ee`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 15 Dec 2023 20:22:49 GMT
COPY dir:fd6bc3e61b31127123e1a8c57613d9baa7f5605d29d858f885c6a105709aa8fd in / 
# Fri, 15 Dec 2023 20:22:50 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 20:42:41 GMT
ARG version=11.0.21.9-1
# Fri, 15 Dec 2023 20:43:04 GMT
# ARGS: version=11.0.21.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 15 Dec 2023 20:43:04 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 20:43:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:497f6fc6e5d7835e37c10dd6462da0d293dc146b7ead757dc61e580b47fd2578`  
		Last Modified: Tue, 12 Dec 2023 02:10:17 GMT  
		Size: 62.6 MB (62645650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e13fc6d99aa0e7f4421920aa7183cbfdcf085462a8bc98d4843d02a3bdeb0f`  
		Last Modified: Fri, 15 Dec 2023 20:54:45 GMT  
		Size: 147.9 MB (147943952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-generic-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:8d72554428bd379a39d4ab69b7c525fbbc34b78aeb18df39283d19de3cec2931
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.5 MB (209456791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6490f38e6b0c579d631339dc38269ef1953752287d1ea5b065af1545f513eae2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 15 Dec 2023 20:44:39 GMT
COPY dir:10ec8ba603fc9dc4661d37af0490e95262fb40302640f3ade11c9c85291feebb in / 
# Fri, 15 Dec 2023 20:44:40 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 21:10:27 GMT
ARG version=11.0.21.9-1
# Fri, 15 Dec 2023 21:10:45 GMT
# ARGS: version=11.0.21.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 15 Dec 2023 21:10:47 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 21:10:47 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:770064597beb3d761f91ecebb678371619bec21864a4248afd29b220625976f2`  
		Last Modified: Tue, 12 Dec 2023 08:31:57 GMT  
		Size: 64.4 MB (64444817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bf360129e802cfe2ba2c878453267103f20b71c447b441d51732d46ecaf219`  
		Last Modified: Fri, 15 Dec 2023 21:19:53 GMT  
		Size: 145.0 MB (145011974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
