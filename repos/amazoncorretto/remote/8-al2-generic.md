## `amazoncorretto:8-al2-generic`

```console
$ docker pull amazoncorretto@sha256:64aaa4859de6212943adb4605c83cdc62969d8c9c55fcbb88411e25260c98669
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2-generic` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:9fdfc994429e1dd5ae8f4fd5dce47b30e66a6e79be817fb2ef481281d03079c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.2 MB (138207414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:608ad74cd88bd3949559526baf7028a130d3e91f966030618165ba92af6be3e9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:21:54 GMT
COPY dir:ddf8ce4c235ebf92718d40c0041035b283a61cbd94b49610e57999ebc78d3ec6 in / 
# Tue, 21 Nov 2023 03:21:55 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 04:13:06 GMT
ARG version=1.8.0_392.b08-1
# Tue, 21 Nov 2023 04:13:26 GMT
# ARGS: version=1.8.0_392.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 21 Nov 2023 04:13:26 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 04:13:27 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:0b4a6f011995244a95bff79a1298e83d230bc0aa22871a9c510745cafebec227`  
		Last Modified: Sun, 19 Nov 2023 03:18:53 GMT  
		Size: 62.6 MB (62641917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae07246600142ccbbcc800cb9ff3d5e4aacfeeaee4985a2a51b0d5701e949add`  
		Last Modified: Tue, 21 Nov 2023 04:25:47 GMT  
		Size: 75.6 MB (75565497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2-generic` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:c0f386e85785be23e4b475bd2e00bf2dfc43046d4c4472fb18fff988794e4718
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (123993301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:645cfb18286e6a1465d047c51aeaefaeb3eabbec8ea5b3b9b7f52024f010aecc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 03 Nov 2023 22:40:19 GMT
COPY dir:fd6882cfe0ef7631745084a3b6ac01566c46fa528d35361defcd296ca1356d38 in / 
# Fri, 03 Nov 2023 22:40:20 GMT
CMD ["/bin/bash"]
# Fri, 03 Nov 2023 22:56:15 GMT
ARG version=1.8.0_392.b08-1
# Fri, 03 Nov 2023 22:56:31 GMT
# ARGS: version=1.8.0_392.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 03 Nov 2023 22:56:32 GMT
ENV LANG=C.UTF-8
# Fri, 03 Nov 2023 22:56:32 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:615a413db4e82f95ffe4a1cef67468f86d056893cb442e21cb7cea8bc622f9d0`  
		Last Modified: Fri, 03 Nov 2023 17:50:57 GMT  
		Size: 64.4 MB (64380203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5a65a128cd0e4a050ccae0c23b1c346c7b82b679bf029de348d4536709ade2`  
		Last Modified: Fri, 03 Nov 2023 23:06:52 GMT  
		Size: 59.6 MB (59613098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
