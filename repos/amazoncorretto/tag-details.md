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
$ docker pull amazoncorretto@sha256:724250743f219901aadb76ae6a27a8668a29c6a0c386741255087225679cce04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:a6f9d92dabbd71daa86e703c5d53e162e012f8c7fd34c064f2889b5b555ff7ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.8 MB (208753364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfe9269e9f22d6251f17ce45d6a1a507783576e1d29fe232cc491be385379df5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:20:24 GMT
ARG version=11.0.12.7-1
# Wed, 21 Jul 2021 00:20:47 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:20:47 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:20:47 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac426d7253aaa8ec4b49b208798a7d7c8cda86ffb0cc7d02bc61a1fabfb0518`  
		Last Modified: Wed, 21 Jul 2021 00:22:44 GMT  
		Size: 146.8 MB (146787358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:2f297a6cba57f6faa23cb73284741102357fbc5d5c7b4ea7f6d4b220f39f81cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.5 MB (207501743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e905ce3d29fd81603085cb2c7cd420b923f696e78d772aee8102a407604e7060`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:39:45 GMT
ARG version=11.0.12.7-1
# Wed, 21 Jul 2021 00:40:04 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:40:04 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:40:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea41d3967e6fc72ca7a70b8846afd61f0043fcb846c06d06eedc019d004bf92e`  
		Last Modified: Wed, 21 Jul 2021 00:41:40 GMT  
		Size: 143.9 MB (143933851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-al2-full`

```console
$ docker pull amazoncorretto@sha256:724250743f219901aadb76ae6a27a8668a29c6a0c386741255087225679cce04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:a6f9d92dabbd71daa86e703c5d53e162e012f8c7fd34c064f2889b5b555ff7ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.8 MB (208753364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfe9269e9f22d6251f17ce45d6a1a507783576e1d29fe232cc491be385379df5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:20:24 GMT
ARG version=11.0.12.7-1
# Wed, 21 Jul 2021 00:20:47 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:20:47 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:20:47 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac426d7253aaa8ec4b49b208798a7d7c8cda86ffb0cc7d02bc61a1fabfb0518`  
		Last Modified: Wed, 21 Jul 2021 00:22:44 GMT  
		Size: 146.8 MB (146787358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:2f297a6cba57f6faa23cb73284741102357fbc5d5c7b4ea7f6d4b220f39f81cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.5 MB (207501743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e905ce3d29fd81603085cb2c7cd420b923f696e78d772aee8102a407604e7060`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:39:45 GMT
ARG version=11.0.12.7-1
# Wed, 21 Jul 2021 00:40:04 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:40:04 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:40:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea41d3967e6fc72ca7a70b8846afd61f0043fcb846c06d06eedc019d004bf92e`  
		Last Modified: Wed, 21 Jul 2021 00:41:40 GMT  
		Size: 143.9 MB (143933851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:724250743f219901aadb76ae6a27a8668a29c6a0c386741255087225679cce04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:a6f9d92dabbd71daa86e703c5d53e162e012f8c7fd34c064f2889b5b555ff7ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.8 MB (208753364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfe9269e9f22d6251f17ce45d6a1a507783576e1d29fe232cc491be385379df5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:20:24 GMT
ARG version=11.0.12.7-1
# Wed, 21 Jul 2021 00:20:47 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:20:47 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:20:47 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac426d7253aaa8ec4b49b208798a7d7c8cda86ffb0cc7d02bc61a1fabfb0518`  
		Last Modified: Wed, 21 Jul 2021 00:22:44 GMT  
		Size: 146.8 MB (146787358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:2f297a6cba57f6faa23cb73284741102357fbc5d5c7b4ea7f6d4b220f39f81cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.5 MB (207501743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e905ce3d29fd81603085cb2c7cd420b923f696e78d772aee8102a407604e7060`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:39:45 GMT
ARG version=11.0.12.7-1
# Wed, 21 Jul 2021 00:40:04 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:40:04 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:40:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea41d3967e6fc72ca7a70b8846afd61f0043fcb846c06d06eedc019d004bf92e`  
		Last Modified: Wed, 21 Jul 2021 00:41:40 GMT  
		Size: 143.9 MB (143933851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-alpine`

```console
$ docker pull amazoncorretto@sha256:bf0a361478158b40d3592ab1cdc8b9c63640e13e22524cecc4805e85039eb565
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:e84fdbf13c8bba52e28de9f845a1fc30866fdf6bba1ff942e35f4c00023991ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.2 MB (196172744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8720e708cea9fc900fd3b0997cad3aa9c4f11da06801c1ee0e235f2fc730ea4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 21 Jul 2021 00:21:10 GMT
ARG version=11.0.12.7.1
# Wed, 21 Jul 2021 00:21:17 GMT
# ARGS: version=11.0.12.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Wed, 21 Jul 2021 00:21:17 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:21:17 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 21 Jul 2021 00:21:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477fef7b3b9fb84dc86e1350700f7c6dfcee763129bea71c593cd7de0c9d516`  
		Last Modified: Wed, 21 Jul 2021 00:23:55 GMT  
		Size: 193.4 MB (193372177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-alpine-full`

```console
$ docker pull amazoncorretto@sha256:bf0a361478158b40d3592ab1cdc8b9c63640e13e22524cecc4805e85039eb565
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:e84fdbf13c8bba52e28de9f845a1fc30866fdf6bba1ff942e35f4c00023991ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.2 MB (196172744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8720e708cea9fc900fd3b0997cad3aa9c4f11da06801c1ee0e235f2fc730ea4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 21 Jul 2021 00:21:10 GMT
ARG version=11.0.12.7.1
# Wed, 21 Jul 2021 00:21:17 GMT
# ARGS: version=11.0.12.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Wed, 21 Jul 2021 00:21:17 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:21:17 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 21 Jul 2021 00:21:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477fef7b3b9fb84dc86e1350700f7c6dfcee763129bea71c593cd7de0c9d516`  
		Last Modified: Wed, 21 Jul 2021 00:23:55 GMT  
		Size: 193.4 MB (193372177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:bf0a361478158b40d3592ab1cdc8b9c63640e13e22524cecc4805e85039eb565
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:e84fdbf13c8bba52e28de9f845a1fc30866fdf6bba1ff942e35f4c00023991ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.2 MB (196172744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8720e708cea9fc900fd3b0997cad3aa9c4f11da06801c1ee0e235f2fc730ea4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 21 Jul 2021 00:21:10 GMT
ARG version=11.0.12.7.1
# Wed, 21 Jul 2021 00:21:17 GMT
# ARGS: version=11.0.12.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Wed, 21 Jul 2021 00:21:17 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:21:17 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 21 Jul 2021 00:21:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477fef7b3b9fb84dc86e1350700f7c6dfcee763129bea71c593cd7de0c9d516`  
		Last Modified: Wed, 21 Jul 2021 00:23:55 GMT  
		Size: 193.4 MB (193372177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11.0.12`

```console
$ docker pull amazoncorretto@sha256:724250743f219901aadb76ae6a27a8668a29c6a0c386741255087225679cce04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11.0.12` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:a6f9d92dabbd71daa86e703c5d53e162e012f8c7fd34c064f2889b5b555ff7ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.8 MB (208753364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfe9269e9f22d6251f17ce45d6a1a507783576e1d29fe232cc491be385379df5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:20:24 GMT
ARG version=11.0.12.7-1
# Wed, 21 Jul 2021 00:20:47 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:20:47 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:20:47 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac426d7253aaa8ec4b49b208798a7d7c8cda86ffb0cc7d02bc61a1fabfb0518`  
		Last Modified: Wed, 21 Jul 2021 00:22:44 GMT  
		Size: 146.8 MB (146787358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11.0.12` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:2f297a6cba57f6faa23cb73284741102357fbc5d5c7b4ea7f6d4b220f39f81cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.5 MB (207501743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e905ce3d29fd81603085cb2c7cd420b923f696e78d772aee8102a407604e7060`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:39:45 GMT
ARG version=11.0.12.7-1
# Wed, 21 Jul 2021 00:40:04 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:40:04 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:40:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea41d3967e6fc72ca7a70b8846afd61f0043fcb846c06d06eedc019d004bf92e`  
		Last Modified: Wed, 21 Jul 2021 00:41:40 GMT  
		Size: 143.9 MB (143933851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11.0.12-al2`

```console
$ docker pull amazoncorretto@sha256:724250743f219901aadb76ae6a27a8668a29c6a0c386741255087225679cce04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11.0.12-al2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:a6f9d92dabbd71daa86e703c5d53e162e012f8c7fd34c064f2889b5b555ff7ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.8 MB (208753364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfe9269e9f22d6251f17ce45d6a1a507783576e1d29fe232cc491be385379df5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:20:24 GMT
ARG version=11.0.12.7-1
# Wed, 21 Jul 2021 00:20:47 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:20:47 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:20:47 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac426d7253aaa8ec4b49b208798a7d7c8cda86ffb0cc7d02bc61a1fabfb0518`  
		Last Modified: Wed, 21 Jul 2021 00:22:44 GMT  
		Size: 146.8 MB (146787358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11.0.12-al2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:2f297a6cba57f6faa23cb73284741102357fbc5d5c7b4ea7f6d4b220f39f81cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.5 MB (207501743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e905ce3d29fd81603085cb2c7cd420b923f696e78d772aee8102a407604e7060`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:39:45 GMT
ARG version=11.0.12.7-1
# Wed, 21 Jul 2021 00:40:04 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:40:04 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:40:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea41d3967e6fc72ca7a70b8846afd61f0043fcb846c06d06eedc019d004bf92e`  
		Last Modified: Wed, 21 Jul 2021 00:41:40 GMT  
		Size: 143.9 MB (143933851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11.0.12-alpine`

```console
$ docker pull amazoncorretto@sha256:bf0a361478158b40d3592ab1cdc8b9c63640e13e22524cecc4805e85039eb565
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11.0.12-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:e84fdbf13c8bba52e28de9f845a1fc30866fdf6bba1ff942e35f4c00023991ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.2 MB (196172744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8720e708cea9fc900fd3b0997cad3aa9c4f11da06801c1ee0e235f2fc730ea4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 21 Jul 2021 00:21:10 GMT
ARG version=11.0.12.7.1
# Wed, 21 Jul 2021 00:21:17 GMT
# ARGS: version=11.0.12.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Wed, 21 Jul 2021 00:21:17 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:21:17 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 21 Jul 2021 00:21:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477fef7b3b9fb84dc86e1350700f7c6dfcee763129bea71c593cd7de0c9d516`  
		Last Modified: Wed, 21 Jul 2021 00:23:55 GMT  
		Size: 193.4 MB (193372177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16`

```console
$ docker pull amazoncorretto@sha256:4cd70fd46abfe11986e9810deac8a85d7614e8c91f70d9922f84deb096233d87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:69884e8bc35a198faabc5262618b9fc5c03ac85801fe1261d032e5e9555cec66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221944577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8afa07247b4363f02d16639253c650aac54a145fa4cca1abfaf03522fe98692e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 18:19:40 GMT
ARG version=16.0.2.7-1
# Mon, 26 Jul 2021 18:20:02 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 26 Jul 2021 18:20:03 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 18:20:03 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aed8a232bf7a40fe973a4cd182928ebe6b7e9c09023452fcf7803138da37056`  
		Last Modified: Mon, 26 Jul 2021 18:21:41 GMT  
		Size: 160.0 MB (159978571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d81b411e5a1d7d53ae526b7c6b3750f9b033ff799a640db9e5d5aabdac819aed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.5 MB (223510361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d21a773d1f1432117d9f554a7f2a5ec59987d64426e5a151da5c4012e86546f5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 17:39:46 GMT
ARG version=16.0.2.7-1
# Mon, 26 Jul 2021 17:40:14 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 26 Jul 2021 17:40:14 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 17:40:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6c00fa286044c267ce902d9051a1210ba685bdeb2e004a2325ab4b854a22e`  
		Last Modified: Mon, 26 Jul 2021 17:41:26 GMT  
		Size: 159.9 MB (159942469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-al2-full`

```console
$ docker pull amazoncorretto@sha256:4cd70fd46abfe11986e9810deac8a85d7614e8c91f70d9922f84deb096233d87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:69884e8bc35a198faabc5262618b9fc5c03ac85801fe1261d032e5e9555cec66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221944577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8afa07247b4363f02d16639253c650aac54a145fa4cca1abfaf03522fe98692e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 18:19:40 GMT
ARG version=16.0.2.7-1
# Mon, 26 Jul 2021 18:20:02 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 26 Jul 2021 18:20:03 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 18:20:03 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aed8a232bf7a40fe973a4cd182928ebe6b7e9c09023452fcf7803138da37056`  
		Last Modified: Mon, 26 Jul 2021 18:21:41 GMT  
		Size: 160.0 MB (159978571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d81b411e5a1d7d53ae526b7c6b3750f9b033ff799a640db9e5d5aabdac819aed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.5 MB (223510361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d21a773d1f1432117d9f554a7f2a5ec59987d64426e5a151da5c4012e86546f5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 17:39:46 GMT
ARG version=16.0.2.7-1
# Mon, 26 Jul 2021 17:40:14 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 26 Jul 2021 17:40:14 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 17:40:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6c00fa286044c267ce902d9051a1210ba685bdeb2e004a2325ab4b854a22e`  
		Last Modified: Mon, 26 Jul 2021 17:41:26 GMT  
		Size: 159.9 MB (159942469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:4cd70fd46abfe11986e9810deac8a85d7614e8c91f70d9922f84deb096233d87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:69884e8bc35a198faabc5262618b9fc5c03ac85801fe1261d032e5e9555cec66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221944577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8afa07247b4363f02d16639253c650aac54a145fa4cca1abfaf03522fe98692e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 18:19:40 GMT
ARG version=16.0.2.7-1
# Mon, 26 Jul 2021 18:20:02 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 26 Jul 2021 18:20:03 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 18:20:03 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aed8a232bf7a40fe973a4cd182928ebe6b7e9c09023452fcf7803138da37056`  
		Last Modified: Mon, 26 Jul 2021 18:21:41 GMT  
		Size: 160.0 MB (159978571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d81b411e5a1d7d53ae526b7c6b3750f9b033ff799a640db9e5d5aabdac819aed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.5 MB (223510361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d21a773d1f1432117d9f554a7f2a5ec59987d64426e5a151da5c4012e86546f5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 17:39:46 GMT
ARG version=16.0.2.7-1
# Mon, 26 Jul 2021 17:40:14 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 26 Jul 2021 17:40:14 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 17:40:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6c00fa286044c267ce902d9051a1210ba685bdeb2e004a2325ab4b854a22e`  
		Last Modified: Mon, 26 Jul 2021 17:41:26 GMT  
		Size: 159.9 MB (159942469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-alpine`

```console
$ docker pull amazoncorretto@sha256:5bbc495064db815b1e9ae3b4f4414bfd1a88312ccb7c70ed757bb95947080c78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:16-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4389c14487b6352cc1791fa3da9fbdb83cfee28d8efcf571b9628236520db39c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.5 MB (212453390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e86a522aee821c91c6ba3e976a752c4c901bd68c983a5fcfabf96e97e86f0e7c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Mon, 26 Jul 2021 18:20:07 GMT
ARG version=16.0.2.7.1
# Mon, 26 Jul 2021 18:20:33 GMT
# ARGS: version=16.0.2.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-16=$version-r0
# Mon, 26 Jul 2021 18:20:34 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 18:20:34 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 26 Jul 2021 18:20:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237e8ec8f6af5a00c2c0ae1aa93844d981ab4cdd90eccb27fb63a64d7b2adaa`  
		Last Modified: Mon, 26 Jul 2021 18:22:19 GMT  
		Size: 209.7 MB (209652823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-alpine-full`

```console
$ docker pull amazoncorretto@sha256:5bbc495064db815b1e9ae3b4f4414bfd1a88312ccb7c70ed757bb95947080c78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:16-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4389c14487b6352cc1791fa3da9fbdb83cfee28d8efcf571b9628236520db39c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.5 MB (212453390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e86a522aee821c91c6ba3e976a752c4c901bd68c983a5fcfabf96e97e86f0e7c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Mon, 26 Jul 2021 18:20:07 GMT
ARG version=16.0.2.7.1
# Mon, 26 Jul 2021 18:20:33 GMT
# ARGS: version=16.0.2.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-16=$version-r0
# Mon, 26 Jul 2021 18:20:34 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 18:20:34 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 26 Jul 2021 18:20:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237e8ec8f6af5a00c2c0ae1aa93844d981ab4cdd90eccb27fb63a64d7b2adaa`  
		Last Modified: Mon, 26 Jul 2021 18:22:19 GMT  
		Size: 209.7 MB (209652823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:5bbc495064db815b1e9ae3b4f4414bfd1a88312ccb7c70ed757bb95947080c78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:16-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4389c14487b6352cc1791fa3da9fbdb83cfee28d8efcf571b9628236520db39c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.5 MB (212453390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e86a522aee821c91c6ba3e976a752c4c901bd68c983a5fcfabf96e97e86f0e7c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Mon, 26 Jul 2021 18:20:07 GMT
ARG version=16.0.2.7.1
# Mon, 26 Jul 2021 18:20:33 GMT
# ARGS: version=16.0.2.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-16=$version-r0
# Mon, 26 Jul 2021 18:20:34 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 18:20:34 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 26 Jul 2021 18:20:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237e8ec8f6af5a00c2c0ae1aa93844d981ab4cdd90eccb27fb63a64d7b2adaa`  
		Last Modified: Mon, 26 Jul 2021 18:22:19 GMT  
		Size: 209.7 MB (209652823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16.0.2`

```console
$ docker pull amazoncorretto@sha256:4cd70fd46abfe11986e9810deac8a85d7614e8c91f70d9922f84deb096233d87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16.0.2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:69884e8bc35a198faabc5262618b9fc5c03ac85801fe1261d032e5e9555cec66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221944577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8afa07247b4363f02d16639253c650aac54a145fa4cca1abfaf03522fe98692e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 18:19:40 GMT
ARG version=16.0.2.7-1
# Mon, 26 Jul 2021 18:20:02 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 26 Jul 2021 18:20:03 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 18:20:03 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aed8a232bf7a40fe973a4cd182928ebe6b7e9c09023452fcf7803138da37056`  
		Last Modified: Mon, 26 Jul 2021 18:21:41 GMT  
		Size: 160.0 MB (159978571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16.0.2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d81b411e5a1d7d53ae526b7c6b3750f9b033ff799a640db9e5d5aabdac819aed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.5 MB (223510361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d21a773d1f1432117d9f554a7f2a5ec59987d64426e5a151da5c4012e86546f5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 17:39:46 GMT
ARG version=16.0.2.7-1
# Mon, 26 Jul 2021 17:40:14 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 26 Jul 2021 17:40:14 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 17:40:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6c00fa286044c267ce902d9051a1210ba685bdeb2e004a2325ab4b854a22e`  
		Last Modified: Mon, 26 Jul 2021 17:41:26 GMT  
		Size: 159.9 MB (159942469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16.0.2-al2`

```console
$ docker pull amazoncorretto@sha256:4cd70fd46abfe11986e9810deac8a85d7614e8c91f70d9922f84deb096233d87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16.0.2-al2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:69884e8bc35a198faabc5262618b9fc5c03ac85801fe1261d032e5e9555cec66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221944577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8afa07247b4363f02d16639253c650aac54a145fa4cca1abfaf03522fe98692e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 18:19:40 GMT
ARG version=16.0.2.7-1
# Mon, 26 Jul 2021 18:20:02 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 26 Jul 2021 18:20:03 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 18:20:03 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aed8a232bf7a40fe973a4cd182928ebe6b7e9c09023452fcf7803138da37056`  
		Last Modified: Mon, 26 Jul 2021 18:21:41 GMT  
		Size: 160.0 MB (159978571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16.0.2-al2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d81b411e5a1d7d53ae526b7c6b3750f9b033ff799a640db9e5d5aabdac819aed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.5 MB (223510361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d21a773d1f1432117d9f554a7f2a5ec59987d64426e5a151da5c4012e86546f5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 17:39:46 GMT
ARG version=16.0.2.7-1
# Mon, 26 Jul 2021 17:40:14 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 26 Jul 2021 17:40:14 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 17:40:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6c00fa286044c267ce902d9051a1210ba685bdeb2e004a2325ab4b854a22e`  
		Last Modified: Mon, 26 Jul 2021 17:41:26 GMT  
		Size: 159.9 MB (159942469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16.0.2-alpine`

```console
$ docker pull amazoncorretto@sha256:5bbc495064db815b1e9ae3b4f4414bfd1a88312ccb7c70ed757bb95947080c78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:16.0.2-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4389c14487b6352cc1791fa3da9fbdb83cfee28d8efcf571b9628236520db39c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.5 MB (212453390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e86a522aee821c91c6ba3e976a752c4c901bd68c983a5fcfabf96e97e86f0e7c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Mon, 26 Jul 2021 18:20:07 GMT
ARG version=16.0.2.7.1
# Mon, 26 Jul 2021 18:20:33 GMT
# ARGS: version=16.0.2.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-16=$version-r0
# Mon, 26 Jul 2021 18:20:34 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 18:20:34 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 26 Jul 2021 18:20:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237e8ec8f6af5a00c2c0ae1aa93844d981ab4cdd90eccb27fb63a64d7b2adaa`  
		Last Modified: Mon, 26 Jul 2021 18:22:19 GMT  
		Size: 209.7 MB (209652823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8`

```console
$ docker pull amazoncorretto@sha256:e517b1051888b935855f19740cdd69faf76b1a5eb5f6ea8c34989c04671f91fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:99383180a63638b69ccce247aa6b7dbb770cf2b108e0d219f0b5f0c9a4e7299f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137299042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df1c4e3803af8fd91c9b8a4f45546ba5c654ab65a15b1e7bff1627cba43a1fd0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:19:58 GMT
ARG version=1.8.0_302.b08-1
# Wed, 28 Jul 2021 23:19:45 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Jul 2021 23:19:46 GMT
ENV LANG=C.UTF-8
# Wed, 28 Jul 2021 23:19:46 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed3eb17202682b67a716d65d9a7b156337c35c258c7d56eaf2f6025921237a4`  
		Last Modified: Wed, 28 Jul 2021 23:20:45 GMT  
		Size: 75.3 MB (75333036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:c3ae270b98b9fe18e7eda62aede47ca5834bc4ad804e848b5c0d590e0f36b7c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122952748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee3949d0817afd993fb56e0c6cb2c60acbb4815eec064750beeb2379fc2c090c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:39:20 GMT
ARG version=1.8.0_302.b08-1
# Wed, 28 Jul 2021 23:39:42 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Jul 2021 23:39:42 GMT
ENV LANG=C.UTF-8
# Wed, 28 Jul 2021 23:39:42 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5230c70e909e8047c9eadb7a1e0fecdf1baf98003a2f6a56063922975157258e`  
		Last Modified: Wed, 28 Jul 2021 23:40:44 GMT  
		Size: 59.4 MB (59384856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-al2-full`

```console
$ docker pull amazoncorretto@sha256:e517b1051888b935855f19740cdd69faf76b1a5eb5f6ea8c34989c04671f91fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:99383180a63638b69ccce247aa6b7dbb770cf2b108e0d219f0b5f0c9a4e7299f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137299042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df1c4e3803af8fd91c9b8a4f45546ba5c654ab65a15b1e7bff1627cba43a1fd0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:19:58 GMT
ARG version=1.8.0_302.b08-1
# Wed, 28 Jul 2021 23:19:45 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Jul 2021 23:19:46 GMT
ENV LANG=C.UTF-8
# Wed, 28 Jul 2021 23:19:46 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed3eb17202682b67a716d65d9a7b156337c35c258c7d56eaf2f6025921237a4`  
		Last Modified: Wed, 28 Jul 2021 23:20:45 GMT  
		Size: 75.3 MB (75333036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:c3ae270b98b9fe18e7eda62aede47ca5834bc4ad804e848b5c0d590e0f36b7c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122952748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee3949d0817afd993fb56e0c6cb2c60acbb4815eec064750beeb2379fc2c090c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:39:20 GMT
ARG version=1.8.0_302.b08-1
# Wed, 28 Jul 2021 23:39:42 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Jul 2021 23:39:42 GMT
ENV LANG=C.UTF-8
# Wed, 28 Jul 2021 23:39:42 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5230c70e909e8047c9eadb7a1e0fecdf1baf98003a2f6a56063922975157258e`  
		Last Modified: Wed, 28 Jul 2021 23:40:44 GMT  
		Size: 59.4 MB (59384856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:e517b1051888b935855f19740cdd69faf76b1a5eb5f6ea8c34989c04671f91fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:99383180a63638b69ccce247aa6b7dbb770cf2b108e0d219f0b5f0c9a4e7299f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137299042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df1c4e3803af8fd91c9b8a4f45546ba5c654ab65a15b1e7bff1627cba43a1fd0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:19:58 GMT
ARG version=1.8.0_302.b08-1
# Wed, 28 Jul 2021 23:19:45 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Jul 2021 23:19:46 GMT
ENV LANG=C.UTF-8
# Wed, 28 Jul 2021 23:19:46 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed3eb17202682b67a716d65d9a7b156337c35c258c7d56eaf2f6025921237a4`  
		Last Modified: Wed, 28 Jul 2021 23:20:45 GMT  
		Size: 75.3 MB (75333036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:c3ae270b98b9fe18e7eda62aede47ca5834bc4ad804e848b5c0d590e0f36b7c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122952748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee3949d0817afd993fb56e0c6cb2c60acbb4815eec064750beeb2379fc2c090c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:39:20 GMT
ARG version=1.8.0_302.b08-1
# Wed, 28 Jul 2021 23:39:42 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Jul 2021 23:39:42 GMT
ENV LANG=C.UTF-8
# Wed, 28 Jul 2021 23:39:42 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5230c70e909e8047c9eadb7a1e0fecdf1baf98003a2f6a56063922975157258e`  
		Last Modified: Wed, 28 Jul 2021 23:40:44 GMT  
		Size: 59.4 MB (59384856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine`

```console
$ docker pull amazoncorretto@sha256:b97cd4e1f357a3d445db6d1566838a6c91b312cea4085ecc791370ac288860d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4edb6c988dbd6611a208f16ec06ee915289808745e32fe27691026a64519229d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101831898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93854338cb3296eb3934ba3706b7ce61dcf904607e3f9fd4139583c5aa4739bb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 21 Jul 2021 00:20:54 GMT
ARG version=8.302.08.1
# Wed, 21 Jul 2021 00:21:00 GMT
# ARGS: version=8.302.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Wed, 21 Jul 2021 00:21:00 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:21:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 21 Jul 2021 00:21:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f141ea8c2ff0050b64f199d6c95d96fef7a0e9f7daac05c2ff20af6a7e0f25`  
		Last Modified: Wed, 21 Jul 2021 00:23:11 GMT  
		Size: 99.0 MB (99031331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine-full`

```console
$ docker pull amazoncorretto@sha256:b97cd4e1f357a3d445db6d1566838a6c91b312cea4085ecc791370ac288860d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4edb6c988dbd6611a208f16ec06ee915289808745e32fe27691026a64519229d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101831898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93854338cb3296eb3934ba3706b7ce61dcf904607e3f9fd4139583c5aa4739bb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 21 Jul 2021 00:20:54 GMT
ARG version=8.302.08.1
# Wed, 21 Jul 2021 00:21:00 GMT
# ARGS: version=8.302.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Wed, 21 Jul 2021 00:21:00 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:21:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 21 Jul 2021 00:21:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f141ea8c2ff0050b64f199d6c95d96fef7a0e9f7daac05c2ff20af6a7e0f25`  
		Last Modified: Wed, 21 Jul 2021 00:23:11 GMT  
		Size: 99.0 MB (99031331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:b97cd4e1f357a3d445db6d1566838a6c91b312cea4085ecc791370ac288860d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4edb6c988dbd6611a208f16ec06ee915289808745e32fe27691026a64519229d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101831898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93854338cb3296eb3934ba3706b7ce61dcf904607e3f9fd4139583c5aa4739bb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 21 Jul 2021 00:20:54 GMT
ARG version=8.302.08.1
# Wed, 21 Jul 2021 00:21:00 GMT
# ARGS: version=8.302.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Wed, 21 Jul 2021 00:21:00 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:21:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 21 Jul 2021 00:21:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f141ea8c2ff0050b64f199d6c95d96fef7a0e9f7daac05c2ff20af6a7e0f25`  
		Last Modified: Wed, 21 Jul 2021 00:23:11 GMT  
		Size: 99.0 MB (99031331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine-jre`

```console
$ docker pull amazoncorretto@sha256:2c978d2e5921d10abf49c845a2a46b502544c15e2ca733d7b552b350aa691068
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:ff95ea78ce154abaa581bf382295bacf13c0474357ef144fcd96ac1d6d5e851d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43148477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7543a33c551dd671bf563addcbfbf76cc5a3020d86a8479847202e8bd0b5dce1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 21 Jul 2021 00:20:54 GMT
ARG version=8.302.08.1
# Wed, 21 Jul 2021 00:21:07 GMT
# ARGS: version=8.302.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Wed, 21 Jul 2021 00:21:07 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:21:07 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be776a268f00c1a39cc8385fff8b6582ba6d26a76a929e1f13dbdf0208d73520`  
		Last Modified: Wed, 21 Jul 2021 00:23:31 GMT  
		Size: 40.3 MB (40347910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u302`

```console
$ docker pull amazoncorretto@sha256:e517b1051888b935855f19740cdd69faf76b1a5eb5f6ea8c34989c04671f91fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u302` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:99383180a63638b69ccce247aa6b7dbb770cf2b108e0d219f0b5f0c9a4e7299f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137299042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df1c4e3803af8fd91c9b8a4f45546ba5c654ab65a15b1e7bff1627cba43a1fd0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:19:58 GMT
ARG version=1.8.0_302.b08-1
# Wed, 28 Jul 2021 23:19:45 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Jul 2021 23:19:46 GMT
ENV LANG=C.UTF-8
# Wed, 28 Jul 2021 23:19:46 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed3eb17202682b67a716d65d9a7b156337c35c258c7d56eaf2f6025921237a4`  
		Last Modified: Wed, 28 Jul 2021 23:20:45 GMT  
		Size: 75.3 MB (75333036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u302` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:c3ae270b98b9fe18e7eda62aede47ca5834bc4ad804e848b5c0d590e0f36b7c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122952748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee3949d0817afd993fb56e0c6cb2c60acbb4815eec064750beeb2379fc2c090c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:39:20 GMT
ARG version=1.8.0_302.b08-1
# Wed, 28 Jul 2021 23:39:42 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Jul 2021 23:39:42 GMT
ENV LANG=C.UTF-8
# Wed, 28 Jul 2021 23:39:42 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5230c70e909e8047c9eadb7a1e0fecdf1baf98003a2f6a56063922975157258e`  
		Last Modified: Wed, 28 Jul 2021 23:40:44 GMT  
		Size: 59.4 MB (59384856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u302-al2`

```console
$ docker pull amazoncorretto@sha256:e517b1051888b935855f19740cdd69faf76b1a5eb5f6ea8c34989c04671f91fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u302-al2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:99383180a63638b69ccce247aa6b7dbb770cf2b108e0d219f0b5f0c9a4e7299f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137299042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df1c4e3803af8fd91c9b8a4f45546ba5c654ab65a15b1e7bff1627cba43a1fd0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:19:58 GMT
ARG version=1.8.0_302.b08-1
# Wed, 28 Jul 2021 23:19:45 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Jul 2021 23:19:46 GMT
ENV LANG=C.UTF-8
# Wed, 28 Jul 2021 23:19:46 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed3eb17202682b67a716d65d9a7b156337c35c258c7d56eaf2f6025921237a4`  
		Last Modified: Wed, 28 Jul 2021 23:20:45 GMT  
		Size: 75.3 MB (75333036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u302-al2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:c3ae270b98b9fe18e7eda62aede47ca5834bc4ad804e848b5c0d590e0f36b7c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122952748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee3949d0817afd993fb56e0c6cb2c60acbb4815eec064750beeb2379fc2c090c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:39:20 GMT
ARG version=1.8.0_302.b08-1
# Wed, 28 Jul 2021 23:39:42 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Jul 2021 23:39:42 GMT
ENV LANG=C.UTF-8
# Wed, 28 Jul 2021 23:39:42 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5230c70e909e8047c9eadb7a1e0fecdf1baf98003a2f6a56063922975157258e`  
		Last Modified: Wed, 28 Jul 2021 23:40:44 GMT  
		Size: 59.4 MB (59384856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u302-alpine`

```console
$ docker pull amazoncorretto@sha256:b97cd4e1f357a3d445db6d1566838a6c91b312cea4085ecc791370ac288860d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u302-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4edb6c988dbd6611a208f16ec06ee915289808745e32fe27691026a64519229d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101831898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93854338cb3296eb3934ba3706b7ce61dcf904607e3f9fd4139583c5aa4739bb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 21 Jul 2021 00:20:54 GMT
ARG version=8.302.08.1
# Wed, 21 Jul 2021 00:21:00 GMT
# ARGS: version=8.302.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Wed, 21 Jul 2021 00:21:00 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:21:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 21 Jul 2021 00:21:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f141ea8c2ff0050b64f199d6c95d96fef7a0e9f7daac05c2ff20af6a7e0f25`  
		Last Modified: Wed, 21 Jul 2021 00:23:11 GMT  
		Size: 99.0 MB (99031331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u302-alpine-jre`

```console
$ docker pull amazoncorretto@sha256:2c978d2e5921d10abf49c845a2a46b502544c15e2ca733d7b552b350aa691068
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u302-alpine-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:ff95ea78ce154abaa581bf382295bacf13c0474357ef144fcd96ac1d6d5e851d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43148477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7543a33c551dd671bf563addcbfbf76cc5a3020d86a8479847202e8bd0b5dce1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 21 Jul 2021 00:20:54 GMT
ARG version=8.302.08.1
# Wed, 21 Jul 2021 00:21:07 GMT
# ARGS: version=8.302.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Wed, 21 Jul 2021 00:21:07 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:21:07 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be776a268f00c1a39cc8385fff8b6582ba6d26a76a929e1f13dbdf0208d73520`  
		Last Modified: Wed, 21 Jul 2021 00:23:31 GMT  
		Size: 40.3 MB (40347910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:latest`

```console
$ docker pull amazoncorretto@sha256:e517b1051888b935855f19740cdd69faf76b1a5eb5f6ea8c34989c04671f91fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:latest` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:99383180a63638b69ccce247aa6b7dbb770cf2b108e0d219f0b5f0c9a4e7299f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137299042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df1c4e3803af8fd91c9b8a4f45546ba5c654ab65a15b1e7bff1627cba43a1fd0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:19:58 GMT
ARG version=1.8.0_302.b08-1
# Wed, 28 Jul 2021 23:19:45 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Jul 2021 23:19:46 GMT
ENV LANG=C.UTF-8
# Wed, 28 Jul 2021 23:19:46 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed3eb17202682b67a716d65d9a7b156337c35c258c7d56eaf2f6025921237a4`  
		Last Modified: Wed, 28 Jul 2021 23:20:45 GMT  
		Size: 75.3 MB (75333036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:latest` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:c3ae270b98b9fe18e7eda62aede47ca5834bc4ad804e848b5c0d590e0f36b7c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122952748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee3949d0817afd993fb56e0c6cb2c60acbb4815eec064750beeb2379fc2c090c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:39:20 GMT
ARG version=1.8.0_302.b08-1
# Wed, 28 Jul 2021 23:39:42 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Jul 2021 23:39:42 GMT
ENV LANG=C.UTF-8
# Wed, 28 Jul 2021 23:39:42 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5230c70e909e8047c9eadb7a1e0fecdf1baf98003a2f6a56063922975157258e`  
		Last Modified: Wed, 28 Jul 2021 23:40:44 GMT  
		Size: 59.4 MB (59384856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
