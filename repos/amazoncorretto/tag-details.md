<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazoncorretto`

-	[`amazoncorretto:11`](#amazoncorretto11)
-	[`amazoncorretto:11-al2-full`](#amazoncorretto11-al2-full)
-	[`amazoncorretto:11-al2-jdk`](#amazoncorretto11-al2-jdk)
-	[`amazoncorretto:11-alpine`](#amazoncorretto11-alpine)
-	[`amazoncorretto:11-alpine-full`](#amazoncorretto11-alpine-full)
-	[`amazoncorretto:11-alpine-jdk`](#amazoncorretto11-alpine-jdk)
-	[`amazoncorretto:11.0.11`](#amazoncorretto11011)
-	[`amazoncorretto:11.0.11-al2`](#amazoncorretto11011-al2)
-	[`amazoncorretto:11.0.11-alpine`](#amazoncorretto11011-alpine)
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
-	[`amazoncorretto:8u282-alpine-jre`](#amazoncorretto8u282-alpine-jre)
-	[`amazoncorretto:8u292`](#amazoncorretto8u292)
-	[`amazoncorretto:8u292-al2`](#amazoncorretto8u292-al2)
-	[`amazoncorretto:8u292-alpine`](#amazoncorretto8u292-alpine)
-	[`amazoncorretto:latest`](#amazoncorrettolatest)

## `amazoncorretto:11`

```console
$ docker pull amazoncorretto@sha256:89d46adf6b405142134a4154710d6a5382e6c72a1eed870f5f7789cf9d1c2e2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:7ea8a1cf6c8559592d5f0b91722a0b5dea817e9f05c1047e554e12e65cd0ba6b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.6 MB (208615443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35d4a605128e9030d172b3f0cede99cd84397383e8687d4b255992346f10a40d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:19:46 GMT
ARG version=11.0.11.9-1
# Tue, 20 Apr 2021 23:20:07 GMT
# ARGS: version=11.0.11.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:20:07 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:20:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdd31bd043e6363617df60f067ba94899a198403d14f6dfea1b534afdebf768`  
		Last Modified: Tue, 20 Apr 2021 23:21:57 GMT  
		Size: 146.7 MB (146668858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:23c10b201bada8aa9fe3da91d2c5030bfe62dca36306708445a8f13104024425
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.4 MB (208406385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a6f460ddb51d30ac7488a7310031992a217a3c6045abf6e1ea41135dfc6a4ae`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:44:08 GMT
ARG version=11.0.11.9-1
# Tue, 20 Apr 2021 23:44:36 GMT
# ARGS: version=11.0.11.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:44:38 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:44:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e32310ed216770786ba120656186e1881af266bd3e84c7a7603a5dcb62fb0f`  
		Last Modified: Tue, 20 Apr 2021 23:45:58 GMT  
		Size: 144.7 MB (144746347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-al2-full`

```console
$ docker pull amazoncorretto@sha256:89d46adf6b405142134a4154710d6a5382e6c72a1eed870f5f7789cf9d1c2e2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:7ea8a1cf6c8559592d5f0b91722a0b5dea817e9f05c1047e554e12e65cd0ba6b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.6 MB (208615443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35d4a605128e9030d172b3f0cede99cd84397383e8687d4b255992346f10a40d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:19:46 GMT
ARG version=11.0.11.9-1
# Tue, 20 Apr 2021 23:20:07 GMT
# ARGS: version=11.0.11.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:20:07 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:20:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdd31bd043e6363617df60f067ba94899a198403d14f6dfea1b534afdebf768`  
		Last Modified: Tue, 20 Apr 2021 23:21:57 GMT  
		Size: 146.7 MB (146668858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:23c10b201bada8aa9fe3da91d2c5030bfe62dca36306708445a8f13104024425
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.4 MB (208406385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a6f460ddb51d30ac7488a7310031992a217a3c6045abf6e1ea41135dfc6a4ae`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:44:08 GMT
ARG version=11.0.11.9-1
# Tue, 20 Apr 2021 23:44:36 GMT
# ARGS: version=11.0.11.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:44:38 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:44:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e32310ed216770786ba120656186e1881af266bd3e84c7a7603a5dcb62fb0f`  
		Last Modified: Tue, 20 Apr 2021 23:45:58 GMT  
		Size: 144.7 MB (144746347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:89d46adf6b405142134a4154710d6a5382e6c72a1eed870f5f7789cf9d1c2e2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:7ea8a1cf6c8559592d5f0b91722a0b5dea817e9f05c1047e554e12e65cd0ba6b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.6 MB (208615443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35d4a605128e9030d172b3f0cede99cd84397383e8687d4b255992346f10a40d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:19:46 GMT
ARG version=11.0.11.9-1
# Tue, 20 Apr 2021 23:20:07 GMT
# ARGS: version=11.0.11.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:20:07 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:20:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdd31bd043e6363617df60f067ba94899a198403d14f6dfea1b534afdebf768`  
		Last Modified: Tue, 20 Apr 2021 23:21:57 GMT  
		Size: 146.7 MB (146668858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:23c10b201bada8aa9fe3da91d2c5030bfe62dca36306708445a8f13104024425
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.4 MB (208406385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a6f460ddb51d30ac7488a7310031992a217a3c6045abf6e1ea41135dfc6a4ae`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:44:08 GMT
ARG version=11.0.11.9-1
# Tue, 20 Apr 2021 23:44:36 GMT
# ARGS: version=11.0.11.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:44:38 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:44:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e32310ed216770786ba120656186e1881af266bd3e84c7a7603a5dcb62fb0f`  
		Last Modified: Tue, 20 Apr 2021 23:45:58 GMT  
		Size: 144.7 MB (144746347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-alpine`

```console
$ docker pull amazoncorretto@sha256:35e8797e008eac2e05264c8a3894767b8cd4661ddca0837db1df7795d142ed1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:11-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4201449d2c1ccd174ed6dd41ec90d21a88e5d12ef00e30ba29a1d642b7bc3a0b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.0 MB (196029750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a895b16a7e33d9d36955302d1cd0844f09db71db7afac4b94263a3d347419c3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Tue, 20 Apr 2021 23:20:30 GMT
ARG version=11.0.11.9.1
# Tue, 20 Apr 2021 23:20:37 GMT
# ARGS: version=11.0.11.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Tue, 20 Apr 2021 23:20:37 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:20:37 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 20 Apr 2021 23:20:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2531042875644865f91c5f2fa487ccced5f1edb710eb483a2f11059a879156`  
		Last Modified: Tue, 20 Apr 2021 23:23:14 GMT  
		Size: 193.2 MB (193229183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-alpine-full`

```console
$ docker pull amazoncorretto@sha256:35e8797e008eac2e05264c8a3894767b8cd4661ddca0837db1df7795d142ed1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:11-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4201449d2c1ccd174ed6dd41ec90d21a88e5d12ef00e30ba29a1d642b7bc3a0b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.0 MB (196029750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a895b16a7e33d9d36955302d1cd0844f09db71db7afac4b94263a3d347419c3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Tue, 20 Apr 2021 23:20:30 GMT
ARG version=11.0.11.9.1
# Tue, 20 Apr 2021 23:20:37 GMT
# ARGS: version=11.0.11.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Tue, 20 Apr 2021 23:20:37 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:20:37 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 20 Apr 2021 23:20:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2531042875644865f91c5f2fa487ccced5f1edb710eb483a2f11059a879156`  
		Last Modified: Tue, 20 Apr 2021 23:23:14 GMT  
		Size: 193.2 MB (193229183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:35e8797e008eac2e05264c8a3894767b8cd4661ddca0837db1df7795d142ed1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:11-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4201449d2c1ccd174ed6dd41ec90d21a88e5d12ef00e30ba29a1d642b7bc3a0b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.0 MB (196029750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a895b16a7e33d9d36955302d1cd0844f09db71db7afac4b94263a3d347419c3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Tue, 20 Apr 2021 23:20:30 GMT
ARG version=11.0.11.9.1
# Tue, 20 Apr 2021 23:20:37 GMT
# ARGS: version=11.0.11.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Tue, 20 Apr 2021 23:20:37 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:20:37 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 20 Apr 2021 23:20:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2531042875644865f91c5f2fa487ccced5f1edb710eb483a2f11059a879156`  
		Last Modified: Tue, 20 Apr 2021 23:23:14 GMT  
		Size: 193.2 MB (193229183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11.0.11`

```console
$ docker pull amazoncorretto@sha256:89d46adf6b405142134a4154710d6a5382e6c72a1eed870f5f7789cf9d1c2e2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11.0.11` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:7ea8a1cf6c8559592d5f0b91722a0b5dea817e9f05c1047e554e12e65cd0ba6b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.6 MB (208615443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35d4a605128e9030d172b3f0cede99cd84397383e8687d4b255992346f10a40d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:19:46 GMT
ARG version=11.0.11.9-1
# Tue, 20 Apr 2021 23:20:07 GMT
# ARGS: version=11.0.11.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:20:07 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:20:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdd31bd043e6363617df60f067ba94899a198403d14f6dfea1b534afdebf768`  
		Last Modified: Tue, 20 Apr 2021 23:21:57 GMT  
		Size: 146.7 MB (146668858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11.0.11` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:23c10b201bada8aa9fe3da91d2c5030bfe62dca36306708445a8f13104024425
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.4 MB (208406385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a6f460ddb51d30ac7488a7310031992a217a3c6045abf6e1ea41135dfc6a4ae`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:44:08 GMT
ARG version=11.0.11.9-1
# Tue, 20 Apr 2021 23:44:36 GMT
# ARGS: version=11.0.11.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:44:38 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:44:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e32310ed216770786ba120656186e1881af266bd3e84c7a7603a5dcb62fb0f`  
		Last Modified: Tue, 20 Apr 2021 23:45:58 GMT  
		Size: 144.7 MB (144746347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11.0.11-al2`

```console
$ docker pull amazoncorretto@sha256:89d46adf6b405142134a4154710d6a5382e6c72a1eed870f5f7789cf9d1c2e2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11.0.11-al2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:7ea8a1cf6c8559592d5f0b91722a0b5dea817e9f05c1047e554e12e65cd0ba6b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.6 MB (208615443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35d4a605128e9030d172b3f0cede99cd84397383e8687d4b255992346f10a40d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:19:46 GMT
ARG version=11.0.11.9-1
# Tue, 20 Apr 2021 23:20:07 GMT
# ARGS: version=11.0.11.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:20:07 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:20:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdd31bd043e6363617df60f067ba94899a198403d14f6dfea1b534afdebf768`  
		Last Modified: Tue, 20 Apr 2021 23:21:57 GMT  
		Size: 146.7 MB (146668858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11.0.11-al2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:23c10b201bada8aa9fe3da91d2c5030bfe62dca36306708445a8f13104024425
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.4 MB (208406385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a6f460ddb51d30ac7488a7310031992a217a3c6045abf6e1ea41135dfc6a4ae`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:44:08 GMT
ARG version=11.0.11.9-1
# Tue, 20 Apr 2021 23:44:36 GMT
# ARGS: version=11.0.11.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:44:38 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:44:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e32310ed216770786ba120656186e1881af266bd3e84c7a7603a5dcb62fb0f`  
		Last Modified: Tue, 20 Apr 2021 23:45:58 GMT  
		Size: 144.7 MB (144746347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11.0.11-alpine`

```console
$ docker pull amazoncorretto@sha256:35e8797e008eac2e05264c8a3894767b8cd4661ddca0837db1df7795d142ed1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:11.0.11-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4201449d2c1ccd174ed6dd41ec90d21a88e5d12ef00e30ba29a1d642b7bc3a0b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.0 MB (196029750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a895b16a7e33d9d36955302d1cd0844f09db71db7afac4b94263a3d347419c3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Tue, 20 Apr 2021 23:20:30 GMT
ARG version=11.0.11.9.1
# Tue, 20 Apr 2021 23:20:37 GMT
# ARGS: version=11.0.11.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Tue, 20 Apr 2021 23:20:37 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:20:37 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 20 Apr 2021 23:20:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2531042875644865f91c5f2fa487ccced5f1edb710eb483a2f11059a879156`  
		Last Modified: Tue, 20 Apr 2021 23:23:14 GMT  
		Size: 193.2 MB (193229183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16`

```console
$ docker pull amazoncorretto@sha256:035030cc50a125eb9cfbdbab4107abecc90c7b7bb70f5951ced407ca05567943
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:1aa2110b46b557478a6ff50831721ca6418938ac66fb09de4092755016dec48b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221904539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c23b2b7b4cbe6ada3791f3b18a83e0a23ddcf8af376b49e43810017a8dd2cc2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 04:40:59 GMT
ARG version=16.0.1.9-1
# Sat, 24 Apr 2021 04:41:21 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Sat, 24 Apr 2021 04:41:21 GMT
ENV LANG=C.UTF-8
# Sat, 24 Apr 2021 04:41:21 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639469cf55fb09ef9908b91956cac3b435540b062229048ead336526abc3546e`  
		Last Modified: Sat, 24 Apr 2021 04:42:30 GMT  
		Size: 160.0 MB (159957954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:04ae32cdab2abeed36f6ca357addc8944152cd3cd4b7f38831dabeb64a3e0324
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.6 MB (223581295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1ed2d42879c507a41faa0990075acbf23c76d184a0eea9fd5412c365a906138`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 02:15:31 GMT
ARG version=16.0.1.9-1
# Sat, 24 Apr 2021 02:16:07 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Sat, 24 Apr 2021 02:16:10 GMT
ENV LANG=C.UTF-8
# Sat, 24 Apr 2021 02:16:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21f9218d896bed8769806cdadee02297ffea4768446608aab77c1fedf6b8acb`  
		Last Modified: Sat, 24 Apr 2021 02:17:03 GMT  
		Size: 159.9 MB (159921257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-al2-full`

```console
$ docker pull amazoncorretto@sha256:035030cc50a125eb9cfbdbab4107abecc90c7b7bb70f5951ced407ca05567943
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:1aa2110b46b557478a6ff50831721ca6418938ac66fb09de4092755016dec48b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221904539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c23b2b7b4cbe6ada3791f3b18a83e0a23ddcf8af376b49e43810017a8dd2cc2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 04:40:59 GMT
ARG version=16.0.1.9-1
# Sat, 24 Apr 2021 04:41:21 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Sat, 24 Apr 2021 04:41:21 GMT
ENV LANG=C.UTF-8
# Sat, 24 Apr 2021 04:41:21 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639469cf55fb09ef9908b91956cac3b435540b062229048ead336526abc3546e`  
		Last Modified: Sat, 24 Apr 2021 04:42:30 GMT  
		Size: 160.0 MB (159957954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:04ae32cdab2abeed36f6ca357addc8944152cd3cd4b7f38831dabeb64a3e0324
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.6 MB (223581295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1ed2d42879c507a41faa0990075acbf23c76d184a0eea9fd5412c365a906138`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 02:15:31 GMT
ARG version=16.0.1.9-1
# Sat, 24 Apr 2021 02:16:07 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Sat, 24 Apr 2021 02:16:10 GMT
ENV LANG=C.UTF-8
# Sat, 24 Apr 2021 02:16:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21f9218d896bed8769806cdadee02297ffea4768446608aab77c1fedf6b8acb`  
		Last Modified: Sat, 24 Apr 2021 02:17:03 GMT  
		Size: 159.9 MB (159921257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:035030cc50a125eb9cfbdbab4107abecc90c7b7bb70f5951ced407ca05567943
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:1aa2110b46b557478a6ff50831721ca6418938ac66fb09de4092755016dec48b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221904539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c23b2b7b4cbe6ada3791f3b18a83e0a23ddcf8af376b49e43810017a8dd2cc2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 04:40:59 GMT
ARG version=16.0.1.9-1
# Sat, 24 Apr 2021 04:41:21 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Sat, 24 Apr 2021 04:41:21 GMT
ENV LANG=C.UTF-8
# Sat, 24 Apr 2021 04:41:21 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639469cf55fb09ef9908b91956cac3b435540b062229048ead336526abc3546e`  
		Last Modified: Sat, 24 Apr 2021 04:42:30 GMT  
		Size: 160.0 MB (159957954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:04ae32cdab2abeed36f6ca357addc8944152cd3cd4b7f38831dabeb64a3e0324
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.6 MB (223581295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1ed2d42879c507a41faa0990075acbf23c76d184a0eea9fd5412c365a906138`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 02:15:31 GMT
ARG version=16.0.1.9-1
# Sat, 24 Apr 2021 02:16:07 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Sat, 24 Apr 2021 02:16:10 GMT
ENV LANG=C.UTF-8
# Sat, 24 Apr 2021 02:16:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21f9218d896bed8769806cdadee02297ffea4768446608aab77c1fedf6b8acb`  
		Last Modified: Sat, 24 Apr 2021 02:17:03 GMT  
		Size: 159.9 MB (159921257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-alpine`

```console
$ docker pull amazoncorretto@sha256:da67cfe4028e29830be8096e81fb46e44cee2481c529b066663808b76947ebf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
-	Platforms:
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
-	Platforms:
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
$ docker pull amazoncorretto@sha256:035030cc50a125eb9cfbdbab4107abecc90c7b7bb70f5951ced407ca05567943
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16.0.1` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:1aa2110b46b557478a6ff50831721ca6418938ac66fb09de4092755016dec48b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221904539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c23b2b7b4cbe6ada3791f3b18a83e0a23ddcf8af376b49e43810017a8dd2cc2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 04:40:59 GMT
ARG version=16.0.1.9-1
# Sat, 24 Apr 2021 04:41:21 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Sat, 24 Apr 2021 04:41:21 GMT
ENV LANG=C.UTF-8
# Sat, 24 Apr 2021 04:41:21 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639469cf55fb09ef9908b91956cac3b435540b062229048ead336526abc3546e`  
		Last Modified: Sat, 24 Apr 2021 04:42:30 GMT  
		Size: 160.0 MB (159957954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16.0.1` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:04ae32cdab2abeed36f6ca357addc8944152cd3cd4b7f38831dabeb64a3e0324
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.6 MB (223581295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1ed2d42879c507a41faa0990075acbf23c76d184a0eea9fd5412c365a906138`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 02:15:31 GMT
ARG version=16.0.1.9-1
# Sat, 24 Apr 2021 02:16:07 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Sat, 24 Apr 2021 02:16:10 GMT
ENV LANG=C.UTF-8
# Sat, 24 Apr 2021 02:16:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21f9218d896bed8769806cdadee02297ffea4768446608aab77c1fedf6b8acb`  
		Last Modified: Sat, 24 Apr 2021 02:17:03 GMT  
		Size: 159.9 MB (159921257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16.0.1-al2`

```console
$ docker pull amazoncorretto@sha256:035030cc50a125eb9cfbdbab4107abecc90c7b7bb70f5951ced407ca05567943
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16.0.1-al2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:1aa2110b46b557478a6ff50831721ca6418938ac66fb09de4092755016dec48b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221904539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c23b2b7b4cbe6ada3791f3b18a83e0a23ddcf8af376b49e43810017a8dd2cc2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 04:40:59 GMT
ARG version=16.0.1.9-1
# Sat, 24 Apr 2021 04:41:21 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Sat, 24 Apr 2021 04:41:21 GMT
ENV LANG=C.UTF-8
# Sat, 24 Apr 2021 04:41:21 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639469cf55fb09ef9908b91956cac3b435540b062229048ead336526abc3546e`  
		Last Modified: Sat, 24 Apr 2021 04:42:30 GMT  
		Size: 160.0 MB (159957954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16.0.1-al2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:04ae32cdab2abeed36f6ca357addc8944152cd3cd4b7f38831dabeb64a3e0324
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.6 MB (223581295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1ed2d42879c507a41faa0990075acbf23c76d184a0eea9fd5412c365a906138`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 02:15:31 GMT
ARG version=16.0.1.9-1
# Sat, 24 Apr 2021 02:16:07 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Sat, 24 Apr 2021 02:16:10 GMT
ENV LANG=C.UTF-8
# Sat, 24 Apr 2021 02:16:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21f9218d896bed8769806cdadee02297ffea4768446608aab77c1fedf6b8acb`  
		Last Modified: Sat, 24 Apr 2021 02:17:03 GMT  
		Size: 159.9 MB (159921257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16.0.1-alpine`

```console
$ docker pull amazoncorretto@sha256:da67cfe4028e29830be8096e81fb46e44cee2481c529b066663808b76947ebf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull amazoncorretto@sha256:7f4379378c791fd02a5c93bd0e8f0694612d782c3665823413f1c5191d6f1262
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:00aee242da8f1dc4212eb0fbf63a1a8d405f3ad7ced4f37d8c47d21d5c7b8b7d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137238262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfaef49ef26491ebd020a02bb485e98c5c6bb9766427900580ae9c41e6e12524`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:19:20 GMT
ARG version=1.8.0_292.b10-1
# Tue, 20 Apr 2021 23:19:40 GMT
# ARGS: version=1.8.0_292.b10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:19:41 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:19:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ece89ed8d5944dabfaaa536301db77053bc6a2a996a272109b639f20b9cfca`  
		Last Modified: Tue, 20 Apr 2021 23:21:24 GMT  
		Size: 75.3 MB (75291677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:63b87dc056c11913fd13a02a6cd6a2d15e881b17021be3cd76bb452d7d09932c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123049888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e7684c1b0eb2a94a3e457a5cc240c76ab7140b4d211a6927a2e712480350a8e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:43:19 GMT
ARG version=1.8.0_292.b10-1
# Tue, 20 Apr 2021 23:43:53 GMT
# ARGS: version=1.8.0_292.b10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:43:55 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:43:55 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19674c905fc4a155e31837e0f8b91c7a503bd185ffae72d35ce7877265d63dae`  
		Last Modified: Tue, 20 Apr 2021 23:45:24 GMT  
		Size: 59.4 MB (59389850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-al2-full`

```console
$ docker pull amazoncorretto@sha256:7f4379378c791fd02a5c93bd0e8f0694612d782c3665823413f1c5191d6f1262
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:00aee242da8f1dc4212eb0fbf63a1a8d405f3ad7ced4f37d8c47d21d5c7b8b7d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137238262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfaef49ef26491ebd020a02bb485e98c5c6bb9766427900580ae9c41e6e12524`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:19:20 GMT
ARG version=1.8.0_292.b10-1
# Tue, 20 Apr 2021 23:19:40 GMT
# ARGS: version=1.8.0_292.b10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:19:41 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:19:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ece89ed8d5944dabfaaa536301db77053bc6a2a996a272109b639f20b9cfca`  
		Last Modified: Tue, 20 Apr 2021 23:21:24 GMT  
		Size: 75.3 MB (75291677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:63b87dc056c11913fd13a02a6cd6a2d15e881b17021be3cd76bb452d7d09932c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123049888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e7684c1b0eb2a94a3e457a5cc240c76ab7140b4d211a6927a2e712480350a8e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:43:19 GMT
ARG version=1.8.0_292.b10-1
# Tue, 20 Apr 2021 23:43:53 GMT
# ARGS: version=1.8.0_292.b10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:43:55 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:43:55 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19674c905fc4a155e31837e0f8b91c7a503bd185ffae72d35ce7877265d63dae`  
		Last Modified: Tue, 20 Apr 2021 23:45:24 GMT  
		Size: 59.4 MB (59389850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:7f4379378c791fd02a5c93bd0e8f0694612d782c3665823413f1c5191d6f1262
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:00aee242da8f1dc4212eb0fbf63a1a8d405f3ad7ced4f37d8c47d21d5c7b8b7d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137238262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfaef49ef26491ebd020a02bb485e98c5c6bb9766427900580ae9c41e6e12524`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:19:20 GMT
ARG version=1.8.0_292.b10-1
# Tue, 20 Apr 2021 23:19:40 GMT
# ARGS: version=1.8.0_292.b10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:19:41 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:19:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ece89ed8d5944dabfaaa536301db77053bc6a2a996a272109b639f20b9cfca`  
		Last Modified: Tue, 20 Apr 2021 23:21:24 GMT  
		Size: 75.3 MB (75291677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:63b87dc056c11913fd13a02a6cd6a2d15e881b17021be3cd76bb452d7d09932c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123049888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e7684c1b0eb2a94a3e457a5cc240c76ab7140b4d211a6927a2e712480350a8e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:43:19 GMT
ARG version=1.8.0_292.b10-1
# Tue, 20 Apr 2021 23:43:53 GMT
# ARGS: version=1.8.0_292.b10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:43:55 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:43:55 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19674c905fc4a155e31837e0f8b91c7a503bd185ffae72d35ce7877265d63dae`  
		Last Modified: Tue, 20 Apr 2021 23:45:24 GMT  
		Size: 59.4 MB (59389850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine`

```console
$ docker pull amazoncorretto@sha256:73939d6cb017bdb3885ea35ae18af6c6bf403ae0000b25e59c84b1e95ec9ffea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:1a3472c57788ef9c33e2b830bea1f5227562e197aac294e3b27305c4a3429b9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101815532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49dc0e3993ba2b79800dfa61af11876aad3ac15bfb8d280b35e81049b7a6ef3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Tue, 20 Apr 2021 23:20:11 GMT
ARG version=8.292.10.1
# Tue, 20 Apr 2021 23:20:19 GMT
# ARGS: version=8.292.10.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Tue, 20 Apr 2021 23:20:19 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:20:20 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 20 Apr 2021 23:20:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ec31fbf474c99d6924bc337c81bd4bfd0bfadb5a7e318c5456a3e110d4e9b9`  
		Last Modified: Tue, 20 Apr 2021 23:22:28 GMT  
		Size: 99.0 MB (99014965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine-full`

```console
$ docker pull amazoncorretto@sha256:73939d6cb017bdb3885ea35ae18af6c6bf403ae0000b25e59c84b1e95ec9ffea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:1a3472c57788ef9c33e2b830bea1f5227562e197aac294e3b27305c4a3429b9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101815532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49dc0e3993ba2b79800dfa61af11876aad3ac15bfb8d280b35e81049b7a6ef3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Tue, 20 Apr 2021 23:20:11 GMT
ARG version=8.292.10.1
# Tue, 20 Apr 2021 23:20:19 GMT
# ARGS: version=8.292.10.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Tue, 20 Apr 2021 23:20:19 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:20:20 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 20 Apr 2021 23:20:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ec31fbf474c99d6924bc337c81bd4bfd0bfadb5a7e318c5456a3e110d4e9b9`  
		Last Modified: Tue, 20 Apr 2021 23:22:28 GMT  
		Size: 99.0 MB (99014965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:73939d6cb017bdb3885ea35ae18af6c6bf403ae0000b25e59c84b1e95ec9ffea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:1a3472c57788ef9c33e2b830bea1f5227562e197aac294e3b27305c4a3429b9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101815532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49dc0e3993ba2b79800dfa61af11876aad3ac15bfb8d280b35e81049b7a6ef3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Tue, 20 Apr 2021 23:20:11 GMT
ARG version=8.292.10.1
# Tue, 20 Apr 2021 23:20:19 GMT
# ARGS: version=8.292.10.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Tue, 20 Apr 2021 23:20:19 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:20:20 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 20 Apr 2021 23:20:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ec31fbf474c99d6924bc337c81bd4bfd0bfadb5a7e318c5456a3e110d4e9b9`  
		Last Modified: Tue, 20 Apr 2021 23:22:28 GMT  
		Size: 99.0 MB (99014965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine-jre`

```console
$ docker pull amazoncorretto@sha256:9b512161b10206d94138a47759ca3e1a503f01d6b97169f99bd9fc52f76fb7b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8-alpine-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:efdb98e9a99c921602eed17fb06c2f0661abfdff42a9490589d523a55afad5b1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43136777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a944531e0b8aaf3cecdd7a3e65440030e6e4cfca9c15b10481a1ef41aa52d423`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Tue, 20 Apr 2021 23:20:11 GMT
ARG version=8.292.10.1
# Tue, 20 Apr 2021 23:20:26 GMT
# ARGS: version=8.292.10.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Tue, 20 Apr 2021 23:20:27 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:20:27 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4daa33c191f16afa306f7b3db9d2d8b3d1acf292d71a9414a041e146d4ba97a`  
		Last Modified: Tue, 20 Apr 2021 23:22:49 GMT  
		Size: 40.3 MB (40336210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u282-alpine-jre`

```console
$ docker pull amazoncorretto@sha256:9b512161b10206d94138a47759ca3e1a503f01d6b97169f99bd9fc52f76fb7b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8u282-alpine-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:efdb98e9a99c921602eed17fb06c2f0661abfdff42a9490589d523a55afad5b1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43136777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a944531e0b8aaf3cecdd7a3e65440030e6e4cfca9c15b10481a1ef41aa52d423`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Tue, 20 Apr 2021 23:20:11 GMT
ARG version=8.292.10.1
# Tue, 20 Apr 2021 23:20:26 GMT
# ARGS: version=8.292.10.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Tue, 20 Apr 2021 23:20:27 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:20:27 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4daa33c191f16afa306f7b3db9d2d8b3d1acf292d71a9414a041e146d4ba97a`  
		Last Modified: Tue, 20 Apr 2021 23:22:49 GMT  
		Size: 40.3 MB (40336210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u292`

```console
$ docker pull amazoncorretto@sha256:7f4379378c791fd02a5c93bd0e8f0694612d782c3665823413f1c5191d6f1262
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u292` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:00aee242da8f1dc4212eb0fbf63a1a8d405f3ad7ced4f37d8c47d21d5c7b8b7d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137238262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfaef49ef26491ebd020a02bb485e98c5c6bb9766427900580ae9c41e6e12524`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:19:20 GMT
ARG version=1.8.0_292.b10-1
# Tue, 20 Apr 2021 23:19:40 GMT
# ARGS: version=1.8.0_292.b10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:19:41 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:19:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ece89ed8d5944dabfaaa536301db77053bc6a2a996a272109b639f20b9cfca`  
		Last Modified: Tue, 20 Apr 2021 23:21:24 GMT  
		Size: 75.3 MB (75291677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u292` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:63b87dc056c11913fd13a02a6cd6a2d15e881b17021be3cd76bb452d7d09932c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123049888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e7684c1b0eb2a94a3e457a5cc240c76ab7140b4d211a6927a2e712480350a8e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:43:19 GMT
ARG version=1.8.0_292.b10-1
# Tue, 20 Apr 2021 23:43:53 GMT
# ARGS: version=1.8.0_292.b10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:43:55 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:43:55 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19674c905fc4a155e31837e0f8b91c7a503bd185ffae72d35ce7877265d63dae`  
		Last Modified: Tue, 20 Apr 2021 23:45:24 GMT  
		Size: 59.4 MB (59389850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u292-al2`

```console
$ docker pull amazoncorretto@sha256:7f4379378c791fd02a5c93bd0e8f0694612d782c3665823413f1c5191d6f1262
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u292-al2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:00aee242da8f1dc4212eb0fbf63a1a8d405f3ad7ced4f37d8c47d21d5c7b8b7d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137238262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfaef49ef26491ebd020a02bb485e98c5c6bb9766427900580ae9c41e6e12524`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:19:20 GMT
ARG version=1.8.0_292.b10-1
# Tue, 20 Apr 2021 23:19:40 GMT
# ARGS: version=1.8.0_292.b10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:19:41 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:19:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ece89ed8d5944dabfaaa536301db77053bc6a2a996a272109b639f20b9cfca`  
		Last Modified: Tue, 20 Apr 2021 23:21:24 GMT  
		Size: 75.3 MB (75291677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u292-al2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:63b87dc056c11913fd13a02a6cd6a2d15e881b17021be3cd76bb452d7d09932c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123049888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e7684c1b0eb2a94a3e457a5cc240c76ab7140b4d211a6927a2e712480350a8e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:43:19 GMT
ARG version=1.8.0_292.b10-1
# Tue, 20 Apr 2021 23:43:53 GMT
# ARGS: version=1.8.0_292.b10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:43:55 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:43:55 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19674c905fc4a155e31837e0f8b91c7a503bd185ffae72d35ce7877265d63dae`  
		Last Modified: Tue, 20 Apr 2021 23:45:24 GMT  
		Size: 59.4 MB (59389850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u292-alpine`

```console
$ docker pull amazoncorretto@sha256:73939d6cb017bdb3885ea35ae18af6c6bf403ae0000b25e59c84b1e95ec9ffea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8u292-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:1a3472c57788ef9c33e2b830bea1f5227562e197aac294e3b27305c4a3429b9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101815532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49dc0e3993ba2b79800dfa61af11876aad3ac15bfb8d280b35e81049b7a6ef3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Tue, 20 Apr 2021 23:20:11 GMT
ARG version=8.292.10.1
# Tue, 20 Apr 2021 23:20:19 GMT
# ARGS: version=8.292.10.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Tue, 20 Apr 2021 23:20:19 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:20:20 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 20 Apr 2021 23:20:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ec31fbf474c99d6924bc337c81bd4bfd0bfadb5a7e318c5456a3e110d4e9b9`  
		Last Modified: Tue, 20 Apr 2021 23:22:28 GMT  
		Size: 99.0 MB (99014965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:latest`

```console
$ docker pull amazoncorretto@sha256:7f4379378c791fd02a5c93bd0e8f0694612d782c3665823413f1c5191d6f1262
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:latest` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:00aee242da8f1dc4212eb0fbf63a1a8d405f3ad7ced4f37d8c47d21d5c7b8b7d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137238262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfaef49ef26491ebd020a02bb485e98c5c6bb9766427900580ae9c41e6e12524`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:19:20 GMT
ARG version=1.8.0_292.b10-1
# Tue, 20 Apr 2021 23:19:40 GMT
# ARGS: version=1.8.0_292.b10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:19:41 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:19:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ece89ed8d5944dabfaaa536301db77053bc6a2a996a272109b639f20b9cfca`  
		Last Modified: Tue, 20 Apr 2021 23:21:24 GMT  
		Size: 75.3 MB (75291677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:latest` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:63b87dc056c11913fd13a02a6cd6a2d15e881b17021be3cd76bb452d7d09932c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123049888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e7684c1b0eb2a94a3e457a5cc240c76ab7140b4d211a6927a2e712480350a8e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Tue, 20 Apr 2021 23:43:19 GMT
ARG version=1.8.0_292.b10-1
# Tue, 20 Apr 2021 23:43:53 GMT
# ARGS: version=1.8.0_292.b10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Apr 2021 23:43:55 GMT
ENV LANG=C.UTF-8
# Tue, 20 Apr 2021 23:43:55 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19674c905fc4a155e31837e0f8b91c7a503bd185ffae72d35ce7877265d63dae`  
		Last Modified: Tue, 20 Apr 2021 23:45:24 GMT  
		Size: 59.4 MB (59389850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
