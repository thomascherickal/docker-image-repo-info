<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `emqx`

-	[`emqx:4`](#emqx4)
-	[`emqx:4.3`](#emqx43)
-	[`emqx:4.3.22`](#emqx4322)
-	[`emqx:4.4`](#emqx44)
-	[`emqx:4.4.11`](#emqx4411)
-	[`emqx:5`](#emqx5)
-	[`emqx:5.0`](#emqx50)
-	[`emqx:5.0.12`](#emqx5012)
-	[`emqx:latest`](#emqxlatest)

## `emqx:4`

```console
$ docker pull emqx@sha256:4d3d6dcc2e315b40e357a060a7bc349232ae2f6e4c5954e11b750ac5acfa8350
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:2d23dcc574f9f82154d041a3c9c213f4a7aac829887c5f5104108d4f5b07dee7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127238717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bd4b6b7c15dd9777f6d2732b818378ba7e4ac8551f8c4341e9540def0d6b71e`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:03:51 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:03:51 GMT
ENV EMQX_VERSION=4.4.11
# Tue, 06 Dec 2022 04:03:51 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 06 Dec 2022 04:03:55 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="652fb25a2a5c9d4e9fc029a4094d39c5bd824c78ad77361fb5fee09a940209a6"; fi;     if [ ${arch} = "arm64" ]; then sha256="6532a0f93fe8ce419633142b376107f3d7a2a79df24ce95551026b9e144a77b8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 06 Dec 2022 04:04:01 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 06 Dec 2022 04:04:02 GMT
WORKDIR /opt/emqx
# Tue, 06 Dec 2022 04:04:02 GMT
USER emqx
# Tue, 06 Dec 2022 04:04:02 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 06 Dec 2022 04:04:02 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 06 Dec 2022 04:04:02 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 06 Dec 2022 04:04:02 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 04:04:02 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3078ffce5d90ff48d82f12269ab8ab64696808bbda5c548acf2699549e57a18`  
		Last Modified: Tue, 06 Dec 2022 04:04:58 GMT  
		Size: 2.6 MB (2571021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00655aeabee69f96756e1946695715aa34d796b40f41401330e62d17227c9720`  
		Last Modified: Tue, 06 Dec 2022 04:05:04 GMT  
		Size: 46.6 MB (46617891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364a34fe9ad4c37e86ba5473a44e9725a3824ca572a8dcb1acb710672aedd0cd`  
		Last Modified: Tue, 06 Dec 2022 04:05:05 GMT  
		Size: 46.6 MB (46635847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fe2652ab31a61b2b21678e07b447848a4114f8483e7fbf17883634f5ea9684`  
		Last Modified: Tue, 06 Dec 2022 04:04:58 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:67675a2c216789b3a51242a69512d7db155ea47571a09ebbc85970b2c9471d75
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111434952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9346d27a125dd180251ad4c0e12ad2f874d2c968059c93b90abf5bea20ba5e6`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 10:50:48 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 10:50:48 GMT
ENV EMQX_VERSION=4.4.11
# Tue, 06 Dec 2022 10:50:48 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 06 Dec 2022 10:50:52 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="652fb25a2a5c9d4e9fc029a4094d39c5bd824c78ad77361fb5fee09a940209a6"; fi;     if [ ${arch} = "arm64" ]; then sha256="6532a0f93fe8ce419633142b376107f3d7a2a79df24ce95551026b9e144a77b8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 06 Dec 2022 10:50:56 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 06 Dec 2022 10:50:56 GMT
WORKDIR /opt/emqx
# Tue, 06 Dec 2022 10:50:56 GMT
USER emqx
# Tue, 06 Dec 2022 10:50:57 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 06 Dec 2022 10:50:57 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 06 Dec 2022 10:50:57 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 06 Dec 2022 10:50:57 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 10:50:57 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dd4ed429be35aed2457dbc8c8da2f237c01ef481f19f1cd6b089b9948530d9`  
		Last Modified: Tue, 06 Dec 2022 10:51:43 GMT  
		Size: 2.6 MB (2560826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96dffc0b180cdc87ae28659646c41c7f3ba6a2b14814a125399517db0db95f27`  
		Last Modified: Tue, 06 Dec 2022 10:51:46 GMT  
		Size: 39.4 MB (39403613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c22531680b9e27e8bcbeb908895d52134a2fdd21d696e93730bf963350ea103`  
		Last Modified: Tue, 06 Dec 2022 10:51:46 GMT  
		Size: 39.4 MB (39409086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8edd7a33f67f2fd65e016a37f56724d539d81e7bf4bd11ccf692f0ed22348a25`  
		Last Modified: Tue, 06 Dec 2022 10:51:43 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3`

```console
$ docker pull emqx@sha256:b62bb161dc2efb7b54bd999942326d45d6ad1e1746084407ac0540c243efe089
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.3` - linux; amd64

```console
$ docker pull emqx@sha256:e9de1f4db098d54c04857658afed662a614ff9776a07f43b39a3b691481fecf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.8 MB (104828560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdcf4ecf3c036cc8186e6c130d3e287718ee121e27c60f4a16528ce2d12f4ef3`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:18 GMT
ADD file:30180333dcb9028c0d2776f05042f6f309238b100863a050f3981fb80604e871 in / 
# Tue, 06 Dec 2022 01:21:18 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:03:28 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:03:28 GMT
ENV EMQX_VERSION=4.3.22
# Tue, 06 Dec 2022 04:03:32 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 06 Dec 2022 04:03:38 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 06 Dec 2022 04:03:39 GMT
WORKDIR /opt/emqx
# Tue, 06 Dec 2022 04:03:39 GMT
USER emqx
# Tue, 06 Dec 2022 04:03:39 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 06 Dec 2022 04:03:39 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 06 Dec 2022 04:03:39 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Tue, 06 Dec 2022 04:03:39 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 04:03:39 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:6eab20599fab240a56b06125a77b4921dd39662d3b9f9008da7306531772a1d0`  
		Last Modified: Tue, 06 Dec 2022 01:25:52 GMT  
		Size: 27.1 MB (27140356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9efc79d145ca2cbe713f132cf4472673fb9801bf19d6b4c2fee21fcd7fd4cc33`  
		Last Modified: Tue, 06 Dec 2022 04:04:46 GMT  
		Size: 4.6 MB (4612576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d36f1157ff83e8657409c76b60a35bb2c8240b84728d3beb776b3feb4bac01`  
		Last Modified: Tue, 06 Dec 2022 04:04:50 GMT  
		Size: 36.5 MB (36537227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a1f4aac9aa65875cf351f9feff18afa0bbaf72ec947c707b0bf7511d79f572`  
		Last Modified: Tue, 06 Dec 2022 04:04:50 GMT  
		Size: 36.5 MB (36537362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34029b6a8c1be3b40f57100eca203020d4d599de74b8f1f14fe817c945d92892`  
		Last Modified: Tue, 06 Dec 2022 04:04:45 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.3` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:3a5a4a084ecc62e0fb5f7c459ca72cec9375607223957da50ca8c8b53666990d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102846240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a8f4e6e449e94bff6adb678bf0b25a12b040f8f77abce5f1deaca8e33761c68`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:34 GMT
ADD file:764288ad3920160093c500e1a7277f174a656030bbe3a0511e7925e84495b6ee in / 
# Tue, 06 Dec 2022 01:40:34 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 10:50:26 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 10:50:27 GMT
ENV EMQX_VERSION=4.3.22
# Tue, 06 Dec 2022 10:50:36 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 06 Dec 2022 10:50:40 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 06 Dec 2022 10:50:40 GMT
WORKDIR /opt/emqx
# Tue, 06 Dec 2022 10:50:40 GMT
USER emqx
# Tue, 06 Dec 2022 10:50:40 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 06 Dec 2022 10:50:40 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 06 Dec 2022 10:50:41 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Tue, 06 Dec 2022 10:50:41 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 10:50:41 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:b473b36a3d93c888196b326b1aad1f802bb6a9fa6fcbc5d2614d99a67899d587`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 25.9 MB (25914951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4403961cfc514c0343fbfb3ee762d1bdfc953a715a86ecffa257e3fc565196`  
		Last Modified: Tue, 06 Dec 2022 10:51:32 GMT  
		Size: 4.5 MB (4490421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a709e473aee986ed24401282037a29c69b76bbb3b623572103ebc70425c3bde`  
		Last Modified: Tue, 06 Dec 2022 10:51:35 GMT  
		Size: 36.2 MB (36216035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7176579f33ec21d804f0d40e97d79b0be6b6bdaa3f006020dcab2dd2439c6b62`  
		Last Modified: Tue, 06 Dec 2022 10:51:35 GMT  
		Size: 36.2 MB (36223794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71de9682c65dcd9565cdc072bfffea1c5f2b48b41a1e48b02658332fea24015d`  
		Last Modified: Tue, 06 Dec 2022 10:51:31 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3.22`

```console
$ docker pull emqx@sha256:b62bb161dc2efb7b54bd999942326d45d6ad1e1746084407ac0540c243efe089
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.3.22` - linux; amd64

```console
$ docker pull emqx@sha256:e9de1f4db098d54c04857658afed662a614ff9776a07f43b39a3b691481fecf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.8 MB (104828560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdcf4ecf3c036cc8186e6c130d3e287718ee121e27c60f4a16528ce2d12f4ef3`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:18 GMT
ADD file:30180333dcb9028c0d2776f05042f6f309238b100863a050f3981fb80604e871 in / 
# Tue, 06 Dec 2022 01:21:18 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:03:28 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:03:28 GMT
ENV EMQX_VERSION=4.3.22
# Tue, 06 Dec 2022 04:03:32 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 06 Dec 2022 04:03:38 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 06 Dec 2022 04:03:39 GMT
WORKDIR /opt/emqx
# Tue, 06 Dec 2022 04:03:39 GMT
USER emqx
# Tue, 06 Dec 2022 04:03:39 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 06 Dec 2022 04:03:39 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 06 Dec 2022 04:03:39 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Tue, 06 Dec 2022 04:03:39 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 04:03:39 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:6eab20599fab240a56b06125a77b4921dd39662d3b9f9008da7306531772a1d0`  
		Last Modified: Tue, 06 Dec 2022 01:25:52 GMT  
		Size: 27.1 MB (27140356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9efc79d145ca2cbe713f132cf4472673fb9801bf19d6b4c2fee21fcd7fd4cc33`  
		Last Modified: Tue, 06 Dec 2022 04:04:46 GMT  
		Size: 4.6 MB (4612576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d36f1157ff83e8657409c76b60a35bb2c8240b84728d3beb776b3feb4bac01`  
		Last Modified: Tue, 06 Dec 2022 04:04:50 GMT  
		Size: 36.5 MB (36537227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a1f4aac9aa65875cf351f9feff18afa0bbaf72ec947c707b0bf7511d79f572`  
		Last Modified: Tue, 06 Dec 2022 04:04:50 GMT  
		Size: 36.5 MB (36537362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34029b6a8c1be3b40f57100eca203020d4d599de74b8f1f14fe817c945d92892`  
		Last Modified: Tue, 06 Dec 2022 04:04:45 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.3.22` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:3a5a4a084ecc62e0fb5f7c459ca72cec9375607223957da50ca8c8b53666990d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102846240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a8f4e6e449e94bff6adb678bf0b25a12b040f8f77abce5f1deaca8e33761c68`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:34 GMT
ADD file:764288ad3920160093c500e1a7277f174a656030bbe3a0511e7925e84495b6ee in / 
# Tue, 06 Dec 2022 01:40:34 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 10:50:26 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 10:50:27 GMT
ENV EMQX_VERSION=4.3.22
# Tue, 06 Dec 2022 10:50:36 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 06 Dec 2022 10:50:40 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 06 Dec 2022 10:50:40 GMT
WORKDIR /opt/emqx
# Tue, 06 Dec 2022 10:50:40 GMT
USER emqx
# Tue, 06 Dec 2022 10:50:40 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 06 Dec 2022 10:50:40 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 06 Dec 2022 10:50:41 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Tue, 06 Dec 2022 10:50:41 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 10:50:41 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:b473b36a3d93c888196b326b1aad1f802bb6a9fa6fcbc5d2614d99a67899d587`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 25.9 MB (25914951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4403961cfc514c0343fbfb3ee762d1bdfc953a715a86ecffa257e3fc565196`  
		Last Modified: Tue, 06 Dec 2022 10:51:32 GMT  
		Size: 4.5 MB (4490421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a709e473aee986ed24401282037a29c69b76bbb3b623572103ebc70425c3bde`  
		Last Modified: Tue, 06 Dec 2022 10:51:35 GMT  
		Size: 36.2 MB (36216035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7176579f33ec21d804f0d40e97d79b0be6b6bdaa3f006020dcab2dd2439c6b62`  
		Last Modified: Tue, 06 Dec 2022 10:51:35 GMT  
		Size: 36.2 MB (36223794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71de9682c65dcd9565cdc072bfffea1c5f2b48b41a1e48b02658332fea24015d`  
		Last Modified: Tue, 06 Dec 2022 10:51:31 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:4d3d6dcc2e315b40e357a060a7bc349232ae2f6e4c5954e11b750ac5acfa8350
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:2d23dcc574f9f82154d041a3c9c213f4a7aac829887c5f5104108d4f5b07dee7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127238717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bd4b6b7c15dd9777f6d2732b818378ba7e4ac8551f8c4341e9540def0d6b71e`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:03:51 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:03:51 GMT
ENV EMQX_VERSION=4.4.11
# Tue, 06 Dec 2022 04:03:51 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 06 Dec 2022 04:03:55 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="652fb25a2a5c9d4e9fc029a4094d39c5bd824c78ad77361fb5fee09a940209a6"; fi;     if [ ${arch} = "arm64" ]; then sha256="6532a0f93fe8ce419633142b376107f3d7a2a79df24ce95551026b9e144a77b8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 06 Dec 2022 04:04:01 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 06 Dec 2022 04:04:02 GMT
WORKDIR /opt/emqx
# Tue, 06 Dec 2022 04:04:02 GMT
USER emqx
# Tue, 06 Dec 2022 04:04:02 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 06 Dec 2022 04:04:02 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 06 Dec 2022 04:04:02 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 06 Dec 2022 04:04:02 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 04:04:02 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3078ffce5d90ff48d82f12269ab8ab64696808bbda5c548acf2699549e57a18`  
		Last Modified: Tue, 06 Dec 2022 04:04:58 GMT  
		Size: 2.6 MB (2571021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00655aeabee69f96756e1946695715aa34d796b40f41401330e62d17227c9720`  
		Last Modified: Tue, 06 Dec 2022 04:05:04 GMT  
		Size: 46.6 MB (46617891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364a34fe9ad4c37e86ba5473a44e9725a3824ca572a8dcb1acb710672aedd0cd`  
		Last Modified: Tue, 06 Dec 2022 04:05:05 GMT  
		Size: 46.6 MB (46635847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fe2652ab31a61b2b21678e07b447848a4114f8483e7fbf17883634f5ea9684`  
		Last Modified: Tue, 06 Dec 2022 04:04:58 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:67675a2c216789b3a51242a69512d7db155ea47571a09ebbc85970b2c9471d75
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111434952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9346d27a125dd180251ad4c0e12ad2f874d2c968059c93b90abf5bea20ba5e6`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 10:50:48 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 10:50:48 GMT
ENV EMQX_VERSION=4.4.11
# Tue, 06 Dec 2022 10:50:48 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 06 Dec 2022 10:50:52 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="652fb25a2a5c9d4e9fc029a4094d39c5bd824c78ad77361fb5fee09a940209a6"; fi;     if [ ${arch} = "arm64" ]; then sha256="6532a0f93fe8ce419633142b376107f3d7a2a79df24ce95551026b9e144a77b8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 06 Dec 2022 10:50:56 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 06 Dec 2022 10:50:56 GMT
WORKDIR /opt/emqx
# Tue, 06 Dec 2022 10:50:56 GMT
USER emqx
# Tue, 06 Dec 2022 10:50:57 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 06 Dec 2022 10:50:57 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 06 Dec 2022 10:50:57 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 06 Dec 2022 10:50:57 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 10:50:57 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dd4ed429be35aed2457dbc8c8da2f237c01ef481f19f1cd6b089b9948530d9`  
		Last Modified: Tue, 06 Dec 2022 10:51:43 GMT  
		Size: 2.6 MB (2560826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96dffc0b180cdc87ae28659646c41c7f3ba6a2b14814a125399517db0db95f27`  
		Last Modified: Tue, 06 Dec 2022 10:51:46 GMT  
		Size: 39.4 MB (39403613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c22531680b9e27e8bcbeb908895d52134a2fdd21d696e93730bf963350ea103`  
		Last Modified: Tue, 06 Dec 2022 10:51:46 GMT  
		Size: 39.4 MB (39409086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8edd7a33f67f2fd65e016a37f56724d539d81e7bf4bd11ccf692f0ed22348a25`  
		Last Modified: Tue, 06 Dec 2022 10:51:43 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.11`

```console
$ docker pull emqx@sha256:4d3d6dcc2e315b40e357a060a7bc349232ae2f6e4c5954e11b750ac5acfa8350
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4.11` - linux; amd64

```console
$ docker pull emqx@sha256:2d23dcc574f9f82154d041a3c9c213f4a7aac829887c5f5104108d4f5b07dee7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127238717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bd4b6b7c15dd9777f6d2732b818378ba7e4ac8551f8c4341e9540def0d6b71e`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:03:51 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:03:51 GMT
ENV EMQX_VERSION=4.4.11
# Tue, 06 Dec 2022 04:03:51 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 06 Dec 2022 04:03:55 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="652fb25a2a5c9d4e9fc029a4094d39c5bd824c78ad77361fb5fee09a940209a6"; fi;     if [ ${arch} = "arm64" ]; then sha256="6532a0f93fe8ce419633142b376107f3d7a2a79df24ce95551026b9e144a77b8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 06 Dec 2022 04:04:01 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 06 Dec 2022 04:04:02 GMT
WORKDIR /opt/emqx
# Tue, 06 Dec 2022 04:04:02 GMT
USER emqx
# Tue, 06 Dec 2022 04:04:02 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 06 Dec 2022 04:04:02 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 06 Dec 2022 04:04:02 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 06 Dec 2022 04:04:02 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 04:04:02 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3078ffce5d90ff48d82f12269ab8ab64696808bbda5c548acf2699549e57a18`  
		Last Modified: Tue, 06 Dec 2022 04:04:58 GMT  
		Size: 2.6 MB (2571021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00655aeabee69f96756e1946695715aa34d796b40f41401330e62d17227c9720`  
		Last Modified: Tue, 06 Dec 2022 04:05:04 GMT  
		Size: 46.6 MB (46617891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364a34fe9ad4c37e86ba5473a44e9725a3824ca572a8dcb1acb710672aedd0cd`  
		Last Modified: Tue, 06 Dec 2022 04:05:05 GMT  
		Size: 46.6 MB (46635847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fe2652ab31a61b2b21678e07b447848a4114f8483e7fbf17883634f5ea9684`  
		Last Modified: Tue, 06 Dec 2022 04:04:58 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4.11` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:67675a2c216789b3a51242a69512d7db155ea47571a09ebbc85970b2c9471d75
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111434952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9346d27a125dd180251ad4c0e12ad2f874d2c968059c93b90abf5bea20ba5e6`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 10:50:48 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 10:50:48 GMT
ENV EMQX_VERSION=4.4.11
# Tue, 06 Dec 2022 10:50:48 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 06 Dec 2022 10:50:52 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="652fb25a2a5c9d4e9fc029a4094d39c5bd824c78ad77361fb5fee09a940209a6"; fi;     if [ ${arch} = "arm64" ]; then sha256="6532a0f93fe8ce419633142b376107f3d7a2a79df24ce95551026b9e144a77b8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 06 Dec 2022 10:50:56 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 06 Dec 2022 10:50:56 GMT
WORKDIR /opt/emqx
# Tue, 06 Dec 2022 10:50:56 GMT
USER emqx
# Tue, 06 Dec 2022 10:50:57 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 06 Dec 2022 10:50:57 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 06 Dec 2022 10:50:57 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 06 Dec 2022 10:50:57 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 10:50:57 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dd4ed429be35aed2457dbc8c8da2f237c01ef481f19f1cd6b089b9948530d9`  
		Last Modified: Tue, 06 Dec 2022 10:51:43 GMT  
		Size: 2.6 MB (2560826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96dffc0b180cdc87ae28659646c41c7f3ba6a2b14814a125399517db0db95f27`  
		Last Modified: Tue, 06 Dec 2022 10:51:46 GMT  
		Size: 39.4 MB (39403613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c22531680b9e27e8bcbeb908895d52134a2fdd21d696e93730bf963350ea103`  
		Last Modified: Tue, 06 Dec 2022 10:51:46 GMT  
		Size: 39.4 MB (39409086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8edd7a33f67f2fd65e016a37f56724d539d81e7bf4bd11ccf692f0ed22348a25`  
		Last Modified: Tue, 06 Dec 2022 10:51:43 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5`

```console
$ docker pull emqx@sha256:5fd23424e47c38bbeda099da995af702ffd718b8d5bff67468976429a819f06a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:195b3c618454faa76d6f5029b0881bb36a7f9e2e8323db8cbdf95d125dfea4ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.1 MB (100081734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cedbe39026299ae846576795162dcfe1df7723be15fd45291faa0d0676d57ad8`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:04:14 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 15 Dec 2022 18:25:47 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 15 Dec 2022 18:25:47 GMT
ENV EMQX_VERSION=5.0.12
# Thu, 15 Dec 2022 18:25:47 GMT
ENV AMD64_SHA256=c137284b389c472f3c2563bc89c8016f5ce9bdb0acf820014afcbbb26a0e81e7
# Thu, 15 Dec 2022 18:25:47 GMT
ENV ARM64_SHA256=5925bb5462d6f163b829c2f1e6490dc5a46e445b5b15c268482bb7310a95f7c4
# Thu, 15 Dec 2022 18:25:47 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 15 Dec 2022 18:25:54 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 15 Dec 2022 18:25:54 GMT
WORKDIR /opt/emqx
# Thu, 15 Dec 2022 18:25:55 GMT
USER emqx
# Thu, 15 Dec 2022 18:25:55 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 15 Dec 2022 18:25:55 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 15 Dec 2022 18:25:55 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 15 Dec 2022 18:25:55 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 15 Dec 2022 18:25:55 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29e5e20fa16580fcb41964870e6c9d3d48072cc1abdbe98fe1645a15c65e9ec`  
		Last Modified: Tue, 06 Dec 2022 04:05:16 GMT  
		Size: 3.0 MB (2988935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca86891f342dfb918e69e1d9909f9489c716b4a0630d00eda5b7da3f0a6faa5`  
		Last Modified: Thu, 15 Dec 2022 18:26:14 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f6fe23c2dfc1f380e42d68c9d8b4d65d15c575ff56f417418c8026e5064b4d`  
		Last Modified: Thu, 15 Dec 2022 18:26:21 GMT  
		Size: 65.7 MB (65674930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c672a158b261dc7c7cccce4017aa3b1a59a62e8d94e72c5e1762340198a9a7`  
		Last Modified: Thu, 15 Dec 2022 18:26:14 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:ff42c1d34ff7bc2546e9533755afb5346971443964d2105bd0a412affb8e7c06
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.8 MB (147767024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0bf741af4a3cb7568ee0a2901b493ba51354c94de68beb92d06e3e6bc97e5a8`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 10:51:04 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 10:51:04 GMT
ENV EMQX_VERSION=5.0.11
# Tue, 06 Dec 2022 10:51:04 GMT
ENV AMD64_SHA256=68609fcc1d74be917f9c28c57c14daabccee22361af91b6e98812a35300a1c80
# Tue, 06 Dec 2022 10:51:04 GMT
ENV ARM64_SHA256=f7c7417951beb490ed3a7347b3879db8e9e80ea214c9ef942e777c7136681d31
# Tue, 06 Dec 2022 10:51:05 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 06 Dec 2022 10:51:09 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Tue, 06 Dec 2022 10:51:09 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 06 Dec 2022 10:51:09 GMT
WORKDIR /opt/emqx
# Tue, 06 Dec 2022 10:51:14 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 06 Dec 2022 10:51:14 GMT
USER emqx
# Tue, 06 Dec 2022 10:51:14 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 06 Dec 2022 10:51:15 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 06 Dec 2022 10:51:15 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 10:51:15 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0384cd65a949b2d9a9f07a689377a09c1c0180066afbebd1aec5b7a8ff60655d`  
		Last Modified: Tue, 06 Dec 2022 10:51:56 GMT  
		Size: 3.0 MB (3004192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9cc25503198e3e8751ac2fab811ff7ec5016530c3d0831de39629cd82a7883`  
		Last Modified: Tue, 06 Dec 2022 10:52:02 GMT  
		Size: 57.3 MB (57348552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4bcb2bff5ab040d41282cf08712f8ab3cf03d6802309182711c26ccc029a9b`  
		Last Modified: Tue, 06 Dec 2022 10:51:56 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36441e61b498fd1d2bab1938dbd755c69c1b8171dff2c56e831d9c472a5e3fc3`  
		Last Modified: Tue, 06 Dec 2022 10:52:02 GMT  
		Size: 57.4 MB (57353058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:5fd23424e47c38bbeda099da995af702ffd718b8d5bff67468976429a819f06a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:195b3c618454faa76d6f5029b0881bb36a7f9e2e8323db8cbdf95d125dfea4ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.1 MB (100081734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cedbe39026299ae846576795162dcfe1df7723be15fd45291faa0d0676d57ad8`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:04:14 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 15 Dec 2022 18:25:47 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 15 Dec 2022 18:25:47 GMT
ENV EMQX_VERSION=5.0.12
# Thu, 15 Dec 2022 18:25:47 GMT
ENV AMD64_SHA256=c137284b389c472f3c2563bc89c8016f5ce9bdb0acf820014afcbbb26a0e81e7
# Thu, 15 Dec 2022 18:25:47 GMT
ENV ARM64_SHA256=5925bb5462d6f163b829c2f1e6490dc5a46e445b5b15c268482bb7310a95f7c4
# Thu, 15 Dec 2022 18:25:47 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 15 Dec 2022 18:25:54 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 15 Dec 2022 18:25:54 GMT
WORKDIR /opt/emqx
# Thu, 15 Dec 2022 18:25:55 GMT
USER emqx
# Thu, 15 Dec 2022 18:25:55 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 15 Dec 2022 18:25:55 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 15 Dec 2022 18:25:55 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 15 Dec 2022 18:25:55 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 15 Dec 2022 18:25:55 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29e5e20fa16580fcb41964870e6c9d3d48072cc1abdbe98fe1645a15c65e9ec`  
		Last Modified: Tue, 06 Dec 2022 04:05:16 GMT  
		Size: 3.0 MB (2988935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca86891f342dfb918e69e1d9909f9489c716b4a0630d00eda5b7da3f0a6faa5`  
		Last Modified: Thu, 15 Dec 2022 18:26:14 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f6fe23c2dfc1f380e42d68c9d8b4d65d15c575ff56f417418c8026e5064b4d`  
		Last Modified: Thu, 15 Dec 2022 18:26:21 GMT  
		Size: 65.7 MB (65674930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c672a158b261dc7c7cccce4017aa3b1a59a62e8d94e72c5e1762340198a9a7`  
		Last Modified: Thu, 15 Dec 2022 18:26:14 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:ff42c1d34ff7bc2546e9533755afb5346971443964d2105bd0a412affb8e7c06
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.8 MB (147767024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0bf741af4a3cb7568ee0a2901b493ba51354c94de68beb92d06e3e6bc97e5a8`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 10:51:04 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 10:51:04 GMT
ENV EMQX_VERSION=5.0.11
# Tue, 06 Dec 2022 10:51:04 GMT
ENV AMD64_SHA256=68609fcc1d74be917f9c28c57c14daabccee22361af91b6e98812a35300a1c80
# Tue, 06 Dec 2022 10:51:04 GMT
ENV ARM64_SHA256=f7c7417951beb490ed3a7347b3879db8e9e80ea214c9ef942e777c7136681d31
# Tue, 06 Dec 2022 10:51:05 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 06 Dec 2022 10:51:09 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Tue, 06 Dec 2022 10:51:09 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 06 Dec 2022 10:51:09 GMT
WORKDIR /opt/emqx
# Tue, 06 Dec 2022 10:51:14 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 06 Dec 2022 10:51:14 GMT
USER emqx
# Tue, 06 Dec 2022 10:51:14 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 06 Dec 2022 10:51:15 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 06 Dec 2022 10:51:15 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 10:51:15 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0384cd65a949b2d9a9f07a689377a09c1c0180066afbebd1aec5b7a8ff60655d`  
		Last Modified: Tue, 06 Dec 2022 10:51:56 GMT  
		Size: 3.0 MB (3004192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9cc25503198e3e8751ac2fab811ff7ec5016530c3d0831de39629cd82a7883`  
		Last Modified: Tue, 06 Dec 2022 10:52:02 GMT  
		Size: 57.3 MB (57348552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4bcb2bff5ab040d41282cf08712f8ab3cf03d6802309182711c26ccc029a9b`  
		Last Modified: Tue, 06 Dec 2022 10:51:56 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36441e61b498fd1d2bab1938dbd755c69c1b8171dff2c56e831d9c472a5e3fc3`  
		Last Modified: Tue, 06 Dec 2022 10:52:02 GMT  
		Size: 57.4 MB (57353058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.12`

```console
$ docker pull emqx@sha256:4fb94d793933333e27fc2f0d24a3ff6953ad353816ddccf63401a2a63588da34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `emqx:5.0.12` - linux; amd64

```console
$ docker pull emqx@sha256:195b3c618454faa76d6f5029b0881bb36a7f9e2e8323db8cbdf95d125dfea4ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.1 MB (100081734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cedbe39026299ae846576795162dcfe1df7723be15fd45291faa0d0676d57ad8`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:04:14 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 15 Dec 2022 18:25:47 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 15 Dec 2022 18:25:47 GMT
ENV EMQX_VERSION=5.0.12
# Thu, 15 Dec 2022 18:25:47 GMT
ENV AMD64_SHA256=c137284b389c472f3c2563bc89c8016f5ce9bdb0acf820014afcbbb26a0e81e7
# Thu, 15 Dec 2022 18:25:47 GMT
ENV ARM64_SHA256=5925bb5462d6f163b829c2f1e6490dc5a46e445b5b15c268482bb7310a95f7c4
# Thu, 15 Dec 2022 18:25:47 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 15 Dec 2022 18:25:54 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 15 Dec 2022 18:25:54 GMT
WORKDIR /opt/emqx
# Thu, 15 Dec 2022 18:25:55 GMT
USER emqx
# Thu, 15 Dec 2022 18:25:55 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 15 Dec 2022 18:25:55 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 15 Dec 2022 18:25:55 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 15 Dec 2022 18:25:55 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 15 Dec 2022 18:25:55 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29e5e20fa16580fcb41964870e6c9d3d48072cc1abdbe98fe1645a15c65e9ec`  
		Last Modified: Tue, 06 Dec 2022 04:05:16 GMT  
		Size: 3.0 MB (2988935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca86891f342dfb918e69e1d9909f9489c716b4a0630d00eda5b7da3f0a6faa5`  
		Last Modified: Thu, 15 Dec 2022 18:26:14 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f6fe23c2dfc1f380e42d68c9d8b4d65d15c575ff56f417418c8026e5064b4d`  
		Last Modified: Thu, 15 Dec 2022 18:26:21 GMT  
		Size: 65.7 MB (65674930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c672a158b261dc7c7cccce4017aa3b1a59a62e8d94e72c5e1762340198a9a7`  
		Last Modified: Thu, 15 Dec 2022 18:26:14 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:5fd23424e47c38bbeda099da995af702ffd718b8d5bff67468976429a819f06a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:195b3c618454faa76d6f5029b0881bb36a7f9e2e8323db8cbdf95d125dfea4ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.1 MB (100081734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cedbe39026299ae846576795162dcfe1df7723be15fd45291faa0d0676d57ad8`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:04:14 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 15 Dec 2022 18:25:47 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 15 Dec 2022 18:25:47 GMT
ENV EMQX_VERSION=5.0.12
# Thu, 15 Dec 2022 18:25:47 GMT
ENV AMD64_SHA256=c137284b389c472f3c2563bc89c8016f5ce9bdb0acf820014afcbbb26a0e81e7
# Thu, 15 Dec 2022 18:25:47 GMT
ENV ARM64_SHA256=5925bb5462d6f163b829c2f1e6490dc5a46e445b5b15c268482bb7310a95f7c4
# Thu, 15 Dec 2022 18:25:47 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 15 Dec 2022 18:25:54 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 15 Dec 2022 18:25:54 GMT
WORKDIR /opt/emqx
# Thu, 15 Dec 2022 18:25:55 GMT
USER emqx
# Thu, 15 Dec 2022 18:25:55 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 15 Dec 2022 18:25:55 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 15 Dec 2022 18:25:55 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 15 Dec 2022 18:25:55 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 15 Dec 2022 18:25:55 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29e5e20fa16580fcb41964870e6c9d3d48072cc1abdbe98fe1645a15c65e9ec`  
		Last Modified: Tue, 06 Dec 2022 04:05:16 GMT  
		Size: 3.0 MB (2988935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca86891f342dfb918e69e1d9909f9489c716b4a0630d00eda5b7da3f0a6faa5`  
		Last Modified: Thu, 15 Dec 2022 18:26:14 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f6fe23c2dfc1f380e42d68c9d8b4d65d15c575ff56f417418c8026e5064b4d`  
		Last Modified: Thu, 15 Dec 2022 18:26:21 GMT  
		Size: 65.7 MB (65674930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c672a158b261dc7c7cccce4017aa3b1a59a62e8d94e72c5e1762340198a9a7`  
		Last Modified: Thu, 15 Dec 2022 18:26:14 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:ff42c1d34ff7bc2546e9533755afb5346971443964d2105bd0a412affb8e7c06
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.8 MB (147767024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0bf741af4a3cb7568ee0a2901b493ba51354c94de68beb92d06e3e6bc97e5a8`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 10:51:04 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 10:51:04 GMT
ENV EMQX_VERSION=5.0.11
# Tue, 06 Dec 2022 10:51:04 GMT
ENV AMD64_SHA256=68609fcc1d74be917f9c28c57c14daabccee22361af91b6e98812a35300a1c80
# Tue, 06 Dec 2022 10:51:04 GMT
ENV ARM64_SHA256=f7c7417951beb490ed3a7347b3879db8e9e80ea214c9ef942e777c7136681d31
# Tue, 06 Dec 2022 10:51:05 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 06 Dec 2022 10:51:09 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Tue, 06 Dec 2022 10:51:09 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 06 Dec 2022 10:51:09 GMT
WORKDIR /opt/emqx
# Tue, 06 Dec 2022 10:51:14 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 06 Dec 2022 10:51:14 GMT
USER emqx
# Tue, 06 Dec 2022 10:51:14 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 06 Dec 2022 10:51:15 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 06 Dec 2022 10:51:15 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 10:51:15 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0384cd65a949b2d9a9f07a689377a09c1c0180066afbebd1aec5b7a8ff60655d`  
		Last Modified: Tue, 06 Dec 2022 10:51:56 GMT  
		Size: 3.0 MB (3004192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9cc25503198e3e8751ac2fab811ff7ec5016530c3d0831de39629cd82a7883`  
		Last Modified: Tue, 06 Dec 2022 10:52:02 GMT  
		Size: 57.3 MB (57348552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4bcb2bff5ab040d41282cf08712f8ab3cf03d6802309182711c26ccc029a9b`  
		Last Modified: Tue, 06 Dec 2022 10:51:56 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36441e61b498fd1d2bab1938dbd755c69c1b8171dff2c56e831d9c472a5e3fc3`  
		Last Modified: Tue, 06 Dec 2022 10:52:02 GMT  
		Size: 57.4 MB (57353058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
