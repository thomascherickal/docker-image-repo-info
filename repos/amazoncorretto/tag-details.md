<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazoncorretto`

-	[`amazoncorretto:11`](#amazoncorretto11)
-	[`amazoncorretto:11-al2-full`](#amazoncorretto11-al2-full)
-	[`amazoncorretto:11-al2-jdk`](#amazoncorretto11-al2-jdk)
-	[`amazoncorretto:11-alpine`](#amazoncorretto11-alpine)
-	[`amazoncorretto:11-alpine-full`](#amazoncorretto11-alpine-full)
-	[`amazoncorretto:11-alpine-jdk`](#amazoncorretto11-alpine-jdk)
-	[`amazoncorretto:11.0.10`](#amazoncorretto11010)
-	[`amazoncorretto:11.0.10-al2`](#amazoncorretto11010-al2)
-	[`amazoncorretto:11.0.10-alpine`](#amazoncorretto11010-alpine)
-	[`amazoncorretto:15`](#amazoncorretto15)
-	[`amazoncorretto:15-al2-full`](#amazoncorretto15-al2-full)
-	[`amazoncorretto:15-al2-jdk`](#amazoncorretto15-al2-jdk)
-	[`amazoncorretto:15-alpine`](#amazoncorretto15-alpine)
-	[`amazoncorretto:15-alpine-full`](#amazoncorretto15-alpine-full)
-	[`amazoncorretto:15-alpine-jdk`](#amazoncorretto15-alpine-jdk)
-	[`amazoncorretto:15.0.2`](#amazoncorretto1502)
-	[`amazoncorretto:15.0.2-al2`](#amazoncorretto1502-al2)
-	[`amazoncorretto:15.0.2-alpine`](#amazoncorretto1502-alpine)
-	[`amazoncorretto:16`](#amazoncorretto16)
-	[`amazoncorretto:16-al2-full`](#amazoncorretto16-al2-full)
-	[`amazoncorretto:16-al2-jdk`](#amazoncorretto16-al2-jdk)
-	[`amazoncorretto:16-alpine`](#amazoncorretto16-alpine)
-	[`amazoncorretto:16-alpine-full`](#amazoncorretto16-alpine-full)
-	[`amazoncorretto:16-alpine-jdk`](#amazoncorretto16-alpine-jdk)
-	[`amazoncorretto:16.0.0`](#amazoncorretto1600)
-	[`amazoncorretto:16.0.0-al2`](#amazoncorretto1600-al2)
-	[`amazoncorretto:16.0.0-alpine`](#amazoncorretto1600-alpine)
-	[`amazoncorretto:8`](#amazoncorretto8)
-	[`amazoncorretto:8-al2-full`](#amazoncorretto8-al2-full)
-	[`amazoncorretto:8-al2-jdk`](#amazoncorretto8-al2-jdk)
-	[`amazoncorretto:8-alpine`](#amazoncorretto8-alpine)
-	[`amazoncorretto:8-alpine-full`](#amazoncorretto8-alpine-full)
-	[`amazoncorretto:8-alpine-jdk`](#amazoncorretto8-alpine-jdk)
-	[`amazoncorretto:8-alpine-jre`](#amazoncorretto8-alpine-jre)
-	[`amazoncorretto:8u282`](#amazoncorretto8u282)
-	[`amazoncorretto:8u282-al2`](#amazoncorretto8u282-al2)
-	[`amazoncorretto:8u282-alpine`](#amazoncorretto8u282-alpine)
-	[`amazoncorretto:8u282-alpine-jre`](#amazoncorretto8u282-alpine-jre)
-	[`amazoncorretto:latest`](#amazoncorrettolatest)

## `amazoncorretto:11`

```console
$ docker pull amazoncorretto@sha256:b0324e90432e338106aa5dfd4dac4304dc4284039168ded07792cdad7b216ecd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:35a5b02442c06f6e8b20f824a2a7c3cef283cc1577c1a2978c5339f2a808aae4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.5 MB (208475193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73ebc812993c71d279c9f00dd90ad2c92ad0889a4d2d355c8f3d54b714c9bb46`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:19:44 GMT
ARG version=11.0.10.9-1
# Thu, 18 Mar 2021 01:19:58 GMT
# ARGS: version=11.0.10.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:19:59 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:19:59 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf985284f9fa24b184b0d16544b81abd2ea6dc25403e2d928da2ec487277b821`  
		Last Modified: Thu, 18 Mar 2021 01:23:26 GMT  
		Size: 146.5 MB (146540033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d57b9863f4df8ed90d61fae7cf7fbca823722ce25e5c238803abc3b3ac3dd7fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.2 MB (208232464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a182002a98cea21fc87722b507e7d8f05e23fe45189f1c2e620e9708eef61be5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:35:39 GMT
ARG version=11.0.10.9-1
# Wed, 24 Feb 2021 19:36:08 GMT
# ARGS: version=11.0.10.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 24 Feb 2021 19:36:10 GMT
ENV LANG=C.UTF-8
# Wed, 24 Feb 2021 19:36:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc87855b7feac70ec7389ae01e43d02841e30c1d550b99eeb4c599b63471ff1`  
		Last Modified: Wed, 24 Feb 2021 19:38:16 GMT  
		Size: 144.6 MB (144607927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-al2-full`

```console
$ docker pull amazoncorretto@sha256:b0324e90432e338106aa5dfd4dac4304dc4284039168ded07792cdad7b216ecd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:35a5b02442c06f6e8b20f824a2a7c3cef283cc1577c1a2978c5339f2a808aae4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.5 MB (208475193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73ebc812993c71d279c9f00dd90ad2c92ad0889a4d2d355c8f3d54b714c9bb46`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:19:44 GMT
ARG version=11.0.10.9-1
# Thu, 18 Mar 2021 01:19:58 GMT
# ARGS: version=11.0.10.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:19:59 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:19:59 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf985284f9fa24b184b0d16544b81abd2ea6dc25403e2d928da2ec487277b821`  
		Last Modified: Thu, 18 Mar 2021 01:23:26 GMT  
		Size: 146.5 MB (146540033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d57b9863f4df8ed90d61fae7cf7fbca823722ce25e5c238803abc3b3ac3dd7fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.2 MB (208232464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a182002a98cea21fc87722b507e7d8f05e23fe45189f1c2e620e9708eef61be5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:35:39 GMT
ARG version=11.0.10.9-1
# Wed, 24 Feb 2021 19:36:08 GMT
# ARGS: version=11.0.10.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 24 Feb 2021 19:36:10 GMT
ENV LANG=C.UTF-8
# Wed, 24 Feb 2021 19:36:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc87855b7feac70ec7389ae01e43d02841e30c1d550b99eeb4c599b63471ff1`  
		Last Modified: Wed, 24 Feb 2021 19:38:16 GMT  
		Size: 144.6 MB (144607927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:b0324e90432e338106aa5dfd4dac4304dc4284039168ded07792cdad7b216ecd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:35a5b02442c06f6e8b20f824a2a7c3cef283cc1577c1a2978c5339f2a808aae4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.5 MB (208475193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73ebc812993c71d279c9f00dd90ad2c92ad0889a4d2d355c8f3d54b714c9bb46`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:19:44 GMT
ARG version=11.0.10.9-1
# Thu, 18 Mar 2021 01:19:58 GMT
# ARGS: version=11.0.10.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:19:59 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:19:59 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf985284f9fa24b184b0d16544b81abd2ea6dc25403e2d928da2ec487277b821`  
		Last Modified: Thu, 18 Mar 2021 01:23:26 GMT  
		Size: 146.5 MB (146540033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d57b9863f4df8ed90d61fae7cf7fbca823722ce25e5c238803abc3b3ac3dd7fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.2 MB (208232464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a182002a98cea21fc87722b507e7d8f05e23fe45189f1c2e620e9708eef61be5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:35:39 GMT
ARG version=11.0.10.9-1
# Wed, 24 Feb 2021 19:36:08 GMT
# ARGS: version=11.0.10.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 24 Feb 2021 19:36:10 GMT
ENV LANG=C.UTF-8
# Wed, 24 Feb 2021 19:36:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc87855b7feac70ec7389ae01e43d02841e30c1d550b99eeb4c599b63471ff1`  
		Last Modified: Wed, 24 Feb 2021 19:38:16 GMT  
		Size: 144.6 MB (144607927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-alpine`

```console
$ docker pull amazoncorretto@sha256:2414bd48272689ee0a33512ac382c7e06fd256ab0fcab832d142a18e7b007315
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:11-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:b3c0e7c1b7afef6019da95821bd89dce5321da1fe08596911a8f338fff43cd3b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.1 MB (195087149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97bf8e55a3a858eb10f42e7b4f2d497493b48870c3b02d371df6ba00caa51be0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:27 GMT
ARG version=11.0.10.9.1
# Fri, 26 Mar 2021 01:59:34 GMT
# ARGS: version=11.0.10.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Fri, 26 Mar 2021 01:59:34 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 26 Mar 2021 01:59:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ce14dd7fb4ebb181c1d830a43ea9cb517096b69188df500efcbfd3079598c9`  
		Last Modified: Fri, 26 Mar 2021 02:02:09 GMT  
		Size: 192.3 MB (192287387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-alpine-full`

```console
$ docker pull amazoncorretto@sha256:2414bd48272689ee0a33512ac382c7e06fd256ab0fcab832d142a18e7b007315
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:11-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:b3c0e7c1b7afef6019da95821bd89dce5321da1fe08596911a8f338fff43cd3b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.1 MB (195087149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97bf8e55a3a858eb10f42e7b4f2d497493b48870c3b02d371df6ba00caa51be0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:27 GMT
ARG version=11.0.10.9.1
# Fri, 26 Mar 2021 01:59:34 GMT
# ARGS: version=11.0.10.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Fri, 26 Mar 2021 01:59:34 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 26 Mar 2021 01:59:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ce14dd7fb4ebb181c1d830a43ea9cb517096b69188df500efcbfd3079598c9`  
		Last Modified: Fri, 26 Mar 2021 02:02:09 GMT  
		Size: 192.3 MB (192287387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:2414bd48272689ee0a33512ac382c7e06fd256ab0fcab832d142a18e7b007315
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:11-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:b3c0e7c1b7afef6019da95821bd89dce5321da1fe08596911a8f338fff43cd3b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.1 MB (195087149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97bf8e55a3a858eb10f42e7b4f2d497493b48870c3b02d371df6ba00caa51be0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:27 GMT
ARG version=11.0.10.9.1
# Fri, 26 Mar 2021 01:59:34 GMT
# ARGS: version=11.0.10.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Fri, 26 Mar 2021 01:59:34 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 26 Mar 2021 01:59:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ce14dd7fb4ebb181c1d830a43ea9cb517096b69188df500efcbfd3079598c9`  
		Last Modified: Fri, 26 Mar 2021 02:02:09 GMT  
		Size: 192.3 MB (192287387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11.0.10`

```console
$ docker pull amazoncorretto@sha256:b0324e90432e338106aa5dfd4dac4304dc4284039168ded07792cdad7b216ecd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11.0.10` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:35a5b02442c06f6e8b20f824a2a7c3cef283cc1577c1a2978c5339f2a808aae4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.5 MB (208475193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73ebc812993c71d279c9f00dd90ad2c92ad0889a4d2d355c8f3d54b714c9bb46`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:19:44 GMT
ARG version=11.0.10.9-1
# Thu, 18 Mar 2021 01:19:58 GMT
# ARGS: version=11.0.10.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:19:59 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:19:59 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf985284f9fa24b184b0d16544b81abd2ea6dc25403e2d928da2ec487277b821`  
		Last Modified: Thu, 18 Mar 2021 01:23:26 GMT  
		Size: 146.5 MB (146540033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11.0.10` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d57b9863f4df8ed90d61fae7cf7fbca823722ce25e5c238803abc3b3ac3dd7fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.2 MB (208232464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a182002a98cea21fc87722b507e7d8f05e23fe45189f1c2e620e9708eef61be5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:35:39 GMT
ARG version=11.0.10.9-1
# Wed, 24 Feb 2021 19:36:08 GMT
# ARGS: version=11.0.10.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 24 Feb 2021 19:36:10 GMT
ENV LANG=C.UTF-8
# Wed, 24 Feb 2021 19:36:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc87855b7feac70ec7389ae01e43d02841e30c1d550b99eeb4c599b63471ff1`  
		Last Modified: Wed, 24 Feb 2021 19:38:16 GMT  
		Size: 144.6 MB (144607927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11.0.10-al2`

```console
$ docker pull amazoncorretto@sha256:b0324e90432e338106aa5dfd4dac4304dc4284039168ded07792cdad7b216ecd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11.0.10-al2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:35a5b02442c06f6e8b20f824a2a7c3cef283cc1577c1a2978c5339f2a808aae4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.5 MB (208475193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73ebc812993c71d279c9f00dd90ad2c92ad0889a4d2d355c8f3d54b714c9bb46`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:19:44 GMT
ARG version=11.0.10.9-1
# Thu, 18 Mar 2021 01:19:58 GMT
# ARGS: version=11.0.10.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:19:59 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:19:59 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf985284f9fa24b184b0d16544b81abd2ea6dc25403e2d928da2ec487277b821`  
		Last Modified: Thu, 18 Mar 2021 01:23:26 GMT  
		Size: 146.5 MB (146540033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11.0.10-al2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d57b9863f4df8ed90d61fae7cf7fbca823722ce25e5c238803abc3b3ac3dd7fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.2 MB (208232464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a182002a98cea21fc87722b507e7d8f05e23fe45189f1c2e620e9708eef61be5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:35:39 GMT
ARG version=11.0.10.9-1
# Wed, 24 Feb 2021 19:36:08 GMT
# ARGS: version=11.0.10.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 24 Feb 2021 19:36:10 GMT
ENV LANG=C.UTF-8
# Wed, 24 Feb 2021 19:36:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc87855b7feac70ec7389ae01e43d02841e30c1d550b99eeb4c599b63471ff1`  
		Last Modified: Wed, 24 Feb 2021 19:38:16 GMT  
		Size: 144.6 MB (144607927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11.0.10-alpine`

```console
$ docker pull amazoncorretto@sha256:2414bd48272689ee0a33512ac382c7e06fd256ab0fcab832d142a18e7b007315
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:11.0.10-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:b3c0e7c1b7afef6019da95821bd89dce5321da1fe08596911a8f338fff43cd3b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.1 MB (195087149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97bf8e55a3a858eb10f42e7b4f2d497493b48870c3b02d371df6ba00caa51be0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:27 GMT
ARG version=11.0.10.9.1
# Fri, 26 Mar 2021 01:59:34 GMT
# ARGS: version=11.0.10.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Fri, 26 Mar 2021 01:59:34 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 26 Mar 2021 01:59:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ce14dd7fb4ebb181c1d830a43ea9cb517096b69188df500efcbfd3079598c9`  
		Last Modified: Fri, 26 Mar 2021 02:02:09 GMT  
		Size: 192.3 MB (192287387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15`

```console
$ docker pull amazoncorretto@sha256:413adb451286cbdc66f53ceb7e9ad0931d3204e7c01f53c750957c19c79bd76d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:15` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:6347e5e7d713700282342ca0ad54f9024a928cba4c983112111bb6377c59b121
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.6 MB (217604678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f2bbfd00d28caa0da08996df4230c98e98d462ea00c0b3d87ef844ae775e2bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:20:48 GMT
ARG version=15.0.2.7-1
# Thu, 18 Mar 2021 01:21:03 GMT
# ARGS: version=15.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:21:04 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:21:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a1b14848cc4fca9939aa433239aa0f8bd6085758a3e249d95a797d5be2dfec`  
		Last Modified: Thu, 18 Mar 2021 01:25:20 GMT  
		Size: 155.7 MB (155669518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:15` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:1a2ec0c89f7ae677ecfd28cc30aab61b938799de29ea30a30281949b77a8ecbd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.2 MB (219172287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cae7dbe3f83ecb9f6f3e1a9974d1345ae1d876c3d5ae785f3d5f8cf073c3566d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:36:22 GMT
ARG version=15.0.2.7-1
# Wed, 24 Feb 2021 19:36:51 GMT
# ARGS: version=15.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 24 Feb 2021 19:36:52 GMT
ENV LANG=C.UTF-8
# Wed, 24 Feb 2021 19:36:53 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d916db12a96784d3ebea43aa5789717cb262499ab047b4b710b403cc2f6db4`  
		Last Modified: Wed, 24 Feb 2021 19:38:57 GMT  
		Size: 155.5 MB (155547750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15-al2-full`

```console
$ docker pull amazoncorretto@sha256:413adb451286cbdc66f53ceb7e9ad0931d3204e7c01f53c750957c19c79bd76d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:15-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:6347e5e7d713700282342ca0ad54f9024a928cba4c983112111bb6377c59b121
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.6 MB (217604678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f2bbfd00d28caa0da08996df4230c98e98d462ea00c0b3d87ef844ae775e2bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:20:48 GMT
ARG version=15.0.2.7-1
# Thu, 18 Mar 2021 01:21:03 GMT
# ARGS: version=15.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:21:04 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:21:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a1b14848cc4fca9939aa433239aa0f8bd6085758a3e249d95a797d5be2dfec`  
		Last Modified: Thu, 18 Mar 2021 01:25:20 GMT  
		Size: 155.7 MB (155669518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:15-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:1a2ec0c89f7ae677ecfd28cc30aab61b938799de29ea30a30281949b77a8ecbd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.2 MB (219172287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cae7dbe3f83ecb9f6f3e1a9974d1345ae1d876c3d5ae785f3d5f8cf073c3566d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:36:22 GMT
ARG version=15.0.2.7-1
# Wed, 24 Feb 2021 19:36:51 GMT
# ARGS: version=15.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 24 Feb 2021 19:36:52 GMT
ENV LANG=C.UTF-8
# Wed, 24 Feb 2021 19:36:53 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d916db12a96784d3ebea43aa5789717cb262499ab047b4b710b403cc2f6db4`  
		Last Modified: Wed, 24 Feb 2021 19:38:57 GMT  
		Size: 155.5 MB (155547750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:413adb451286cbdc66f53ceb7e9ad0931d3204e7c01f53c750957c19c79bd76d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:15-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:6347e5e7d713700282342ca0ad54f9024a928cba4c983112111bb6377c59b121
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.6 MB (217604678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f2bbfd00d28caa0da08996df4230c98e98d462ea00c0b3d87ef844ae775e2bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:20:48 GMT
ARG version=15.0.2.7-1
# Thu, 18 Mar 2021 01:21:03 GMT
# ARGS: version=15.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:21:04 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:21:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a1b14848cc4fca9939aa433239aa0f8bd6085758a3e249d95a797d5be2dfec`  
		Last Modified: Thu, 18 Mar 2021 01:25:20 GMT  
		Size: 155.7 MB (155669518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:15-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:1a2ec0c89f7ae677ecfd28cc30aab61b938799de29ea30a30281949b77a8ecbd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.2 MB (219172287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cae7dbe3f83ecb9f6f3e1a9974d1345ae1d876c3d5ae785f3d5f8cf073c3566d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:36:22 GMT
ARG version=15.0.2.7-1
# Wed, 24 Feb 2021 19:36:51 GMT
# ARGS: version=15.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 24 Feb 2021 19:36:52 GMT
ENV LANG=C.UTF-8
# Wed, 24 Feb 2021 19:36:53 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d916db12a96784d3ebea43aa5789717cb262499ab047b4b710b403cc2f6db4`  
		Last Modified: Wed, 24 Feb 2021 19:38:57 GMT  
		Size: 155.5 MB (155547750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15-alpine`

```console
$ docker pull amazoncorretto@sha256:435762204cc194628c190bd1e7ae1314d2e244b2faf42cfec1f8b0efb6183e6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:15-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:3a4e2dde42bfc4d93a28aaf0e5cfc2ba0b173787fc8147601ec081228c8ea515
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.7 MB (207723606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:284fac6862c63db92b6b441c27f75a5797ac17bb31c65185a629588778b2ec50`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:42 GMT
ARG version=15.0.2.7.1
# Fri, 26 Mar 2021 01:59:52 GMT
# ARGS: version=15.0.2.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-15=$version-r0
# Fri, 26 Mar 2021 01:59:52 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 26 Mar 2021 01:59:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc105230db47cb4483a93980f608f1d629c2bab534c153fd386eb601dcd65d4`  
		Last Modified: Fri, 26 Mar 2021 02:02:53 GMT  
		Size: 204.9 MB (204923844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15-alpine-full`

```console
$ docker pull amazoncorretto@sha256:435762204cc194628c190bd1e7ae1314d2e244b2faf42cfec1f8b0efb6183e6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:15-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:3a4e2dde42bfc4d93a28aaf0e5cfc2ba0b173787fc8147601ec081228c8ea515
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.7 MB (207723606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:284fac6862c63db92b6b441c27f75a5797ac17bb31c65185a629588778b2ec50`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:42 GMT
ARG version=15.0.2.7.1
# Fri, 26 Mar 2021 01:59:52 GMT
# ARGS: version=15.0.2.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-15=$version-r0
# Fri, 26 Mar 2021 01:59:52 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 26 Mar 2021 01:59:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc105230db47cb4483a93980f608f1d629c2bab534c153fd386eb601dcd65d4`  
		Last Modified: Fri, 26 Mar 2021 02:02:53 GMT  
		Size: 204.9 MB (204923844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:435762204cc194628c190bd1e7ae1314d2e244b2faf42cfec1f8b0efb6183e6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:15-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:3a4e2dde42bfc4d93a28aaf0e5cfc2ba0b173787fc8147601ec081228c8ea515
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.7 MB (207723606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:284fac6862c63db92b6b441c27f75a5797ac17bb31c65185a629588778b2ec50`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:42 GMT
ARG version=15.0.2.7.1
# Fri, 26 Mar 2021 01:59:52 GMT
# ARGS: version=15.0.2.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-15=$version-r0
# Fri, 26 Mar 2021 01:59:52 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 26 Mar 2021 01:59:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc105230db47cb4483a93980f608f1d629c2bab534c153fd386eb601dcd65d4`  
		Last Modified: Fri, 26 Mar 2021 02:02:53 GMT  
		Size: 204.9 MB (204923844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15.0.2`

```console
$ docker pull amazoncorretto@sha256:413adb451286cbdc66f53ceb7e9ad0931d3204e7c01f53c750957c19c79bd76d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:15.0.2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:6347e5e7d713700282342ca0ad54f9024a928cba4c983112111bb6377c59b121
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.6 MB (217604678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f2bbfd00d28caa0da08996df4230c98e98d462ea00c0b3d87ef844ae775e2bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:20:48 GMT
ARG version=15.0.2.7-1
# Thu, 18 Mar 2021 01:21:03 GMT
# ARGS: version=15.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:21:04 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:21:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a1b14848cc4fca9939aa433239aa0f8bd6085758a3e249d95a797d5be2dfec`  
		Last Modified: Thu, 18 Mar 2021 01:25:20 GMT  
		Size: 155.7 MB (155669518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:15.0.2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:1a2ec0c89f7ae677ecfd28cc30aab61b938799de29ea30a30281949b77a8ecbd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.2 MB (219172287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cae7dbe3f83ecb9f6f3e1a9974d1345ae1d876c3d5ae785f3d5f8cf073c3566d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:36:22 GMT
ARG version=15.0.2.7-1
# Wed, 24 Feb 2021 19:36:51 GMT
# ARGS: version=15.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 24 Feb 2021 19:36:52 GMT
ENV LANG=C.UTF-8
# Wed, 24 Feb 2021 19:36:53 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d916db12a96784d3ebea43aa5789717cb262499ab047b4b710b403cc2f6db4`  
		Last Modified: Wed, 24 Feb 2021 19:38:57 GMT  
		Size: 155.5 MB (155547750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15.0.2-al2`

```console
$ docker pull amazoncorretto@sha256:413adb451286cbdc66f53ceb7e9ad0931d3204e7c01f53c750957c19c79bd76d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:15.0.2-al2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:6347e5e7d713700282342ca0ad54f9024a928cba4c983112111bb6377c59b121
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.6 MB (217604678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f2bbfd00d28caa0da08996df4230c98e98d462ea00c0b3d87ef844ae775e2bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:20:48 GMT
ARG version=15.0.2.7-1
# Thu, 18 Mar 2021 01:21:03 GMT
# ARGS: version=15.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:21:04 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:21:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a1b14848cc4fca9939aa433239aa0f8bd6085758a3e249d95a797d5be2dfec`  
		Last Modified: Thu, 18 Mar 2021 01:25:20 GMT  
		Size: 155.7 MB (155669518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:15.0.2-al2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:1a2ec0c89f7ae677ecfd28cc30aab61b938799de29ea30a30281949b77a8ecbd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.2 MB (219172287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cae7dbe3f83ecb9f6f3e1a9974d1345ae1d876c3d5ae785f3d5f8cf073c3566d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:36:22 GMT
ARG version=15.0.2.7-1
# Wed, 24 Feb 2021 19:36:51 GMT
# ARGS: version=15.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 24 Feb 2021 19:36:52 GMT
ENV LANG=C.UTF-8
# Wed, 24 Feb 2021 19:36:53 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d916db12a96784d3ebea43aa5789717cb262499ab047b4b710b403cc2f6db4`  
		Last Modified: Wed, 24 Feb 2021 19:38:57 GMT  
		Size: 155.5 MB (155547750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15.0.2-alpine`

```console
$ docker pull amazoncorretto@sha256:435762204cc194628c190bd1e7ae1314d2e244b2faf42cfec1f8b0efb6183e6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:15.0.2-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:3a4e2dde42bfc4d93a28aaf0e5cfc2ba0b173787fc8147601ec081228c8ea515
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.7 MB (207723606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:284fac6862c63db92b6b441c27f75a5797ac17bb31c65185a629588778b2ec50`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:42 GMT
ARG version=15.0.2.7.1
# Fri, 26 Mar 2021 01:59:52 GMT
# ARGS: version=15.0.2.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-15=$version-r0
# Fri, 26 Mar 2021 01:59:52 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 26 Mar 2021 01:59:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc105230db47cb4483a93980f608f1d629c2bab534c153fd386eb601dcd65d4`  
		Last Modified: Fri, 26 Mar 2021 02:02:53 GMT  
		Size: 204.9 MB (204923844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16`

```console
$ docker pull amazoncorretto@sha256:fba1f65d4c482aabdc953f07a7cc71e5eaf29ee27989836dc00d369c098957d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:049000605566e78edc28620584d15be53d6a52a4523b9127959590ab9bf03f9a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221870649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:574534f6ee837df7df893438e0813be532c93273c3cc96d874b09e37b7cd8e44`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:21:21 GMT
ARG version=16.0.0.36-1
# Thu, 18 Mar 2021 01:21:37 GMT
# ARGS: version=16.0.0.36-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:21:38 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:21:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9092c7df833910471d3e8ee541a2f28a3659972660474f01a9fab4e6ae8f56`  
		Last Modified: Thu, 18 Mar 2021 01:26:31 GMT  
		Size: 159.9 MB (159935489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:0f126d71e74c4b61b4b8cf4dc4f9dd5a1375fc1dda1ff281ddd63b6a1d9a9f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.5 MB (223515735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b2dec0095bd7699386451e858d5eb8062256c862bf1702753d05553bf6f191`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 00:39:54 GMT
ARG version=16.0.0.36-1
# Thu, 18 Mar 2021 00:40:33 GMT
# ARGS: version=16.0.0.36-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 00:40:35 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 00:40:36 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2214528904f7c29ecf0ff8106a2ca25b33ec6dbc5e51ff3e0e8cc46c35d3d97c`  
		Last Modified: Thu, 18 Mar 2021 00:41:35 GMT  
		Size: 159.9 MB (159891198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-al2-full`

```console
$ docker pull amazoncorretto@sha256:fba1f65d4c482aabdc953f07a7cc71e5eaf29ee27989836dc00d369c098957d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:049000605566e78edc28620584d15be53d6a52a4523b9127959590ab9bf03f9a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221870649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:574534f6ee837df7df893438e0813be532c93273c3cc96d874b09e37b7cd8e44`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:21:21 GMT
ARG version=16.0.0.36-1
# Thu, 18 Mar 2021 01:21:37 GMT
# ARGS: version=16.0.0.36-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:21:38 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:21:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9092c7df833910471d3e8ee541a2f28a3659972660474f01a9fab4e6ae8f56`  
		Last Modified: Thu, 18 Mar 2021 01:26:31 GMT  
		Size: 159.9 MB (159935489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:0f126d71e74c4b61b4b8cf4dc4f9dd5a1375fc1dda1ff281ddd63b6a1d9a9f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.5 MB (223515735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b2dec0095bd7699386451e858d5eb8062256c862bf1702753d05553bf6f191`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 00:39:54 GMT
ARG version=16.0.0.36-1
# Thu, 18 Mar 2021 00:40:33 GMT
# ARGS: version=16.0.0.36-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 00:40:35 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 00:40:36 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2214528904f7c29ecf0ff8106a2ca25b33ec6dbc5e51ff3e0e8cc46c35d3d97c`  
		Last Modified: Thu, 18 Mar 2021 00:41:35 GMT  
		Size: 159.9 MB (159891198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:fba1f65d4c482aabdc953f07a7cc71e5eaf29ee27989836dc00d369c098957d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:049000605566e78edc28620584d15be53d6a52a4523b9127959590ab9bf03f9a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221870649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:574534f6ee837df7df893438e0813be532c93273c3cc96d874b09e37b7cd8e44`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:21:21 GMT
ARG version=16.0.0.36-1
# Thu, 18 Mar 2021 01:21:37 GMT
# ARGS: version=16.0.0.36-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:21:38 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:21:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9092c7df833910471d3e8ee541a2f28a3659972660474f01a9fab4e6ae8f56`  
		Last Modified: Thu, 18 Mar 2021 01:26:31 GMT  
		Size: 159.9 MB (159935489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:0f126d71e74c4b61b4b8cf4dc4f9dd5a1375fc1dda1ff281ddd63b6a1d9a9f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.5 MB (223515735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b2dec0095bd7699386451e858d5eb8062256c862bf1702753d05553bf6f191`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 00:39:54 GMT
ARG version=16.0.0.36-1
# Thu, 18 Mar 2021 00:40:33 GMT
# ARGS: version=16.0.0.36-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 00:40:35 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 00:40:36 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2214528904f7c29ecf0ff8106a2ca25b33ec6dbc5e51ff3e0e8cc46c35d3d97c`  
		Last Modified: Thu, 18 Mar 2021 00:41:35 GMT  
		Size: 159.9 MB (159891198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-alpine`

```console
$ docker pull amazoncorretto@sha256:7470817f274ef355d35690f0880905489ce5dd31c7072b92207f5d9cea662f76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:16-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:810a21f19ee4242395d47f04165e325f226e6f42f792f73beb66aa76f9accf2e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.4 MB (212399833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bddb13d1ed31573664d38308570713573c159bff9c8a4eb8b75a30ad73ba2ee`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:00:00 GMT
ARG version=16.0.0.36.1
# Fri, 26 Mar 2021 02:00:13 GMT
# ARGS: version=16.0.0.36.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-16=$version-r0
# Fri, 26 Mar 2021 02:00:14 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 02:00:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 26 Mar 2021 02:00:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda1db7c9f353cfa836d313a19574ada78804bc8939be7a3d3dd8d0ff41ccd6f`  
		Last Modified: Fri, 26 Mar 2021 02:03:37 GMT  
		Size: 209.6 MB (209600071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-alpine-full`

```console
$ docker pull amazoncorretto@sha256:7470817f274ef355d35690f0880905489ce5dd31c7072b92207f5d9cea662f76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:16-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:810a21f19ee4242395d47f04165e325f226e6f42f792f73beb66aa76f9accf2e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.4 MB (212399833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bddb13d1ed31573664d38308570713573c159bff9c8a4eb8b75a30ad73ba2ee`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:00:00 GMT
ARG version=16.0.0.36.1
# Fri, 26 Mar 2021 02:00:13 GMT
# ARGS: version=16.0.0.36.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-16=$version-r0
# Fri, 26 Mar 2021 02:00:14 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 02:00:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 26 Mar 2021 02:00:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda1db7c9f353cfa836d313a19574ada78804bc8939be7a3d3dd8d0ff41ccd6f`  
		Last Modified: Fri, 26 Mar 2021 02:03:37 GMT  
		Size: 209.6 MB (209600071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:7470817f274ef355d35690f0880905489ce5dd31c7072b92207f5d9cea662f76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:16-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:810a21f19ee4242395d47f04165e325f226e6f42f792f73beb66aa76f9accf2e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.4 MB (212399833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bddb13d1ed31573664d38308570713573c159bff9c8a4eb8b75a30ad73ba2ee`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:00:00 GMT
ARG version=16.0.0.36.1
# Fri, 26 Mar 2021 02:00:13 GMT
# ARGS: version=16.0.0.36.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-16=$version-r0
# Fri, 26 Mar 2021 02:00:14 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 02:00:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 26 Mar 2021 02:00:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda1db7c9f353cfa836d313a19574ada78804bc8939be7a3d3dd8d0ff41ccd6f`  
		Last Modified: Fri, 26 Mar 2021 02:03:37 GMT  
		Size: 209.6 MB (209600071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16.0.0`

```console
$ docker pull amazoncorretto@sha256:fba1f65d4c482aabdc953f07a7cc71e5eaf29ee27989836dc00d369c098957d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16.0.0` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:049000605566e78edc28620584d15be53d6a52a4523b9127959590ab9bf03f9a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221870649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:574534f6ee837df7df893438e0813be532c93273c3cc96d874b09e37b7cd8e44`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:21:21 GMT
ARG version=16.0.0.36-1
# Thu, 18 Mar 2021 01:21:37 GMT
# ARGS: version=16.0.0.36-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:21:38 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:21:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9092c7df833910471d3e8ee541a2f28a3659972660474f01a9fab4e6ae8f56`  
		Last Modified: Thu, 18 Mar 2021 01:26:31 GMT  
		Size: 159.9 MB (159935489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16.0.0` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:0f126d71e74c4b61b4b8cf4dc4f9dd5a1375fc1dda1ff281ddd63b6a1d9a9f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.5 MB (223515735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b2dec0095bd7699386451e858d5eb8062256c862bf1702753d05553bf6f191`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 00:39:54 GMT
ARG version=16.0.0.36-1
# Thu, 18 Mar 2021 00:40:33 GMT
# ARGS: version=16.0.0.36-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 00:40:35 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 00:40:36 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2214528904f7c29ecf0ff8106a2ca25b33ec6dbc5e51ff3e0e8cc46c35d3d97c`  
		Last Modified: Thu, 18 Mar 2021 00:41:35 GMT  
		Size: 159.9 MB (159891198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16.0.0-al2`

```console
$ docker pull amazoncorretto@sha256:fba1f65d4c482aabdc953f07a7cc71e5eaf29ee27989836dc00d369c098957d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:16.0.0-al2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:049000605566e78edc28620584d15be53d6a52a4523b9127959590ab9bf03f9a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221870649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:574534f6ee837df7df893438e0813be532c93273c3cc96d874b09e37b7cd8e44`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:21:21 GMT
ARG version=16.0.0.36-1
# Thu, 18 Mar 2021 01:21:37 GMT
# ARGS: version=16.0.0.36-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:21:38 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:21:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9092c7df833910471d3e8ee541a2f28a3659972660474f01a9fab4e6ae8f56`  
		Last Modified: Thu, 18 Mar 2021 01:26:31 GMT  
		Size: 159.9 MB (159935489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:16.0.0-al2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:0f126d71e74c4b61b4b8cf4dc4f9dd5a1375fc1dda1ff281ddd63b6a1d9a9f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.5 MB (223515735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b2dec0095bd7699386451e858d5eb8062256c862bf1702753d05553bf6f191`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 00:39:54 GMT
ARG version=16.0.0.36-1
# Thu, 18 Mar 2021 00:40:33 GMT
# ARGS: version=16.0.0.36-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 00:40:35 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 00:40:36 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2214528904f7c29ecf0ff8106a2ca25b33ec6dbc5e51ff3e0e8cc46c35d3d97c`  
		Last Modified: Thu, 18 Mar 2021 00:41:35 GMT  
		Size: 159.9 MB (159891198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:16.0.0-alpine`

```console
$ docker pull amazoncorretto@sha256:7470817f274ef355d35690f0880905489ce5dd31c7072b92207f5d9cea662f76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:16.0.0-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:810a21f19ee4242395d47f04165e325f226e6f42f792f73beb66aa76f9accf2e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.4 MB (212399833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bddb13d1ed31573664d38308570713573c159bff9c8a4eb8b75a30ad73ba2ee`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:00:00 GMT
ARG version=16.0.0.36.1
# Fri, 26 Mar 2021 02:00:13 GMT
# ARGS: version=16.0.0.36.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-16=$version-r0
# Fri, 26 Mar 2021 02:00:14 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 02:00:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 26 Mar 2021 02:00:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda1db7c9f353cfa836d313a19574ada78804bc8939be7a3d3dd8d0ff41ccd6f`  
		Last Modified: Fri, 26 Mar 2021 02:03:37 GMT  
		Size: 209.6 MB (209600071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8`

```console
$ docker pull amazoncorretto@sha256:8d63e7a8fa23f9911e168e293efd12a3d7c071170a1f12573daedd75863525e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:36ede9ee499243c633c9f1a564d6e6778bcecc0a1dd54ac04f6e3b2c5edededb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137228963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bf2504e87fa9a72b931331c3a8896094bace65ae2a2315d1e299d6296299313`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:19:26 GMT
ARG version=1.8.0_282.b08-1
# Thu, 18 Mar 2021 01:19:40 GMT
# ARGS: version=1.8.0_282.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:19:40 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:19:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376e88159f3d6c2882e0ed403c2a5a0c9e9deb0bd43bed9e388ce2f142ef7534`  
		Last Modified: Thu, 18 Mar 2021 01:22:53 GMT  
		Size: 75.3 MB (75293803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:8f4acd8b2dc74007708d0b702ff8691bdd48cc53d9a04dd212adc4b3717ee1ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122993322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94ca05b6a97afeb0c2290f5690cc6991118113271816cbf04cee4588495f59b1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:35:03 GMT
ARG version=1.8.0_282.b08-1
# Wed, 24 Feb 2021 19:35:27 GMT
# ARGS: version=1.8.0_282.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 24 Feb 2021 19:35:29 GMT
ENV LANG=C.UTF-8
# Wed, 24 Feb 2021 19:35:29 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1179eb6d5a9474bde2c1234c9e205f5845bd0420cb1c5439411d483f14c142`  
		Last Modified: Wed, 24 Feb 2021 19:37:40 GMT  
		Size: 59.4 MB (59368785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-al2-full`

```console
$ docker pull amazoncorretto@sha256:8d63e7a8fa23f9911e168e293efd12a3d7c071170a1f12573daedd75863525e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:36ede9ee499243c633c9f1a564d6e6778bcecc0a1dd54ac04f6e3b2c5edededb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137228963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bf2504e87fa9a72b931331c3a8896094bace65ae2a2315d1e299d6296299313`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:19:26 GMT
ARG version=1.8.0_282.b08-1
# Thu, 18 Mar 2021 01:19:40 GMT
# ARGS: version=1.8.0_282.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:19:40 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:19:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376e88159f3d6c2882e0ed403c2a5a0c9e9deb0bd43bed9e388ce2f142ef7534`  
		Last Modified: Thu, 18 Mar 2021 01:22:53 GMT  
		Size: 75.3 MB (75293803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:8f4acd8b2dc74007708d0b702ff8691bdd48cc53d9a04dd212adc4b3717ee1ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122993322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94ca05b6a97afeb0c2290f5690cc6991118113271816cbf04cee4588495f59b1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:35:03 GMT
ARG version=1.8.0_282.b08-1
# Wed, 24 Feb 2021 19:35:27 GMT
# ARGS: version=1.8.0_282.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 24 Feb 2021 19:35:29 GMT
ENV LANG=C.UTF-8
# Wed, 24 Feb 2021 19:35:29 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1179eb6d5a9474bde2c1234c9e205f5845bd0420cb1c5439411d483f14c142`  
		Last Modified: Wed, 24 Feb 2021 19:37:40 GMT  
		Size: 59.4 MB (59368785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:8d63e7a8fa23f9911e168e293efd12a3d7c071170a1f12573daedd75863525e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:36ede9ee499243c633c9f1a564d6e6778bcecc0a1dd54ac04f6e3b2c5edededb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137228963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bf2504e87fa9a72b931331c3a8896094bace65ae2a2315d1e299d6296299313`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:19:26 GMT
ARG version=1.8.0_282.b08-1
# Thu, 18 Mar 2021 01:19:40 GMT
# ARGS: version=1.8.0_282.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:19:40 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:19:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376e88159f3d6c2882e0ed403c2a5a0c9e9deb0bd43bed9e388ce2f142ef7534`  
		Last Modified: Thu, 18 Mar 2021 01:22:53 GMT  
		Size: 75.3 MB (75293803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:8f4acd8b2dc74007708d0b702ff8691bdd48cc53d9a04dd212adc4b3717ee1ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122993322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94ca05b6a97afeb0c2290f5690cc6991118113271816cbf04cee4588495f59b1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:35:03 GMT
ARG version=1.8.0_282.b08-1
# Wed, 24 Feb 2021 19:35:27 GMT
# ARGS: version=1.8.0_282.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 24 Feb 2021 19:35:29 GMT
ENV LANG=C.UTF-8
# Wed, 24 Feb 2021 19:35:29 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1179eb6d5a9474bde2c1234c9e205f5845bd0420cb1c5439411d483f14c142`  
		Last Modified: Wed, 24 Feb 2021 19:37:40 GMT  
		Size: 59.4 MB (59368785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine`

```console
$ docker pull amazoncorretto@sha256:9a482474fd3b479ca9e76b56299a1a8bb90b1438f00db394e8b3e8046d1e395c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:5d8fa137aaafbdaa949dc14710411d0117e7c0a773bdb17a6cbfa2f9326af9d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101784206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ac15e1627ba64d9fa78a26b62d555c17485222b12da4380da9233b436382ba`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:11 GMT
ARG version=8.282.08.1
# Fri, 26 Mar 2021 01:59:17 GMT
# ARGS: version=8.282.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Fri, 26 Mar 2021 01:59:18 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 26 Mar 2021 01:59:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c445d315c10961d8ec4eae05e42c6f61168f5806b2a44a35ba2b9f6a1f5df59`  
		Last Modified: Fri, 26 Mar 2021 02:01:22 GMT  
		Size: 99.0 MB (98984444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine-full`

```console
$ docker pull amazoncorretto@sha256:9a482474fd3b479ca9e76b56299a1a8bb90b1438f00db394e8b3e8046d1e395c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:5d8fa137aaafbdaa949dc14710411d0117e7c0a773bdb17a6cbfa2f9326af9d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101784206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ac15e1627ba64d9fa78a26b62d555c17485222b12da4380da9233b436382ba`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:11 GMT
ARG version=8.282.08.1
# Fri, 26 Mar 2021 01:59:17 GMT
# ARGS: version=8.282.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Fri, 26 Mar 2021 01:59:18 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 26 Mar 2021 01:59:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c445d315c10961d8ec4eae05e42c6f61168f5806b2a44a35ba2b9f6a1f5df59`  
		Last Modified: Fri, 26 Mar 2021 02:01:22 GMT  
		Size: 99.0 MB (98984444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:9a482474fd3b479ca9e76b56299a1a8bb90b1438f00db394e8b3e8046d1e395c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:5d8fa137aaafbdaa949dc14710411d0117e7c0a773bdb17a6cbfa2f9326af9d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101784206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ac15e1627ba64d9fa78a26b62d555c17485222b12da4380da9233b436382ba`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:11 GMT
ARG version=8.282.08.1
# Fri, 26 Mar 2021 01:59:17 GMT
# ARGS: version=8.282.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Fri, 26 Mar 2021 01:59:18 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 26 Mar 2021 01:59:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c445d315c10961d8ec4eae05e42c6f61168f5806b2a44a35ba2b9f6a1f5df59`  
		Last Modified: Fri, 26 Mar 2021 02:01:22 GMT  
		Size: 99.0 MB (98984444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine-jre`

```console
$ docker pull amazoncorretto@sha256:a23867ac09ff44cd0a12eadc7b04dabf3fa5426ecdcc21fbe430f90852a04395
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8-alpine-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:12c06f0d634b03374eb6c7876a503b9e5d77da91bdb1d401259fac75c1c06509
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43115748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42c2e48c59c15ff17d4f3061ec18152fa3daaa050d48542ee894818bccf15531`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:11 GMT
ARG version=8.282.08.1
# Fri, 26 Mar 2021 01:59:24 GMT
# ARGS: version=8.282.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Fri, 26 Mar 2021 01:59:24 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65cc8853ab18e84a7be865c72f2b25f59f3723f3a3ce5943d4680aa16d59fc2`  
		Last Modified: Fri, 26 Mar 2021 02:01:43 GMT  
		Size: 40.3 MB (40315986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u282`

```console
$ docker pull amazoncorretto@sha256:8d63e7a8fa23f9911e168e293efd12a3d7c071170a1f12573daedd75863525e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u282` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:36ede9ee499243c633c9f1a564d6e6778bcecc0a1dd54ac04f6e3b2c5edededb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137228963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bf2504e87fa9a72b931331c3a8896094bace65ae2a2315d1e299d6296299313`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:19:26 GMT
ARG version=1.8.0_282.b08-1
# Thu, 18 Mar 2021 01:19:40 GMT
# ARGS: version=1.8.0_282.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:19:40 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:19:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376e88159f3d6c2882e0ed403c2a5a0c9e9deb0bd43bed9e388ce2f142ef7534`  
		Last Modified: Thu, 18 Mar 2021 01:22:53 GMT  
		Size: 75.3 MB (75293803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u282` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:8f4acd8b2dc74007708d0b702ff8691bdd48cc53d9a04dd212adc4b3717ee1ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122993322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94ca05b6a97afeb0c2290f5690cc6991118113271816cbf04cee4588495f59b1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:35:03 GMT
ARG version=1.8.0_282.b08-1
# Wed, 24 Feb 2021 19:35:27 GMT
# ARGS: version=1.8.0_282.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 24 Feb 2021 19:35:29 GMT
ENV LANG=C.UTF-8
# Wed, 24 Feb 2021 19:35:29 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1179eb6d5a9474bde2c1234c9e205f5845bd0420cb1c5439411d483f14c142`  
		Last Modified: Wed, 24 Feb 2021 19:37:40 GMT  
		Size: 59.4 MB (59368785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u282-al2`

```console
$ docker pull amazoncorretto@sha256:8d63e7a8fa23f9911e168e293efd12a3d7c071170a1f12573daedd75863525e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u282-al2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:36ede9ee499243c633c9f1a564d6e6778bcecc0a1dd54ac04f6e3b2c5edededb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137228963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bf2504e87fa9a72b931331c3a8896094bace65ae2a2315d1e299d6296299313`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:19:26 GMT
ARG version=1.8.0_282.b08-1
# Thu, 18 Mar 2021 01:19:40 GMT
# ARGS: version=1.8.0_282.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:19:40 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:19:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376e88159f3d6c2882e0ed403c2a5a0c9e9deb0bd43bed9e388ce2f142ef7534`  
		Last Modified: Thu, 18 Mar 2021 01:22:53 GMT  
		Size: 75.3 MB (75293803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u282-al2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:8f4acd8b2dc74007708d0b702ff8691bdd48cc53d9a04dd212adc4b3717ee1ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122993322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94ca05b6a97afeb0c2290f5690cc6991118113271816cbf04cee4588495f59b1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:35:03 GMT
ARG version=1.8.0_282.b08-1
# Wed, 24 Feb 2021 19:35:27 GMT
# ARGS: version=1.8.0_282.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 24 Feb 2021 19:35:29 GMT
ENV LANG=C.UTF-8
# Wed, 24 Feb 2021 19:35:29 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1179eb6d5a9474bde2c1234c9e205f5845bd0420cb1c5439411d483f14c142`  
		Last Modified: Wed, 24 Feb 2021 19:37:40 GMT  
		Size: 59.4 MB (59368785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u282-alpine`

```console
$ docker pull amazoncorretto@sha256:9a482474fd3b479ca9e76b56299a1a8bb90b1438f00db394e8b3e8046d1e395c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8u282-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:5d8fa137aaafbdaa949dc14710411d0117e7c0a773bdb17a6cbfa2f9326af9d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101784206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ac15e1627ba64d9fa78a26b62d555c17485222b12da4380da9233b436382ba`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:11 GMT
ARG version=8.282.08.1
# Fri, 26 Mar 2021 01:59:17 GMT
# ARGS: version=8.282.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Fri, 26 Mar 2021 01:59:18 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 26 Mar 2021 01:59:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c445d315c10961d8ec4eae05e42c6f61168f5806b2a44a35ba2b9f6a1f5df59`  
		Last Modified: Fri, 26 Mar 2021 02:01:22 GMT  
		Size: 99.0 MB (98984444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u282-alpine-jre`

```console
$ docker pull amazoncorretto@sha256:a23867ac09ff44cd0a12eadc7b04dabf3fa5426ecdcc21fbe430f90852a04395
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8u282-alpine-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:12c06f0d634b03374eb6c7876a503b9e5d77da91bdb1d401259fac75c1c06509
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43115748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42c2e48c59c15ff17d4f3061ec18152fa3daaa050d48542ee894818bccf15531`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:11 GMT
ARG version=8.282.08.1
# Fri, 26 Mar 2021 01:59:24 GMT
# ARGS: version=8.282.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Fri, 26 Mar 2021 01:59:24 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65cc8853ab18e84a7be865c72f2b25f59f3723f3a3ce5943d4680aa16d59fc2`  
		Last Modified: Fri, 26 Mar 2021 02:01:43 GMT  
		Size: 40.3 MB (40315986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:latest`

```console
$ docker pull amazoncorretto@sha256:8d63e7a8fa23f9911e168e293efd12a3d7c071170a1f12573daedd75863525e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:latest` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:36ede9ee499243c633c9f1a564d6e6778bcecc0a1dd54ac04f6e3b2c5edededb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137228963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bf2504e87fa9a72b931331c3a8896094bace65ae2a2315d1e299d6296299313`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:19:26 GMT
ARG version=1.8.0_282.b08-1
# Thu, 18 Mar 2021 01:19:40 GMT
# ARGS: version=1.8.0_282.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:19:40 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:19:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376e88159f3d6c2882e0ed403c2a5a0c9e9deb0bd43bed9e388ce2f142ef7534`  
		Last Modified: Thu, 18 Mar 2021 01:22:53 GMT  
		Size: 75.3 MB (75293803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:latest` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:8f4acd8b2dc74007708d0b702ff8691bdd48cc53d9a04dd212adc4b3717ee1ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122993322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94ca05b6a97afeb0c2290f5690cc6991118113271816cbf04cee4588495f59b1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:35:03 GMT
ARG version=1.8.0_282.b08-1
# Wed, 24 Feb 2021 19:35:27 GMT
# ARGS: version=1.8.0_282.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 24 Feb 2021 19:35:29 GMT
ENV LANG=C.UTF-8
# Wed, 24 Feb 2021 19:35:29 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1179eb6d5a9474bde2c1234c9e205f5845bd0420cb1c5439411d483f14c142`  
		Last Modified: Wed, 24 Feb 2021 19:37:40 GMT  
		Size: 59.4 MB (59368785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
