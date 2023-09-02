## `sapmachine:jdk-ubuntu-11.0.20`

```console
$ docker pull sapmachine@sha256:9d98d62615dd9fb3c77e0fb8b0bf0f153ee362d1cb4529898740c74971e39978
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `sapmachine:jdk-ubuntu-11.0.20` - linux; amd64

```console
$ docker pull sapmachine@sha256:24a0d0e093e75c381f74458575126db76312ff0f1d469d75ed8d2cc73ee67d50
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.7 MB (230692459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82e68f32b7f14084ac5f9efc20ac1b8fe6d921a13ea7de0e9b5efbb7c0ed56ce`
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
# Thu, 17 Aug 2023 08:01:22 GMT
RUN apt-get update     && apt-get -y --no-install-recommends install ca-certificates gnupg     && export GNUPGHOME="$(mktemp -d)"     && gpg --no-default-keyring --keyring gnupg-ring:/etc/apt/trusted.gpg.d/sapmachine.gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && chmod 644 /etc/apt/trusted.gpg.d/sapmachine.gpg     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.20     && apt-get remove -y --purge --autoremove ca-certificates gnupg     && rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 17 Aug 2023 08:01:23 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Thu, 17 Aug 2023 08:01:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:99de9192b4afd13ed65aeae58d55b38e5231eb97a743921357b7d5b4c0c903c4`  
		Last Modified: Fri, 04 Aug 2023 09:25:19 GMT  
		Size: 30.4 MB (30437960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5585f521c90415b576413acd65cafa275b1842c0922a70f9b7223f52c8b6745`  
		Last Modified: Thu, 17 Aug 2023 08:07:18 GMT  
		Size: 200.3 MB (200254499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:jdk-ubuntu-11.0.20` - linux; arm64 variant v8

```console
$ docker pull sapmachine@sha256:becf89171521f251517291b9eb39b00485d41295f119bcc223df12708ad0077f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.0 MB (227028504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a08baad1e6664aff01f51658b76a3fc83f9fe7b8ac47d913aba7418d46d1f56`
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
# Fri, 01 Sep 2023 23:53:40 GMT
RUN apt-get update     && apt-get -y --no-install-recommends install ca-certificates gnupg     && export GNUPGHOME="$(mktemp -d)"     && gpg --no-default-keyring --keyring gnupg-ring:/etc/apt/trusted.gpg.d/sapmachine.gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && chmod 644 /etc/apt/trusted.gpg.d/sapmachine.gpg     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.20     && apt-get remove -y --purge --autoremove ca-certificates gnupg     && rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:53:42 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Fri, 01 Sep 2023 23:53:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf77e4981acd8fcc2165d31787abc21dfbac511fde792613986c8a9f68c37ad`  
		Last Modified: Sat, 02 Sep 2023 00:04:07 GMT  
		Size: 198.6 MB (198635526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:jdk-ubuntu-11.0.20` - linux; ppc64le

```console
$ docker pull sapmachine@sha256:40691bdb7c77cdc23d8bce90896124843cc59e6ebdf8617958406b8f08a2de1c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.5 MB (222541337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c45c677527d4ebfb21a6df939278a58d3aedc7a718e3d02b3da32ecb48954f9`
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
# Thu, 17 Aug 2023 07:35:08 GMT
RUN apt-get update     && apt-get -y --no-install-recommends install ca-certificates gnupg     && export GNUPGHOME="$(mktemp -d)"     && gpg --no-default-keyring --keyring gnupg-ring:/etc/apt/trusted.gpg.d/sapmachine.gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && chmod 644 /etc/apt/trusted.gpg.d/sapmachine.gpg     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.20     && apt-get remove -y --purge --autoremove ca-certificates gnupg     && rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:35:11 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Thu, 17 Aug 2023 07:35:11 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:09f4821f68917c7929419fff8bc583c406640180ea7d58eea03a95e463b8fb21`  
		Last Modified: Wed, 16 Aug 2023 02:15:01 GMT  
		Size: 35.7 MB (35712693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edca6db0edc565f1a188c05a71240567e285648126c85099a06307947c52fd1`  
		Last Modified: Thu, 17 Aug 2023 07:47:51 GMT  
		Size: 186.8 MB (186828644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
