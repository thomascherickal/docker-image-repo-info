<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `emqx`

-	[`emqx:4`](#emqx4)
-	[`emqx:4.4`](#emqx44)
-	[`emqx:4.4.17`](#emqx4417)
-	[`emqx:5`](#emqx5)
-	[`emqx:5.0`](#emqx50)
-	[`emqx:5.0.23`](#emqx5023)
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
$ docker pull emqx@sha256:386cabf97b0cbf3fde558b08a4d4fb27d02da66a530937ab9f13661e2a48c671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:12e2463b0de9fe52971a2584364e2c9b304474670813cdf24b0c8a5ef67d6121
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.1 MB (111077435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd1fc2469f25a8b9a360f6b9875686f5951073b1c64aa22cc09d5ed87c4b81f8`
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
# Tue, 18 Apr 2023 19:23:44 GMT
ENV EMQX_VERSION=5.0.23
# Tue, 18 Apr 2023 19:23:44 GMT
ENV AMD64_SHA256=66322a18c2c1677d9ee07f44d06410d8b3914782f7b56dceb67c44ab946bc8bd
# Tue, 18 Apr 2023 19:23:44 GMT
ENV ARM64_SHA256=74c0f096fbd8b480f79b45918de83148ba0c1defcf997f268557ed27f85d9159
# Tue, 18 Apr 2023 19:23:44 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 18 Apr 2023 19:23:51 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 18 Apr 2023 19:23:51 GMT
WORKDIR /opt/emqx
# Tue, 18 Apr 2023 19:23:51 GMT
USER emqx
# Tue, 18 Apr 2023 19:23:51 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 18 Apr 2023 19:23:52 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 18 Apr 2023 19:23:52 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 18 Apr 2023 19:23:52 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 19:23:52 GMT
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
	-	`sha256:0ce2d792f43e68e6f144aad7a024ec68c528c45f63e1e46075ce51f13488b832`  
		Last Modified: Tue, 18 Apr 2023 19:24:27 GMT  
		Size: 76.7 MB (76666377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8af10bdd33f36ef136f5ef915af25bde6c0a0dd652ac95b6ec3c6bbb88524d7`  
		Last Modified: Tue, 18 Apr 2023 19:24:17 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:b20b0908ec021f4ec179fd55b0b1fd1ad2573dfa23b060e333fb695394a561ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102157787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7bae0c81f826ed909247451fba3ee3518fb415381812dcbbf2209b9d24d3795`
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
# Tue, 18 Apr 2023 18:39:29 GMT
ENV EMQX_VERSION=5.0.23
# Tue, 18 Apr 2023 18:39:29 GMT
ENV AMD64_SHA256=66322a18c2c1677d9ee07f44d06410d8b3914782f7b56dceb67c44ab946bc8bd
# Tue, 18 Apr 2023 18:39:29 GMT
ENV ARM64_SHA256=74c0f096fbd8b480f79b45918de83148ba0c1defcf997f268557ed27f85d9159
# Tue, 18 Apr 2023 18:39:29 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 18 Apr 2023 18:39:34 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 18 Apr 2023 18:39:35 GMT
WORKDIR /opt/emqx
# Tue, 18 Apr 2023 18:39:35 GMT
USER emqx
# Tue, 18 Apr 2023 18:39:35 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 18 Apr 2023 18:39:35 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 18 Apr 2023 18:39:35 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 18 Apr 2023 18:39:36 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 18:39:36 GMT
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
	-	`sha256:81826c36e478507e264f8473188bd6a67787268ae42d90ed3468e89afd28f271`  
		Last Modified: Tue, 18 Apr 2023 18:40:06 GMT  
		Size: 69.1 MB (69086004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb58189c390f19b6def2d0a892c2211334d48973166ef7574b3ccb3e5f1f24f0`  
		Last Modified: Tue, 18 Apr 2023 18:39:59 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:386cabf97b0cbf3fde558b08a4d4fb27d02da66a530937ab9f13661e2a48c671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:12e2463b0de9fe52971a2584364e2c9b304474670813cdf24b0c8a5ef67d6121
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.1 MB (111077435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd1fc2469f25a8b9a360f6b9875686f5951073b1c64aa22cc09d5ed87c4b81f8`
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
# Tue, 18 Apr 2023 19:23:44 GMT
ENV EMQX_VERSION=5.0.23
# Tue, 18 Apr 2023 19:23:44 GMT
ENV AMD64_SHA256=66322a18c2c1677d9ee07f44d06410d8b3914782f7b56dceb67c44ab946bc8bd
# Tue, 18 Apr 2023 19:23:44 GMT
ENV ARM64_SHA256=74c0f096fbd8b480f79b45918de83148ba0c1defcf997f268557ed27f85d9159
# Tue, 18 Apr 2023 19:23:44 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 18 Apr 2023 19:23:51 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 18 Apr 2023 19:23:51 GMT
WORKDIR /opt/emqx
# Tue, 18 Apr 2023 19:23:51 GMT
USER emqx
# Tue, 18 Apr 2023 19:23:51 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 18 Apr 2023 19:23:52 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 18 Apr 2023 19:23:52 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 18 Apr 2023 19:23:52 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 19:23:52 GMT
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
	-	`sha256:0ce2d792f43e68e6f144aad7a024ec68c528c45f63e1e46075ce51f13488b832`  
		Last Modified: Tue, 18 Apr 2023 19:24:27 GMT  
		Size: 76.7 MB (76666377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8af10bdd33f36ef136f5ef915af25bde6c0a0dd652ac95b6ec3c6bbb88524d7`  
		Last Modified: Tue, 18 Apr 2023 19:24:17 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:b20b0908ec021f4ec179fd55b0b1fd1ad2573dfa23b060e333fb695394a561ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102157787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7bae0c81f826ed909247451fba3ee3518fb415381812dcbbf2209b9d24d3795`
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
# Tue, 18 Apr 2023 18:39:29 GMT
ENV EMQX_VERSION=5.0.23
# Tue, 18 Apr 2023 18:39:29 GMT
ENV AMD64_SHA256=66322a18c2c1677d9ee07f44d06410d8b3914782f7b56dceb67c44ab946bc8bd
# Tue, 18 Apr 2023 18:39:29 GMT
ENV ARM64_SHA256=74c0f096fbd8b480f79b45918de83148ba0c1defcf997f268557ed27f85d9159
# Tue, 18 Apr 2023 18:39:29 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 18 Apr 2023 18:39:34 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 18 Apr 2023 18:39:35 GMT
WORKDIR /opt/emqx
# Tue, 18 Apr 2023 18:39:35 GMT
USER emqx
# Tue, 18 Apr 2023 18:39:35 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 18 Apr 2023 18:39:35 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 18 Apr 2023 18:39:35 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 18 Apr 2023 18:39:36 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 18:39:36 GMT
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
	-	`sha256:81826c36e478507e264f8473188bd6a67787268ae42d90ed3468e89afd28f271`  
		Last Modified: Tue, 18 Apr 2023 18:40:06 GMT  
		Size: 69.1 MB (69086004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb58189c390f19b6def2d0a892c2211334d48973166ef7574b3ccb3e5f1f24f0`  
		Last Modified: Tue, 18 Apr 2023 18:39:59 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.23`

```console
$ docker pull emqx@sha256:386cabf97b0cbf3fde558b08a4d4fb27d02da66a530937ab9f13661e2a48c671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0.23` - linux; amd64

```console
$ docker pull emqx@sha256:12e2463b0de9fe52971a2584364e2c9b304474670813cdf24b0c8a5ef67d6121
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.1 MB (111077435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd1fc2469f25a8b9a360f6b9875686f5951073b1c64aa22cc09d5ed87c4b81f8`
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
# Tue, 18 Apr 2023 19:23:44 GMT
ENV EMQX_VERSION=5.0.23
# Tue, 18 Apr 2023 19:23:44 GMT
ENV AMD64_SHA256=66322a18c2c1677d9ee07f44d06410d8b3914782f7b56dceb67c44ab946bc8bd
# Tue, 18 Apr 2023 19:23:44 GMT
ENV ARM64_SHA256=74c0f096fbd8b480f79b45918de83148ba0c1defcf997f268557ed27f85d9159
# Tue, 18 Apr 2023 19:23:44 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 18 Apr 2023 19:23:51 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 18 Apr 2023 19:23:51 GMT
WORKDIR /opt/emqx
# Tue, 18 Apr 2023 19:23:51 GMT
USER emqx
# Tue, 18 Apr 2023 19:23:51 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 18 Apr 2023 19:23:52 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 18 Apr 2023 19:23:52 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 18 Apr 2023 19:23:52 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 19:23:52 GMT
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
	-	`sha256:0ce2d792f43e68e6f144aad7a024ec68c528c45f63e1e46075ce51f13488b832`  
		Last Modified: Tue, 18 Apr 2023 19:24:27 GMT  
		Size: 76.7 MB (76666377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8af10bdd33f36ef136f5ef915af25bde6c0a0dd652ac95b6ec3c6bbb88524d7`  
		Last Modified: Tue, 18 Apr 2023 19:24:17 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0.23` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:b20b0908ec021f4ec179fd55b0b1fd1ad2573dfa23b060e333fb695394a561ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102157787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7bae0c81f826ed909247451fba3ee3518fb415381812dcbbf2209b9d24d3795`
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
# Tue, 18 Apr 2023 18:39:29 GMT
ENV EMQX_VERSION=5.0.23
# Tue, 18 Apr 2023 18:39:29 GMT
ENV AMD64_SHA256=66322a18c2c1677d9ee07f44d06410d8b3914782f7b56dceb67c44ab946bc8bd
# Tue, 18 Apr 2023 18:39:29 GMT
ENV ARM64_SHA256=74c0f096fbd8b480f79b45918de83148ba0c1defcf997f268557ed27f85d9159
# Tue, 18 Apr 2023 18:39:29 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 18 Apr 2023 18:39:34 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 18 Apr 2023 18:39:35 GMT
WORKDIR /opt/emqx
# Tue, 18 Apr 2023 18:39:35 GMT
USER emqx
# Tue, 18 Apr 2023 18:39:35 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 18 Apr 2023 18:39:35 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 18 Apr 2023 18:39:35 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 18 Apr 2023 18:39:36 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 18:39:36 GMT
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
	-	`sha256:81826c36e478507e264f8473188bd6a67787268ae42d90ed3468e89afd28f271`  
		Last Modified: Tue, 18 Apr 2023 18:40:06 GMT  
		Size: 69.1 MB (69086004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb58189c390f19b6def2d0a892c2211334d48973166ef7574b3ccb3e5f1f24f0`  
		Last Modified: Tue, 18 Apr 2023 18:39:59 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:386cabf97b0cbf3fde558b08a4d4fb27d02da66a530937ab9f13661e2a48c671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:12e2463b0de9fe52971a2584364e2c9b304474670813cdf24b0c8a5ef67d6121
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.1 MB (111077435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd1fc2469f25a8b9a360f6b9875686f5951073b1c64aa22cc09d5ed87c4b81f8`
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
# Tue, 18 Apr 2023 19:23:44 GMT
ENV EMQX_VERSION=5.0.23
# Tue, 18 Apr 2023 19:23:44 GMT
ENV AMD64_SHA256=66322a18c2c1677d9ee07f44d06410d8b3914782f7b56dceb67c44ab946bc8bd
# Tue, 18 Apr 2023 19:23:44 GMT
ENV ARM64_SHA256=74c0f096fbd8b480f79b45918de83148ba0c1defcf997f268557ed27f85d9159
# Tue, 18 Apr 2023 19:23:44 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 18 Apr 2023 19:23:51 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 18 Apr 2023 19:23:51 GMT
WORKDIR /opt/emqx
# Tue, 18 Apr 2023 19:23:51 GMT
USER emqx
# Tue, 18 Apr 2023 19:23:51 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 18 Apr 2023 19:23:52 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 18 Apr 2023 19:23:52 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 18 Apr 2023 19:23:52 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 19:23:52 GMT
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
	-	`sha256:0ce2d792f43e68e6f144aad7a024ec68c528c45f63e1e46075ce51f13488b832`  
		Last Modified: Tue, 18 Apr 2023 19:24:27 GMT  
		Size: 76.7 MB (76666377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8af10bdd33f36ef136f5ef915af25bde6c0a0dd652ac95b6ec3c6bbb88524d7`  
		Last Modified: Tue, 18 Apr 2023 19:24:17 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:b20b0908ec021f4ec179fd55b0b1fd1ad2573dfa23b060e333fb695394a561ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102157787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7bae0c81f826ed909247451fba3ee3518fb415381812dcbbf2209b9d24d3795`
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
# Tue, 18 Apr 2023 18:39:29 GMT
ENV EMQX_VERSION=5.0.23
# Tue, 18 Apr 2023 18:39:29 GMT
ENV AMD64_SHA256=66322a18c2c1677d9ee07f44d06410d8b3914782f7b56dceb67c44ab946bc8bd
# Tue, 18 Apr 2023 18:39:29 GMT
ENV ARM64_SHA256=74c0f096fbd8b480f79b45918de83148ba0c1defcf997f268557ed27f85d9159
# Tue, 18 Apr 2023 18:39:29 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 18 Apr 2023 18:39:34 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 18 Apr 2023 18:39:35 GMT
WORKDIR /opt/emqx
# Tue, 18 Apr 2023 18:39:35 GMT
USER emqx
# Tue, 18 Apr 2023 18:39:35 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 18 Apr 2023 18:39:35 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 18 Apr 2023 18:39:35 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 18 Apr 2023 18:39:36 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 18:39:36 GMT
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
	-	`sha256:81826c36e478507e264f8473188bd6a67787268ae42d90ed3468e89afd28f271`  
		Last Modified: Tue, 18 Apr 2023 18:40:06 GMT  
		Size: 69.1 MB (69086004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb58189c390f19b6def2d0a892c2211334d48973166ef7574b3ccb3e5f1f24f0`  
		Last Modified: Tue, 18 Apr 2023 18:39:59 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
