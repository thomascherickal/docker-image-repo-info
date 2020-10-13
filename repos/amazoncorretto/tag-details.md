<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazoncorretto`

-	[`amazoncorretto:11`](#amazoncorretto11)
-	[`amazoncorretto:11.0.8`](#amazoncorretto1108)
-	[`amazoncorretto:11.0.8-al2`](#amazoncorretto1108-al2)
-	[`amazoncorretto:11.0.8-alpine`](#amazoncorretto1108-alpine)
-	[`amazoncorretto:11-al2-full`](#amazoncorretto11-al2-full)
-	[`amazoncorretto:11-al2-jdk`](#amazoncorretto11-al2-jdk)
-	[`amazoncorretto:11-alpine`](#amazoncorretto11-alpine)
-	[`amazoncorretto:11-alpine-full`](#amazoncorretto11-alpine-full)
-	[`amazoncorretto:11-alpine-jdk`](#amazoncorretto11-alpine-jdk)
-	[`amazoncorretto:15`](#amazoncorretto15)
-	[`amazoncorretto:15-al2-full`](#amazoncorretto15-al2-full)
-	[`amazoncorretto:15-al2-jdk`](#amazoncorretto15-al2-jdk)
-	[`amazoncorretto:15-alpine`](#amazoncorretto15-alpine)
-	[`amazoncorretto:15-alpine-full`](#amazoncorretto15-alpine-full)
-	[`amazoncorretto:15-alpine-jdk`](#amazoncorretto15-alpine-jdk)
-	[`amazoncorretto:8`](#amazoncorretto8)
-	[`amazoncorretto:8-al2-full`](#amazoncorretto8-al2-full)
-	[`amazoncorretto:8-al2-jdk`](#amazoncorretto8-al2-jdk)
-	[`amazoncorretto:8-alpine`](#amazoncorretto8-alpine)
-	[`amazoncorretto:8-alpine-full`](#amazoncorretto8-alpine-full)
-	[`amazoncorretto:8-alpine-jdk`](#amazoncorretto8-alpine-jdk)
-	[`amazoncorretto:8-alpine-jre`](#amazoncorretto8-alpine-jre)
-	[`amazoncorretto:8u262-alpine`](#amazoncorretto8u262-alpine)
-	[`amazoncorretto:8u262-alpine-jre`](#amazoncorretto8u262-alpine-jre)
-	[`amazoncorretto:8u265`](#amazoncorretto8u265)
-	[`amazoncorretto:8u265-al2`](#amazoncorretto8u265-al2)
-	[`amazoncorretto:latest`](#amazoncorrettolatest)

## `amazoncorretto:11`

```console
$ docker pull amazoncorretto@sha256:9ef093d153724c89e490856ae323b7e82966b98b4c2ff8d327be8c0c0b020ce9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:f7a7126645e48c54535e36bcae9a7fbeba6fd5fc7dbb0071ce4534cad101616a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.9 MB (206868062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0912c541a67af7a4d7879ac81af6a8ee516ee49ba5bc0005d367101b612499f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 22:43:23 GMT
ARG version=11.0.8.10-1
# Fri, 31 Jul 2020 22:43:47 GMT
# ARGS: version=11.0.8.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 22:43:48 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 22:43:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bf440f7cb963ac775c46ed051bc640e2bff5a973c8f315f7f57b8319f2d261`  
		Last Modified: Fri, 31 Jul 2020 22:44:29 GMT  
		Size: 145.2 MB (145151522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:e8214c624c083bd6e62079474645c3d6228cacee4583f070f14b8919fa076125
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.4 MB (207375737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:985922b918538377309760454a52f9a5b2b94d66ef73e0010e7cc36afe3accc9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 23:01:32 GMT
ARG version=11.0.8.10-1
# Fri, 31 Jul 2020 23:02:07 GMT
# ARGS: version=11.0.8.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 23:02:09 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 23:02:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69b79657d5aea582ebde55909185198144b362fb5dba4bc4c0fed20f8559a17`  
		Last Modified: Fri, 31 Jul 2020 23:03:18 GMT  
		Size: 144.0 MB (144021601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11.0.8`

```console
$ docker pull amazoncorretto@sha256:9ef093d153724c89e490856ae323b7e82966b98b4c2ff8d327be8c0c0b020ce9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11.0.8` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:f7a7126645e48c54535e36bcae9a7fbeba6fd5fc7dbb0071ce4534cad101616a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.9 MB (206868062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0912c541a67af7a4d7879ac81af6a8ee516ee49ba5bc0005d367101b612499f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 22:43:23 GMT
ARG version=11.0.8.10-1
# Fri, 31 Jul 2020 22:43:47 GMT
# ARGS: version=11.0.8.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 22:43:48 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 22:43:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bf440f7cb963ac775c46ed051bc640e2bff5a973c8f315f7f57b8319f2d261`  
		Last Modified: Fri, 31 Jul 2020 22:44:29 GMT  
		Size: 145.2 MB (145151522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11.0.8` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:e8214c624c083bd6e62079474645c3d6228cacee4583f070f14b8919fa076125
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.4 MB (207375737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:985922b918538377309760454a52f9a5b2b94d66ef73e0010e7cc36afe3accc9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 23:01:32 GMT
ARG version=11.0.8.10-1
# Fri, 31 Jul 2020 23:02:07 GMT
# ARGS: version=11.0.8.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 23:02:09 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 23:02:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69b79657d5aea582ebde55909185198144b362fb5dba4bc4c0fed20f8559a17`  
		Last Modified: Fri, 31 Jul 2020 23:03:18 GMT  
		Size: 144.0 MB (144021601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11.0.8-al2`

```console
$ docker pull amazoncorretto@sha256:9ef093d153724c89e490856ae323b7e82966b98b4c2ff8d327be8c0c0b020ce9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11.0.8-al2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:f7a7126645e48c54535e36bcae9a7fbeba6fd5fc7dbb0071ce4534cad101616a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.9 MB (206868062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0912c541a67af7a4d7879ac81af6a8ee516ee49ba5bc0005d367101b612499f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 22:43:23 GMT
ARG version=11.0.8.10-1
# Fri, 31 Jul 2020 22:43:47 GMT
# ARGS: version=11.0.8.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 22:43:48 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 22:43:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bf440f7cb963ac775c46ed051bc640e2bff5a973c8f315f7f57b8319f2d261`  
		Last Modified: Fri, 31 Jul 2020 22:44:29 GMT  
		Size: 145.2 MB (145151522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11.0.8-al2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:e8214c624c083bd6e62079474645c3d6228cacee4583f070f14b8919fa076125
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.4 MB (207375737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:985922b918538377309760454a52f9a5b2b94d66ef73e0010e7cc36afe3accc9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 23:01:32 GMT
ARG version=11.0.8.10-1
# Fri, 31 Jul 2020 23:02:07 GMT
# ARGS: version=11.0.8.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 23:02:09 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 23:02:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69b79657d5aea582ebde55909185198144b362fb5dba4bc4c0fed20f8559a17`  
		Last Modified: Fri, 31 Jul 2020 23:03:18 GMT  
		Size: 144.0 MB (144021601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11.0.8-alpine`

```console
$ docker pull amazoncorretto@sha256:9329870f78d72a47fbf2d6fc32800ad159622a2f278cce49ed1923f5154e9db2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:11.0.8-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:7826ab1e4e2cc8d1ed03e250025145056e5777917ce5c90261a4bf0b4f875927
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.4 MB (194418780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99316547dbe167b2eec207242456b2ad1e42013a878230df4253ff128b42bab4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Wed, 26 Aug 2020 18:20:09 GMT
ARG version=11.0.8.10.1
# Tue, 06 Oct 2020 21:20:08 GMT
# ARGS: version=11.0.8.10.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Tue, 06 Oct 2020 21:20:08 GMT
ENV LANG=C.UTF-8
# Tue, 06 Oct 2020 21:20:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 06 Oct 2020 21:20:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db5cf833ba8b07cbf049e0accc16c06214c8ce6d880df7d5777bfe20e6d6546`  
		Last Modified: Tue, 06 Oct 2020 21:21:10 GMT  
		Size: 191.6 MB (191621239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-al2-full`

```console
$ docker pull amazoncorretto@sha256:9ef093d153724c89e490856ae323b7e82966b98b4c2ff8d327be8c0c0b020ce9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:f7a7126645e48c54535e36bcae9a7fbeba6fd5fc7dbb0071ce4534cad101616a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.9 MB (206868062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0912c541a67af7a4d7879ac81af6a8ee516ee49ba5bc0005d367101b612499f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 22:43:23 GMT
ARG version=11.0.8.10-1
# Fri, 31 Jul 2020 22:43:47 GMT
# ARGS: version=11.0.8.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 22:43:48 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 22:43:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bf440f7cb963ac775c46ed051bc640e2bff5a973c8f315f7f57b8319f2d261`  
		Last Modified: Fri, 31 Jul 2020 22:44:29 GMT  
		Size: 145.2 MB (145151522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:e8214c624c083bd6e62079474645c3d6228cacee4583f070f14b8919fa076125
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.4 MB (207375737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:985922b918538377309760454a52f9a5b2b94d66ef73e0010e7cc36afe3accc9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 23:01:32 GMT
ARG version=11.0.8.10-1
# Fri, 31 Jul 2020 23:02:07 GMT
# ARGS: version=11.0.8.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 23:02:09 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 23:02:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69b79657d5aea582ebde55909185198144b362fb5dba4bc4c0fed20f8559a17`  
		Last Modified: Fri, 31 Jul 2020 23:03:18 GMT  
		Size: 144.0 MB (144021601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:9ef093d153724c89e490856ae323b7e82966b98b4c2ff8d327be8c0c0b020ce9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:f7a7126645e48c54535e36bcae9a7fbeba6fd5fc7dbb0071ce4534cad101616a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.9 MB (206868062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0912c541a67af7a4d7879ac81af6a8ee516ee49ba5bc0005d367101b612499f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 22:43:23 GMT
ARG version=11.0.8.10-1
# Fri, 31 Jul 2020 22:43:47 GMT
# ARGS: version=11.0.8.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 22:43:48 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 22:43:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bf440f7cb963ac775c46ed051bc640e2bff5a973c8f315f7f57b8319f2d261`  
		Last Modified: Fri, 31 Jul 2020 22:44:29 GMT  
		Size: 145.2 MB (145151522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:e8214c624c083bd6e62079474645c3d6228cacee4583f070f14b8919fa076125
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.4 MB (207375737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:985922b918538377309760454a52f9a5b2b94d66ef73e0010e7cc36afe3accc9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 23:01:32 GMT
ARG version=11.0.8.10-1
# Fri, 31 Jul 2020 23:02:07 GMT
# ARGS: version=11.0.8.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 23:02:09 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 23:02:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69b79657d5aea582ebde55909185198144b362fb5dba4bc4c0fed20f8559a17`  
		Last Modified: Fri, 31 Jul 2020 23:03:18 GMT  
		Size: 144.0 MB (144021601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-alpine`

```console
$ docker pull amazoncorretto@sha256:9329870f78d72a47fbf2d6fc32800ad159622a2f278cce49ed1923f5154e9db2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:11-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:7826ab1e4e2cc8d1ed03e250025145056e5777917ce5c90261a4bf0b4f875927
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.4 MB (194418780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99316547dbe167b2eec207242456b2ad1e42013a878230df4253ff128b42bab4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Wed, 26 Aug 2020 18:20:09 GMT
ARG version=11.0.8.10.1
# Tue, 06 Oct 2020 21:20:08 GMT
# ARGS: version=11.0.8.10.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Tue, 06 Oct 2020 21:20:08 GMT
ENV LANG=C.UTF-8
# Tue, 06 Oct 2020 21:20:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 06 Oct 2020 21:20:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db5cf833ba8b07cbf049e0accc16c06214c8ce6d880df7d5777bfe20e6d6546`  
		Last Modified: Tue, 06 Oct 2020 21:21:10 GMT  
		Size: 191.6 MB (191621239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-alpine-full`

```console
$ docker pull amazoncorretto@sha256:9329870f78d72a47fbf2d6fc32800ad159622a2f278cce49ed1923f5154e9db2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:11-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:7826ab1e4e2cc8d1ed03e250025145056e5777917ce5c90261a4bf0b4f875927
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.4 MB (194418780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99316547dbe167b2eec207242456b2ad1e42013a878230df4253ff128b42bab4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Wed, 26 Aug 2020 18:20:09 GMT
ARG version=11.0.8.10.1
# Tue, 06 Oct 2020 21:20:08 GMT
# ARGS: version=11.0.8.10.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Tue, 06 Oct 2020 21:20:08 GMT
ENV LANG=C.UTF-8
# Tue, 06 Oct 2020 21:20:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 06 Oct 2020 21:20:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db5cf833ba8b07cbf049e0accc16c06214c8ce6d880df7d5777bfe20e6d6546`  
		Last Modified: Tue, 06 Oct 2020 21:21:10 GMT  
		Size: 191.6 MB (191621239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:9329870f78d72a47fbf2d6fc32800ad159622a2f278cce49ed1923f5154e9db2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:11-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:7826ab1e4e2cc8d1ed03e250025145056e5777917ce5c90261a4bf0b4f875927
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.4 MB (194418780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99316547dbe167b2eec207242456b2ad1e42013a878230df4253ff128b42bab4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Wed, 26 Aug 2020 18:20:09 GMT
ARG version=11.0.8.10.1
# Tue, 06 Oct 2020 21:20:08 GMT
# ARGS: version=11.0.8.10.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Tue, 06 Oct 2020 21:20:08 GMT
ENV LANG=C.UTF-8
# Tue, 06 Oct 2020 21:20:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 06 Oct 2020 21:20:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db5cf833ba8b07cbf049e0accc16c06214c8ce6d880df7d5777bfe20e6d6546`  
		Last Modified: Tue, 06 Oct 2020 21:21:10 GMT  
		Size: 191.6 MB (191621239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15`

```console
$ docker pull amazoncorretto@sha256:df04cb1319a2c5d2fd0ef20b3a2c3bf7bdb66898f12843f667948f2435f23b60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:15` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:5ca527dc41ba6947e6ca81a944a3e0b3065ba530a40c04df37d6b39298881292
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.3 MB (217321840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:490bde902fa3a33e5a5e0aab40c6333eaa3ea13574e97827cdcd6003c2557568`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Mon, 12 Oct 2020 23:19:29 GMT
ARG version=15.0.0.36-1
# Mon, 12 Oct 2020 23:19:55 GMT
# ARGS: version=15.0.0.36-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 12 Oct 2020 23:19:55 GMT
ENV LANG=C.UTF-8
# Mon, 12 Oct 2020 23:19:56 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2854c7d8fc6af180bfd359fa713f1ca4977a1aa067ede0c5fb3750c9e8dd7f6b`  
		Last Modified: Mon, 12 Oct 2020 23:21:10 GMT  
		Size: 155.6 MB (155605300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:15` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:e4d52794e15ee02085555784e477eb1de6061dba4bcd9fa44173156cd9768645
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.8 MB (218839873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694d0842ba570a080b6465355d894bb98325324ba18d9005061b06c63b47345c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Mon, 12 Oct 2020 23:52:59 GMT
ARG version=15.0.0.36-1
# Mon, 12 Oct 2020 23:53:44 GMT
# ARGS: version=15.0.0.36-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 12 Oct 2020 23:53:46 GMT
ENV LANG=C.UTF-8
# Mon, 12 Oct 2020 23:53:46 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9cec919617a88eeabffbf23ba397a8d0242ca3c914df2b6bd7d7b0e73b12e6`  
		Last Modified: Mon, 12 Oct 2020 23:54:34 GMT  
		Size: 155.5 MB (155485737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15-al2-full`

```console
$ docker pull amazoncorretto@sha256:df04cb1319a2c5d2fd0ef20b3a2c3bf7bdb66898f12843f667948f2435f23b60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:15-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:5ca527dc41ba6947e6ca81a944a3e0b3065ba530a40c04df37d6b39298881292
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.3 MB (217321840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:490bde902fa3a33e5a5e0aab40c6333eaa3ea13574e97827cdcd6003c2557568`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Mon, 12 Oct 2020 23:19:29 GMT
ARG version=15.0.0.36-1
# Mon, 12 Oct 2020 23:19:55 GMT
# ARGS: version=15.0.0.36-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 12 Oct 2020 23:19:55 GMT
ENV LANG=C.UTF-8
# Mon, 12 Oct 2020 23:19:56 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2854c7d8fc6af180bfd359fa713f1ca4977a1aa067ede0c5fb3750c9e8dd7f6b`  
		Last Modified: Mon, 12 Oct 2020 23:21:10 GMT  
		Size: 155.6 MB (155605300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:15-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:e4d52794e15ee02085555784e477eb1de6061dba4bcd9fa44173156cd9768645
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.8 MB (218839873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694d0842ba570a080b6465355d894bb98325324ba18d9005061b06c63b47345c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Mon, 12 Oct 2020 23:52:59 GMT
ARG version=15.0.0.36-1
# Mon, 12 Oct 2020 23:53:44 GMT
# ARGS: version=15.0.0.36-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 12 Oct 2020 23:53:46 GMT
ENV LANG=C.UTF-8
# Mon, 12 Oct 2020 23:53:46 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9cec919617a88eeabffbf23ba397a8d0242ca3c914df2b6bd7d7b0e73b12e6`  
		Last Modified: Mon, 12 Oct 2020 23:54:34 GMT  
		Size: 155.5 MB (155485737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:df04cb1319a2c5d2fd0ef20b3a2c3bf7bdb66898f12843f667948f2435f23b60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:15-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:5ca527dc41ba6947e6ca81a944a3e0b3065ba530a40c04df37d6b39298881292
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.3 MB (217321840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:490bde902fa3a33e5a5e0aab40c6333eaa3ea13574e97827cdcd6003c2557568`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Mon, 12 Oct 2020 23:19:29 GMT
ARG version=15.0.0.36-1
# Mon, 12 Oct 2020 23:19:55 GMT
# ARGS: version=15.0.0.36-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 12 Oct 2020 23:19:55 GMT
ENV LANG=C.UTF-8
# Mon, 12 Oct 2020 23:19:56 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2854c7d8fc6af180bfd359fa713f1ca4977a1aa067ede0c5fb3750c9e8dd7f6b`  
		Last Modified: Mon, 12 Oct 2020 23:21:10 GMT  
		Size: 155.6 MB (155605300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:15-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:e4d52794e15ee02085555784e477eb1de6061dba4bcd9fa44173156cd9768645
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.8 MB (218839873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694d0842ba570a080b6465355d894bb98325324ba18d9005061b06c63b47345c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Mon, 12 Oct 2020 23:52:59 GMT
ARG version=15.0.0.36-1
# Mon, 12 Oct 2020 23:53:44 GMT
# ARGS: version=15.0.0.36-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 12 Oct 2020 23:53:46 GMT
ENV LANG=C.UTF-8
# Mon, 12 Oct 2020 23:53:46 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9cec919617a88eeabffbf23ba397a8d0242ca3c914df2b6bd7d7b0e73b12e6`  
		Last Modified: Mon, 12 Oct 2020 23:54:34 GMT  
		Size: 155.5 MB (155485737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15-alpine`

```console
$ docker pull amazoncorretto@sha256:bc52c0002cf2982ff8a3635e4abcd1d7075ac4fbe1348446e812a7b49bc6ae02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:15-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:2610ccc798acfabc6fe0eaabc826791dc5c247838248ba6bb68d96d26427ec55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.7 MB (207694943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26ea94061bc9b4edc8bb17a4ce9960b1c9ffdfc9e996f4c35eb444d61688c057`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 12 Oct 2020 23:20:14 GMT
ARG version=15.0.0.36.1
# Mon, 12 Oct 2020 23:20:24 GMT
# ARGS: version=15.0.0.36.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-15=$version-r0
# Mon, 12 Oct 2020 23:20:24 GMT
ENV LANG=C.UTF-8
# Mon, 12 Oct 2020 23:20:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 12 Oct 2020 23:20:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a7ca4ddf82070ebcb8ebb450bf522384130967f4d6dbe499f850cd869adaa2`  
		Last Modified: Mon, 12 Oct 2020 23:21:50 GMT  
		Size: 204.9 MB (204897402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15-alpine-full`

```console
$ docker pull amazoncorretto@sha256:bc52c0002cf2982ff8a3635e4abcd1d7075ac4fbe1348446e812a7b49bc6ae02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:15-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:2610ccc798acfabc6fe0eaabc826791dc5c247838248ba6bb68d96d26427ec55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.7 MB (207694943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26ea94061bc9b4edc8bb17a4ce9960b1c9ffdfc9e996f4c35eb444d61688c057`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 12 Oct 2020 23:20:14 GMT
ARG version=15.0.0.36.1
# Mon, 12 Oct 2020 23:20:24 GMT
# ARGS: version=15.0.0.36.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-15=$version-r0
# Mon, 12 Oct 2020 23:20:24 GMT
ENV LANG=C.UTF-8
# Mon, 12 Oct 2020 23:20:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 12 Oct 2020 23:20:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a7ca4ddf82070ebcb8ebb450bf522384130967f4d6dbe499f850cd869adaa2`  
		Last Modified: Mon, 12 Oct 2020 23:21:50 GMT  
		Size: 204.9 MB (204897402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:bc52c0002cf2982ff8a3635e4abcd1d7075ac4fbe1348446e812a7b49bc6ae02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:15-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:2610ccc798acfabc6fe0eaabc826791dc5c247838248ba6bb68d96d26427ec55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.7 MB (207694943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26ea94061bc9b4edc8bb17a4ce9960b1c9ffdfc9e996f4c35eb444d61688c057`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 12 Oct 2020 23:20:14 GMT
ARG version=15.0.0.36.1
# Mon, 12 Oct 2020 23:20:24 GMT
# ARGS: version=15.0.0.36.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-15=$version-r0
# Mon, 12 Oct 2020 23:20:24 GMT
ENV LANG=C.UTF-8
# Mon, 12 Oct 2020 23:20:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 12 Oct 2020 23:20:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a7ca4ddf82070ebcb8ebb450bf522384130967f4d6dbe499f850cd869adaa2`  
		Last Modified: Mon, 12 Oct 2020 23:21:50 GMT  
		Size: 204.9 MB (204897402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8`

```console
$ docker pull amazoncorretto@sha256:e13c7e7853cca113c6336297f46ec10512192926ef42d958698251f23583b393
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:f1f253dd5be74598ade8a7a7d9c100a06046928a14c8ff573be94daa5ae5f123
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136684178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9af30af8ca03289fbf53d120cd092435f7ef329d9b1c4575fd8d9b64a10e46f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 22:42:53 GMT
ARG version=1.8.0_265.b01-1
# Fri, 31 Jul 2020 22:43:15 GMT
# ARGS: version=1.8.0_265.b01-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 22:43:15 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 22:43:15 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0ac67ad9e0cff3afe4e22f26152734ff4f5938fd301e98bb95e8fe5a84ab3e`  
		Last Modified: Fri, 31 Jul 2020 22:44:09 GMT  
		Size: 75.0 MB (74967638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:1f6e2c8e4b3c635259019b081780b81949ed0c01d2394e9a57917e3a8fe7df80
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122386271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d486d9755457dd2503ed1d1d5017d4bdc92d6b628684939956a94bc6e7dba5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 23:00:43 GMT
ARG version=1.8.0_265.b01-1
# Fri, 31 Jul 2020 23:01:20 GMT
# ARGS: version=1.8.0_265.b01-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 23:01:21 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 23:01:22 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c06f2af458d5f17f4008a4870b2a52c7ede41d84afe60328d1bad9611597a15`  
		Last Modified: Fri, 31 Jul 2020 23:02:42 GMT  
		Size: 59.0 MB (59032135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-al2-full`

```console
$ docker pull amazoncorretto@sha256:e13c7e7853cca113c6336297f46ec10512192926ef42d958698251f23583b393
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:f1f253dd5be74598ade8a7a7d9c100a06046928a14c8ff573be94daa5ae5f123
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136684178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9af30af8ca03289fbf53d120cd092435f7ef329d9b1c4575fd8d9b64a10e46f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 22:42:53 GMT
ARG version=1.8.0_265.b01-1
# Fri, 31 Jul 2020 22:43:15 GMT
# ARGS: version=1.8.0_265.b01-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 22:43:15 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 22:43:15 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0ac67ad9e0cff3afe4e22f26152734ff4f5938fd301e98bb95e8fe5a84ab3e`  
		Last Modified: Fri, 31 Jul 2020 22:44:09 GMT  
		Size: 75.0 MB (74967638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:1f6e2c8e4b3c635259019b081780b81949ed0c01d2394e9a57917e3a8fe7df80
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122386271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d486d9755457dd2503ed1d1d5017d4bdc92d6b628684939956a94bc6e7dba5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 23:00:43 GMT
ARG version=1.8.0_265.b01-1
# Fri, 31 Jul 2020 23:01:20 GMT
# ARGS: version=1.8.0_265.b01-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 23:01:21 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 23:01:22 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c06f2af458d5f17f4008a4870b2a52c7ede41d84afe60328d1bad9611597a15`  
		Last Modified: Fri, 31 Jul 2020 23:02:42 GMT  
		Size: 59.0 MB (59032135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:e13c7e7853cca113c6336297f46ec10512192926ef42d958698251f23583b393
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:f1f253dd5be74598ade8a7a7d9c100a06046928a14c8ff573be94daa5ae5f123
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136684178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9af30af8ca03289fbf53d120cd092435f7ef329d9b1c4575fd8d9b64a10e46f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 22:42:53 GMT
ARG version=1.8.0_265.b01-1
# Fri, 31 Jul 2020 22:43:15 GMT
# ARGS: version=1.8.0_265.b01-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 22:43:15 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 22:43:15 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0ac67ad9e0cff3afe4e22f26152734ff4f5938fd301e98bb95e8fe5a84ab3e`  
		Last Modified: Fri, 31 Jul 2020 22:44:09 GMT  
		Size: 75.0 MB (74967638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:1f6e2c8e4b3c635259019b081780b81949ed0c01d2394e9a57917e3a8fe7df80
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122386271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d486d9755457dd2503ed1d1d5017d4bdc92d6b628684939956a94bc6e7dba5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 23:00:43 GMT
ARG version=1.8.0_265.b01-1
# Fri, 31 Jul 2020 23:01:20 GMT
# ARGS: version=1.8.0_265.b01-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 23:01:21 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 23:01:22 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c06f2af458d5f17f4008a4870b2a52c7ede41d84afe60328d1bad9611597a15`  
		Last Modified: Fri, 31 Jul 2020 23:02:42 GMT  
		Size: 59.0 MB (59032135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine`

```console
$ docker pull amazoncorretto@sha256:1b23753f9c88f392903e259dfa88f33efd56967a48a2218427c5d5e4c6f25ba2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:08ac0ca81ec0c71147e2dd4bf30ad7a939882608e5d9ea0315e5068ef161612c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100775241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6384a9bae147e34524f30710be28d84434544ec7ae4d040ea385b1b9688f186`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Wed, 26 Aug 2020 18:19:51 GMT
ARG version=8.265.01.2
# Tue, 06 Oct 2020 21:19:49 GMT
# ARGS: version=8.265.01.2
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Tue, 06 Oct 2020 21:19:50 GMT
ENV LANG=C.UTF-8
# Tue, 06 Oct 2020 21:19:50 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 06 Oct 2020 21:19:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28abb265ef054ab569bdf61165437eb5472ff7966dd2bbe4b8b84323df6e8650`  
		Last Modified: Tue, 06 Oct 2020 21:20:37 GMT  
		Size: 98.0 MB (97977700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine-full`

```console
$ docker pull amazoncorretto@sha256:1b23753f9c88f392903e259dfa88f33efd56967a48a2218427c5d5e4c6f25ba2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:08ac0ca81ec0c71147e2dd4bf30ad7a939882608e5d9ea0315e5068ef161612c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100775241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6384a9bae147e34524f30710be28d84434544ec7ae4d040ea385b1b9688f186`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Wed, 26 Aug 2020 18:19:51 GMT
ARG version=8.265.01.2
# Tue, 06 Oct 2020 21:19:49 GMT
# ARGS: version=8.265.01.2
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Tue, 06 Oct 2020 21:19:50 GMT
ENV LANG=C.UTF-8
# Tue, 06 Oct 2020 21:19:50 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 06 Oct 2020 21:19:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28abb265ef054ab569bdf61165437eb5472ff7966dd2bbe4b8b84323df6e8650`  
		Last Modified: Tue, 06 Oct 2020 21:20:37 GMT  
		Size: 98.0 MB (97977700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:1b23753f9c88f392903e259dfa88f33efd56967a48a2218427c5d5e4c6f25ba2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:08ac0ca81ec0c71147e2dd4bf30ad7a939882608e5d9ea0315e5068ef161612c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100775241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6384a9bae147e34524f30710be28d84434544ec7ae4d040ea385b1b9688f186`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Wed, 26 Aug 2020 18:19:51 GMT
ARG version=8.265.01.2
# Tue, 06 Oct 2020 21:19:49 GMT
# ARGS: version=8.265.01.2
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Tue, 06 Oct 2020 21:19:50 GMT
ENV LANG=C.UTF-8
# Tue, 06 Oct 2020 21:19:50 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 06 Oct 2020 21:19:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28abb265ef054ab569bdf61165437eb5472ff7966dd2bbe4b8b84323df6e8650`  
		Last Modified: Tue, 06 Oct 2020 21:20:37 GMT  
		Size: 98.0 MB (97977700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine-jre`

```console
$ docker pull amazoncorretto@sha256:787cc6343f2afb5b4d6dc9a0d2614213dc0d9efa7b0fc83576437db9c19a246b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8-alpine-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:3cca6287f4624a454a193416f3491421910fea976c20b9f42a59fe1ba8f51396
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42196069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f5334b49f68e0ec90bdaaac87196fae0c1373baa10a879fb8654db7a4786358`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Wed, 26 Aug 2020 18:19:51 GMT
ARG version=8.265.01.2
# Tue, 06 Oct 2020 21:19:56 GMT
# ARGS: version=8.265.01.2
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Tue, 06 Oct 2020 21:19:57 GMT
ENV LANG=C.UTF-8
# Tue, 06 Oct 2020 21:19:57 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62388fccdb2d4cd4f2ebc59e5480c280fc56d7569662437e1b74599e213f1b34`  
		Last Modified: Tue, 06 Oct 2020 21:20:49 GMT  
		Size: 39.4 MB (39398528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u262-alpine`

```console
$ docker pull amazoncorretto@sha256:1b23753f9c88f392903e259dfa88f33efd56967a48a2218427c5d5e4c6f25ba2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8u262-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:08ac0ca81ec0c71147e2dd4bf30ad7a939882608e5d9ea0315e5068ef161612c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100775241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6384a9bae147e34524f30710be28d84434544ec7ae4d040ea385b1b9688f186`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Wed, 26 Aug 2020 18:19:51 GMT
ARG version=8.265.01.2
# Tue, 06 Oct 2020 21:19:49 GMT
# ARGS: version=8.265.01.2
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Tue, 06 Oct 2020 21:19:50 GMT
ENV LANG=C.UTF-8
# Tue, 06 Oct 2020 21:19:50 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 06 Oct 2020 21:19:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28abb265ef054ab569bdf61165437eb5472ff7966dd2bbe4b8b84323df6e8650`  
		Last Modified: Tue, 06 Oct 2020 21:20:37 GMT  
		Size: 98.0 MB (97977700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u262-alpine-jre`

```console
$ docker pull amazoncorretto@sha256:787cc6343f2afb5b4d6dc9a0d2614213dc0d9efa7b0fc83576437db9c19a246b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8u262-alpine-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:3cca6287f4624a454a193416f3491421910fea976c20b9f42a59fe1ba8f51396
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42196069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f5334b49f68e0ec90bdaaac87196fae0c1373baa10a879fb8654db7a4786358`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Wed, 26 Aug 2020 18:19:51 GMT
ARG version=8.265.01.2
# Tue, 06 Oct 2020 21:19:56 GMT
# ARGS: version=8.265.01.2
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Tue, 06 Oct 2020 21:19:57 GMT
ENV LANG=C.UTF-8
# Tue, 06 Oct 2020 21:19:57 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62388fccdb2d4cd4f2ebc59e5480c280fc56d7569662437e1b74599e213f1b34`  
		Last Modified: Tue, 06 Oct 2020 21:20:49 GMT  
		Size: 39.4 MB (39398528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u265`

```console
$ docker pull amazoncorretto@sha256:e13c7e7853cca113c6336297f46ec10512192926ef42d958698251f23583b393
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u265` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:f1f253dd5be74598ade8a7a7d9c100a06046928a14c8ff573be94daa5ae5f123
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136684178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9af30af8ca03289fbf53d120cd092435f7ef329d9b1c4575fd8d9b64a10e46f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 22:42:53 GMT
ARG version=1.8.0_265.b01-1
# Fri, 31 Jul 2020 22:43:15 GMT
# ARGS: version=1.8.0_265.b01-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 22:43:15 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 22:43:15 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0ac67ad9e0cff3afe4e22f26152734ff4f5938fd301e98bb95e8fe5a84ab3e`  
		Last Modified: Fri, 31 Jul 2020 22:44:09 GMT  
		Size: 75.0 MB (74967638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u265` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:1f6e2c8e4b3c635259019b081780b81949ed0c01d2394e9a57917e3a8fe7df80
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122386271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d486d9755457dd2503ed1d1d5017d4bdc92d6b628684939956a94bc6e7dba5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 23:00:43 GMT
ARG version=1.8.0_265.b01-1
# Fri, 31 Jul 2020 23:01:20 GMT
# ARGS: version=1.8.0_265.b01-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 23:01:21 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 23:01:22 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c06f2af458d5f17f4008a4870b2a52c7ede41d84afe60328d1bad9611597a15`  
		Last Modified: Fri, 31 Jul 2020 23:02:42 GMT  
		Size: 59.0 MB (59032135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u265-al2`

```console
$ docker pull amazoncorretto@sha256:e13c7e7853cca113c6336297f46ec10512192926ef42d958698251f23583b393
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u265-al2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:f1f253dd5be74598ade8a7a7d9c100a06046928a14c8ff573be94daa5ae5f123
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136684178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9af30af8ca03289fbf53d120cd092435f7ef329d9b1c4575fd8d9b64a10e46f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 22:42:53 GMT
ARG version=1.8.0_265.b01-1
# Fri, 31 Jul 2020 22:43:15 GMT
# ARGS: version=1.8.0_265.b01-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 22:43:15 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 22:43:15 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0ac67ad9e0cff3afe4e22f26152734ff4f5938fd301e98bb95e8fe5a84ab3e`  
		Last Modified: Fri, 31 Jul 2020 22:44:09 GMT  
		Size: 75.0 MB (74967638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u265-al2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:1f6e2c8e4b3c635259019b081780b81949ed0c01d2394e9a57917e3a8fe7df80
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122386271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d486d9755457dd2503ed1d1d5017d4bdc92d6b628684939956a94bc6e7dba5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 23:00:43 GMT
ARG version=1.8.0_265.b01-1
# Fri, 31 Jul 2020 23:01:20 GMT
# ARGS: version=1.8.0_265.b01-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 23:01:21 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 23:01:22 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c06f2af458d5f17f4008a4870b2a52c7ede41d84afe60328d1bad9611597a15`  
		Last Modified: Fri, 31 Jul 2020 23:02:42 GMT  
		Size: 59.0 MB (59032135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:latest`

```console
$ docker pull amazoncorretto@sha256:e13c7e7853cca113c6336297f46ec10512192926ef42d958698251f23583b393
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:latest` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:f1f253dd5be74598ade8a7a7d9c100a06046928a14c8ff573be94daa5ae5f123
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136684178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9af30af8ca03289fbf53d120cd092435f7ef329d9b1c4575fd8d9b64a10e46f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 22:42:53 GMT
ARG version=1.8.0_265.b01-1
# Fri, 31 Jul 2020 22:43:15 GMT
# ARGS: version=1.8.0_265.b01-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 22:43:15 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 22:43:15 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0ac67ad9e0cff3afe4e22f26152734ff4f5938fd301e98bb95e8fe5a84ab3e`  
		Last Modified: Fri, 31 Jul 2020 22:44:09 GMT  
		Size: 75.0 MB (74967638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:latest` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:1f6e2c8e4b3c635259019b081780b81949ed0c01d2394e9a57917e3a8fe7df80
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122386271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d486d9755457dd2503ed1d1d5017d4bdc92d6b628684939956a94bc6e7dba5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 23:00:43 GMT
ARG version=1.8.0_265.b01-1
# Fri, 31 Jul 2020 23:01:20 GMT
# ARGS: version=1.8.0_265.b01-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 31 Jul 2020 23:01:21 GMT
ENV LANG=C.UTF-8
# Fri, 31 Jul 2020 23:01:22 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c06f2af458d5f17f4008a4870b2a52c7ede41d84afe60328d1bad9611597a15`  
		Last Modified: Fri, 31 Jul 2020 23:02:42 GMT  
		Size: 59.0 MB (59032135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
