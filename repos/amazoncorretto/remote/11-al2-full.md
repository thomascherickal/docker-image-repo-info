## `amazoncorretto:11-al2-full`

```console
$ docker pull amazoncorretto@sha256:7e23191e7b80797bf51f479427ca4cee1986a54460aabcb7728bb7ad6bc028bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:1239e9e0eec19c9ea4ab988b0e7fb20e22ff966172de17086b8357e3c4ec31ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.8 MB (209776425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cc7448a0d960eaa052f4a9f432612722b2fca5e1c2e0a24ec7707afff1e3d9b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Aug 2022 01:19:36 GMT
ADD file:ebfd33425a17b16a9e560de15c91108bf2ee740f284a1482a7105b420ff22678 in / 
# Fri, 26 Aug 2022 01:19:37 GMT
CMD ["/bin/bash"]
# Fri, 26 Aug 2022 02:03:37 GMT
ARG version=11.0.16.9-1
# Fri, 26 Aug 2022 02:04:01 GMT
# ARGS: version=11.0.16.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 26 Aug 2022 02:04:02 GMT
ENV LANG=C.UTF-8
# Fri, 26 Aug 2022 02:04:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:fd06b60db4951fd95b43a9e73fb084fe7d2afcd4ff464472ead5548cd1c28717`  
		Last Modified: Mon, 22 Aug 2022 22:09:44 GMT  
		Size: 62.3 MB (62326701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e806ef017442d9e0f611cb049e442935f8b228820877e1239ddba2e048b634`  
		Last Modified: Fri, 26 Aug 2022 02:07:46 GMT  
		Size: 147.4 MB (147449724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:5188e539e8a258564443aa9f9ec9e292e3fb63afc1b7fc8e42fc08a0868a26f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.5 MB (208512499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0b2f3226e082059adbc7c8726eb5f6e4a9c9ca05dc5818c30374fb1bdf858df`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Aug 2022 00:39:31 GMT
ADD file:a0918d3dfd5c1b4e0594c53d0dfc4c97f1ebaf14085279c79f36f06cf7ed95ee in / 
# Fri, 26 Aug 2022 00:39:32 GMT
CMD ["/bin/bash"]
# Fri, 26 Aug 2022 01:01:26 GMT
ARG version=11.0.16.9-1
# Fri, 26 Aug 2022 01:01:39 GMT
# ARGS: version=11.0.16.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 26 Aug 2022 01:01:40 GMT
ENV LANG=C.UTF-8
# Fri, 26 Aug 2022 01:01:40 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:12df598bc31e0ff3cadc2667d34dc645b837d712e7e15ce3e9080ae91744dcd0`  
		Last Modified: Mon, 22 Aug 2022 22:09:44 GMT  
		Size: 63.9 MB (63938765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27eb91a4547e1bb6153357482beae6fd003894417903c684578e4fb0ebaeeab0`  
		Last Modified: Fri, 26 Aug 2022 01:04:09 GMT  
		Size: 144.6 MB (144573734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
