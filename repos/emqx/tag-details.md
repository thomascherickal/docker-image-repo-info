<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `emqx`

-	[`emqx:4`](#emqx4)
-	[`emqx:4.4`](#emqx44)
-	[`emqx:4.4.17`](#emqx4417)
-	[`emqx:5`](#emqx5)
-	[`emqx:5.0`](#emqx50)
-	[`emqx:5.0.24`](#emqx5024)
-	[`emqx:latest`](#emqxlatest)

## `emqx:4`

```console
$ docker pull emqx@sha256:efb42eb4c4201f0bc813732e05e5b400c7cbcf82eae240669a25836de95e2d86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:fa6124a46631fb7773814409ef36869405b2fddc6356b2fd7ed9c9b2ce758716
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81291619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779ea7d294a716bc616999386b5538d20c6034e5b0bf044a99112761ff1f5bc6`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:42:35 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:42:35 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 18 Apr 2023 19:23:36 GMT
ENV EMQX_VERSION=4.4.17
# Tue, 18 Apr 2023 19:23:36 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 18 Apr 2023 19:23:41 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b078cfe835799485748a4d31b4af2a4f7bc696da8f64e22662b46a95bfec74af"; fi;     if [ ${arch} = "arm64" ]; then sha256="4d2cc9d908490d3ba5f6d2d53e0280dee0753783f78f8e6701e5d5c9550e75f4"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 18 Apr 2023 19:23:41 GMT
WORKDIR /opt/emqx
# Tue, 18 Apr 2023 19:23:41 GMT
USER emqx
# Tue, 18 Apr 2023 19:23:41 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 18 Apr 2023 19:23:41 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 18 Apr 2023 19:23:41 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 18 Apr 2023 19:23:41 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 19:23:41 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e901aaad2c36dc10a256fae9d94810d0bcd1d3732eb3e172f7d18eba970956df`  
		Last Modified: Wed, 12 Apr 2023 00:43:09 GMT  
		Size: 2.6 MB (2569627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f607aa293305bd4722109d3b17853a91b8de9754b42fe37d71be6cf3c9abb42`  
		Last Modified: Wed, 12 Apr 2023 00:43:08 GMT  
		Size: 4.1 KB (4105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e373660f2b074988b14b445797e5e459946a789b7e4981e69fbed00b959571`  
		Last Modified: Tue, 18 Apr 2023 19:24:07 GMT  
		Size: 47.3 MB (47298553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22311b4086c25ed91b21e8e5fec900750420d095f40f047cd61940b299f9c3df`  
		Last Modified: Tue, 18 Apr 2023 19:24:02 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:a6f997e81d50a04ba433686109a70031148c52a8ee5768605ad468eec8fb07d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72707877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a05a7ba17574b3be0da7935a562b2a553595666a86c3b0441689024fe6b5e1d4`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:38:12 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:38:13 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 18 Apr 2023 18:39:23 GMT
ENV EMQX_VERSION=4.4.17
# Tue, 18 Apr 2023 18:39:23 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 18 Apr 2023 18:39:26 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b078cfe835799485748a4d31b4af2a4f7bc696da8f64e22662b46a95bfec74af"; fi;     if [ ${arch} = "arm64" ]; then sha256="4d2cc9d908490d3ba5f6d2d53e0280dee0753783f78f8e6701e5d5c9550e75f4"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 18 Apr 2023 18:39:27 GMT
WORKDIR /opt/emqx
# Tue, 18 Apr 2023 18:39:27 GMT
USER emqx
# Tue, 18 Apr 2023 18:39:27 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 18 Apr 2023 18:39:27 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 18 Apr 2023 18:39:27 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 18 Apr 2023 18:39:27 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 18:39:27 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4322e90f757b16a8adb2d40ade499d3006e85ca6d83f0eb96ea9691b6871dd`  
		Last Modified: Wed, 12 Apr 2023 01:38:39 GMT  
		Size: 2.6 MB (2559482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3071e2b66079e6214608516ff2e6a436738f7da65ae6bb2c5357edcfb8d54a78`  
		Last Modified: Wed, 12 Apr 2023 01:38:38 GMT  
		Size: 4.1 KB (4116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745b037587ac726ae947e23c5a90c1b664d676bc4ed966e8824782fbb0a43de2`  
		Last Modified: Tue, 18 Apr 2023 18:39:49 GMT  
		Size: 40.1 MB (40079345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cecd1cab1d85ea166bf8809c679d6df88f9e1aaa7fcdea562997208abeb7e175`  
		Last Modified: Tue, 18 Apr 2023 18:39:46 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:efb42eb4c4201f0bc813732e05e5b400c7cbcf82eae240669a25836de95e2d86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:fa6124a46631fb7773814409ef36869405b2fddc6356b2fd7ed9c9b2ce758716
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81291619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779ea7d294a716bc616999386b5538d20c6034e5b0bf044a99112761ff1f5bc6`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:42:35 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:42:35 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 18 Apr 2023 19:23:36 GMT
ENV EMQX_VERSION=4.4.17
# Tue, 18 Apr 2023 19:23:36 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 18 Apr 2023 19:23:41 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b078cfe835799485748a4d31b4af2a4f7bc696da8f64e22662b46a95bfec74af"; fi;     if [ ${arch} = "arm64" ]; then sha256="4d2cc9d908490d3ba5f6d2d53e0280dee0753783f78f8e6701e5d5c9550e75f4"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 18 Apr 2023 19:23:41 GMT
WORKDIR /opt/emqx
# Tue, 18 Apr 2023 19:23:41 GMT
USER emqx
# Tue, 18 Apr 2023 19:23:41 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 18 Apr 2023 19:23:41 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 18 Apr 2023 19:23:41 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 18 Apr 2023 19:23:41 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 19:23:41 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e901aaad2c36dc10a256fae9d94810d0bcd1d3732eb3e172f7d18eba970956df`  
		Last Modified: Wed, 12 Apr 2023 00:43:09 GMT  
		Size: 2.6 MB (2569627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f607aa293305bd4722109d3b17853a91b8de9754b42fe37d71be6cf3c9abb42`  
		Last Modified: Wed, 12 Apr 2023 00:43:08 GMT  
		Size: 4.1 KB (4105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e373660f2b074988b14b445797e5e459946a789b7e4981e69fbed00b959571`  
		Last Modified: Tue, 18 Apr 2023 19:24:07 GMT  
		Size: 47.3 MB (47298553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22311b4086c25ed91b21e8e5fec900750420d095f40f047cd61940b299f9c3df`  
		Last Modified: Tue, 18 Apr 2023 19:24:02 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:a6f997e81d50a04ba433686109a70031148c52a8ee5768605ad468eec8fb07d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72707877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a05a7ba17574b3be0da7935a562b2a553595666a86c3b0441689024fe6b5e1d4`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:38:12 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:38:13 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 18 Apr 2023 18:39:23 GMT
ENV EMQX_VERSION=4.4.17
# Tue, 18 Apr 2023 18:39:23 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 18 Apr 2023 18:39:26 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b078cfe835799485748a4d31b4af2a4f7bc696da8f64e22662b46a95bfec74af"; fi;     if [ ${arch} = "arm64" ]; then sha256="4d2cc9d908490d3ba5f6d2d53e0280dee0753783f78f8e6701e5d5c9550e75f4"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 18 Apr 2023 18:39:27 GMT
WORKDIR /opt/emqx
# Tue, 18 Apr 2023 18:39:27 GMT
USER emqx
# Tue, 18 Apr 2023 18:39:27 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 18 Apr 2023 18:39:27 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 18 Apr 2023 18:39:27 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 18 Apr 2023 18:39:27 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 18:39:27 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4322e90f757b16a8adb2d40ade499d3006e85ca6d83f0eb96ea9691b6871dd`  
		Last Modified: Wed, 12 Apr 2023 01:38:39 GMT  
		Size: 2.6 MB (2559482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3071e2b66079e6214608516ff2e6a436738f7da65ae6bb2c5357edcfb8d54a78`  
		Last Modified: Wed, 12 Apr 2023 01:38:38 GMT  
		Size: 4.1 KB (4116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745b037587ac726ae947e23c5a90c1b664d676bc4ed966e8824782fbb0a43de2`  
		Last Modified: Tue, 18 Apr 2023 18:39:49 GMT  
		Size: 40.1 MB (40079345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cecd1cab1d85ea166bf8809c679d6df88f9e1aaa7fcdea562997208abeb7e175`  
		Last Modified: Tue, 18 Apr 2023 18:39:46 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.17`

```console
$ docker pull emqx@sha256:efb42eb4c4201f0bc813732e05e5b400c7cbcf82eae240669a25836de95e2d86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4.17` - linux; amd64

```console
$ docker pull emqx@sha256:fa6124a46631fb7773814409ef36869405b2fddc6356b2fd7ed9c9b2ce758716
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81291619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779ea7d294a716bc616999386b5538d20c6034e5b0bf044a99112761ff1f5bc6`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:42:35 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:42:35 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 18 Apr 2023 19:23:36 GMT
ENV EMQX_VERSION=4.4.17
# Tue, 18 Apr 2023 19:23:36 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 18 Apr 2023 19:23:41 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b078cfe835799485748a4d31b4af2a4f7bc696da8f64e22662b46a95bfec74af"; fi;     if [ ${arch} = "arm64" ]; then sha256="4d2cc9d908490d3ba5f6d2d53e0280dee0753783f78f8e6701e5d5c9550e75f4"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 18 Apr 2023 19:23:41 GMT
WORKDIR /opt/emqx
# Tue, 18 Apr 2023 19:23:41 GMT
USER emqx
# Tue, 18 Apr 2023 19:23:41 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 18 Apr 2023 19:23:41 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 18 Apr 2023 19:23:41 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 18 Apr 2023 19:23:41 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 19:23:41 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e901aaad2c36dc10a256fae9d94810d0bcd1d3732eb3e172f7d18eba970956df`  
		Last Modified: Wed, 12 Apr 2023 00:43:09 GMT  
		Size: 2.6 MB (2569627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f607aa293305bd4722109d3b17853a91b8de9754b42fe37d71be6cf3c9abb42`  
		Last Modified: Wed, 12 Apr 2023 00:43:08 GMT  
		Size: 4.1 KB (4105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e373660f2b074988b14b445797e5e459946a789b7e4981e69fbed00b959571`  
		Last Modified: Tue, 18 Apr 2023 19:24:07 GMT  
		Size: 47.3 MB (47298553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22311b4086c25ed91b21e8e5fec900750420d095f40f047cd61940b299f9c3df`  
		Last Modified: Tue, 18 Apr 2023 19:24:02 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4.17` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:a6f997e81d50a04ba433686109a70031148c52a8ee5768605ad468eec8fb07d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72707877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a05a7ba17574b3be0da7935a562b2a553595666a86c3b0441689024fe6b5e1d4`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:38:12 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:38:13 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 18 Apr 2023 18:39:23 GMT
ENV EMQX_VERSION=4.4.17
# Tue, 18 Apr 2023 18:39:23 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 18 Apr 2023 18:39:26 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b078cfe835799485748a4d31b4af2a4f7bc696da8f64e22662b46a95bfec74af"; fi;     if [ ${arch} = "arm64" ]; then sha256="4d2cc9d908490d3ba5f6d2d53e0280dee0753783f78f8e6701e5d5c9550e75f4"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 18 Apr 2023 18:39:27 GMT
WORKDIR /opt/emqx
# Tue, 18 Apr 2023 18:39:27 GMT
USER emqx
# Tue, 18 Apr 2023 18:39:27 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 18 Apr 2023 18:39:27 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 18 Apr 2023 18:39:27 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 18 Apr 2023 18:39:27 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 18:39:27 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4322e90f757b16a8adb2d40ade499d3006e85ca6d83f0eb96ea9691b6871dd`  
		Last Modified: Wed, 12 Apr 2023 01:38:39 GMT  
		Size: 2.6 MB (2559482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3071e2b66079e6214608516ff2e6a436738f7da65ae6bb2c5357edcfb8d54a78`  
		Last Modified: Wed, 12 Apr 2023 01:38:38 GMT  
		Size: 4.1 KB (4116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745b037587ac726ae947e23c5a90c1b664d676bc4ed966e8824782fbb0a43de2`  
		Last Modified: Tue, 18 Apr 2023 18:39:49 GMT  
		Size: 40.1 MB (40079345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cecd1cab1d85ea166bf8809c679d6df88f9e1aaa7fcdea562997208abeb7e175`  
		Last Modified: Tue, 18 Apr 2023 18:39:46 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5`

```console
$ docker pull emqx@sha256:7a9b96afd62a453c1d94beffd4bbd9f7a21ca7706efcd97d52d6a97a816c73ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:bf9cbff4d72692150db0b8e71c12169682e4a1ecabaf31a0815a124b2c8c7191
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110351254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:324d003bff51e7326b599161e64280e9fb441616cc376c65b64979a6e57e1fca`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:42:50 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:42:51 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 27 Apr 2023 18:19:36 GMT
ENV EMQX_VERSION=5.0.24
# Thu, 27 Apr 2023 18:19:36 GMT
ENV AMD64_SHA256=d104bc3e1839447f5ceeaadbb3feb6c604c5f74b07ca33ab4c37baf2a9b33ae3
# Thu, 27 Apr 2023 18:19:36 GMT
ENV ARM64_SHA256=40d387b7d4dfc4aa7162ef628f25bcb33e8a3fc67740b3cdb5a6d843aa87c2ec
# Thu, 27 Apr 2023 18:19:36 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 27 Apr 2023 18:19:43 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 27 Apr 2023 18:19:43 GMT
WORKDIR /opt/emqx
# Thu, 27 Apr 2023 18:19:44 GMT
USER emqx
# Thu, 27 Apr 2023 18:19:44 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 27 Apr 2023 18:19:44 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 27 Apr 2023 18:19:44 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 27 Apr 2023 18:19:44 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 27 Apr 2023 18:19:44 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f79c821cbd23fa1420033390e2828e0922b8efe06687c960eb7ff40edfbd0d6`  
		Last Modified: Wed, 12 Apr 2023 00:43:23 GMT  
		Size: 3.0 MB (2987825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048c1bdd86f15f4d429d049f898a2d3c0f0732c5b7e68a31b824acae055655d8`  
		Last Modified: Wed, 12 Apr 2023 00:43:22 GMT  
		Size: 4.1 KB (4105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ffb33fdb8e8734d8315c830f113b34280d1b709d9b2022540e77ce0012c71a`  
		Last Modified: Thu, 27 Apr 2023 18:20:04 GMT  
		Size: 75.9 MB (75940194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baedd37ee870a8649d239a5d45f6d6c498c1a0da32321dfdf8af290f463d9969`  
		Last Modified: Thu, 27 Apr 2023 18:19:55 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:fde8c0241c8356e182740b53501c749503566f7325cf2b18879b193e69cb4e34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.4 MB (101431939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e429d23a3660ac23a51b2e7a39925e123821d8772626c4ed67ee8ed2ebea519`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:38:23 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:38:24 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 27 Apr 2023 18:39:23 GMT
ENV EMQX_VERSION=5.0.24
# Thu, 27 Apr 2023 18:39:23 GMT
ENV AMD64_SHA256=d104bc3e1839447f5ceeaadbb3feb6c604c5f74b07ca33ab4c37baf2a9b33ae3
# Thu, 27 Apr 2023 18:39:24 GMT
ENV ARM64_SHA256=40d387b7d4dfc4aa7162ef628f25bcb33e8a3fc67740b3cdb5a6d843aa87c2ec
# Thu, 27 Apr 2023 18:39:24 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 27 Apr 2023 18:39:29 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 27 Apr 2023 18:39:32 GMT
WORKDIR /opt/emqx
# Thu, 27 Apr 2023 18:39:32 GMT
USER emqx
# Thu, 27 Apr 2023 18:39:32 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 27 Apr 2023 18:39:32 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 27 Apr 2023 18:39:32 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 27 Apr 2023 18:39:32 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 27 Apr 2023 18:39:32 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b64e3be9abc32d122bd4b9c6cbdc2adc75085b08f7644acbd1e9a963977cd48`  
		Last Modified: Wed, 12 Apr 2023 01:38:53 GMT  
		Size: 3.0 MB (3002944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b665badbe1ecc88ea2bdc4962042f6412551d166e4bc0bfbfcd3e00d159e605`  
		Last Modified: Wed, 12 Apr 2023 01:38:52 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b96efd53a797fc858ff4162a501d037ed7f47c0b5c364ddfc162a9e4ca783d1`  
		Last Modified: Thu, 27 Apr 2023 18:39:48 GMT  
		Size: 68.4 MB (68360154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f412c45dfb5508d58a91d176738d5ff194b387c8b23426099de883ed14b5f4`  
		Last Modified: Thu, 27 Apr 2023 18:39:41 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:7a9b96afd62a453c1d94beffd4bbd9f7a21ca7706efcd97d52d6a97a816c73ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:bf9cbff4d72692150db0b8e71c12169682e4a1ecabaf31a0815a124b2c8c7191
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110351254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:324d003bff51e7326b599161e64280e9fb441616cc376c65b64979a6e57e1fca`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:42:50 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:42:51 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 27 Apr 2023 18:19:36 GMT
ENV EMQX_VERSION=5.0.24
# Thu, 27 Apr 2023 18:19:36 GMT
ENV AMD64_SHA256=d104bc3e1839447f5ceeaadbb3feb6c604c5f74b07ca33ab4c37baf2a9b33ae3
# Thu, 27 Apr 2023 18:19:36 GMT
ENV ARM64_SHA256=40d387b7d4dfc4aa7162ef628f25bcb33e8a3fc67740b3cdb5a6d843aa87c2ec
# Thu, 27 Apr 2023 18:19:36 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 27 Apr 2023 18:19:43 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 27 Apr 2023 18:19:43 GMT
WORKDIR /opt/emqx
# Thu, 27 Apr 2023 18:19:44 GMT
USER emqx
# Thu, 27 Apr 2023 18:19:44 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 27 Apr 2023 18:19:44 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 27 Apr 2023 18:19:44 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 27 Apr 2023 18:19:44 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 27 Apr 2023 18:19:44 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f79c821cbd23fa1420033390e2828e0922b8efe06687c960eb7ff40edfbd0d6`  
		Last Modified: Wed, 12 Apr 2023 00:43:23 GMT  
		Size: 3.0 MB (2987825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048c1bdd86f15f4d429d049f898a2d3c0f0732c5b7e68a31b824acae055655d8`  
		Last Modified: Wed, 12 Apr 2023 00:43:22 GMT  
		Size: 4.1 KB (4105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ffb33fdb8e8734d8315c830f113b34280d1b709d9b2022540e77ce0012c71a`  
		Last Modified: Thu, 27 Apr 2023 18:20:04 GMT  
		Size: 75.9 MB (75940194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baedd37ee870a8649d239a5d45f6d6c498c1a0da32321dfdf8af290f463d9969`  
		Last Modified: Thu, 27 Apr 2023 18:19:55 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:fde8c0241c8356e182740b53501c749503566f7325cf2b18879b193e69cb4e34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.4 MB (101431939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e429d23a3660ac23a51b2e7a39925e123821d8772626c4ed67ee8ed2ebea519`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:38:23 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:38:24 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 27 Apr 2023 18:39:23 GMT
ENV EMQX_VERSION=5.0.24
# Thu, 27 Apr 2023 18:39:23 GMT
ENV AMD64_SHA256=d104bc3e1839447f5ceeaadbb3feb6c604c5f74b07ca33ab4c37baf2a9b33ae3
# Thu, 27 Apr 2023 18:39:24 GMT
ENV ARM64_SHA256=40d387b7d4dfc4aa7162ef628f25bcb33e8a3fc67740b3cdb5a6d843aa87c2ec
# Thu, 27 Apr 2023 18:39:24 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 27 Apr 2023 18:39:29 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 27 Apr 2023 18:39:32 GMT
WORKDIR /opt/emqx
# Thu, 27 Apr 2023 18:39:32 GMT
USER emqx
# Thu, 27 Apr 2023 18:39:32 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 27 Apr 2023 18:39:32 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 27 Apr 2023 18:39:32 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 27 Apr 2023 18:39:32 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 27 Apr 2023 18:39:32 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b64e3be9abc32d122bd4b9c6cbdc2adc75085b08f7644acbd1e9a963977cd48`  
		Last Modified: Wed, 12 Apr 2023 01:38:53 GMT  
		Size: 3.0 MB (3002944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b665badbe1ecc88ea2bdc4962042f6412551d166e4bc0bfbfcd3e00d159e605`  
		Last Modified: Wed, 12 Apr 2023 01:38:52 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b96efd53a797fc858ff4162a501d037ed7f47c0b5c364ddfc162a9e4ca783d1`  
		Last Modified: Thu, 27 Apr 2023 18:39:48 GMT  
		Size: 68.4 MB (68360154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f412c45dfb5508d58a91d176738d5ff194b387c8b23426099de883ed14b5f4`  
		Last Modified: Thu, 27 Apr 2023 18:39:41 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.24`

```console
$ docker pull emqx@sha256:7a9b96afd62a453c1d94beffd4bbd9f7a21ca7706efcd97d52d6a97a816c73ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0.24` - linux; amd64

```console
$ docker pull emqx@sha256:bf9cbff4d72692150db0b8e71c12169682e4a1ecabaf31a0815a124b2c8c7191
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110351254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:324d003bff51e7326b599161e64280e9fb441616cc376c65b64979a6e57e1fca`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:42:50 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:42:51 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 27 Apr 2023 18:19:36 GMT
ENV EMQX_VERSION=5.0.24
# Thu, 27 Apr 2023 18:19:36 GMT
ENV AMD64_SHA256=d104bc3e1839447f5ceeaadbb3feb6c604c5f74b07ca33ab4c37baf2a9b33ae3
# Thu, 27 Apr 2023 18:19:36 GMT
ENV ARM64_SHA256=40d387b7d4dfc4aa7162ef628f25bcb33e8a3fc67740b3cdb5a6d843aa87c2ec
# Thu, 27 Apr 2023 18:19:36 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 27 Apr 2023 18:19:43 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 27 Apr 2023 18:19:43 GMT
WORKDIR /opt/emqx
# Thu, 27 Apr 2023 18:19:44 GMT
USER emqx
# Thu, 27 Apr 2023 18:19:44 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 27 Apr 2023 18:19:44 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 27 Apr 2023 18:19:44 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 27 Apr 2023 18:19:44 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 27 Apr 2023 18:19:44 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f79c821cbd23fa1420033390e2828e0922b8efe06687c960eb7ff40edfbd0d6`  
		Last Modified: Wed, 12 Apr 2023 00:43:23 GMT  
		Size: 3.0 MB (2987825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048c1bdd86f15f4d429d049f898a2d3c0f0732c5b7e68a31b824acae055655d8`  
		Last Modified: Wed, 12 Apr 2023 00:43:22 GMT  
		Size: 4.1 KB (4105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ffb33fdb8e8734d8315c830f113b34280d1b709d9b2022540e77ce0012c71a`  
		Last Modified: Thu, 27 Apr 2023 18:20:04 GMT  
		Size: 75.9 MB (75940194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baedd37ee870a8649d239a5d45f6d6c498c1a0da32321dfdf8af290f463d9969`  
		Last Modified: Thu, 27 Apr 2023 18:19:55 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0.24` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:fde8c0241c8356e182740b53501c749503566f7325cf2b18879b193e69cb4e34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.4 MB (101431939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e429d23a3660ac23a51b2e7a39925e123821d8772626c4ed67ee8ed2ebea519`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:38:23 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:38:24 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 27 Apr 2023 18:39:23 GMT
ENV EMQX_VERSION=5.0.24
# Thu, 27 Apr 2023 18:39:23 GMT
ENV AMD64_SHA256=d104bc3e1839447f5ceeaadbb3feb6c604c5f74b07ca33ab4c37baf2a9b33ae3
# Thu, 27 Apr 2023 18:39:24 GMT
ENV ARM64_SHA256=40d387b7d4dfc4aa7162ef628f25bcb33e8a3fc67740b3cdb5a6d843aa87c2ec
# Thu, 27 Apr 2023 18:39:24 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 27 Apr 2023 18:39:29 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 27 Apr 2023 18:39:32 GMT
WORKDIR /opt/emqx
# Thu, 27 Apr 2023 18:39:32 GMT
USER emqx
# Thu, 27 Apr 2023 18:39:32 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 27 Apr 2023 18:39:32 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 27 Apr 2023 18:39:32 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 27 Apr 2023 18:39:32 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 27 Apr 2023 18:39:32 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b64e3be9abc32d122bd4b9c6cbdc2adc75085b08f7644acbd1e9a963977cd48`  
		Last Modified: Wed, 12 Apr 2023 01:38:53 GMT  
		Size: 3.0 MB (3002944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b665badbe1ecc88ea2bdc4962042f6412551d166e4bc0bfbfcd3e00d159e605`  
		Last Modified: Wed, 12 Apr 2023 01:38:52 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b96efd53a797fc858ff4162a501d037ed7f47c0b5c364ddfc162a9e4ca783d1`  
		Last Modified: Thu, 27 Apr 2023 18:39:48 GMT  
		Size: 68.4 MB (68360154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f412c45dfb5508d58a91d176738d5ff194b387c8b23426099de883ed14b5f4`  
		Last Modified: Thu, 27 Apr 2023 18:39:41 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:7a9b96afd62a453c1d94beffd4bbd9f7a21ca7706efcd97d52d6a97a816c73ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:bf9cbff4d72692150db0b8e71c12169682e4a1ecabaf31a0815a124b2c8c7191
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110351254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:324d003bff51e7326b599161e64280e9fb441616cc376c65b64979a6e57e1fca`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:42:50 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:42:51 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 27 Apr 2023 18:19:36 GMT
ENV EMQX_VERSION=5.0.24
# Thu, 27 Apr 2023 18:19:36 GMT
ENV AMD64_SHA256=d104bc3e1839447f5ceeaadbb3feb6c604c5f74b07ca33ab4c37baf2a9b33ae3
# Thu, 27 Apr 2023 18:19:36 GMT
ENV ARM64_SHA256=40d387b7d4dfc4aa7162ef628f25bcb33e8a3fc67740b3cdb5a6d843aa87c2ec
# Thu, 27 Apr 2023 18:19:36 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 27 Apr 2023 18:19:43 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 27 Apr 2023 18:19:43 GMT
WORKDIR /opt/emqx
# Thu, 27 Apr 2023 18:19:44 GMT
USER emqx
# Thu, 27 Apr 2023 18:19:44 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 27 Apr 2023 18:19:44 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 27 Apr 2023 18:19:44 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 27 Apr 2023 18:19:44 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 27 Apr 2023 18:19:44 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f79c821cbd23fa1420033390e2828e0922b8efe06687c960eb7ff40edfbd0d6`  
		Last Modified: Wed, 12 Apr 2023 00:43:23 GMT  
		Size: 3.0 MB (2987825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048c1bdd86f15f4d429d049f898a2d3c0f0732c5b7e68a31b824acae055655d8`  
		Last Modified: Wed, 12 Apr 2023 00:43:22 GMT  
		Size: 4.1 KB (4105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ffb33fdb8e8734d8315c830f113b34280d1b709d9b2022540e77ce0012c71a`  
		Last Modified: Thu, 27 Apr 2023 18:20:04 GMT  
		Size: 75.9 MB (75940194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baedd37ee870a8649d239a5d45f6d6c498c1a0da32321dfdf8af290f463d9969`  
		Last Modified: Thu, 27 Apr 2023 18:19:55 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:fde8c0241c8356e182740b53501c749503566f7325cf2b18879b193e69cb4e34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.4 MB (101431939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e429d23a3660ac23a51b2e7a39925e123821d8772626c4ed67ee8ed2ebea519`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:38:23 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:38:24 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 27 Apr 2023 18:39:23 GMT
ENV EMQX_VERSION=5.0.24
# Thu, 27 Apr 2023 18:39:23 GMT
ENV AMD64_SHA256=d104bc3e1839447f5ceeaadbb3feb6c604c5f74b07ca33ab4c37baf2a9b33ae3
# Thu, 27 Apr 2023 18:39:24 GMT
ENV ARM64_SHA256=40d387b7d4dfc4aa7162ef628f25bcb33e8a3fc67740b3cdb5a6d843aa87c2ec
# Thu, 27 Apr 2023 18:39:24 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 27 Apr 2023 18:39:29 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 27 Apr 2023 18:39:32 GMT
WORKDIR /opt/emqx
# Thu, 27 Apr 2023 18:39:32 GMT
USER emqx
# Thu, 27 Apr 2023 18:39:32 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 27 Apr 2023 18:39:32 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 27 Apr 2023 18:39:32 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 27 Apr 2023 18:39:32 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 27 Apr 2023 18:39:32 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b64e3be9abc32d122bd4b9c6cbdc2adc75085b08f7644acbd1e9a963977cd48`  
		Last Modified: Wed, 12 Apr 2023 01:38:53 GMT  
		Size: 3.0 MB (3002944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b665badbe1ecc88ea2bdc4962042f6412551d166e4bc0bfbfcd3e00d159e605`  
		Last Modified: Wed, 12 Apr 2023 01:38:52 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b96efd53a797fc858ff4162a501d037ed7f47c0b5c364ddfc162a9e4ca783d1`  
		Last Modified: Thu, 27 Apr 2023 18:39:48 GMT  
		Size: 68.4 MB (68360154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f412c45dfb5508d58a91d176738d5ff194b387c8b23426099de883ed14b5f4`  
		Last Modified: Thu, 27 Apr 2023 18:39:41 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
