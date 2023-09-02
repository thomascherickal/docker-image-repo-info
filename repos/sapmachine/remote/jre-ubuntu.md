## `sapmachine:jre-ubuntu`

```console
$ docker pull sapmachine@sha256:f64a170a3be37411868c5e7fbcc4eb3cb9a660a278775e6a210b9b58edf6400c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `sapmachine:jre-ubuntu` - linux; amd64

```console
$ docker pull sapmachine@sha256:19901ce1954351d5c3c84b7f48ef52970a7834118bf17bb81fbf7c1318a01902
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87115272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae6abe124879dbdd2f4495fe70cb46356dbba08a3b1fde7fd3627c398858ba99`
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
# Thu, 17 Aug 2023 08:04:21 GMT
RUN apt-get update     && apt-get -y --no-install-recommends install ca-certificates gnupg     && export GNUPGHOME="$(mktemp -d)"     && gpg --no-default-keyring --keyring gnupg-ring:/etc/apt/trusted.gpg.d/sapmachine.gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && chmod 644 /etc/apt/trusted.gpg.d/sapmachine.gpg     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-20-jre=20.0.2     && apt-get remove -y --purge --autoremove ca-certificates gnupg     && rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 17 Aug 2023 08:04:22 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-20
# Thu, 17 Aug 2023 08:04:22 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:99de9192b4afd13ed65aeae58d55b38e5231eb97a743921357b7d5b4c0c903c4`  
		Last Modified: Fri, 04 Aug 2023 09:25:19 GMT  
		Size: 30.4 MB (30437960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598314d6162d2a200e3bdbba9bf857c96d8ff837f3acd5e3cddee2daa630a3e7`  
		Last Modified: Thu, 17 Aug 2023 08:09:34 GMT  
		Size: 56.7 MB (56677312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:jre-ubuntu` - linux; arm64 variant v8

```console
$ docker pull sapmachine@sha256:02994b46c24d881adbaef0c339a74d23f453f9d6dd07d2e653a9e999736a9fc3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84210794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1d99fc059da4d3a87e9bdf070f58c3d13957338d30e3f2f0f83ba6b34a5671b`
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
# Fri, 01 Sep 2023 23:56:16 GMT
RUN apt-get update     && apt-get -y --no-install-recommends install ca-certificates gnupg     && export GNUPGHOME="$(mktemp -d)"     && gpg --no-default-keyring --keyring gnupg-ring:/etc/apt/trusted.gpg.d/sapmachine.gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && chmod 644 /etc/apt/trusted.gpg.d/sapmachine.gpg     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-20-jre=20.0.2     && apt-get remove -y --purge --autoremove ca-certificates gnupg     && rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:56:17 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-20
# Fri, 01 Sep 2023 23:56:17 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b862d6d2bfdabb7fd13547313e8c98960925e3e7e83415cc9d50f286ceb796d`  
		Last Modified: Sat, 02 Sep 2023 00:06:00 GMT  
		Size: 55.8 MB (55817816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:jre-ubuntu` - linux; ppc64le

```console
$ docker pull sapmachine@sha256:744337427d0bf36e16e1c59ce86aaa3a8369900955557aae9b83bfd03e1d3123
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.9 MB (93949663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7437d75b1f7f7435909675fd501d87ec7e1007f54ddc7039773d32a2b3e516`
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
# Thu, 17 Aug 2023 07:41:02 GMT
RUN apt-get update     && apt-get -y --no-install-recommends install ca-certificates gnupg     && export GNUPGHOME="$(mktemp -d)"     && gpg --no-default-keyring --keyring gnupg-ring:/etc/apt/trusted.gpg.d/sapmachine.gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && chmod 644 /etc/apt/trusted.gpg.d/sapmachine.gpg     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-20-jre=20.0.2     && apt-get remove -y --purge --autoremove ca-certificates gnupg     && rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:41:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-20
# Thu, 17 Aug 2023 07:41:05 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:09f4821f68917c7929419fff8bc583c406640180ea7d58eea03a95e463b8fb21`  
		Last Modified: Wed, 16 Aug 2023 02:15:01 GMT  
		Size: 35.7 MB (35712693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f86dd69e60f7f3831da695f52bcf88c8f8ab872ed7843873e3153b88e52ae6`  
		Last Modified: Thu, 17 Aug 2023 07:51:16 GMT  
		Size: 58.2 MB (58236970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
