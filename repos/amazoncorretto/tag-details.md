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
-	[`amazoncorretto:16.0.1`](#amazoncorretto1601)
-	[`amazoncorretto:16.0.1-al2`](#amazoncorretto1601-al2)
-	[`amazoncorretto:16.0.1-alpine`](#amazoncorretto1601-alpine)
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
$ docker pull amazoncorretto@sha256:a435f9eeefaf77808e3fe640b17479f5b0b7f3f9e2567fffe0efa5a56d994eea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:91b016d12d68324fafa8cd6eb78151fc13dc1b8a74b873b874647a1efa9e8872
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221934790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cabd0141d5affefc3f5e6cf078212f38a5ce49b92435c9791d3e6fa67146d55a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Fri, 16 Jul 2021 00:33:46 GMT
ARG version=16.0.1.9-1
# Fri, 16 Jul 2021 00:34:08 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 16 Jul 2021 00:34:09 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jul 2021 00:34:09 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ae2aa5d553ef6e7cdc431e50b69567e861535def955f13b149e1d1faae3b7c`  
		Last Modified: Fri, 16 Jul 2021 00:36:04 GMT  
		Size: 160.0 MB (159968784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:f9280442f9dd018d5a21ed28afefd75207c45c7454fc762c9975c5aae11ca7a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.5 MB (223483348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f07aa695e0473b234a53a0d0a700c62aa1ff55c9fa532d15b5910876cf1b2a4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Fri, 16 Jul 2021 00:40:07 GMT
ARG version=16.0.1.9-1
# Fri, 16 Jul 2021 00:40:32 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 16 Jul 2021 00:40:32 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jul 2021 00:40:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a884ee1e30947553d9866a95fa0913be7a964863f8e4e8658af0c81e21e35a`  
		Last Modified: Fri, 16 Jul 2021 00:42:44 GMT  
		Size: 159.9 MB (159915456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-al2-full`

```console
$ docker pull amazoncorretto@sha256:a435f9eeefaf77808e3fe640b17479f5b0b7f3f9e2567fffe0efa5a56d994eea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:91b016d12d68324fafa8cd6eb78151fc13dc1b8a74b873b874647a1efa9e8872
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221934790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cabd0141d5affefc3f5e6cf078212f38a5ce49b92435c9791d3e6fa67146d55a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Fri, 16 Jul 2021 00:33:46 GMT
ARG version=16.0.1.9-1
# Fri, 16 Jul 2021 00:34:08 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 16 Jul 2021 00:34:09 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jul 2021 00:34:09 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ae2aa5d553ef6e7cdc431e50b69567e861535def955f13b149e1d1faae3b7c`  
		Last Modified: Fri, 16 Jul 2021 00:36:04 GMT  
		Size: 160.0 MB (159968784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:f9280442f9dd018d5a21ed28afefd75207c45c7454fc762c9975c5aae11ca7a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.5 MB (223483348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f07aa695e0473b234a53a0d0a700c62aa1ff55c9fa532d15b5910876cf1b2a4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Fri, 16 Jul 2021 00:40:07 GMT
ARG version=16.0.1.9-1
# Fri, 16 Jul 2021 00:40:32 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 16 Jul 2021 00:40:32 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jul 2021 00:40:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a884ee1e30947553d9866a95fa0913be7a964863f8e4e8658af0c81e21e35a`  
		Last Modified: Fri, 16 Jul 2021 00:42:44 GMT  
		Size: 159.9 MB (159915456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:a435f9eeefaf77808e3fe640b17479f5b0b7f3f9e2567fffe0efa5a56d994eea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:91b016d12d68324fafa8cd6eb78151fc13dc1b8a74b873b874647a1efa9e8872
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221934790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cabd0141d5affefc3f5e6cf078212f38a5ce49b92435c9791d3e6fa67146d55a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Fri, 16 Jul 2021 00:33:46 GMT
ARG version=16.0.1.9-1
# Fri, 16 Jul 2021 00:34:08 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 16 Jul 2021 00:34:09 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jul 2021 00:34:09 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ae2aa5d553ef6e7cdc431e50b69567e861535def955f13b149e1d1faae3b7c`  
		Last Modified: Fri, 16 Jul 2021 00:36:04 GMT  
		Size: 160.0 MB (159968784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:f9280442f9dd018d5a21ed28afefd75207c45c7454fc762c9975c5aae11ca7a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.5 MB (223483348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f07aa695e0473b234a53a0d0a700c62aa1ff55c9fa532d15b5910876cf1b2a4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Fri, 16 Jul 2021 00:40:07 GMT
ARG version=16.0.1.9-1
# Fri, 16 Jul 2021 00:40:32 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 16 Jul 2021 00:40:32 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jul 2021 00:40:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a884ee1e30947553d9866a95fa0913be7a964863f8e4e8658af0c81e21e35a`  
		Last Modified: Fri, 16 Jul 2021 00:42:44 GMT  
		Size: 159.9 MB (159915456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-alpine`

```console
$ docker pull amazoncorretto@sha256:da67cfe4028e29830be8096e81fb46e44cee2481c529b066663808b76947ebf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:16-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:404f02e2ef1cc041b323a7976f631917badeec3b4d43f8ae5b0f0361dab0439e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.4 MB (212433843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b2ad03654b54cda4c95f8b862f1f47b7c0e9287be30ce020dfb51973ae161c5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Sat, 24 Apr 2021 04:41:25 GMT
ARG version=16.0.1.9.1
# Sat, 24 Apr 2021 04:41:33 GMT
# ARGS: version=16.0.1.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-16=$version-r0
# Sat, 24 Apr 2021 04:41:33 GMT
ENV LANG=C.UTF-8
# Sat, 24 Apr 2021 04:41:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Sat, 24 Apr 2021 04:41:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5d31824e596a5e7174f37f27e0af4babbe7745e7a1eb51f3ee8bc2ee3dcdbe`  
		Last Modified: Sat, 24 Apr 2021 04:43:04 GMT  
		Size: 209.6 MB (209633276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-alpine-full`

```console
$ docker pull amazoncorretto@sha256:da67cfe4028e29830be8096e81fb46e44cee2481c529b066663808b76947ebf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:16-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:404f02e2ef1cc041b323a7976f631917badeec3b4d43f8ae5b0f0361dab0439e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.4 MB (212433843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b2ad03654b54cda4c95f8b862f1f47b7c0e9287be30ce020dfb51973ae161c5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Sat, 24 Apr 2021 04:41:25 GMT
ARG version=16.0.1.9.1
# Sat, 24 Apr 2021 04:41:33 GMT
# ARGS: version=16.0.1.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-16=$version-r0
# Sat, 24 Apr 2021 04:41:33 GMT
ENV LANG=C.UTF-8
# Sat, 24 Apr 2021 04:41:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Sat, 24 Apr 2021 04:41:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5d31824e596a5e7174f37f27e0af4babbe7745e7a1eb51f3ee8bc2ee3dcdbe`  
		Last Modified: Sat, 24 Apr 2021 04:43:04 GMT  
		Size: 209.6 MB (209633276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:da67cfe4028e29830be8096e81fb46e44cee2481c529b066663808b76947ebf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:16-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:404f02e2ef1cc041b323a7976f631917badeec3b4d43f8ae5b0f0361dab0439e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.4 MB (212433843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b2ad03654b54cda4c95f8b862f1f47b7c0e9287be30ce020dfb51973ae161c5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Sat, 24 Apr 2021 04:41:25 GMT
ARG version=16.0.1.9.1
# Sat, 24 Apr 2021 04:41:33 GMT
# ARGS: version=16.0.1.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-16=$version-r0
# Sat, 24 Apr 2021 04:41:33 GMT
ENV LANG=C.UTF-8
# Sat, 24 Apr 2021 04:41:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Sat, 24 Apr 2021 04:41:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5d31824e596a5e7174f37f27e0af4babbe7745e7a1eb51f3ee8bc2ee3dcdbe`  
		Last Modified: Sat, 24 Apr 2021 04:43:04 GMT  
		Size: 209.6 MB (209633276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16.0.1`

```console
$ docker pull amazoncorretto@sha256:a435f9eeefaf77808e3fe640b17479f5b0b7f3f9e2567fffe0efa5a56d994eea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16.0.1` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:91b016d12d68324fafa8cd6eb78151fc13dc1b8a74b873b874647a1efa9e8872
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221934790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cabd0141d5affefc3f5e6cf078212f38a5ce49b92435c9791d3e6fa67146d55a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Fri, 16 Jul 2021 00:33:46 GMT
ARG version=16.0.1.9-1
# Fri, 16 Jul 2021 00:34:08 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 16 Jul 2021 00:34:09 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jul 2021 00:34:09 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ae2aa5d553ef6e7cdc431e50b69567e861535def955f13b149e1d1faae3b7c`  
		Last Modified: Fri, 16 Jul 2021 00:36:04 GMT  
		Size: 160.0 MB (159968784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16.0.1` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:f9280442f9dd018d5a21ed28afefd75207c45c7454fc762c9975c5aae11ca7a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.5 MB (223483348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f07aa695e0473b234a53a0d0a700c62aa1ff55c9fa532d15b5910876cf1b2a4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Fri, 16 Jul 2021 00:40:07 GMT
ARG version=16.0.1.9-1
# Fri, 16 Jul 2021 00:40:32 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 16 Jul 2021 00:40:32 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jul 2021 00:40:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a884ee1e30947553d9866a95fa0913be7a964863f8e4e8658af0c81e21e35a`  
		Last Modified: Fri, 16 Jul 2021 00:42:44 GMT  
		Size: 159.9 MB (159915456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16.0.1-al2`

```console
$ docker pull amazoncorretto@sha256:a435f9eeefaf77808e3fe640b17479f5b0b7f3f9e2567fffe0efa5a56d994eea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16.0.1-al2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:91b016d12d68324fafa8cd6eb78151fc13dc1b8a74b873b874647a1efa9e8872
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221934790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cabd0141d5affefc3f5e6cf078212f38a5ce49b92435c9791d3e6fa67146d55a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Fri, 16 Jul 2021 00:33:46 GMT
ARG version=16.0.1.9-1
# Fri, 16 Jul 2021 00:34:08 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 16 Jul 2021 00:34:09 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jul 2021 00:34:09 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ae2aa5d553ef6e7cdc431e50b69567e861535def955f13b149e1d1faae3b7c`  
		Last Modified: Fri, 16 Jul 2021 00:36:04 GMT  
		Size: 160.0 MB (159968784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16.0.1-al2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:f9280442f9dd018d5a21ed28afefd75207c45c7454fc762c9975c5aae11ca7a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.5 MB (223483348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f07aa695e0473b234a53a0d0a700c62aa1ff55c9fa532d15b5910876cf1b2a4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Fri, 16 Jul 2021 00:40:07 GMT
ARG version=16.0.1.9-1
# Fri, 16 Jul 2021 00:40:32 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 16 Jul 2021 00:40:32 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jul 2021 00:40:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a884ee1e30947553d9866a95fa0913be7a964863f8e4e8658af0c81e21e35a`  
		Last Modified: Fri, 16 Jul 2021 00:42:44 GMT  
		Size: 159.9 MB (159915456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16.0.1-alpine`

```console
$ docker pull amazoncorretto@sha256:da67cfe4028e29830be8096e81fb46e44cee2481c529b066663808b76947ebf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:16.0.1-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:404f02e2ef1cc041b323a7976f631917badeec3b4d43f8ae5b0f0361dab0439e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.4 MB (212433843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b2ad03654b54cda4c95f8b862f1f47b7c0e9287be30ce020dfb51973ae161c5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Sat, 24 Apr 2021 04:41:25 GMT
ARG version=16.0.1.9.1
# Sat, 24 Apr 2021 04:41:33 GMT
# ARGS: version=16.0.1.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-16=$version-r0
# Sat, 24 Apr 2021 04:41:33 GMT
ENV LANG=C.UTF-8
# Sat, 24 Apr 2021 04:41:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Sat, 24 Apr 2021 04:41:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5d31824e596a5e7174f37f27e0af4babbe7745e7a1eb51f3ee8bc2ee3dcdbe`  
		Last Modified: Sat, 24 Apr 2021 04:43:04 GMT  
		Size: 209.6 MB (209633276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8`

```console
$ docker pull amazoncorretto@sha256:81956f584cab7299043125c9a3b92f11d6d82658bc5d4683cde24543999f62ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:c0b919781ba3a5562647ef462498de174c06355a3aa2c494dd5a61b5a93cb58f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137298994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:940da094e12101ea77abd14cd1f07fedc72d6b7d2c8db7af8c3e415f653f2b3b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:19:58 GMT
ARG version=1.8.0_302.b08-1
# Wed, 21 Jul 2021 00:20:19 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && if [[ `arch` == 'aarch64' ]]; then version=1.8.0_292.b10-2; fi     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:20:19 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:20:20 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb7345e871527554f60a16d3ccbb1227c55c86687fe1b3a27de765c1dd3b461`  
		Last Modified: Wed, 21 Jul 2021 00:22:06 GMT  
		Size: 75.3 MB (75332988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:177857b0ae589b166ff820384a1b64b3004c2eea938b5d7d805e61f34732f1f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122953715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b8d5108387d4b26fa217560ed9f0048bcdae56151829645d3ef7477a19ff43f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:39:20 GMT
ARG version=1.8.0_302.b08-1
# Wed, 21 Jul 2021 00:39:37 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && if [[ `arch` == 'aarch64' ]]; then version=1.8.0_292.b10-2; fi     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:39:38 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:39:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8400adb2e143e69e28d625f26dcb11c7261437ddaf5acd161e70e5fe4c60ed`  
		Last Modified: Wed, 21 Jul 2021 00:41:00 GMT  
		Size: 59.4 MB (59385823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-al2-full`

```console
$ docker pull amazoncorretto@sha256:81956f584cab7299043125c9a3b92f11d6d82658bc5d4683cde24543999f62ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:c0b919781ba3a5562647ef462498de174c06355a3aa2c494dd5a61b5a93cb58f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137298994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:940da094e12101ea77abd14cd1f07fedc72d6b7d2c8db7af8c3e415f653f2b3b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:19:58 GMT
ARG version=1.8.0_302.b08-1
# Wed, 21 Jul 2021 00:20:19 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && if [[ `arch` == 'aarch64' ]]; then version=1.8.0_292.b10-2; fi     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:20:19 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:20:20 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb7345e871527554f60a16d3ccbb1227c55c86687fe1b3a27de765c1dd3b461`  
		Last Modified: Wed, 21 Jul 2021 00:22:06 GMT  
		Size: 75.3 MB (75332988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:177857b0ae589b166ff820384a1b64b3004c2eea938b5d7d805e61f34732f1f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122953715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b8d5108387d4b26fa217560ed9f0048bcdae56151829645d3ef7477a19ff43f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:39:20 GMT
ARG version=1.8.0_302.b08-1
# Wed, 21 Jul 2021 00:39:37 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && if [[ `arch` == 'aarch64' ]]; then version=1.8.0_292.b10-2; fi     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:39:38 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:39:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8400adb2e143e69e28d625f26dcb11c7261437ddaf5acd161e70e5fe4c60ed`  
		Last Modified: Wed, 21 Jul 2021 00:41:00 GMT  
		Size: 59.4 MB (59385823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:81956f584cab7299043125c9a3b92f11d6d82658bc5d4683cde24543999f62ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:c0b919781ba3a5562647ef462498de174c06355a3aa2c494dd5a61b5a93cb58f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137298994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:940da094e12101ea77abd14cd1f07fedc72d6b7d2c8db7af8c3e415f653f2b3b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:19:58 GMT
ARG version=1.8.0_302.b08-1
# Wed, 21 Jul 2021 00:20:19 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && if [[ `arch` == 'aarch64' ]]; then version=1.8.0_292.b10-2; fi     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:20:19 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:20:20 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb7345e871527554f60a16d3ccbb1227c55c86687fe1b3a27de765c1dd3b461`  
		Last Modified: Wed, 21 Jul 2021 00:22:06 GMT  
		Size: 75.3 MB (75332988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:177857b0ae589b166ff820384a1b64b3004c2eea938b5d7d805e61f34732f1f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122953715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b8d5108387d4b26fa217560ed9f0048bcdae56151829645d3ef7477a19ff43f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:39:20 GMT
ARG version=1.8.0_302.b08-1
# Wed, 21 Jul 2021 00:39:37 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && if [[ `arch` == 'aarch64' ]]; then version=1.8.0_292.b10-2; fi     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:39:38 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:39:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8400adb2e143e69e28d625f26dcb11c7261437ddaf5acd161e70e5fe4c60ed`  
		Last Modified: Wed, 21 Jul 2021 00:41:00 GMT  
		Size: 59.4 MB (59385823 bytes)  
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
$ docker pull amazoncorretto@sha256:81956f584cab7299043125c9a3b92f11d6d82658bc5d4683cde24543999f62ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u302` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:c0b919781ba3a5562647ef462498de174c06355a3aa2c494dd5a61b5a93cb58f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137298994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:940da094e12101ea77abd14cd1f07fedc72d6b7d2c8db7af8c3e415f653f2b3b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:19:58 GMT
ARG version=1.8.0_302.b08-1
# Wed, 21 Jul 2021 00:20:19 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && if [[ `arch` == 'aarch64' ]]; then version=1.8.0_292.b10-2; fi     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:20:19 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:20:20 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb7345e871527554f60a16d3ccbb1227c55c86687fe1b3a27de765c1dd3b461`  
		Last Modified: Wed, 21 Jul 2021 00:22:06 GMT  
		Size: 75.3 MB (75332988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u302` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:177857b0ae589b166ff820384a1b64b3004c2eea938b5d7d805e61f34732f1f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122953715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b8d5108387d4b26fa217560ed9f0048bcdae56151829645d3ef7477a19ff43f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:39:20 GMT
ARG version=1.8.0_302.b08-1
# Wed, 21 Jul 2021 00:39:37 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && if [[ `arch` == 'aarch64' ]]; then version=1.8.0_292.b10-2; fi     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:39:38 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:39:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8400adb2e143e69e28d625f26dcb11c7261437ddaf5acd161e70e5fe4c60ed`  
		Last Modified: Wed, 21 Jul 2021 00:41:00 GMT  
		Size: 59.4 MB (59385823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u302-al2`

```console
$ docker pull amazoncorretto@sha256:81956f584cab7299043125c9a3b92f11d6d82658bc5d4683cde24543999f62ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u302-al2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:c0b919781ba3a5562647ef462498de174c06355a3aa2c494dd5a61b5a93cb58f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137298994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:940da094e12101ea77abd14cd1f07fedc72d6b7d2c8db7af8c3e415f653f2b3b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:19:58 GMT
ARG version=1.8.0_302.b08-1
# Wed, 21 Jul 2021 00:20:19 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && if [[ `arch` == 'aarch64' ]]; then version=1.8.0_292.b10-2; fi     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:20:19 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:20:20 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb7345e871527554f60a16d3ccbb1227c55c86687fe1b3a27de765c1dd3b461`  
		Last Modified: Wed, 21 Jul 2021 00:22:06 GMT  
		Size: 75.3 MB (75332988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u302-al2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:177857b0ae589b166ff820384a1b64b3004c2eea938b5d7d805e61f34732f1f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122953715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b8d5108387d4b26fa217560ed9f0048bcdae56151829645d3ef7477a19ff43f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:39:20 GMT
ARG version=1.8.0_302.b08-1
# Wed, 21 Jul 2021 00:39:37 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && if [[ `arch` == 'aarch64' ]]; then version=1.8.0_292.b10-2; fi     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:39:38 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:39:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8400adb2e143e69e28d625f26dcb11c7261437ddaf5acd161e70e5fe4c60ed`  
		Last Modified: Wed, 21 Jul 2021 00:41:00 GMT  
		Size: 59.4 MB (59385823 bytes)  
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
$ docker pull amazoncorretto@sha256:81956f584cab7299043125c9a3b92f11d6d82658bc5d4683cde24543999f62ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:latest` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:c0b919781ba3a5562647ef462498de174c06355a3aa2c494dd5a61b5a93cb58f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137298994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:940da094e12101ea77abd14cd1f07fedc72d6b7d2c8db7af8c3e415f653f2b3b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:19:58 GMT
ARG version=1.8.0_302.b08-1
# Wed, 21 Jul 2021 00:20:19 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && if [[ `arch` == 'aarch64' ]]; then version=1.8.0_292.b10-2; fi     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:20:19 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:20:20 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb7345e871527554f60a16d3ccbb1227c55c86687fe1b3a27de765c1dd3b461`  
		Last Modified: Wed, 21 Jul 2021 00:22:06 GMT  
		Size: 75.3 MB (75332988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:latest` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:177857b0ae589b166ff820384a1b64b3004c2eea938b5d7d805e61f34732f1f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122953715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b8d5108387d4b26fa217560ed9f0048bcdae56151829645d3ef7477a19ff43f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:39:20 GMT
ARG version=1.8.0_302.b08-1
# Wed, 21 Jul 2021 00:39:37 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && if [[ `arch` == 'aarch64' ]]; then version=1.8.0_292.b10-2; fi     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:39:38 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:39:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8400adb2e143e69e28d625f26dcb11c7261437ddaf5acd161e70e5fe4c60ed`  
		Last Modified: Wed, 21 Jul 2021 00:41:00 GMT  
		Size: 59.4 MB (59385823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
