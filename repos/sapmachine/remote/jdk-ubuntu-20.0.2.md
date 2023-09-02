## `sapmachine:jdk-ubuntu-20.0.2`

```console
$ docker pull sapmachine@sha256:836a7237d927252aed6f7a3875de6664e95a27b11e96bf16903470244ba25e0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `sapmachine:jdk-ubuntu-20.0.2` - linux; amd64

```console
$ docker pull sapmachine@sha256:d5d9c016c06570cc5e87f4a41d0f75cf9c8cbd81cf7ca4240919869d990cd64f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.8 MB (239768989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673b0e83e91902a804ee858ea943e8a9b803208d4ea9e2df649d2866086a1812`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 04 Aug 2023 04:52:57 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:52:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:52:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:52:58 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:52:59 GMT
ADD file:bb1fa1d9d012ae826908afdce8c9fa2feebf221b2ab032e1535255905144411a in / 
# Fri, 04 Aug 2023 04:53:00 GMT
CMD ["/bin/bash"]
# Thu, 17 Aug 2023 08:05:44 GMT
RUN apt-get update     && apt-get -y --no-install-recommends install ca-certificates gnupg     && export GNUPGHOME="$(mktemp -d)"     && gpg --no-default-keyring --keyring gnupg-ring:/etc/apt/trusted.gpg.d/sapmachine.gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && chmod 644 /etc/apt/trusted.gpg.d/sapmachine.gpg     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-20-jdk=20.0.2     && apt-get remove -y --purge --autoremove ca-certificates gnupg     && rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 17 Aug 2023 08:05:45 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-20
# Thu, 17 Aug 2023 08:05:45 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:99de9192b4afd13ed65aeae58d55b38e5231eb97a743921357b7d5b4c0c903c4`  
		Last Modified: Fri, 04 Aug 2023 09:25:19 GMT  
		Size: 30.4 MB (30437960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95546972c1b8a95d6033065b1672567c5af170ca7e4f8591d964490526dbeb0`  
		Last Modified: Thu, 17 Aug 2023 08:10:34 GMT  
		Size: 209.3 MB (209331029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:jdk-ubuntu-20.0.2` - linux; arm64 variant v8

```console
$ docker pull sapmachine@sha256:157907d5e72234610e60ff355b725cd198dfd489db2318da6d6043051d555c86
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.0 MB (235979452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faedc7f476cd5c290dce087535f0adfac543212a328920d9f589706140dc248d`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:57:30 GMT
RUN apt-get update     && apt-get -y --no-install-recommends install ca-certificates gnupg     && export GNUPGHOME="$(mktemp -d)"     && gpg --no-default-keyring --keyring gnupg-ring:/etc/apt/trusted.gpg.d/sapmachine.gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && chmod 644 /etc/apt/trusted.gpg.d/sapmachine.gpg     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-20-jdk=20.0.2     && apt-get remove -y --purge --autoremove ca-certificates gnupg     && rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:57:32 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-20
# Fri, 01 Sep 2023 23:57:32 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfca4b4f4aa51b5530718e632987a8e3894e923e070b8201eaeab97409ab1e8a`  
		Last Modified: Sat, 02 Sep 2023 00:06:46 GMT  
		Size: 207.6 MB (207586474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:jdk-ubuntu-20.0.2` - linux; ppc64le

```console
$ docker pull sapmachine@sha256:d111158cc7a8bb3093793b65f7efd4744e268ab328a299bf532af17d58255319
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.4 MB (246371825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25bb37c28af0d0e6762bc84c6b49ae29d0d921ff5bc3b28b107cae1ae4703562`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 04 Aug 2023 04:56:16 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:56:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:56:20 GMT
ADD file:0e9b840e6824ee009acbddc2d337fd5083ebe606393cf7532cdca4f108813ca3 in / 
# Fri, 04 Aug 2023 04:56:20 GMT
CMD ["/bin/bash"]
# Thu, 17 Aug 2023 07:43:37 GMT
RUN apt-get update     && apt-get -y --no-install-recommends install ca-certificates gnupg     && export GNUPGHOME="$(mktemp -d)"     && gpg --no-default-keyring --keyring gnupg-ring:/etc/apt/trusted.gpg.d/sapmachine.gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && chmod 644 /etc/apt/trusted.gpg.d/sapmachine.gpg     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-20-jdk=20.0.2     && apt-get remove -y --purge --autoremove ca-certificates gnupg     && rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:43:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-20
# Thu, 17 Aug 2023 07:43:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:09f4821f68917c7929419fff8bc583c406640180ea7d58eea03a95e463b8fb21`  
		Last Modified: Wed, 16 Aug 2023 02:15:01 GMT  
		Size: 35.7 MB (35712693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f80709b210e5bdcf5c0414da3cac33724347c0f11a6670b68b16ab908cb06c`  
		Last Modified: Thu, 17 Aug 2023 07:52:42 GMT  
		Size: 210.7 MB (210659132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
