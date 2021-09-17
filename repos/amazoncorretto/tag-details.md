<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazoncorretto`

-	[`amazoncorretto:11`](#amazoncorretto11)
-	[`amazoncorretto:11-al2-full`](#amazoncorretto11-al2-full)
-	[`amazoncorretto:11-al2-jdk`](#amazoncorretto11-al2-jdk)
-	[`amazoncorretto:11-alpine`](#amazoncorretto11-alpine)
-	[`amazoncorretto:11-alpine-full`](#amazoncorretto11-alpine-full)
-	[`amazoncorretto:11-alpine-jdk`](#amazoncorretto11-alpine-jdk)
-	[`amazoncorretto:11.0.12`](#amazoncorretto11012)
-	[`amazoncorretto:11.0.12-al2`](#amazoncorretto11012-al2)
-	[`amazoncorretto:11.0.12-alpine`](#amazoncorretto11012-alpine)
-	[`amazoncorretto:16`](#amazoncorretto16)
-	[`amazoncorretto:16-al2-full`](#amazoncorretto16-al2-full)
-	[`amazoncorretto:16-al2-jdk`](#amazoncorretto16-al2-jdk)
-	[`amazoncorretto:16-alpine`](#amazoncorretto16-alpine)
-	[`amazoncorretto:16-alpine-full`](#amazoncorretto16-alpine-full)
-	[`amazoncorretto:16-alpine-jdk`](#amazoncorretto16-alpine-jdk)
-	[`amazoncorretto:16.0.2`](#amazoncorretto1602)
-	[`amazoncorretto:16.0.2-al2`](#amazoncorretto1602-al2)
-	[`amazoncorretto:16.0.2-alpine`](#amazoncorretto1602-alpine)
-	[`amazoncorretto:17`](#amazoncorretto17)
-	[`amazoncorretto:17-al2-full`](#amazoncorretto17-al2-full)
-	[`amazoncorretto:17-al2-jdk`](#amazoncorretto17-al2-jdk)
-	[`amazoncorretto:17-alpine`](#amazoncorretto17-alpine)
-	[`amazoncorretto:17-alpine-full`](#amazoncorretto17-alpine-full)
-	[`amazoncorretto:17-alpine-jdk`](#amazoncorretto17-alpine-jdk)
-	[`amazoncorretto:17.0.0`](#amazoncorretto1700)
-	[`amazoncorretto:17.0.0-al2`](#amazoncorretto1700-al2)
-	[`amazoncorretto:17.0.0-alpine`](#amazoncorretto1700-alpine)
-	[`amazoncorretto:8`](#amazoncorretto8)
-	[`amazoncorretto:8-al2-full`](#amazoncorretto8-al2-full)
-	[`amazoncorretto:8-al2-jdk`](#amazoncorretto8-al2-jdk)
-	[`amazoncorretto:8-alpine`](#amazoncorretto8-alpine)
-	[`amazoncorretto:8-alpine-full`](#amazoncorretto8-alpine-full)
-	[`amazoncorretto:8-alpine-jdk`](#amazoncorretto8-alpine-jdk)
-	[`amazoncorretto:8-alpine-jre`](#amazoncorretto8-alpine-jre)
-	[`amazoncorretto:8u302`](#amazoncorretto8u302)
-	[`amazoncorretto:8u302-al2`](#amazoncorretto8u302-al2)
-	[`amazoncorretto:8u302-alpine`](#amazoncorretto8u302-alpine)
-	[`amazoncorretto:8u302-alpine-jre`](#amazoncorretto8u302-alpine-jre)
-	[`amazoncorretto:latest`](#amazoncorrettolatest)

## `amazoncorretto:11`

```console
$ docker pull amazoncorretto@sha256:22fca4ce7eb9569ecc80e215fed65cbe8f1aa505400b219a6c4379df071ab207
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:c24c93a542d744c12c7dab6d32270258a7df95831912500d5fb7b13d1ecf3e23
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.8 MB (208784216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d45eed37d84951e78b45e613f890eb0158dcc65c6dc86d5113fcd5512add7e95`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 01:05:40 GMT
ARG version=11.0.12.7-1
# Thu, 09 Sep 2021 01:06:02 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 01:06:02 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 01:06:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b77619ee11e9d9ecda8ead06a29c0ea4f57a356c56012cff0d44c49caa1ca96`  
		Last Modified: Thu, 09 Sep 2021 01:07:51 GMT  
		Size: 146.8 MB (146783913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:fa940aad514c88570f09a5dad7ef7956decde3ff080333941a03b8394afe6a3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.4 MB (207371784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89056cc7eae26794d4c950dd8fb3211666c44ccee28ae43ae32eaed8e791055e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 00:57:44 GMT
ARG version=11.0.12.7-1
# Thu, 09 Sep 2021 00:58:05 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 00:58:05 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 00:58:05 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58548b6552b9cf3a57fd10f20ffc573698eeb3280a1ecca6f83c154fe1aa894f`  
		Last Modified: Thu, 09 Sep 2021 01:00:03 GMT  
		Size: 143.9 MB (143940982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-al2-full`

```console
$ docker pull amazoncorretto@sha256:22fca4ce7eb9569ecc80e215fed65cbe8f1aa505400b219a6c4379df071ab207
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:c24c93a542d744c12c7dab6d32270258a7df95831912500d5fb7b13d1ecf3e23
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.8 MB (208784216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d45eed37d84951e78b45e613f890eb0158dcc65c6dc86d5113fcd5512add7e95`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 01:05:40 GMT
ARG version=11.0.12.7-1
# Thu, 09 Sep 2021 01:06:02 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 01:06:02 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 01:06:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b77619ee11e9d9ecda8ead06a29c0ea4f57a356c56012cff0d44c49caa1ca96`  
		Last Modified: Thu, 09 Sep 2021 01:07:51 GMT  
		Size: 146.8 MB (146783913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:fa940aad514c88570f09a5dad7ef7956decde3ff080333941a03b8394afe6a3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.4 MB (207371784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89056cc7eae26794d4c950dd8fb3211666c44ccee28ae43ae32eaed8e791055e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 00:57:44 GMT
ARG version=11.0.12.7-1
# Thu, 09 Sep 2021 00:58:05 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 00:58:05 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 00:58:05 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58548b6552b9cf3a57fd10f20ffc573698eeb3280a1ecca6f83c154fe1aa894f`  
		Last Modified: Thu, 09 Sep 2021 01:00:03 GMT  
		Size: 143.9 MB (143940982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:22fca4ce7eb9569ecc80e215fed65cbe8f1aa505400b219a6c4379df071ab207
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:c24c93a542d744c12c7dab6d32270258a7df95831912500d5fb7b13d1ecf3e23
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.8 MB (208784216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d45eed37d84951e78b45e613f890eb0158dcc65c6dc86d5113fcd5512add7e95`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 01:05:40 GMT
ARG version=11.0.12.7-1
# Thu, 09 Sep 2021 01:06:02 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 01:06:02 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 01:06:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b77619ee11e9d9ecda8ead06a29c0ea4f57a356c56012cff0d44c49caa1ca96`  
		Last Modified: Thu, 09 Sep 2021 01:07:51 GMT  
		Size: 146.8 MB (146783913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:fa940aad514c88570f09a5dad7ef7956decde3ff080333941a03b8394afe6a3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.4 MB (207371784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89056cc7eae26794d4c950dd8fb3211666c44ccee28ae43ae32eaed8e791055e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 00:57:44 GMT
ARG version=11.0.12.7-1
# Thu, 09 Sep 2021 00:58:05 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 00:58:05 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 00:58:05 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58548b6552b9cf3a57fd10f20ffc573698eeb3280a1ecca6f83c154fe1aa894f`  
		Last Modified: Thu, 09 Sep 2021 01:00:03 GMT  
		Size: 143.9 MB (143940982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-alpine`

```console
$ docker pull amazoncorretto@sha256:c225131e21c08557e8fc67093d2d754cbcb60acd87a5b76705536a289cc0e906
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:6c7d2b8ea57c59261869b9fccaf539922bee14bd0369592e33a774896b1e9e5d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.2 MB (196173778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44d331805194149821fc0bcd3df484be70e89bee0a11400e41d38b99b0df65b8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:30:50 GMT
ARG version=11.0.12.7.1
# Wed, 01 Sep 2021 00:31:00 GMT
# ARGS: version=11.0.12.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Wed, 01 Sep 2021 00:31:01 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 00:31:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 01 Sep 2021 00:31:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3e805fde94ec062176cd36ed45061f412bb1e5ccd372790eb4f0f9674e0ff5`  
		Last Modified: Wed, 01 Sep 2021 00:33:22 GMT  
		Size: 193.4 MB (193372071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-alpine-full`

```console
$ docker pull amazoncorretto@sha256:c225131e21c08557e8fc67093d2d754cbcb60acd87a5b76705536a289cc0e906
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:6c7d2b8ea57c59261869b9fccaf539922bee14bd0369592e33a774896b1e9e5d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.2 MB (196173778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44d331805194149821fc0bcd3df484be70e89bee0a11400e41d38b99b0df65b8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:30:50 GMT
ARG version=11.0.12.7.1
# Wed, 01 Sep 2021 00:31:00 GMT
# ARGS: version=11.0.12.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Wed, 01 Sep 2021 00:31:01 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 00:31:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 01 Sep 2021 00:31:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3e805fde94ec062176cd36ed45061f412bb1e5ccd372790eb4f0f9674e0ff5`  
		Last Modified: Wed, 01 Sep 2021 00:33:22 GMT  
		Size: 193.4 MB (193372071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:c225131e21c08557e8fc67093d2d754cbcb60acd87a5b76705536a289cc0e906
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:6c7d2b8ea57c59261869b9fccaf539922bee14bd0369592e33a774896b1e9e5d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.2 MB (196173778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44d331805194149821fc0bcd3df484be70e89bee0a11400e41d38b99b0df65b8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:30:50 GMT
ARG version=11.0.12.7.1
# Wed, 01 Sep 2021 00:31:00 GMT
# ARGS: version=11.0.12.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Wed, 01 Sep 2021 00:31:01 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 00:31:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 01 Sep 2021 00:31:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3e805fde94ec062176cd36ed45061f412bb1e5ccd372790eb4f0f9674e0ff5`  
		Last Modified: Wed, 01 Sep 2021 00:33:22 GMT  
		Size: 193.4 MB (193372071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11.0.12`

```console
$ docker pull amazoncorretto@sha256:22fca4ce7eb9569ecc80e215fed65cbe8f1aa505400b219a6c4379df071ab207
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11.0.12` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:c24c93a542d744c12c7dab6d32270258a7df95831912500d5fb7b13d1ecf3e23
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.8 MB (208784216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d45eed37d84951e78b45e613f890eb0158dcc65c6dc86d5113fcd5512add7e95`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 01:05:40 GMT
ARG version=11.0.12.7-1
# Thu, 09 Sep 2021 01:06:02 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 01:06:02 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 01:06:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b77619ee11e9d9ecda8ead06a29c0ea4f57a356c56012cff0d44c49caa1ca96`  
		Last Modified: Thu, 09 Sep 2021 01:07:51 GMT  
		Size: 146.8 MB (146783913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11.0.12` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:fa940aad514c88570f09a5dad7ef7956decde3ff080333941a03b8394afe6a3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.4 MB (207371784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89056cc7eae26794d4c950dd8fb3211666c44ccee28ae43ae32eaed8e791055e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 00:57:44 GMT
ARG version=11.0.12.7-1
# Thu, 09 Sep 2021 00:58:05 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 00:58:05 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 00:58:05 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58548b6552b9cf3a57fd10f20ffc573698eeb3280a1ecca6f83c154fe1aa894f`  
		Last Modified: Thu, 09 Sep 2021 01:00:03 GMT  
		Size: 143.9 MB (143940982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11.0.12-al2`

```console
$ docker pull amazoncorretto@sha256:22fca4ce7eb9569ecc80e215fed65cbe8f1aa505400b219a6c4379df071ab207
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11.0.12-al2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:c24c93a542d744c12c7dab6d32270258a7df95831912500d5fb7b13d1ecf3e23
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.8 MB (208784216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d45eed37d84951e78b45e613f890eb0158dcc65c6dc86d5113fcd5512add7e95`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 01:05:40 GMT
ARG version=11.0.12.7-1
# Thu, 09 Sep 2021 01:06:02 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 01:06:02 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 01:06:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b77619ee11e9d9ecda8ead06a29c0ea4f57a356c56012cff0d44c49caa1ca96`  
		Last Modified: Thu, 09 Sep 2021 01:07:51 GMT  
		Size: 146.8 MB (146783913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11.0.12-al2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:fa940aad514c88570f09a5dad7ef7956decde3ff080333941a03b8394afe6a3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.4 MB (207371784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89056cc7eae26794d4c950dd8fb3211666c44ccee28ae43ae32eaed8e791055e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 00:57:44 GMT
ARG version=11.0.12.7-1
# Thu, 09 Sep 2021 00:58:05 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 00:58:05 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 00:58:05 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58548b6552b9cf3a57fd10f20ffc573698eeb3280a1ecca6f83c154fe1aa894f`  
		Last Modified: Thu, 09 Sep 2021 01:00:03 GMT  
		Size: 143.9 MB (143940982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11.0.12-alpine`

```console
$ docker pull amazoncorretto@sha256:c225131e21c08557e8fc67093d2d754cbcb60acd87a5b76705536a289cc0e906
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11.0.12-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:6c7d2b8ea57c59261869b9fccaf539922bee14bd0369592e33a774896b1e9e5d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.2 MB (196173778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44d331805194149821fc0bcd3df484be70e89bee0a11400e41d38b99b0df65b8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:30:50 GMT
ARG version=11.0.12.7.1
# Wed, 01 Sep 2021 00:31:00 GMT
# ARGS: version=11.0.12.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Wed, 01 Sep 2021 00:31:01 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 00:31:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 01 Sep 2021 00:31:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3e805fde94ec062176cd36ed45061f412bb1e5ccd372790eb4f0f9674e0ff5`  
		Last Modified: Wed, 01 Sep 2021 00:33:22 GMT  
		Size: 193.4 MB (193372071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16`

```console
$ docker pull amazoncorretto@sha256:d9680a2c53b1b2891a2ddb340c87f44e438d419f74d8b4936303a3389e2286b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:80cc6be110094476a463ed885735f813b6b22dd4b44b2a902c72063fad34e278
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.0 MB (221970188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee84b5cd602c03ff19afe80d2feb1255a2e9a94965614acac6f894a5d34f3bb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 01:06:14 GMT
ARG version=16.0.2.7-1
# Thu, 09 Sep 2021 01:06:35 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 01:06:35 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 01:06:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7253b94dc9693b8579464ae8831e09e7487e1759e5c94665a32de6736cffc600`  
		Last Modified: Thu, 09 Sep 2021 01:08:26 GMT  
		Size: 160.0 MB (159969885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:0dadd48a3f379b9cf9f5357b6add89a61ee90a7142f729c07cd02f3ef2994f38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.4 MB (223374936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df89120e6e6535f9b57d8a61206f601f339d9a96e5c2caff8186a0d26923dcb0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 00:58:12 GMT
ARG version=16.0.2.7-1
# Thu, 09 Sep 2021 00:58:31 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 00:58:32 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 00:58:32 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768c36d5e73d6e867b4f08fd0e94ddf4f1e08e282c11c7e9b493cb02269f5715`  
		Last Modified: Thu, 09 Sep 2021 01:00:43 GMT  
		Size: 159.9 MB (159944134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-al2-full`

```console
$ docker pull amazoncorretto@sha256:d9680a2c53b1b2891a2ddb340c87f44e438d419f74d8b4936303a3389e2286b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:80cc6be110094476a463ed885735f813b6b22dd4b44b2a902c72063fad34e278
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.0 MB (221970188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee84b5cd602c03ff19afe80d2feb1255a2e9a94965614acac6f894a5d34f3bb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 01:06:14 GMT
ARG version=16.0.2.7-1
# Thu, 09 Sep 2021 01:06:35 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 01:06:35 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 01:06:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7253b94dc9693b8579464ae8831e09e7487e1759e5c94665a32de6736cffc600`  
		Last Modified: Thu, 09 Sep 2021 01:08:26 GMT  
		Size: 160.0 MB (159969885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:0dadd48a3f379b9cf9f5357b6add89a61ee90a7142f729c07cd02f3ef2994f38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.4 MB (223374936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df89120e6e6535f9b57d8a61206f601f339d9a96e5c2caff8186a0d26923dcb0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 00:58:12 GMT
ARG version=16.0.2.7-1
# Thu, 09 Sep 2021 00:58:31 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 00:58:32 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 00:58:32 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768c36d5e73d6e867b4f08fd0e94ddf4f1e08e282c11c7e9b493cb02269f5715`  
		Last Modified: Thu, 09 Sep 2021 01:00:43 GMT  
		Size: 159.9 MB (159944134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:d9680a2c53b1b2891a2ddb340c87f44e438d419f74d8b4936303a3389e2286b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:80cc6be110094476a463ed885735f813b6b22dd4b44b2a902c72063fad34e278
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.0 MB (221970188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee84b5cd602c03ff19afe80d2feb1255a2e9a94965614acac6f894a5d34f3bb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 01:06:14 GMT
ARG version=16.0.2.7-1
# Thu, 09 Sep 2021 01:06:35 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 01:06:35 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 01:06:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7253b94dc9693b8579464ae8831e09e7487e1759e5c94665a32de6736cffc600`  
		Last Modified: Thu, 09 Sep 2021 01:08:26 GMT  
		Size: 160.0 MB (159969885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:0dadd48a3f379b9cf9f5357b6add89a61ee90a7142f729c07cd02f3ef2994f38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.4 MB (223374936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df89120e6e6535f9b57d8a61206f601f339d9a96e5c2caff8186a0d26923dcb0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 00:58:12 GMT
ARG version=16.0.2.7-1
# Thu, 09 Sep 2021 00:58:31 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 00:58:32 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 00:58:32 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768c36d5e73d6e867b4f08fd0e94ddf4f1e08e282c11c7e9b493cb02269f5715`  
		Last Modified: Thu, 09 Sep 2021 01:00:43 GMT  
		Size: 159.9 MB (159944134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-alpine`

```console
$ docker pull amazoncorretto@sha256:3ba7ea36df85e9a00e428aca3cbf1d77aace7d135de555e9533a5a40db7ef707
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:16-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:67f6a2dc5ae8bf75bd6ee5af504a9de65e6a32c2989f1a7ba0d5543c8c94b238
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.5 MB (212454350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e0d9c5ca59bd0e46cc3968299511a805f34b32bc066019289d5fb484c893160`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:31:11 GMT
ARG version=16.0.2.7.1
# Wed, 01 Sep 2021 00:31:23 GMT
# ARGS: version=16.0.2.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-16=$version-r0
# Wed, 01 Sep 2021 00:31:24 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 00:31:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 01 Sep 2021 00:31:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e812a6b7beb13efdcc4765fefd7b00d8d9868aaaa70990ea919d8a7a447682ba`  
		Last Modified: Wed, 01 Sep 2021 00:33:57 GMT  
		Size: 209.7 MB (209652643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-alpine-full`

```console
$ docker pull amazoncorretto@sha256:3ba7ea36df85e9a00e428aca3cbf1d77aace7d135de555e9533a5a40db7ef707
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:16-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:67f6a2dc5ae8bf75bd6ee5af504a9de65e6a32c2989f1a7ba0d5543c8c94b238
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.5 MB (212454350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e0d9c5ca59bd0e46cc3968299511a805f34b32bc066019289d5fb484c893160`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:31:11 GMT
ARG version=16.0.2.7.1
# Wed, 01 Sep 2021 00:31:23 GMT
# ARGS: version=16.0.2.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-16=$version-r0
# Wed, 01 Sep 2021 00:31:24 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 00:31:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 01 Sep 2021 00:31:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e812a6b7beb13efdcc4765fefd7b00d8d9868aaaa70990ea919d8a7a447682ba`  
		Last Modified: Wed, 01 Sep 2021 00:33:57 GMT  
		Size: 209.7 MB (209652643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:3ba7ea36df85e9a00e428aca3cbf1d77aace7d135de555e9533a5a40db7ef707
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:16-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:67f6a2dc5ae8bf75bd6ee5af504a9de65e6a32c2989f1a7ba0d5543c8c94b238
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.5 MB (212454350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e0d9c5ca59bd0e46cc3968299511a805f34b32bc066019289d5fb484c893160`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:31:11 GMT
ARG version=16.0.2.7.1
# Wed, 01 Sep 2021 00:31:23 GMT
# ARGS: version=16.0.2.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-16=$version-r0
# Wed, 01 Sep 2021 00:31:24 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 00:31:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 01 Sep 2021 00:31:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e812a6b7beb13efdcc4765fefd7b00d8d9868aaaa70990ea919d8a7a447682ba`  
		Last Modified: Wed, 01 Sep 2021 00:33:57 GMT  
		Size: 209.7 MB (209652643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16.0.2`

```console
$ docker pull amazoncorretto@sha256:d9680a2c53b1b2891a2ddb340c87f44e438d419f74d8b4936303a3389e2286b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16.0.2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:80cc6be110094476a463ed885735f813b6b22dd4b44b2a902c72063fad34e278
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.0 MB (221970188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee84b5cd602c03ff19afe80d2feb1255a2e9a94965614acac6f894a5d34f3bb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 01:06:14 GMT
ARG version=16.0.2.7-1
# Thu, 09 Sep 2021 01:06:35 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 01:06:35 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 01:06:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7253b94dc9693b8579464ae8831e09e7487e1759e5c94665a32de6736cffc600`  
		Last Modified: Thu, 09 Sep 2021 01:08:26 GMT  
		Size: 160.0 MB (159969885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16.0.2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:0dadd48a3f379b9cf9f5357b6add89a61ee90a7142f729c07cd02f3ef2994f38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.4 MB (223374936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df89120e6e6535f9b57d8a61206f601f339d9a96e5c2caff8186a0d26923dcb0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 00:58:12 GMT
ARG version=16.0.2.7-1
# Thu, 09 Sep 2021 00:58:31 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 00:58:32 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 00:58:32 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768c36d5e73d6e867b4f08fd0e94ddf4f1e08e282c11c7e9b493cb02269f5715`  
		Last Modified: Thu, 09 Sep 2021 01:00:43 GMT  
		Size: 159.9 MB (159944134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16.0.2-al2`

```console
$ docker pull amazoncorretto@sha256:d9680a2c53b1b2891a2ddb340c87f44e438d419f74d8b4936303a3389e2286b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16.0.2-al2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:80cc6be110094476a463ed885735f813b6b22dd4b44b2a902c72063fad34e278
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.0 MB (221970188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee84b5cd602c03ff19afe80d2feb1255a2e9a94965614acac6f894a5d34f3bb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 01:06:14 GMT
ARG version=16.0.2.7-1
# Thu, 09 Sep 2021 01:06:35 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 01:06:35 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 01:06:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7253b94dc9693b8579464ae8831e09e7487e1759e5c94665a32de6736cffc600`  
		Last Modified: Thu, 09 Sep 2021 01:08:26 GMT  
		Size: 160.0 MB (159969885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16.0.2-al2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:0dadd48a3f379b9cf9f5357b6add89a61ee90a7142f729c07cd02f3ef2994f38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.4 MB (223374936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df89120e6e6535f9b57d8a61206f601f339d9a96e5c2caff8186a0d26923dcb0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 00:58:12 GMT
ARG version=16.0.2.7-1
# Thu, 09 Sep 2021 00:58:31 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 00:58:32 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 00:58:32 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768c36d5e73d6e867b4f08fd0e94ddf4f1e08e282c11c7e9b493cb02269f5715`  
		Last Modified: Thu, 09 Sep 2021 01:00:43 GMT  
		Size: 159.9 MB (159944134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16.0.2-alpine`

```console
$ docker pull amazoncorretto@sha256:3ba7ea36df85e9a00e428aca3cbf1d77aace7d135de555e9533a5a40db7ef707
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:16.0.2-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:67f6a2dc5ae8bf75bd6ee5af504a9de65e6a32c2989f1a7ba0d5543c8c94b238
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.5 MB (212454350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e0d9c5ca59bd0e46cc3968299511a805f34b32bc066019289d5fb484c893160`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:31:11 GMT
ARG version=16.0.2.7.1
# Wed, 01 Sep 2021 00:31:23 GMT
# ARGS: version=16.0.2.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-16=$version-r0
# Wed, 01 Sep 2021 00:31:24 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 00:31:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 01 Sep 2021 00:31:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e812a6b7beb13efdcc4765fefd7b00d8d9868aaaa70990ea919d8a7a447682ba`  
		Last Modified: Wed, 01 Sep 2021 00:33:57 GMT  
		Size: 209.7 MB (209652643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:17`

```console
$ docker pull amazoncorretto@sha256:175957b964349d8d75850e43603cf65f740ced597faed22ee7db4f575a841d4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:e0fc6d3ddca7584f723d25870c58c7c5a7c71935699f7577d24150bbfe1f5a1d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.6 MB (213580807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa37b839189a8440ab7c82fd0b0f6efa23178842ca51421ac930153cf456e764`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Fri, 17 Sep 2021 18:19:45 GMT
ARG version=17.0.0.35-1
# Fri, 17 Sep 2021 18:20:07 GMT
# ARGS: version=17.0.0.35-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 17 Sep 2021 18:20:08 GMT
ENV LANG=C.UTF-8
# Fri, 17 Sep 2021 18:20:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635fde6e75efd3bf06de5b8adc0596067708e0eedb7c38ce2aff0a9feb1cf3cc`  
		Last Modified: Fri, 17 Sep 2021 18:21:34 GMT  
		Size: 151.6 MB (151580504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:afa3611ea4bda1ed87fb662bb08aaf18753860a8cccd55c9e4c173035abf6bce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.6 MB (213561011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6784df627675ec02f3c13c966491ff522d95e0313af01de2d514a95863b06af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Fri, 17 Sep 2021 18:39:43 GMT
ARG version=17.0.0.35-1
# Fri, 17 Sep 2021 18:40:04 GMT
# ARGS: version=17.0.0.35-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 17 Sep 2021 18:40:04 GMT
ENV LANG=C.UTF-8
# Fri, 17 Sep 2021 18:40:05 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e542c9ec83cb03f286aa01111e95fc150024f9a3b3aac06f1ced16b03bafe445`  
		Last Modified: Fri, 17 Sep 2021 18:41:24 GMT  
		Size: 150.1 MB (150130209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:17-al2-full`

```console
$ docker pull amazoncorretto@sha256:175957b964349d8d75850e43603cf65f740ced597faed22ee7db4f575a841d4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:e0fc6d3ddca7584f723d25870c58c7c5a7c71935699f7577d24150bbfe1f5a1d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.6 MB (213580807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa37b839189a8440ab7c82fd0b0f6efa23178842ca51421ac930153cf456e764`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Fri, 17 Sep 2021 18:19:45 GMT
ARG version=17.0.0.35-1
# Fri, 17 Sep 2021 18:20:07 GMT
# ARGS: version=17.0.0.35-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 17 Sep 2021 18:20:08 GMT
ENV LANG=C.UTF-8
# Fri, 17 Sep 2021 18:20:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635fde6e75efd3bf06de5b8adc0596067708e0eedb7c38ce2aff0a9feb1cf3cc`  
		Last Modified: Fri, 17 Sep 2021 18:21:34 GMT  
		Size: 151.6 MB (151580504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:afa3611ea4bda1ed87fb662bb08aaf18753860a8cccd55c9e4c173035abf6bce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.6 MB (213561011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6784df627675ec02f3c13c966491ff522d95e0313af01de2d514a95863b06af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Fri, 17 Sep 2021 18:39:43 GMT
ARG version=17.0.0.35-1
# Fri, 17 Sep 2021 18:40:04 GMT
# ARGS: version=17.0.0.35-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 17 Sep 2021 18:40:04 GMT
ENV LANG=C.UTF-8
# Fri, 17 Sep 2021 18:40:05 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e542c9ec83cb03f286aa01111e95fc150024f9a3b3aac06f1ced16b03bafe445`  
		Last Modified: Fri, 17 Sep 2021 18:41:24 GMT  
		Size: 150.1 MB (150130209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:17-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:175957b964349d8d75850e43603cf65f740ced597faed22ee7db4f575a841d4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:e0fc6d3ddca7584f723d25870c58c7c5a7c71935699f7577d24150bbfe1f5a1d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.6 MB (213580807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa37b839189a8440ab7c82fd0b0f6efa23178842ca51421ac930153cf456e764`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Fri, 17 Sep 2021 18:19:45 GMT
ARG version=17.0.0.35-1
# Fri, 17 Sep 2021 18:20:07 GMT
# ARGS: version=17.0.0.35-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 17 Sep 2021 18:20:08 GMT
ENV LANG=C.UTF-8
# Fri, 17 Sep 2021 18:20:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635fde6e75efd3bf06de5b8adc0596067708e0eedb7c38ce2aff0a9feb1cf3cc`  
		Last Modified: Fri, 17 Sep 2021 18:21:34 GMT  
		Size: 151.6 MB (151580504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:afa3611ea4bda1ed87fb662bb08aaf18753860a8cccd55c9e4c173035abf6bce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.6 MB (213561011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6784df627675ec02f3c13c966491ff522d95e0313af01de2d514a95863b06af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Fri, 17 Sep 2021 18:39:43 GMT
ARG version=17.0.0.35-1
# Fri, 17 Sep 2021 18:40:04 GMT
# ARGS: version=17.0.0.35-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 17 Sep 2021 18:40:04 GMT
ENV LANG=C.UTF-8
# Fri, 17 Sep 2021 18:40:05 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e542c9ec83cb03f286aa01111e95fc150024f9a3b3aac06f1ced16b03bafe445`  
		Last Modified: Fri, 17 Sep 2021 18:41:24 GMT  
		Size: 150.1 MB (150130209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:17-alpine`

```console
$ docker pull amazoncorretto@sha256:d4715e627365f5a1487ece0a87f1ad4dcf67eddf0ae937fd61f43e57c347eb41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4f0aaacb432a483fb06b79567ee74a5b7ce7218625e05ded20a3d057de92e75a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.9 MB (198930683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4a8136cf53529ca159d604c8a823ab34c17f77986ebb604be5dec7f0e20740b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 17 Sep 2021 18:20:15 GMT
ARG version=17.0.0.35.1
# Fri, 17 Sep 2021 18:20:23 GMT
# ARGS: version=17.0.0.35.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Fri, 17 Sep 2021 18:20:24 GMT
ENV LANG=C.UTF-8
# Fri, 17 Sep 2021 18:20:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 17 Sep 2021 18:20:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0129aa7f582aeb95bed9cd254e70c135ee2a28bbc71ca382c177eb21b46fb06`  
		Last Modified: Fri, 17 Sep 2021 18:22:06 GMT  
		Size: 196.1 MB (196116237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:17-alpine-full`

```console
$ docker pull amazoncorretto@sha256:d4715e627365f5a1487ece0a87f1ad4dcf67eddf0ae937fd61f43e57c347eb41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4f0aaacb432a483fb06b79567ee74a5b7ce7218625e05ded20a3d057de92e75a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.9 MB (198930683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4a8136cf53529ca159d604c8a823ab34c17f77986ebb604be5dec7f0e20740b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 17 Sep 2021 18:20:15 GMT
ARG version=17.0.0.35.1
# Fri, 17 Sep 2021 18:20:23 GMT
# ARGS: version=17.0.0.35.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Fri, 17 Sep 2021 18:20:24 GMT
ENV LANG=C.UTF-8
# Fri, 17 Sep 2021 18:20:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 17 Sep 2021 18:20:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0129aa7f582aeb95bed9cd254e70c135ee2a28bbc71ca382c177eb21b46fb06`  
		Last Modified: Fri, 17 Sep 2021 18:22:06 GMT  
		Size: 196.1 MB (196116237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:17-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:d4715e627365f5a1487ece0a87f1ad4dcf67eddf0ae937fd61f43e57c347eb41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4f0aaacb432a483fb06b79567ee74a5b7ce7218625e05ded20a3d057de92e75a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.9 MB (198930683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4a8136cf53529ca159d604c8a823ab34c17f77986ebb604be5dec7f0e20740b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 17 Sep 2021 18:20:15 GMT
ARG version=17.0.0.35.1
# Fri, 17 Sep 2021 18:20:23 GMT
# ARGS: version=17.0.0.35.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Fri, 17 Sep 2021 18:20:24 GMT
ENV LANG=C.UTF-8
# Fri, 17 Sep 2021 18:20:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 17 Sep 2021 18:20:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0129aa7f582aeb95bed9cd254e70c135ee2a28bbc71ca382c177eb21b46fb06`  
		Last Modified: Fri, 17 Sep 2021 18:22:06 GMT  
		Size: 196.1 MB (196116237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:17.0.0`

```console
$ docker pull amazoncorretto@sha256:175957b964349d8d75850e43603cf65f740ced597faed22ee7db4f575a841d4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17.0.0` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:e0fc6d3ddca7584f723d25870c58c7c5a7c71935699f7577d24150bbfe1f5a1d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.6 MB (213580807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa37b839189a8440ab7c82fd0b0f6efa23178842ca51421ac930153cf456e764`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Fri, 17 Sep 2021 18:19:45 GMT
ARG version=17.0.0.35-1
# Fri, 17 Sep 2021 18:20:07 GMT
# ARGS: version=17.0.0.35-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 17 Sep 2021 18:20:08 GMT
ENV LANG=C.UTF-8
# Fri, 17 Sep 2021 18:20:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635fde6e75efd3bf06de5b8adc0596067708e0eedb7c38ce2aff0a9feb1cf3cc`  
		Last Modified: Fri, 17 Sep 2021 18:21:34 GMT  
		Size: 151.6 MB (151580504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17.0.0` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:afa3611ea4bda1ed87fb662bb08aaf18753860a8cccd55c9e4c173035abf6bce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.6 MB (213561011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6784df627675ec02f3c13c966491ff522d95e0313af01de2d514a95863b06af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Fri, 17 Sep 2021 18:39:43 GMT
ARG version=17.0.0.35-1
# Fri, 17 Sep 2021 18:40:04 GMT
# ARGS: version=17.0.0.35-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 17 Sep 2021 18:40:04 GMT
ENV LANG=C.UTF-8
# Fri, 17 Sep 2021 18:40:05 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e542c9ec83cb03f286aa01111e95fc150024f9a3b3aac06f1ced16b03bafe445`  
		Last Modified: Fri, 17 Sep 2021 18:41:24 GMT  
		Size: 150.1 MB (150130209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:17.0.0-al2`

```console
$ docker pull amazoncorretto@sha256:175957b964349d8d75850e43603cf65f740ced597faed22ee7db4f575a841d4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17.0.0-al2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:e0fc6d3ddca7584f723d25870c58c7c5a7c71935699f7577d24150bbfe1f5a1d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.6 MB (213580807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa37b839189a8440ab7c82fd0b0f6efa23178842ca51421ac930153cf456e764`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Fri, 17 Sep 2021 18:19:45 GMT
ARG version=17.0.0.35-1
# Fri, 17 Sep 2021 18:20:07 GMT
# ARGS: version=17.0.0.35-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 17 Sep 2021 18:20:08 GMT
ENV LANG=C.UTF-8
# Fri, 17 Sep 2021 18:20:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635fde6e75efd3bf06de5b8adc0596067708e0eedb7c38ce2aff0a9feb1cf3cc`  
		Last Modified: Fri, 17 Sep 2021 18:21:34 GMT  
		Size: 151.6 MB (151580504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17.0.0-al2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:afa3611ea4bda1ed87fb662bb08aaf18753860a8cccd55c9e4c173035abf6bce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.6 MB (213561011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6784df627675ec02f3c13c966491ff522d95e0313af01de2d514a95863b06af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Fri, 17 Sep 2021 18:39:43 GMT
ARG version=17.0.0.35-1
# Fri, 17 Sep 2021 18:40:04 GMT
# ARGS: version=17.0.0.35-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 17 Sep 2021 18:40:04 GMT
ENV LANG=C.UTF-8
# Fri, 17 Sep 2021 18:40:05 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e542c9ec83cb03f286aa01111e95fc150024f9a3b3aac06f1ced16b03bafe445`  
		Last Modified: Fri, 17 Sep 2021 18:41:24 GMT  
		Size: 150.1 MB (150130209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:17.0.0-alpine`

```console
$ docker pull amazoncorretto@sha256:d4715e627365f5a1487ece0a87f1ad4dcf67eddf0ae937fd61f43e57c347eb41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17.0.0-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4f0aaacb432a483fb06b79567ee74a5b7ce7218625e05ded20a3d057de92e75a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.9 MB (198930683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4a8136cf53529ca159d604c8a823ab34c17f77986ebb604be5dec7f0e20740b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 17 Sep 2021 18:20:15 GMT
ARG version=17.0.0.35.1
# Fri, 17 Sep 2021 18:20:23 GMT
# ARGS: version=17.0.0.35.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Fri, 17 Sep 2021 18:20:24 GMT
ENV LANG=C.UTF-8
# Fri, 17 Sep 2021 18:20:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 17 Sep 2021 18:20:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0129aa7f582aeb95bed9cd254e70c135ee2a28bbc71ca382c177eb21b46fb06`  
		Last Modified: Fri, 17 Sep 2021 18:22:06 GMT  
		Size: 196.1 MB (196116237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8`

```console
$ docker pull amazoncorretto@sha256:e175b24aa013564005e9dd989e07066ae58d0198d4812358923c60f291b02a01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:816052a72fca894f760da9360f70f2c513e9a2c6383ee59fbd6402ced2747728
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137313556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eb77df6627f2ccc45eee8c98580b72c2c8678e27c2d1bdedf6c72fedd8201d0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 01:05:10 GMT
ARG version=1.8.0_302.b08-1
# Thu, 09 Sep 2021 01:05:32 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 01:05:33 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 01:05:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1def2328938d61155f42900949edc55ba0065dfb89b10b8df6b4345a90dde597`  
		Last Modified: Thu, 09 Sep 2021 01:07:20 GMT  
		Size: 75.3 MB (75313253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:9d4ca5a24062c33c9a4bcb69f9ef1c655c8853e56be46f0d7c23b0715fa3c564
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122834746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0e5a2da64ec62111331620a563b2e6eed82a1195540b135f8b25c11219aaacd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 00:57:15 GMT
ARG version=1.8.0_302.b08-1
# Thu, 09 Sep 2021 00:57:36 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 00:57:36 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 00:57:36 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d7644ce683e6644a778a58cf71d3afd72066587a1faac0efaa43e346216b57`  
		Last Modified: Thu, 09 Sep 2021 00:59:24 GMT  
		Size: 59.4 MB (59403944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-al2-full`

```console
$ docker pull amazoncorretto@sha256:e175b24aa013564005e9dd989e07066ae58d0198d4812358923c60f291b02a01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:816052a72fca894f760da9360f70f2c513e9a2c6383ee59fbd6402ced2747728
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137313556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eb77df6627f2ccc45eee8c98580b72c2c8678e27c2d1bdedf6c72fedd8201d0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 01:05:10 GMT
ARG version=1.8.0_302.b08-1
# Thu, 09 Sep 2021 01:05:32 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 01:05:33 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 01:05:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1def2328938d61155f42900949edc55ba0065dfb89b10b8df6b4345a90dde597`  
		Last Modified: Thu, 09 Sep 2021 01:07:20 GMT  
		Size: 75.3 MB (75313253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:9d4ca5a24062c33c9a4bcb69f9ef1c655c8853e56be46f0d7c23b0715fa3c564
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122834746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0e5a2da64ec62111331620a563b2e6eed82a1195540b135f8b25c11219aaacd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 00:57:15 GMT
ARG version=1.8.0_302.b08-1
# Thu, 09 Sep 2021 00:57:36 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 00:57:36 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 00:57:36 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d7644ce683e6644a778a58cf71d3afd72066587a1faac0efaa43e346216b57`  
		Last Modified: Thu, 09 Sep 2021 00:59:24 GMT  
		Size: 59.4 MB (59403944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:e175b24aa013564005e9dd989e07066ae58d0198d4812358923c60f291b02a01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:816052a72fca894f760da9360f70f2c513e9a2c6383ee59fbd6402ced2747728
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137313556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eb77df6627f2ccc45eee8c98580b72c2c8678e27c2d1bdedf6c72fedd8201d0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 01:05:10 GMT
ARG version=1.8.0_302.b08-1
# Thu, 09 Sep 2021 01:05:32 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 01:05:33 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 01:05:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1def2328938d61155f42900949edc55ba0065dfb89b10b8df6b4345a90dde597`  
		Last Modified: Thu, 09 Sep 2021 01:07:20 GMT  
		Size: 75.3 MB (75313253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:9d4ca5a24062c33c9a4bcb69f9ef1c655c8853e56be46f0d7c23b0715fa3c564
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122834746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0e5a2da64ec62111331620a563b2e6eed82a1195540b135f8b25c11219aaacd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 00:57:15 GMT
ARG version=1.8.0_302.b08-1
# Thu, 09 Sep 2021 00:57:36 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 00:57:36 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 00:57:36 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d7644ce683e6644a778a58cf71d3afd72066587a1faac0efaa43e346216b57`  
		Last Modified: Thu, 09 Sep 2021 00:59:24 GMT  
		Size: 59.4 MB (59403944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine`

```console
$ docker pull amazoncorretto@sha256:999e2b7f9279e0f260329b67bfae43cc994e88d691f7bc96e2d455d67030f1e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:d0450e2743c8ae7b546387eb747fe27ff28caa6a700a2053b68b7d9d0a787573
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101833069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3ceb59abcee83c29f6388844aac2c9745ba11c877e94aa4a1e2dd829000ed8c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:30:26 GMT
ARG version=8.302.08.1
# Wed, 01 Sep 2021 00:30:33 GMT
# ARGS: version=8.302.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Wed, 01 Sep 2021 00:30:34 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 00:30:34 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 01 Sep 2021 00:30:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d34235dfe864bd38e7376e34561b8d34096f5870b751c61514b43013316a413`  
		Last Modified: Wed, 01 Sep 2021 00:32:33 GMT  
		Size: 99.0 MB (99031362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine-full`

```console
$ docker pull amazoncorretto@sha256:999e2b7f9279e0f260329b67bfae43cc994e88d691f7bc96e2d455d67030f1e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:d0450e2743c8ae7b546387eb747fe27ff28caa6a700a2053b68b7d9d0a787573
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101833069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3ceb59abcee83c29f6388844aac2c9745ba11c877e94aa4a1e2dd829000ed8c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:30:26 GMT
ARG version=8.302.08.1
# Wed, 01 Sep 2021 00:30:33 GMT
# ARGS: version=8.302.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Wed, 01 Sep 2021 00:30:34 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 00:30:34 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 01 Sep 2021 00:30:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d34235dfe864bd38e7376e34561b8d34096f5870b751c61514b43013316a413`  
		Last Modified: Wed, 01 Sep 2021 00:32:33 GMT  
		Size: 99.0 MB (99031362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:999e2b7f9279e0f260329b67bfae43cc994e88d691f7bc96e2d455d67030f1e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:d0450e2743c8ae7b546387eb747fe27ff28caa6a700a2053b68b7d9d0a787573
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101833069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3ceb59abcee83c29f6388844aac2c9745ba11c877e94aa4a1e2dd829000ed8c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:30:26 GMT
ARG version=8.302.08.1
# Wed, 01 Sep 2021 00:30:33 GMT
# ARGS: version=8.302.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Wed, 01 Sep 2021 00:30:34 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 00:30:34 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 01 Sep 2021 00:30:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d34235dfe864bd38e7376e34561b8d34096f5870b751c61514b43013316a413`  
		Last Modified: Wed, 01 Sep 2021 00:32:33 GMT  
		Size: 99.0 MB (99031362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine-jre`

```console
$ docker pull amazoncorretto@sha256:194ba48bd933d08ae25ac70cd945695be946c1290709d8e85f6d77a3a30fb880
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:f5308d8d67a303e8cb1ef37e8d5973f8e6cdd5584cb6dc2be33dcdccc47f9ca4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43149754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a694f896151049eacf27770741a8298a444bfa342cc490d54d33bfdce087c9f8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:30:26 GMT
ARG version=8.302.08.1
# Wed, 01 Sep 2021 00:30:44 GMT
# ARGS: version=8.302.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Wed, 01 Sep 2021 00:30:45 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 00:30:45 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123dc5594dbc3dde316acc44a6ee7ec1ecbcb40b936dc192d2fe06fb8e53df18`  
		Last Modified: Wed, 01 Sep 2021 00:32:56 GMT  
		Size: 40.3 MB (40348047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u302`

```console
$ docker pull amazoncorretto@sha256:e175b24aa013564005e9dd989e07066ae58d0198d4812358923c60f291b02a01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u302` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:816052a72fca894f760da9360f70f2c513e9a2c6383ee59fbd6402ced2747728
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137313556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eb77df6627f2ccc45eee8c98580b72c2c8678e27c2d1bdedf6c72fedd8201d0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 01:05:10 GMT
ARG version=1.8.0_302.b08-1
# Thu, 09 Sep 2021 01:05:32 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 01:05:33 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 01:05:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1def2328938d61155f42900949edc55ba0065dfb89b10b8df6b4345a90dde597`  
		Last Modified: Thu, 09 Sep 2021 01:07:20 GMT  
		Size: 75.3 MB (75313253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u302` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:9d4ca5a24062c33c9a4bcb69f9ef1c655c8853e56be46f0d7c23b0715fa3c564
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122834746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0e5a2da64ec62111331620a563b2e6eed82a1195540b135f8b25c11219aaacd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 00:57:15 GMT
ARG version=1.8.0_302.b08-1
# Thu, 09 Sep 2021 00:57:36 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 00:57:36 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 00:57:36 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d7644ce683e6644a778a58cf71d3afd72066587a1faac0efaa43e346216b57`  
		Last Modified: Thu, 09 Sep 2021 00:59:24 GMT  
		Size: 59.4 MB (59403944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u302-al2`

```console
$ docker pull amazoncorretto@sha256:e175b24aa013564005e9dd989e07066ae58d0198d4812358923c60f291b02a01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u302-al2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:816052a72fca894f760da9360f70f2c513e9a2c6383ee59fbd6402ced2747728
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137313556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eb77df6627f2ccc45eee8c98580b72c2c8678e27c2d1bdedf6c72fedd8201d0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 01:05:10 GMT
ARG version=1.8.0_302.b08-1
# Thu, 09 Sep 2021 01:05:32 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 01:05:33 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 01:05:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1def2328938d61155f42900949edc55ba0065dfb89b10b8df6b4345a90dde597`  
		Last Modified: Thu, 09 Sep 2021 01:07:20 GMT  
		Size: 75.3 MB (75313253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u302-al2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:9d4ca5a24062c33c9a4bcb69f9ef1c655c8853e56be46f0d7c23b0715fa3c564
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122834746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0e5a2da64ec62111331620a563b2e6eed82a1195540b135f8b25c11219aaacd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 00:57:15 GMT
ARG version=1.8.0_302.b08-1
# Thu, 09 Sep 2021 00:57:36 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 00:57:36 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 00:57:36 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d7644ce683e6644a778a58cf71d3afd72066587a1faac0efaa43e346216b57`  
		Last Modified: Thu, 09 Sep 2021 00:59:24 GMT  
		Size: 59.4 MB (59403944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u302-alpine`

```console
$ docker pull amazoncorretto@sha256:999e2b7f9279e0f260329b67bfae43cc994e88d691f7bc96e2d455d67030f1e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u302-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:d0450e2743c8ae7b546387eb747fe27ff28caa6a700a2053b68b7d9d0a787573
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101833069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3ceb59abcee83c29f6388844aac2c9745ba11c877e94aa4a1e2dd829000ed8c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:30:26 GMT
ARG version=8.302.08.1
# Wed, 01 Sep 2021 00:30:33 GMT
# ARGS: version=8.302.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Wed, 01 Sep 2021 00:30:34 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 00:30:34 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 01 Sep 2021 00:30:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d34235dfe864bd38e7376e34561b8d34096f5870b751c61514b43013316a413`  
		Last Modified: Wed, 01 Sep 2021 00:32:33 GMT  
		Size: 99.0 MB (99031362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u302-alpine-jre`

```console
$ docker pull amazoncorretto@sha256:194ba48bd933d08ae25ac70cd945695be946c1290709d8e85f6d77a3a30fb880
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u302-alpine-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:f5308d8d67a303e8cb1ef37e8d5973f8e6cdd5584cb6dc2be33dcdccc47f9ca4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43149754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a694f896151049eacf27770741a8298a444bfa342cc490d54d33bfdce087c9f8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:30:26 GMT
ARG version=8.302.08.1
# Wed, 01 Sep 2021 00:30:44 GMT
# ARGS: version=8.302.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Wed, 01 Sep 2021 00:30:45 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 00:30:45 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123dc5594dbc3dde316acc44a6ee7ec1ecbcb40b936dc192d2fe06fb8e53df18`  
		Last Modified: Wed, 01 Sep 2021 00:32:56 GMT  
		Size: 40.3 MB (40348047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:latest`

```console
$ docker pull amazoncorretto@sha256:e175b24aa013564005e9dd989e07066ae58d0198d4812358923c60f291b02a01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:latest` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:816052a72fca894f760da9360f70f2c513e9a2c6383ee59fbd6402ced2747728
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137313556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eb77df6627f2ccc45eee8c98580b72c2c8678e27c2d1bdedf6c72fedd8201d0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 01:05:10 GMT
ARG version=1.8.0_302.b08-1
# Thu, 09 Sep 2021 01:05:32 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 01:05:33 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 01:05:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1def2328938d61155f42900949edc55ba0065dfb89b10b8df6b4345a90dde597`  
		Last Modified: Thu, 09 Sep 2021 01:07:20 GMT  
		Size: 75.3 MB (75313253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:latest` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:9d4ca5a24062c33c9a4bcb69f9ef1c655c8853e56be46f0d7c23b0715fa3c564
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122834746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0e5a2da64ec62111331620a563b2e6eed82a1195540b135f8b25c11219aaacd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 00:57:15 GMT
ARG version=1.8.0_302.b08-1
# Thu, 09 Sep 2021 00:57:36 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 00:57:36 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 00:57:36 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d7644ce683e6644a778a58cf71d3afd72066587a1faac0efaa43e346216b57`  
		Last Modified: Thu, 09 Sep 2021 00:59:24 GMT  
		Size: 59.4 MB (59403944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
