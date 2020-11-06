<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazoncorretto`

-	[`amazoncorretto:11`](#amazoncorretto11)
-	[`amazoncorretto:11.0.9`](#amazoncorretto1109)
-	[`amazoncorretto:11.0.9-al2`](#amazoncorretto1109-al2)
-	[`amazoncorretto:11.0.9-alpine`](#amazoncorretto1109-alpine)
-	[`amazoncorretto:11-al2-full`](#amazoncorretto11-al2-full)
-	[`amazoncorretto:11-al2-jdk`](#amazoncorretto11-al2-jdk)
-	[`amazoncorretto:11-alpine`](#amazoncorretto11-alpine)
-	[`amazoncorretto:11-alpine-full`](#amazoncorretto11-alpine-full)
-	[`amazoncorretto:11-alpine-jdk`](#amazoncorretto11-alpine-jdk)
-	[`amazoncorretto:15`](#amazoncorretto15)
-	[`amazoncorretto:15.0.1`](#amazoncorretto1501)
-	[`amazoncorretto:15.0.1-al2`](#amazoncorretto1501-al2)
-	[`amazoncorretto:15.0.1-alpine`](#amazoncorretto1501-alpine)
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
-	[`amazoncorretto:8u275`](#amazoncorretto8u275)
-	[`amazoncorretto:8u275-al2`](#amazoncorretto8u275-al2)
-	[`amazoncorretto:8u275-alpine`](#amazoncorretto8u275-alpine)
-	[`amazoncorretto:8u275-alpine-jre`](#amazoncorretto8u275-alpine-jre)
-	[`amazoncorretto:latest`](#amazoncorrettolatest)

## `amazoncorretto:11`

```console
$ docker pull amazoncorretto@sha256:4acf98d2647f52699d095bab657d0b8ce8b64a7a7e25c76d54f2c5e31fae3b0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:b76d8718f3d707bc8dceca4c6001d2acd6d774143f652f91949b0cf9c96cd82e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.1 MB (208142287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d85001ab90727c3892049781704b19d20c96d118b97fb826ccf9266f72b900f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Wed, 21 Oct 2020 18:19:36 GMT
ARG version=11.0.9.11-1
# Wed, 21 Oct 2020 18:20:01 GMT
# ARGS: version=11.0.9.11-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Oct 2020 18:20:01 GMT
ENV LANG=C.UTF-8
# Wed, 21 Oct 2020 18:20:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43676934e9169078a38f87d17afecd63945013ccba151fb61ba8de2551018f62`  
		Last Modified: Wed, 21 Oct 2020 18:21:04 GMT  
		Size: 146.4 MB (146425747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d6710149c1614a82d3b1d32f3288262b6b2df4c5dd91fbf9503020fb661d8b2c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.8 MB (207822028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6810e115c664bb2ed066b2fd37df7ddea75c129c2a9a96c95ea05f3cc5a8f900`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Wed, 21 Oct 2020 18:39:42 GMT
ARG version=11.0.9.11-1
# Wed, 21 Oct 2020 18:41:59 GMT
# ARGS: version=11.0.9.11-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Oct 2020 18:42:01 GMT
ENV LANG=C.UTF-8
# Wed, 21 Oct 2020 18:42:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c8d5eedc3ac385be353b13808647b5c5702617c8a142eeda9f910d9fc0d2bb`  
		Last Modified: Wed, 21 Oct 2020 18:43:14 GMT  
		Size: 144.5 MB (144467892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11.0.9`

```console
$ docker pull amazoncorretto@sha256:4acf98d2647f52699d095bab657d0b8ce8b64a7a7e25c76d54f2c5e31fae3b0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11.0.9` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:b76d8718f3d707bc8dceca4c6001d2acd6d774143f652f91949b0cf9c96cd82e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.1 MB (208142287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d85001ab90727c3892049781704b19d20c96d118b97fb826ccf9266f72b900f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Wed, 21 Oct 2020 18:19:36 GMT
ARG version=11.0.9.11-1
# Wed, 21 Oct 2020 18:20:01 GMT
# ARGS: version=11.0.9.11-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Oct 2020 18:20:01 GMT
ENV LANG=C.UTF-8
# Wed, 21 Oct 2020 18:20:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43676934e9169078a38f87d17afecd63945013ccba151fb61ba8de2551018f62`  
		Last Modified: Wed, 21 Oct 2020 18:21:04 GMT  
		Size: 146.4 MB (146425747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11.0.9` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d6710149c1614a82d3b1d32f3288262b6b2df4c5dd91fbf9503020fb661d8b2c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.8 MB (207822028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6810e115c664bb2ed066b2fd37df7ddea75c129c2a9a96c95ea05f3cc5a8f900`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Wed, 21 Oct 2020 18:39:42 GMT
ARG version=11.0.9.11-1
# Wed, 21 Oct 2020 18:41:59 GMT
# ARGS: version=11.0.9.11-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Oct 2020 18:42:01 GMT
ENV LANG=C.UTF-8
# Wed, 21 Oct 2020 18:42:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c8d5eedc3ac385be353b13808647b5c5702617c8a142eeda9f910d9fc0d2bb`  
		Last Modified: Wed, 21 Oct 2020 18:43:14 GMT  
		Size: 144.5 MB (144467892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11.0.9-al2`

```console
$ docker pull amazoncorretto@sha256:4acf98d2647f52699d095bab657d0b8ce8b64a7a7e25c76d54f2c5e31fae3b0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11.0.9-al2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:b76d8718f3d707bc8dceca4c6001d2acd6d774143f652f91949b0cf9c96cd82e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.1 MB (208142287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d85001ab90727c3892049781704b19d20c96d118b97fb826ccf9266f72b900f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Wed, 21 Oct 2020 18:19:36 GMT
ARG version=11.0.9.11-1
# Wed, 21 Oct 2020 18:20:01 GMT
# ARGS: version=11.0.9.11-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Oct 2020 18:20:01 GMT
ENV LANG=C.UTF-8
# Wed, 21 Oct 2020 18:20:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43676934e9169078a38f87d17afecd63945013ccba151fb61ba8de2551018f62`  
		Last Modified: Wed, 21 Oct 2020 18:21:04 GMT  
		Size: 146.4 MB (146425747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11.0.9-al2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d6710149c1614a82d3b1d32f3288262b6b2df4c5dd91fbf9503020fb661d8b2c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.8 MB (207822028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6810e115c664bb2ed066b2fd37df7ddea75c129c2a9a96c95ea05f3cc5a8f900`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Wed, 21 Oct 2020 18:39:42 GMT
ARG version=11.0.9.11-1
# Wed, 21 Oct 2020 18:41:59 GMT
# ARGS: version=11.0.9.11-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Oct 2020 18:42:01 GMT
ENV LANG=C.UTF-8
# Wed, 21 Oct 2020 18:42:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c8d5eedc3ac385be353b13808647b5c5702617c8a142eeda9f910d9fc0d2bb`  
		Last Modified: Wed, 21 Oct 2020 18:43:14 GMT  
		Size: 144.5 MB (144467892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11.0.9-alpine`

```console
$ docker pull amazoncorretto@sha256:8e9bb1bc18954fc2634632ebf4f2322f4a34202466cfdd2573110d281bea66f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:11.0.9-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:ce812cc8bc2345fd2fb1b046150bf75837a6ee9042530b672224fa4276089ea2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.0 MB (195003745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3a89243ece990a938647c53ed624ec6a8555155c5bc0d23c5319dd9be55dc2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:52:00 GMT
ARG version=11.0.9.11.1
# Thu, 22 Oct 2020 02:52:10 GMT
# ARGS: version=11.0.9.11.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Thu, 22 Oct 2020 02:52:11 GMT
ENV LANG=C.UTF-8
# Thu, 22 Oct 2020 02:52:11 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 22 Oct 2020 02:52:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4650ec59cfb84326c52d7ff96d2a71e1ac9ee09cb8419aad8530c44076138251`  
		Last Modified: Thu, 22 Oct 2020 02:53:57 GMT  
		Size: 192.2 MB (192206885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-al2-full`

```console
$ docker pull amazoncorretto@sha256:4acf98d2647f52699d095bab657d0b8ce8b64a7a7e25c76d54f2c5e31fae3b0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:b76d8718f3d707bc8dceca4c6001d2acd6d774143f652f91949b0cf9c96cd82e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.1 MB (208142287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d85001ab90727c3892049781704b19d20c96d118b97fb826ccf9266f72b900f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Wed, 21 Oct 2020 18:19:36 GMT
ARG version=11.0.9.11-1
# Wed, 21 Oct 2020 18:20:01 GMT
# ARGS: version=11.0.9.11-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Oct 2020 18:20:01 GMT
ENV LANG=C.UTF-8
# Wed, 21 Oct 2020 18:20:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43676934e9169078a38f87d17afecd63945013ccba151fb61ba8de2551018f62`  
		Last Modified: Wed, 21 Oct 2020 18:21:04 GMT  
		Size: 146.4 MB (146425747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d6710149c1614a82d3b1d32f3288262b6b2df4c5dd91fbf9503020fb661d8b2c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.8 MB (207822028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6810e115c664bb2ed066b2fd37df7ddea75c129c2a9a96c95ea05f3cc5a8f900`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Wed, 21 Oct 2020 18:39:42 GMT
ARG version=11.0.9.11-1
# Wed, 21 Oct 2020 18:41:59 GMT
# ARGS: version=11.0.9.11-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Oct 2020 18:42:01 GMT
ENV LANG=C.UTF-8
# Wed, 21 Oct 2020 18:42:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c8d5eedc3ac385be353b13808647b5c5702617c8a142eeda9f910d9fc0d2bb`  
		Last Modified: Wed, 21 Oct 2020 18:43:14 GMT  
		Size: 144.5 MB (144467892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:4acf98d2647f52699d095bab657d0b8ce8b64a7a7e25c76d54f2c5e31fae3b0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:b76d8718f3d707bc8dceca4c6001d2acd6d774143f652f91949b0cf9c96cd82e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.1 MB (208142287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d85001ab90727c3892049781704b19d20c96d118b97fb826ccf9266f72b900f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Wed, 21 Oct 2020 18:19:36 GMT
ARG version=11.0.9.11-1
# Wed, 21 Oct 2020 18:20:01 GMT
# ARGS: version=11.0.9.11-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Oct 2020 18:20:01 GMT
ENV LANG=C.UTF-8
# Wed, 21 Oct 2020 18:20:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43676934e9169078a38f87d17afecd63945013ccba151fb61ba8de2551018f62`  
		Last Modified: Wed, 21 Oct 2020 18:21:04 GMT  
		Size: 146.4 MB (146425747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d6710149c1614a82d3b1d32f3288262b6b2df4c5dd91fbf9503020fb661d8b2c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.8 MB (207822028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6810e115c664bb2ed066b2fd37df7ddea75c129c2a9a96c95ea05f3cc5a8f900`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Wed, 21 Oct 2020 18:39:42 GMT
ARG version=11.0.9.11-1
# Wed, 21 Oct 2020 18:41:59 GMT
# ARGS: version=11.0.9.11-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Oct 2020 18:42:01 GMT
ENV LANG=C.UTF-8
# Wed, 21 Oct 2020 18:42:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c8d5eedc3ac385be353b13808647b5c5702617c8a142eeda9f910d9fc0d2bb`  
		Last Modified: Wed, 21 Oct 2020 18:43:14 GMT  
		Size: 144.5 MB (144467892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-alpine`

```console
$ docker pull amazoncorretto@sha256:8e9bb1bc18954fc2634632ebf4f2322f4a34202466cfdd2573110d281bea66f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:11-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:ce812cc8bc2345fd2fb1b046150bf75837a6ee9042530b672224fa4276089ea2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.0 MB (195003745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3a89243ece990a938647c53ed624ec6a8555155c5bc0d23c5319dd9be55dc2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:52:00 GMT
ARG version=11.0.9.11.1
# Thu, 22 Oct 2020 02:52:10 GMT
# ARGS: version=11.0.9.11.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Thu, 22 Oct 2020 02:52:11 GMT
ENV LANG=C.UTF-8
# Thu, 22 Oct 2020 02:52:11 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 22 Oct 2020 02:52:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4650ec59cfb84326c52d7ff96d2a71e1ac9ee09cb8419aad8530c44076138251`  
		Last Modified: Thu, 22 Oct 2020 02:53:57 GMT  
		Size: 192.2 MB (192206885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-alpine-full`

```console
$ docker pull amazoncorretto@sha256:8e9bb1bc18954fc2634632ebf4f2322f4a34202466cfdd2573110d281bea66f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:11-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:ce812cc8bc2345fd2fb1b046150bf75837a6ee9042530b672224fa4276089ea2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.0 MB (195003745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3a89243ece990a938647c53ed624ec6a8555155c5bc0d23c5319dd9be55dc2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:52:00 GMT
ARG version=11.0.9.11.1
# Thu, 22 Oct 2020 02:52:10 GMT
# ARGS: version=11.0.9.11.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Thu, 22 Oct 2020 02:52:11 GMT
ENV LANG=C.UTF-8
# Thu, 22 Oct 2020 02:52:11 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 22 Oct 2020 02:52:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4650ec59cfb84326c52d7ff96d2a71e1ac9ee09cb8419aad8530c44076138251`  
		Last Modified: Thu, 22 Oct 2020 02:53:57 GMT  
		Size: 192.2 MB (192206885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:11-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:8e9bb1bc18954fc2634632ebf4f2322f4a34202466cfdd2573110d281bea66f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:11-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:ce812cc8bc2345fd2fb1b046150bf75837a6ee9042530b672224fa4276089ea2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.0 MB (195003745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3a89243ece990a938647c53ed624ec6a8555155c5bc0d23c5319dd9be55dc2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:52:00 GMT
ARG version=11.0.9.11.1
# Thu, 22 Oct 2020 02:52:10 GMT
# ARGS: version=11.0.9.11.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Thu, 22 Oct 2020 02:52:11 GMT
ENV LANG=C.UTF-8
# Thu, 22 Oct 2020 02:52:11 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 22 Oct 2020 02:52:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4650ec59cfb84326c52d7ff96d2a71e1ac9ee09cb8419aad8530c44076138251`  
		Last Modified: Thu, 22 Oct 2020 02:53:57 GMT  
		Size: 192.2 MB (192206885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15`

```console
$ docker pull amazoncorretto@sha256:b1b9eb9e10827cedfd6c10c2e121f1a6afcdc5d8d6b2fdef1d88da40fd5b6ab3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:15` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:8de06d3a5c0cd1c69bf18730214f5f23cfa0bc6745ed1dc53fb1c851add1b9d7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.3 MB (217348464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:987efd713809d9d86d659d999e9c17a840553850d1d59f45724ff6de9cf925bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:20:38 GMT
ARG version=15.0.1.9-1
# Wed, 28 Oct 2020 00:21:04 GMT
# ARGS: version=15.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:21:04 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:21:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f63bb5d5eb2077eabce2a847bd08bfed17d34b549ba4b4839b065a377194a54`  
		Last Modified: Wed, 28 Oct 2020 00:22:52 GMT  
		Size: 155.6 MB (155631924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:15` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:27d8a7fc62043fd7d12dda21eac478b63558106f05ddf8d5b49c430b91757e17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.9 MB (218857049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:577b845bb89b00f8f2fb899ff74444415edb18bab356e0eb1e9298bb903b12ca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:41:10 GMT
ARG version=15.0.1.9-1
# Wed, 28 Oct 2020 00:41:59 GMT
# ARGS: version=15.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:42:02 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:42:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4844a846e201e89f85fa7c7c2a2c256867445498cf78b6411d49fb9587517f`  
		Last Modified: Wed, 28 Oct 2020 00:43:35 GMT  
		Size: 155.5 MB (155502913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15.0.1`

```console
$ docker pull amazoncorretto@sha256:b1b9eb9e10827cedfd6c10c2e121f1a6afcdc5d8d6b2fdef1d88da40fd5b6ab3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:15.0.1` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:8de06d3a5c0cd1c69bf18730214f5f23cfa0bc6745ed1dc53fb1c851add1b9d7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.3 MB (217348464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:987efd713809d9d86d659d999e9c17a840553850d1d59f45724ff6de9cf925bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:20:38 GMT
ARG version=15.0.1.9-1
# Wed, 28 Oct 2020 00:21:04 GMT
# ARGS: version=15.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:21:04 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:21:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f63bb5d5eb2077eabce2a847bd08bfed17d34b549ba4b4839b065a377194a54`  
		Last Modified: Wed, 28 Oct 2020 00:22:52 GMT  
		Size: 155.6 MB (155631924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:15.0.1` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:27d8a7fc62043fd7d12dda21eac478b63558106f05ddf8d5b49c430b91757e17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.9 MB (218857049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:577b845bb89b00f8f2fb899ff74444415edb18bab356e0eb1e9298bb903b12ca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:41:10 GMT
ARG version=15.0.1.9-1
# Wed, 28 Oct 2020 00:41:59 GMT
# ARGS: version=15.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:42:02 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:42:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4844a846e201e89f85fa7c7c2a2c256867445498cf78b6411d49fb9587517f`  
		Last Modified: Wed, 28 Oct 2020 00:43:35 GMT  
		Size: 155.5 MB (155502913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15.0.1-al2`

```console
$ docker pull amazoncorretto@sha256:b1b9eb9e10827cedfd6c10c2e121f1a6afcdc5d8d6b2fdef1d88da40fd5b6ab3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:15.0.1-al2` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:8de06d3a5c0cd1c69bf18730214f5f23cfa0bc6745ed1dc53fb1c851add1b9d7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.3 MB (217348464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:987efd713809d9d86d659d999e9c17a840553850d1d59f45724ff6de9cf925bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:20:38 GMT
ARG version=15.0.1.9-1
# Wed, 28 Oct 2020 00:21:04 GMT
# ARGS: version=15.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:21:04 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:21:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f63bb5d5eb2077eabce2a847bd08bfed17d34b549ba4b4839b065a377194a54`  
		Last Modified: Wed, 28 Oct 2020 00:22:52 GMT  
		Size: 155.6 MB (155631924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:15.0.1-al2` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:27d8a7fc62043fd7d12dda21eac478b63558106f05ddf8d5b49c430b91757e17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.9 MB (218857049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:577b845bb89b00f8f2fb899ff74444415edb18bab356e0eb1e9298bb903b12ca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:41:10 GMT
ARG version=15.0.1.9-1
# Wed, 28 Oct 2020 00:41:59 GMT
# ARGS: version=15.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:42:02 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:42:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4844a846e201e89f85fa7c7c2a2c256867445498cf78b6411d49fb9587517f`  
		Last Modified: Wed, 28 Oct 2020 00:43:35 GMT  
		Size: 155.5 MB (155502913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15.0.1-alpine`

```console
$ docker pull amazoncorretto@sha256:0cfdc770fdbc39457bf06a1549a9c5e9762a02f19e380104c4d6a1bfc734915a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:15.0.1-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:2d49338d06551b0a31848cecad668c1b877f8f27818d66b45de7f763bc3e1972
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.7 MB (207714787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e96f35759b93bdadf20ca3e05a6982515670dfb155f0d700abc50d6b91ac00`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Wed, 28 Oct 2020 00:21:12 GMT
ARG version=15.0.1.9.1
# Wed, 28 Oct 2020 00:21:19 GMT
# ARGS: version=15.0.1.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-15=$version-r0
# Wed, 28 Oct 2020 00:21:19 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:21:19 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 28 Oct 2020 00:21:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de3f84eb66e9b0962199bb01018f641091674b315a07635034f849249cadb56`  
		Last Modified: Wed, 28 Oct 2020 00:23:30 GMT  
		Size: 204.9 MB (204917927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15-al2-full`

```console
$ docker pull amazoncorretto@sha256:b1b9eb9e10827cedfd6c10c2e121f1a6afcdc5d8d6b2fdef1d88da40fd5b6ab3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:15-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:8de06d3a5c0cd1c69bf18730214f5f23cfa0bc6745ed1dc53fb1c851add1b9d7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.3 MB (217348464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:987efd713809d9d86d659d999e9c17a840553850d1d59f45724ff6de9cf925bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:20:38 GMT
ARG version=15.0.1.9-1
# Wed, 28 Oct 2020 00:21:04 GMT
# ARGS: version=15.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:21:04 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:21:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f63bb5d5eb2077eabce2a847bd08bfed17d34b549ba4b4839b065a377194a54`  
		Last Modified: Wed, 28 Oct 2020 00:22:52 GMT  
		Size: 155.6 MB (155631924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:15-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:27d8a7fc62043fd7d12dda21eac478b63558106f05ddf8d5b49c430b91757e17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.9 MB (218857049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:577b845bb89b00f8f2fb899ff74444415edb18bab356e0eb1e9298bb903b12ca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:41:10 GMT
ARG version=15.0.1.9-1
# Wed, 28 Oct 2020 00:41:59 GMT
# ARGS: version=15.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:42:02 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:42:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4844a846e201e89f85fa7c7c2a2c256867445498cf78b6411d49fb9587517f`  
		Last Modified: Wed, 28 Oct 2020 00:43:35 GMT  
		Size: 155.5 MB (155502913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:b1b9eb9e10827cedfd6c10c2e121f1a6afcdc5d8d6b2fdef1d88da40fd5b6ab3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:15-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:8de06d3a5c0cd1c69bf18730214f5f23cfa0bc6745ed1dc53fb1c851add1b9d7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.3 MB (217348464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:987efd713809d9d86d659d999e9c17a840553850d1d59f45724ff6de9cf925bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:20:38 GMT
ARG version=15.0.1.9-1
# Wed, 28 Oct 2020 00:21:04 GMT
# ARGS: version=15.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:21:04 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:21:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f63bb5d5eb2077eabce2a847bd08bfed17d34b549ba4b4839b065a377194a54`  
		Last Modified: Wed, 28 Oct 2020 00:22:52 GMT  
		Size: 155.6 MB (155631924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:15-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:27d8a7fc62043fd7d12dda21eac478b63558106f05ddf8d5b49c430b91757e17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.9 MB (218857049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:577b845bb89b00f8f2fb899ff74444415edb18bab356e0eb1e9298bb903b12ca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:41:10 GMT
ARG version=15.0.1.9-1
# Wed, 28 Oct 2020 00:41:59 GMT
# ARGS: version=15.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:42:02 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:42:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4844a846e201e89f85fa7c7c2a2c256867445498cf78b6411d49fb9587517f`  
		Last Modified: Wed, 28 Oct 2020 00:43:35 GMT  
		Size: 155.5 MB (155502913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15-alpine`

```console
$ docker pull amazoncorretto@sha256:0cfdc770fdbc39457bf06a1549a9c5e9762a02f19e380104c4d6a1bfc734915a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:15-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:2d49338d06551b0a31848cecad668c1b877f8f27818d66b45de7f763bc3e1972
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.7 MB (207714787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e96f35759b93bdadf20ca3e05a6982515670dfb155f0d700abc50d6b91ac00`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Wed, 28 Oct 2020 00:21:12 GMT
ARG version=15.0.1.9.1
# Wed, 28 Oct 2020 00:21:19 GMT
# ARGS: version=15.0.1.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-15=$version-r0
# Wed, 28 Oct 2020 00:21:19 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:21:19 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 28 Oct 2020 00:21:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de3f84eb66e9b0962199bb01018f641091674b315a07635034f849249cadb56`  
		Last Modified: Wed, 28 Oct 2020 00:23:30 GMT  
		Size: 204.9 MB (204917927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15-alpine-full`

```console
$ docker pull amazoncorretto@sha256:0cfdc770fdbc39457bf06a1549a9c5e9762a02f19e380104c4d6a1bfc734915a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:15-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:2d49338d06551b0a31848cecad668c1b877f8f27818d66b45de7f763bc3e1972
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.7 MB (207714787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e96f35759b93bdadf20ca3e05a6982515670dfb155f0d700abc50d6b91ac00`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Wed, 28 Oct 2020 00:21:12 GMT
ARG version=15.0.1.9.1
# Wed, 28 Oct 2020 00:21:19 GMT
# ARGS: version=15.0.1.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-15=$version-r0
# Wed, 28 Oct 2020 00:21:19 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:21:19 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 28 Oct 2020 00:21:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de3f84eb66e9b0962199bb01018f641091674b315a07635034f849249cadb56`  
		Last Modified: Wed, 28 Oct 2020 00:23:30 GMT  
		Size: 204.9 MB (204917927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:15-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:0cfdc770fdbc39457bf06a1549a9c5e9762a02f19e380104c4d6a1bfc734915a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:15-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:2d49338d06551b0a31848cecad668c1b877f8f27818d66b45de7f763bc3e1972
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.7 MB (207714787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e96f35759b93bdadf20ca3e05a6982515670dfb155f0d700abc50d6b91ac00`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Wed, 28 Oct 2020 00:21:12 GMT
ARG version=15.0.1.9.1
# Wed, 28 Oct 2020 00:21:19 GMT
# ARGS: version=15.0.1.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-15=$version-r0
# Wed, 28 Oct 2020 00:21:19 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:21:19 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 28 Oct 2020 00:21:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de3f84eb66e9b0962199bb01018f641091674b315a07635034f849249cadb56`  
		Last Modified: Wed, 28 Oct 2020 00:23:30 GMT  
		Size: 204.9 MB (204917927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8`

```console
$ docker pull amazoncorretto@sha256:ea0efa54199a1a1eea417bdd4efc946c8a0f61c5a109c92f076143fff1baa622
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:712bdb3c0aa07d83e31487d40497abfc8242783a9d3aa6d03166aa6609c0cdde
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.0 MB (136957574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f3c781fd53841334246dd242e57264ad4c0d3fa68a98af1a24f87e932574cb9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:19:28 GMT
ARG version=1.8.0_272.b10-3
# Wed, 28 Oct 2020 00:19:52 GMT
# ARGS: version=1.8.0_272.b10-3
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:19:52 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:19:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a3c2059a8a90e1819eafb917f66ddf3baae20fcfd47bb182749d9d7ca8a2d4`  
		Last Modified: Wed, 28 Oct 2020 00:21:51 GMT  
		Size: 75.2 MB (75241034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:5fd283c837716326af81b032e3ed23873d539eb2253481d26fe22e11954e2b3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.7 MB (122690092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b30f1ad38b039c21c07add368fe2458cc5c1cf5430fea6cd025e1bde4b1e1cb5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:39:50 GMT
ARG version=1.8.0_272.b10-3
# Wed, 28 Oct 2020 00:40:33 GMT
# ARGS: version=1.8.0_272.b10-3
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:40:42 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:40:47 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bceaa740c3f1368a605094068479b55a57d62eb653f2548f24cf4af693e7b345`  
		Last Modified: Wed, 28 Oct 2020 00:42:47 GMT  
		Size: 59.3 MB (59335956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-al2-full`

```console
$ docker pull amazoncorretto@sha256:ea0efa54199a1a1eea417bdd4efc946c8a0f61c5a109c92f076143fff1baa622
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:712bdb3c0aa07d83e31487d40497abfc8242783a9d3aa6d03166aa6609c0cdde
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.0 MB (136957574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f3c781fd53841334246dd242e57264ad4c0d3fa68a98af1a24f87e932574cb9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:19:28 GMT
ARG version=1.8.0_272.b10-3
# Wed, 28 Oct 2020 00:19:52 GMT
# ARGS: version=1.8.0_272.b10-3
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:19:52 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:19:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a3c2059a8a90e1819eafb917f66ddf3baae20fcfd47bb182749d9d7ca8a2d4`  
		Last Modified: Wed, 28 Oct 2020 00:21:51 GMT  
		Size: 75.2 MB (75241034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:5fd283c837716326af81b032e3ed23873d539eb2253481d26fe22e11954e2b3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.7 MB (122690092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b30f1ad38b039c21c07add368fe2458cc5c1cf5430fea6cd025e1bde4b1e1cb5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:39:50 GMT
ARG version=1.8.0_272.b10-3
# Wed, 28 Oct 2020 00:40:33 GMT
# ARGS: version=1.8.0_272.b10-3
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:40:42 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:40:47 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bceaa740c3f1368a605094068479b55a57d62eb653f2548f24cf4af693e7b345`  
		Last Modified: Wed, 28 Oct 2020 00:42:47 GMT  
		Size: 59.3 MB (59335956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:ea0efa54199a1a1eea417bdd4efc946c8a0f61c5a109c92f076143fff1baa622
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:712bdb3c0aa07d83e31487d40497abfc8242783a9d3aa6d03166aa6609c0cdde
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.0 MB (136957574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f3c781fd53841334246dd242e57264ad4c0d3fa68a98af1a24f87e932574cb9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:19:28 GMT
ARG version=1.8.0_272.b10-3
# Wed, 28 Oct 2020 00:19:52 GMT
# ARGS: version=1.8.0_272.b10-3
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:19:52 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:19:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a3c2059a8a90e1819eafb917f66ddf3baae20fcfd47bb182749d9d7ca8a2d4`  
		Last Modified: Wed, 28 Oct 2020 00:21:51 GMT  
		Size: 75.2 MB (75241034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:5fd283c837716326af81b032e3ed23873d539eb2253481d26fe22e11954e2b3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.7 MB (122690092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b30f1ad38b039c21c07add368fe2458cc5c1cf5430fea6cd025e1bde4b1e1cb5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:39:50 GMT
ARG version=1.8.0_272.b10-3
# Wed, 28 Oct 2020 00:40:33 GMT
# ARGS: version=1.8.0_272.b10-3
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:40:42 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:40:47 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bceaa740c3f1368a605094068479b55a57d62eb653f2548f24cf4af693e7b345`  
		Last Modified: Wed, 28 Oct 2020 00:42:47 GMT  
		Size: 59.3 MB (59335956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine`

```console
$ docker pull amazoncorretto@sha256:8d1066057e460bb18119533df28fd36403d926dbf4e10576e03dd7f80eff21a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:76fc6ca6fc6c038cd5f54778418ad8901a80971994590222145091db38f6a19e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101765845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c48bb5281a8e51b8a2af9d0996e7860e9c1cff7281f94bfb07d13a6fb7f4f4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Wed, 28 Oct 2020 00:20:01 GMT
ARG version=8.272.10.4
# Wed, 28 Oct 2020 00:20:18 GMT
# ARGS: version=8.272.10.4
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Wed, 28 Oct 2020 00:20:19 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:20:19 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 28 Oct 2020 00:20:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3401c03af81c0a0987aae5fe034b6952731a8a6a765fdd627e04490d9d8e69`  
		Last Modified: Wed, 28 Oct 2020 00:22:17 GMT  
		Size: 99.0 MB (98968985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine-full`

```console
$ docker pull amazoncorretto@sha256:8d1066057e460bb18119533df28fd36403d926dbf4e10576e03dd7f80eff21a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:76fc6ca6fc6c038cd5f54778418ad8901a80971994590222145091db38f6a19e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101765845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c48bb5281a8e51b8a2af9d0996e7860e9c1cff7281f94bfb07d13a6fb7f4f4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Wed, 28 Oct 2020 00:20:01 GMT
ARG version=8.272.10.4
# Wed, 28 Oct 2020 00:20:18 GMT
# ARGS: version=8.272.10.4
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Wed, 28 Oct 2020 00:20:19 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:20:19 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 28 Oct 2020 00:20:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3401c03af81c0a0987aae5fe034b6952731a8a6a765fdd627e04490d9d8e69`  
		Last Modified: Wed, 28 Oct 2020 00:22:17 GMT  
		Size: 99.0 MB (98968985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:8d1066057e460bb18119533df28fd36403d926dbf4e10576e03dd7f80eff21a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:76fc6ca6fc6c038cd5f54778418ad8901a80971994590222145091db38f6a19e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101765845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c48bb5281a8e51b8a2af9d0996e7860e9c1cff7281f94bfb07d13a6fb7f4f4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Wed, 28 Oct 2020 00:20:01 GMT
ARG version=8.272.10.4
# Wed, 28 Oct 2020 00:20:18 GMT
# ARGS: version=8.272.10.4
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Wed, 28 Oct 2020 00:20:19 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:20:19 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 28 Oct 2020 00:20:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3401c03af81c0a0987aae5fe034b6952731a8a6a765fdd627e04490d9d8e69`  
		Last Modified: Wed, 28 Oct 2020 00:22:17 GMT  
		Size: 99.0 MB (98968985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8-alpine-jre`

```console
$ docker pull amazoncorretto@sha256:82af01d1fae8d62ba1e8d822f475d44eac45e83df270a9d05a5fd9b018bd0e09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8-alpine-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:055542e352146833e0683f78f6dfbdc5f86e2b564aef24dc8e72944af44c06fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43107091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12264aa4481f050f8c035b87cf7ff09d4a2e49130b8c1fc0ace4dded1acf8e9c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Wed, 28 Oct 2020 00:20:01 GMT
ARG version=8.272.10.4
# Wed, 28 Oct 2020 00:20:29 GMT
# ARGS: version=8.272.10.4
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Wed, 28 Oct 2020 00:20:30 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:20:30 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b48d574c305da5c1b53dbaf7a78de17fa14c8677219545c016444dee8b1a6a0`  
		Last Modified: Wed, 28 Oct 2020 00:22:29 GMT  
		Size: 40.3 MB (40310231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazoncorretto:8u275`

**does not exist** (yet?)

## `amazoncorretto:8u275-al2`

**does not exist** (yet?)

## `amazoncorretto:8u275-alpine`

**does not exist** (yet?)

## `amazoncorretto:8u275-alpine-jre`

**does not exist** (yet?)

## `amazoncorretto:latest`

```console
$ docker pull amazoncorretto@sha256:ea0efa54199a1a1eea417bdd4efc946c8a0f61c5a109c92f076143fff1baa622
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:latest` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:712bdb3c0aa07d83e31487d40497abfc8242783a9d3aa6d03166aa6609c0cdde
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.0 MB (136957574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f3c781fd53841334246dd242e57264ad4c0d3fa68a98af1a24f87e932574cb9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:19:28 GMT
ARG version=1.8.0_272.b10-3
# Wed, 28 Oct 2020 00:19:52 GMT
# ARGS: version=1.8.0_272.b10-3
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:19:52 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:19:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a3c2059a8a90e1819eafb917f66ddf3baae20fcfd47bb182749d9d7ca8a2d4`  
		Last Modified: Wed, 28 Oct 2020 00:21:51 GMT  
		Size: 75.2 MB (75241034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:latest` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:5fd283c837716326af81b032e3ed23873d539eb2253481d26fe22e11954e2b3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.7 MB (122690092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b30f1ad38b039c21c07add368fe2458cc5c1cf5430fea6cd025e1bde4b1e1cb5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:39:50 GMT
ARG version=1.8.0_272.b10-3
# Wed, 28 Oct 2020 00:40:33 GMT
# ARGS: version=1.8.0_272.b10-3
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:40:42 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:40:47 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bceaa740c3f1368a605094068479b55a57d62eb653f2548f24cf4af693e7b345`  
		Last Modified: Wed, 28 Oct 2020 00:42:47 GMT  
		Size: 59.3 MB (59335956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
