## `amazoncorretto:17-al2-full`

```console
$ docker pull amazoncorretto@sha256:26a8eb2853afb7b6a0231bd67410f3ad8682c77d347d53902e5eb7f50a59829e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:0b94658e8cf6d7c79e0dfd50afc90463704345a237f35fe8194296248639d82f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.6 MB (214613296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bcdd1052911135d2dfa48a6ae18b82821523732a4746e7f7d7b84e25c698c40`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 15 Dec 2023 20:22:49 GMT
COPY dir:fd6bc3e61b31127123e1a8c57613d9baa7f5605d29d858f885c6a105709aa8fd in / 
# Fri, 15 Dec 2023 20:22:50 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 20:45:52 GMT
ARG version=17.0.9.8-1
# Fri, 15 Dec 2023 20:46:17 GMT
# ARGS: version=17.0.9.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 15 Dec 2023 20:46:18 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 20:46:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:497f6fc6e5d7835e37c10dd6462da0d293dc146b7ead757dc61e580b47fd2578`  
		Last Modified: Tue, 12 Dec 2023 02:10:17 GMT  
		Size: 62.6 MB (62645650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4496685617b196f33f0ce3fbfa0675b4497c025c5017fa36830c110df48a1a54`  
		Last Modified: Fri, 15 Dec 2023 20:57:01 GMT  
		Size: 152.0 MB (151967646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:43e0b5de86a34bf8473cf69ed3ab7948ec5f5a6463efa1ffd994561c415d9861
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.9 MB (214944873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d7d6c7b22d1d771ddcfb7228a223d9d72793676a0650fd6b092bfcd9ca7e3b7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 15 Dec 2023 20:44:39 GMT
COPY dir:10ec8ba603fc9dc4661d37af0490e95262fb40302640f3ade11c9c85291feebb in / 
# Fri, 15 Dec 2023 20:44:40 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 21:12:52 GMT
ARG version=17.0.9.8-1
# Fri, 15 Dec 2023 21:13:12 GMT
# ARGS: version=17.0.9.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 15 Dec 2023 21:13:14 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 21:13:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:770064597beb3d761f91ecebb678371619bec21864a4248afd29b220625976f2`  
		Last Modified: Tue, 12 Dec 2023 08:31:57 GMT  
		Size: 64.4 MB (64444817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609caa77d0d8cbb9ec4a3c8708e2e7b8b34b7f97bf1237381066d4f56479bfea`  
		Last Modified: Fri, 15 Dec 2023 21:21:52 GMT  
		Size: 150.5 MB (150500056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
