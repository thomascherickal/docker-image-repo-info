<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `emqx`

-	[`emqx:4`](#emqx4)
-	[`emqx:4.3`](#emqx43)
-	[`emqx:4.3.22`](#emqx4322)
-	[`emqx:4.4`](#emqx44)
-	[`emqx:4.4.14`](#emqx4414)
-	[`emqx:5`](#emqx5)
-	[`emqx:5.0`](#emqx50)
-	[`emqx:5.0.16`](#emqx5016)
-	[`emqx:latest`](#emqxlatest)

## `emqx:4`

```console
$ docker pull emqx@sha256:f37a823975d64ff16532a0f4040e2a5b24ed0f33c641a74f70d93f9511f7b8a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:694fec8a03aa7424cd8fc9ae19b70d863567fa18751d6908d3148f7b8edbc48a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81163520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e156deb9005fb2fc2d647f71d5986a4077805155a66566408e5a646ecc17dcc`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:48:56 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 19:22:14 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 12 Jan 2023 19:22:14 GMT
ENV EMQX_VERSION=4.4.14
# Thu, 12 Jan 2023 19:22:14 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 12 Jan 2023 19:22:19 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b70590c16effa60759f6ab08a4a0e666ad4487cf0eb88263ab992e44b440b815"; fi;     if [ ${arch} = "arm64" ]; then sha256="98b78798577ddb7685c42dc41b7a758aacfe27924c8be4510e2057527a142ba0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 12 Jan 2023 19:22:20 GMT
WORKDIR /opt/emqx
# Thu, 12 Jan 2023 19:22:20 GMT
USER emqx
# Thu, 12 Jan 2023 19:22:20 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 12 Jan 2023 19:22:20 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 12 Jan 2023 19:22:20 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 12 Jan 2023 19:22:20 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 12 Jan 2023 19:22:20 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d3e57ec5f70305a1554472a8bc80d1caf9263b899fdc9e84d30606e2e849d5`  
		Last Modified: Wed, 11 Jan 2023 03:49:51 GMT  
		Size: 2.6 MB (2569545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f63c8cab2b9d61d2f3471896c134214a6509df1ae6015168016b844882fb732`  
		Last Modified: Thu, 12 Jan 2023 19:22:59 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e57fdce70951ec51dd6c25118be99b7c8872affb93ce95cea5b9f537c76e18c`  
		Last Modified: Thu, 12 Jan 2023 19:23:04 GMT  
		Size: 47.2 MB (47191782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1902d059c5ab510e3ecb3817b29cb4a75202de84e9d5532dff27a0c63709575d`  
		Last Modified: Thu, 12 Jan 2023 19:22:59 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:4f3833eb279e1fd88cb92fe8b65d47e9007fd389ec4800c5b3b8937ccb66308b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72585164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d075ee49d59bb1a9b2aa85050fa39d32355859539ee9561ae4c1d144c171503d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:58:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:58:17 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Sat, 04 Feb 2023 06:58:17 GMT
ENV EMQX_VERSION=4.4.14
# Sat, 04 Feb 2023 06:58:17 GMT
ENV OTP=otp24.3.4.2-1
# Sat, 04 Feb 2023 06:58:21 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b70590c16effa60759f6ab08a4a0e666ad4487cf0eb88263ab992e44b440b815"; fi;     if [ ${arch} = "arm64" ]; then sha256="98b78798577ddb7685c42dc41b7a758aacfe27924c8be4510e2057527a142ba0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Sat, 04 Feb 2023 06:58:21 GMT
WORKDIR /opt/emqx
# Sat, 04 Feb 2023 06:58:21 GMT
USER emqx
# Sat, 04 Feb 2023 06:58:21 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Sat, 04 Feb 2023 06:58:21 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Sat, 04 Feb 2023 06:58:21 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Sat, 04 Feb 2023 06:58:21 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 06:58:21 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec19e49c9f1b83bf7a10aa9acb42fc320322675664694fcef2fae78ffac35be`  
		Last Modified: Sat, 04 Feb 2023 06:59:01 GMT  
		Size: 2.6 MB (2559256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d493f75b8396c6e4a7f2feffd26ee8057d9b7b6cad297c3996cfb6d5bc0ac8`  
		Last Modified: Sat, 04 Feb 2023 06:59:00 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c811c1943693213c6c81a5bf842a147189dcae0bfef07a44a0cd6bc208374c20`  
		Last Modified: Sat, 04 Feb 2023 06:59:04 GMT  
		Size: 40.0 MB (39975894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d52f0f105891e2e78398c2176de25fd53665f62bdb4d8e89440eb852607184`  
		Last Modified: Sat, 04 Feb 2023 06:59:00 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3`

```console
$ docker pull emqx@sha256:c34a8c6c34ad0ac5884539f6416c89ab0ef23ca519f1f4d6cf0ccb6ed6782a5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.3` - linux; amd64

```console
$ docker pull emqx@sha256:60d34652fe2f2a17a67e2b670e70b85bd9f6929ada7b8c471297af2a986e7b58
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68296745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905184f8643e4175bd260191db499a3c504ff4c8744568a7f368e7072751b6a2`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 11 Jan 2023 02:35:07 GMT
ADD file:67ceb946e54c26c505b5f9f393d77befbd5e9b3b5c069ca301e314ecc74456b0 in / 
# Wed, 11 Jan 2023 02:35:07 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:48:37 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 19:22:04 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 12 Jan 2023 19:22:04 GMT
ENV EMQX_VERSION=4.3.22
# Thu, 12 Jan 2023 19:22:09 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 12 Jan 2023 19:22:09 GMT
WORKDIR /opt/emqx
# Thu, 12 Jan 2023 19:22:10 GMT
USER emqx
# Thu, 12 Jan 2023 19:22:10 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 12 Jan 2023 19:22:10 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 12 Jan 2023 19:22:10 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Thu, 12 Jan 2023 19:22:10 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 12 Jan 2023 19:22:10 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:548fcab5fe888f589dd092c68b813bfd65359878bd1950d6b753f749e82ebd7c`  
		Last Modified: Wed, 11 Jan 2023 02:39:48 GMT  
		Size: 27.1 MB (27140352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661145169f684ea6623410a6b2e6bac4fff75dcec9474b51911e88a29706557f`  
		Last Modified: Wed, 11 Jan 2023 03:49:39 GMT  
		Size: 4.6 MB (4612517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c729c292ec153abc1a59a47bbbaeec2775a873a39ce5578f9211146d447eb24c`  
		Last Modified: Thu, 12 Jan 2023 19:22:46 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b41a70a2a0cbe37bd893a6f30513e5848362f11a72767d3ba0241f0680f9f7`  
		Last Modified: Thu, 12 Jan 2023 19:22:50 GMT  
		Size: 36.5 MB (36538722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b20fd74f38c808dff2d1a3b046e365e320984cb93075a176f997825ab6e878e`  
		Last Modified: Thu, 12 Jan 2023 19:22:46 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.3` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:fc7986c666bd10ad6a53c1acb232080b84174434a5d36ecb4b2fa3a0d4666108
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66636280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:130ef8d5f10e6b27081e90fc43f04a5b782e56f97adda24785cabc80a7153f9d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:54 GMT
ADD file:cf6ecb1d6b034b0d4fc309542cb25fff0c997661b323f524ecc258ac323e43f6 in / 
# Sat, 04 Feb 2023 06:17:55 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:58:05 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:58:05 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Sat, 04 Feb 2023 06:58:06 GMT
ENV EMQX_VERSION=4.3.22
# Sat, 04 Feb 2023 06:58:09 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Sat, 04 Feb 2023 06:58:09 GMT
WORKDIR /opt/emqx
# Sat, 04 Feb 2023 06:58:09 GMT
USER emqx
# Sat, 04 Feb 2023 06:58:09 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Sat, 04 Feb 2023 06:58:10 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Sat, 04 Feb 2023 06:58:10 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Sat, 04 Feb 2023 06:58:10 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 06:58:10 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:bd2853c1424a5596deda2f31e1f82920613a03c667c3ff58cb461340b7bb89cd`  
		Last Modified: Sat, 04 Feb 2023 06:22:04 GMT  
		Size: 25.9 MB (25922631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ad649ff2be9c41db4434f42a3e7a7481d41fcfa1259fb1c8290eb259812a26`  
		Last Modified: Sat, 04 Feb 2023 06:58:50 GMT  
		Size: 4.5 MB (4490611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be082951b179c83e960fdc4c9f869e0cc81c0af48b34c3b20ca99daf78bdc36`  
		Last Modified: Sat, 04 Feb 2023 06:58:49 GMT  
		Size: 4.1 KB (4111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90827bc4623d04b7905a87aeb3b35f60f34699f3c6d3cd9611cd20be107f1fe`  
		Last Modified: Sat, 04 Feb 2023 06:58:52 GMT  
		Size: 36.2 MB (36217886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3487570ed0dd7c61b0d01a35bf1f3fd9a948cbaa24f05951e6538397cbeef454`  
		Last Modified: Sat, 04 Feb 2023 06:58:49 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3.22`

```console
$ docker pull emqx@sha256:c34a8c6c34ad0ac5884539f6416c89ab0ef23ca519f1f4d6cf0ccb6ed6782a5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.3.22` - linux; amd64

```console
$ docker pull emqx@sha256:60d34652fe2f2a17a67e2b670e70b85bd9f6929ada7b8c471297af2a986e7b58
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68296745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905184f8643e4175bd260191db499a3c504ff4c8744568a7f368e7072751b6a2`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 11 Jan 2023 02:35:07 GMT
ADD file:67ceb946e54c26c505b5f9f393d77befbd5e9b3b5c069ca301e314ecc74456b0 in / 
# Wed, 11 Jan 2023 02:35:07 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:48:37 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 19:22:04 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 12 Jan 2023 19:22:04 GMT
ENV EMQX_VERSION=4.3.22
# Thu, 12 Jan 2023 19:22:09 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 12 Jan 2023 19:22:09 GMT
WORKDIR /opt/emqx
# Thu, 12 Jan 2023 19:22:10 GMT
USER emqx
# Thu, 12 Jan 2023 19:22:10 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 12 Jan 2023 19:22:10 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 12 Jan 2023 19:22:10 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Thu, 12 Jan 2023 19:22:10 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 12 Jan 2023 19:22:10 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:548fcab5fe888f589dd092c68b813bfd65359878bd1950d6b753f749e82ebd7c`  
		Last Modified: Wed, 11 Jan 2023 02:39:48 GMT  
		Size: 27.1 MB (27140352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661145169f684ea6623410a6b2e6bac4fff75dcec9474b51911e88a29706557f`  
		Last Modified: Wed, 11 Jan 2023 03:49:39 GMT  
		Size: 4.6 MB (4612517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c729c292ec153abc1a59a47bbbaeec2775a873a39ce5578f9211146d447eb24c`  
		Last Modified: Thu, 12 Jan 2023 19:22:46 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b41a70a2a0cbe37bd893a6f30513e5848362f11a72767d3ba0241f0680f9f7`  
		Last Modified: Thu, 12 Jan 2023 19:22:50 GMT  
		Size: 36.5 MB (36538722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b20fd74f38c808dff2d1a3b046e365e320984cb93075a176f997825ab6e878e`  
		Last Modified: Thu, 12 Jan 2023 19:22:46 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.3.22` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:fc7986c666bd10ad6a53c1acb232080b84174434a5d36ecb4b2fa3a0d4666108
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66636280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:130ef8d5f10e6b27081e90fc43f04a5b782e56f97adda24785cabc80a7153f9d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:54 GMT
ADD file:cf6ecb1d6b034b0d4fc309542cb25fff0c997661b323f524ecc258ac323e43f6 in / 
# Sat, 04 Feb 2023 06:17:55 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:58:05 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:58:05 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Sat, 04 Feb 2023 06:58:06 GMT
ENV EMQX_VERSION=4.3.22
# Sat, 04 Feb 2023 06:58:09 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Sat, 04 Feb 2023 06:58:09 GMT
WORKDIR /opt/emqx
# Sat, 04 Feb 2023 06:58:09 GMT
USER emqx
# Sat, 04 Feb 2023 06:58:09 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Sat, 04 Feb 2023 06:58:10 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Sat, 04 Feb 2023 06:58:10 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Sat, 04 Feb 2023 06:58:10 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 06:58:10 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:bd2853c1424a5596deda2f31e1f82920613a03c667c3ff58cb461340b7bb89cd`  
		Last Modified: Sat, 04 Feb 2023 06:22:04 GMT  
		Size: 25.9 MB (25922631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ad649ff2be9c41db4434f42a3e7a7481d41fcfa1259fb1c8290eb259812a26`  
		Last Modified: Sat, 04 Feb 2023 06:58:50 GMT  
		Size: 4.5 MB (4490611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be082951b179c83e960fdc4c9f869e0cc81c0af48b34c3b20ca99daf78bdc36`  
		Last Modified: Sat, 04 Feb 2023 06:58:49 GMT  
		Size: 4.1 KB (4111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90827bc4623d04b7905a87aeb3b35f60f34699f3c6d3cd9611cd20be107f1fe`  
		Last Modified: Sat, 04 Feb 2023 06:58:52 GMT  
		Size: 36.2 MB (36217886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3487570ed0dd7c61b0d01a35bf1f3fd9a948cbaa24f05951e6538397cbeef454`  
		Last Modified: Sat, 04 Feb 2023 06:58:49 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:f37a823975d64ff16532a0f4040e2a5b24ed0f33c641a74f70d93f9511f7b8a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:694fec8a03aa7424cd8fc9ae19b70d863567fa18751d6908d3148f7b8edbc48a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81163520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e156deb9005fb2fc2d647f71d5986a4077805155a66566408e5a646ecc17dcc`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:48:56 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 19:22:14 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 12 Jan 2023 19:22:14 GMT
ENV EMQX_VERSION=4.4.14
# Thu, 12 Jan 2023 19:22:14 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 12 Jan 2023 19:22:19 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b70590c16effa60759f6ab08a4a0e666ad4487cf0eb88263ab992e44b440b815"; fi;     if [ ${arch} = "arm64" ]; then sha256="98b78798577ddb7685c42dc41b7a758aacfe27924c8be4510e2057527a142ba0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 12 Jan 2023 19:22:20 GMT
WORKDIR /opt/emqx
# Thu, 12 Jan 2023 19:22:20 GMT
USER emqx
# Thu, 12 Jan 2023 19:22:20 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 12 Jan 2023 19:22:20 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 12 Jan 2023 19:22:20 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 12 Jan 2023 19:22:20 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 12 Jan 2023 19:22:20 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d3e57ec5f70305a1554472a8bc80d1caf9263b899fdc9e84d30606e2e849d5`  
		Last Modified: Wed, 11 Jan 2023 03:49:51 GMT  
		Size: 2.6 MB (2569545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f63c8cab2b9d61d2f3471896c134214a6509df1ae6015168016b844882fb732`  
		Last Modified: Thu, 12 Jan 2023 19:22:59 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e57fdce70951ec51dd6c25118be99b7c8872affb93ce95cea5b9f537c76e18c`  
		Last Modified: Thu, 12 Jan 2023 19:23:04 GMT  
		Size: 47.2 MB (47191782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1902d059c5ab510e3ecb3817b29cb4a75202de84e9d5532dff27a0c63709575d`  
		Last Modified: Thu, 12 Jan 2023 19:22:59 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:4f3833eb279e1fd88cb92fe8b65d47e9007fd389ec4800c5b3b8937ccb66308b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72585164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d075ee49d59bb1a9b2aa85050fa39d32355859539ee9561ae4c1d144c171503d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:58:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:58:17 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Sat, 04 Feb 2023 06:58:17 GMT
ENV EMQX_VERSION=4.4.14
# Sat, 04 Feb 2023 06:58:17 GMT
ENV OTP=otp24.3.4.2-1
# Sat, 04 Feb 2023 06:58:21 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b70590c16effa60759f6ab08a4a0e666ad4487cf0eb88263ab992e44b440b815"; fi;     if [ ${arch} = "arm64" ]; then sha256="98b78798577ddb7685c42dc41b7a758aacfe27924c8be4510e2057527a142ba0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Sat, 04 Feb 2023 06:58:21 GMT
WORKDIR /opt/emqx
# Sat, 04 Feb 2023 06:58:21 GMT
USER emqx
# Sat, 04 Feb 2023 06:58:21 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Sat, 04 Feb 2023 06:58:21 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Sat, 04 Feb 2023 06:58:21 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Sat, 04 Feb 2023 06:58:21 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 06:58:21 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec19e49c9f1b83bf7a10aa9acb42fc320322675664694fcef2fae78ffac35be`  
		Last Modified: Sat, 04 Feb 2023 06:59:01 GMT  
		Size: 2.6 MB (2559256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d493f75b8396c6e4a7f2feffd26ee8057d9b7b6cad297c3996cfb6d5bc0ac8`  
		Last Modified: Sat, 04 Feb 2023 06:59:00 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c811c1943693213c6c81a5bf842a147189dcae0bfef07a44a0cd6bc208374c20`  
		Last Modified: Sat, 04 Feb 2023 06:59:04 GMT  
		Size: 40.0 MB (39975894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d52f0f105891e2e78398c2176de25fd53665f62bdb4d8e89440eb852607184`  
		Last Modified: Sat, 04 Feb 2023 06:59:00 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.14`

```console
$ docker pull emqx@sha256:f37a823975d64ff16532a0f4040e2a5b24ed0f33c641a74f70d93f9511f7b8a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4.14` - linux; amd64

```console
$ docker pull emqx@sha256:694fec8a03aa7424cd8fc9ae19b70d863567fa18751d6908d3148f7b8edbc48a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81163520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e156deb9005fb2fc2d647f71d5986a4077805155a66566408e5a646ecc17dcc`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:48:56 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 19:22:14 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 12 Jan 2023 19:22:14 GMT
ENV EMQX_VERSION=4.4.14
# Thu, 12 Jan 2023 19:22:14 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 12 Jan 2023 19:22:19 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b70590c16effa60759f6ab08a4a0e666ad4487cf0eb88263ab992e44b440b815"; fi;     if [ ${arch} = "arm64" ]; then sha256="98b78798577ddb7685c42dc41b7a758aacfe27924c8be4510e2057527a142ba0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 12 Jan 2023 19:22:20 GMT
WORKDIR /opt/emqx
# Thu, 12 Jan 2023 19:22:20 GMT
USER emqx
# Thu, 12 Jan 2023 19:22:20 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 12 Jan 2023 19:22:20 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 12 Jan 2023 19:22:20 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 12 Jan 2023 19:22:20 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 12 Jan 2023 19:22:20 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d3e57ec5f70305a1554472a8bc80d1caf9263b899fdc9e84d30606e2e849d5`  
		Last Modified: Wed, 11 Jan 2023 03:49:51 GMT  
		Size: 2.6 MB (2569545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f63c8cab2b9d61d2f3471896c134214a6509df1ae6015168016b844882fb732`  
		Last Modified: Thu, 12 Jan 2023 19:22:59 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e57fdce70951ec51dd6c25118be99b7c8872affb93ce95cea5b9f537c76e18c`  
		Last Modified: Thu, 12 Jan 2023 19:23:04 GMT  
		Size: 47.2 MB (47191782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1902d059c5ab510e3ecb3817b29cb4a75202de84e9d5532dff27a0c63709575d`  
		Last Modified: Thu, 12 Jan 2023 19:22:59 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4.14` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:4f3833eb279e1fd88cb92fe8b65d47e9007fd389ec4800c5b3b8937ccb66308b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72585164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d075ee49d59bb1a9b2aa85050fa39d32355859539ee9561ae4c1d144c171503d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:58:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:58:17 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Sat, 04 Feb 2023 06:58:17 GMT
ENV EMQX_VERSION=4.4.14
# Sat, 04 Feb 2023 06:58:17 GMT
ENV OTP=otp24.3.4.2-1
# Sat, 04 Feb 2023 06:58:21 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b70590c16effa60759f6ab08a4a0e666ad4487cf0eb88263ab992e44b440b815"; fi;     if [ ${arch} = "arm64" ]; then sha256="98b78798577ddb7685c42dc41b7a758aacfe27924c8be4510e2057527a142ba0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Sat, 04 Feb 2023 06:58:21 GMT
WORKDIR /opt/emqx
# Sat, 04 Feb 2023 06:58:21 GMT
USER emqx
# Sat, 04 Feb 2023 06:58:21 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Sat, 04 Feb 2023 06:58:21 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Sat, 04 Feb 2023 06:58:21 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Sat, 04 Feb 2023 06:58:21 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 06:58:21 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec19e49c9f1b83bf7a10aa9acb42fc320322675664694fcef2fae78ffac35be`  
		Last Modified: Sat, 04 Feb 2023 06:59:01 GMT  
		Size: 2.6 MB (2559256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d493f75b8396c6e4a7f2feffd26ee8057d9b7b6cad297c3996cfb6d5bc0ac8`  
		Last Modified: Sat, 04 Feb 2023 06:59:00 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c811c1943693213c6c81a5bf842a147189dcae0bfef07a44a0cd6bc208374c20`  
		Last Modified: Sat, 04 Feb 2023 06:59:04 GMT  
		Size: 40.0 MB (39975894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d52f0f105891e2e78398c2176de25fd53665f62bdb4d8e89440eb852607184`  
		Last Modified: Sat, 04 Feb 2023 06:59:00 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5`

```console
$ docker pull emqx@sha256:96fb7dd67bda2e969eaef1581a2e8671be7264134ff193ae3dcefe9476ab8764
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:bd014838f39530946a140dfd5cbc7be83db45b9f48813cbbe7c0395ed701026c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.3 MB (100331823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a2bcdd65b094e16104c87ef96feb844d67a668ddfa41aa6ecaeca5972046d83`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:49:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:49:16 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Fri, 03 Feb 2023 20:19:35 GMT
ENV EMQX_VERSION=5.0.16
# Fri, 03 Feb 2023 20:19:35 GMT
ENV AMD64_SHA256=ee95db4baeaa51ff19bb37104013d0a954be64478d02015466a2dfc8d825d19c
# Fri, 03 Feb 2023 20:19:35 GMT
ENV ARM64_SHA256=8bf96461796da3bb0640c0f7456e3bc36b68ddd1ab9c5dae950553645d4859a6
# Fri, 03 Feb 2023 20:19:35 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 03 Feb 2023 20:19:41 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Fri, 03 Feb 2023 20:19:42 GMT
WORKDIR /opt/emqx
# Fri, 03 Feb 2023 20:19:42 GMT
USER emqx
# Fri, 03 Feb 2023 20:19:42 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 03 Feb 2023 20:19:42 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 03 Feb 2023 20:19:42 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 03 Feb 2023 20:19:42 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 03 Feb 2023 20:19:42 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1226f5729eeebf1d9e397edf672aef9dc2809741454ab2d1a2f58a4bb3f67eb0`  
		Last Modified: Wed, 11 Jan 2023 03:50:07 GMT  
		Size: 3.0 MB (2987690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a786684ff862ef4f11abc26cfb08583cf925746ea80d7c34769aa93aa99660e7`  
		Last Modified: Wed, 11 Jan 2023 03:50:06 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff87a028868183f43bf60f7ec66589cc7db564a5c43989c32f882ca2ee99d4d8`  
		Last Modified: Fri, 03 Feb 2023 20:20:08 GMT  
		Size: 65.9 MB (65942153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3aa195277547c3f7d9ff37a7c6feb1d8a622e35b9a480d6cf2027e7cd7da42`  
		Last Modified: Fri, 03 Feb 2023 20:19:59 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:75aeeada68d11f4130ee5572f39867ef58f4d6e1b2cbf144b6f1cd4de82adf69
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.4 MB (91426110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:771d1a97b5fc626468184c1ec01292eb3fb63c91fcca97411350c7898154d897`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:58:28 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:58:29 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Sat, 04 Feb 2023 06:58:29 GMT
ENV EMQX_VERSION=5.0.16
# Sat, 04 Feb 2023 06:58:29 GMT
ENV AMD64_SHA256=ee95db4baeaa51ff19bb37104013d0a954be64478d02015466a2dfc8d825d19c
# Sat, 04 Feb 2023 06:58:29 GMT
ENV ARM64_SHA256=8bf96461796da3bb0640c0f7456e3bc36b68ddd1ab9c5dae950553645d4859a6
# Sat, 04 Feb 2023 06:58:29 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Sat, 04 Feb 2023 06:58:33 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Sat, 04 Feb 2023 06:58:34 GMT
WORKDIR /opt/emqx
# Sat, 04 Feb 2023 06:58:34 GMT
USER emqx
# Sat, 04 Feb 2023 06:58:34 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Sat, 04 Feb 2023 06:58:34 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Sat, 04 Feb 2023 06:58:34 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Sat, 04 Feb 2023 06:58:34 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 06:58:34 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df3b032d76ee04c762ca45c13d20cc97e3a552190bf307bb662aa8ad8a6b74f`  
		Last Modified: Sat, 04 Feb 2023 06:59:15 GMT  
		Size: 3.0 MB (3002716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc23a2f376c6744b63203db8042aed32611c322263c42d2247668e256b60ec4`  
		Last Modified: Sat, 04 Feb 2023 06:59:14 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651de4374a28919ba86a076a0c255e4fe0e94de8069906a5dea43db5c34562d5`  
		Last Modified: Sat, 04 Feb 2023 06:59:20 GMT  
		Size: 58.4 MB (58373588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3932ab6d8b453c204fa46e29e69624f4b7d516c6096902028d45c137d92c71ff`  
		Last Modified: Sat, 04 Feb 2023 06:59:14 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:96fb7dd67bda2e969eaef1581a2e8671be7264134ff193ae3dcefe9476ab8764
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:bd014838f39530946a140dfd5cbc7be83db45b9f48813cbbe7c0395ed701026c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.3 MB (100331823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a2bcdd65b094e16104c87ef96feb844d67a668ddfa41aa6ecaeca5972046d83`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:49:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:49:16 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Fri, 03 Feb 2023 20:19:35 GMT
ENV EMQX_VERSION=5.0.16
# Fri, 03 Feb 2023 20:19:35 GMT
ENV AMD64_SHA256=ee95db4baeaa51ff19bb37104013d0a954be64478d02015466a2dfc8d825d19c
# Fri, 03 Feb 2023 20:19:35 GMT
ENV ARM64_SHA256=8bf96461796da3bb0640c0f7456e3bc36b68ddd1ab9c5dae950553645d4859a6
# Fri, 03 Feb 2023 20:19:35 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 03 Feb 2023 20:19:41 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Fri, 03 Feb 2023 20:19:42 GMT
WORKDIR /opt/emqx
# Fri, 03 Feb 2023 20:19:42 GMT
USER emqx
# Fri, 03 Feb 2023 20:19:42 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 03 Feb 2023 20:19:42 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 03 Feb 2023 20:19:42 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 03 Feb 2023 20:19:42 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 03 Feb 2023 20:19:42 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1226f5729eeebf1d9e397edf672aef9dc2809741454ab2d1a2f58a4bb3f67eb0`  
		Last Modified: Wed, 11 Jan 2023 03:50:07 GMT  
		Size: 3.0 MB (2987690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a786684ff862ef4f11abc26cfb08583cf925746ea80d7c34769aa93aa99660e7`  
		Last Modified: Wed, 11 Jan 2023 03:50:06 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff87a028868183f43bf60f7ec66589cc7db564a5c43989c32f882ca2ee99d4d8`  
		Last Modified: Fri, 03 Feb 2023 20:20:08 GMT  
		Size: 65.9 MB (65942153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3aa195277547c3f7d9ff37a7c6feb1d8a622e35b9a480d6cf2027e7cd7da42`  
		Last Modified: Fri, 03 Feb 2023 20:19:59 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:75aeeada68d11f4130ee5572f39867ef58f4d6e1b2cbf144b6f1cd4de82adf69
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.4 MB (91426110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:771d1a97b5fc626468184c1ec01292eb3fb63c91fcca97411350c7898154d897`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:58:28 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:58:29 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Sat, 04 Feb 2023 06:58:29 GMT
ENV EMQX_VERSION=5.0.16
# Sat, 04 Feb 2023 06:58:29 GMT
ENV AMD64_SHA256=ee95db4baeaa51ff19bb37104013d0a954be64478d02015466a2dfc8d825d19c
# Sat, 04 Feb 2023 06:58:29 GMT
ENV ARM64_SHA256=8bf96461796da3bb0640c0f7456e3bc36b68ddd1ab9c5dae950553645d4859a6
# Sat, 04 Feb 2023 06:58:29 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Sat, 04 Feb 2023 06:58:33 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Sat, 04 Feb 2023 06:58:34 GMT
WORKDIR /opt/emqx
# Sat, 04 Feb 2023 06:58:34 GMT
USER emqx
# Sat, 04 Feb 2023 06:58:34 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Sat, 04 Feb 2023 06:58:34 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Sat, 04 Feb 2023 06:58:34 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Sat, 04 Feb 2023 06:58:34 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 06:58:34 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df3b032d76ee04c762ca45c13d20cc97e3a552190bf307bb662aa8ad8a6b74f`  
		Last Modified: Sat, 04 Feb 2023 06:59:15 GMT  
		Size: 3.0 MB (3002716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc23a2f376c6744b63203db8042aed32611c322263c42d2247668e256b60ec4`  
		Last Modified: Sat, 04 Feb 2023 06:59:14 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651de4374a28919ba86a076a0c255e4fe0e94de8069906a5dea43db5c34562d5`  
		Last Modified: Sat, 04 Feb 2023 06:59:20 GMT  
		Size: 58.4 MB (58373588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3932ab6d8b453c204fa46e29e69624f4b7d516c6096902028d45c137d92c71ff`  
		Last Modified: Sat, 04 Feb 2023 06:59:14 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.16`

```console
$ docker pull emqx@sha256:96fb7dd67bda2e969eaef1581a2e8671be7264134ff193ae3dcefe9476ab8764
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0.16` - linux; amd64

```console
$ docker pull emqx@sha256:bd014838f39530946a140dfd5cbc7be83db45b9f48813cbbe7c0395ed701026c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.3 MB (100331823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a2bcdd65b094e16104c87ef96feb844d67a668ddfa41aa6ecaeca5972046d83`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:49:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:49:16 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Fri, 03 Feb 2023 20:19:35 GMT
ENV EMQX_VERSION=5.0.16
# Fri, 03 Feb 2023 20:19:35 GMT
ENV AMD64_SHA256=ee95db4baeaa51ff19bb37104013d0a954be64478d02015466a2dfc8d825d19c
# Fri, 03 Feb 2023 20:19:35 GMT
ENV ARM64_SHA256=8bf96461796da3bb0640c0f7456e3bc36b68ddd1ab9c5dae950553645d4859a6
# Fri, 03 Feb 2023 20:19:35 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 03 Feb 2023 20:19:41 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Fri, 03 Feb 2023 20:19:42 GMT
WORKDIR /opt/emqx
# Fri, 03 Feb 2023 20:19:42 GMT
USER emqx
# Fri, 03 Feb 2023 20:19:42 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 03 Feb 2023 20:19:42 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 03 Feb 2023 20:19:42 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 03 Feb 2023 20:19:42 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 03 Feb 2023 20:19:42 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1226f5729eeebf1d9e397edf672aef9dc2809741454ab2d1a2f58a4bb3f67eb0`  
		Last Modified: Wed, 11 Jan 2023 03:50:07 GMT  
		Size: 3.0 MB (2987690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a786684ff862ef4f11abc26cfb08583cf925746ea80d7c34769aa93aa99660e7`  
		Last Modified: Wed, 11 Jan 2023 03:50:06 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff87a028868183f43bf60f7ec66589cc7db564a5c43989c32f882ca2ee99d4d8`  
		Last Modified: Fri, 03 Feb 2023 20:20:08 GMT  
		Size: 65.9 MB (65942153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3aa195277547c3f7d9ff37a7c6feb1d8a622e35b9a480d6cf2027e7cd7da42`  
		Last Modified: Fri, 03 Feb 2023 20:19:59 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0.16` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:75aeeada68d11f4130ee5572f39867ef58f4d6e1b2cbf144b6f1cd4de82adf69
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.4 MB (91426110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:771d1a97b5fc626468184c1ec01292eb3fb63c91fcca97411350c7898154d897`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:58:28 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:58:29 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Sat, 04 Feb 2023 06:58:29 GMT
ENV EMQX_VERSION=5.0.16
# Sat, 04 Feb 2023 06:58:29 GMT
ENV AMD64_SHA256=ee95db4baeaa51ff19bb37104013d0a954be64478d02015466a2dfc8d825d19c
# Sat, 04 Feb 2023 06:58:29 GMT
ENV ARM64_SHA256=8bf96461796da3bb0640c0f7456e3bc36b68ddd1ab9c5dae950553645d4859a6
# Sat, 04 Feb 2023 06:58:29 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Sat, 04 Feb 2023 06:58:33 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Sat, 04 Feb 2023 06:58:34 GMT
WORKDIR /opt/emqx
# Sat, 04 Feb 2023 06:58:34 GMT
USER emqx
# Sat, 04 Feb 2023 06:58:34 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Sat, 04 Feb 2023 06:58:34 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Sat, 04 Feb 2023 06:58:34 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Sat, 04 Feb 2023 06:58:34 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 06:58:34 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df3b032d76ee04c762ca45c13d20cc97e3a552190bf307bb662aa8ad8a6b74f`  
		Last Modified: Sat, 04 Feb 2023 06:59:15 GMT  
		Size: 3.0 MB (3002716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc23a2f376c6744b63203db8042aed32611c322263c42d2247668e256b60ec4`  
		Last Modified: Sat, 04 Feb 2023 06:59:14 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651de4374a28919ba86a076a0c255e4fe0e94de8069906a5dea43db5c34562d5`  
		Last Modified: Sat, 04 Feb 2023 06:59:20 GMT  
		Size: 58.4 MB (58373588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3932ab6d8b453c204fa46e29e69624f4b7d516c6096902028d45c137d92c71ff`  
		Last Modified: Sat, 04 Feb 2023 06:59:14 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:96fb7dd67bda2e969eaef1581a2e8671be7264134ff193ae3dcefe9476ab8764
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:bd014838f39530946a140dfd5cbc7be83db45b9f48813cbbe7c0395ed701026c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.3 MB (100331823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a2bcdd65b094e16104c87ef96feb844d67a668ddfa41aa6ecaeca5972046d83`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:49:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:49:16 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Fri, 03 Feb 2023 20:19:35 GMT
ENV EMQX_VERSION=5.0.16
# Fri, 03 Feb 2023 20:19:35 GMT
ENV AMD64_SHA256=ee95db4baeaa51ff19bb37104013d0a954be64478d02015466a2dfc8d825d19c
# Fri, 03 Feb 2023 20:19:35 GMT
ENV ARM64_SHA256=8bf96461796da3bb0640c0f7456e3bc36b68ddd1ab9c5dae950553645d4859a6
# Fri, 03 Feb 2023 20:19:35 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 03 Feb 2023 20:19:41 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Fri, 03 Feb 2023 20:19:42 GMT
WORKDIR /opt/emqx
# Fri, 03 Feb 2023 20:19:42 GMT
USER emqx
# Fri, 03 Feb 2023 20:19:42 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 03 Feb 2023 20:19:42 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 03 Feb 2023 20:19:42 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 03 Feb 2023 20:19:42 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 03 Feb 2023 20:19:42 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1226f5729eeebf1d9e397edf672aef9dc2809741454ab2d1a2f58a4bb3f67eb0`  
		Last Modified: Wed, 11 Jan 2023 03:50:07 GMT  
		Size: 3.0 MB (2987690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a786684ff862ef4f11abc26cfb08583cf925746ea80d7c34769aa93aa99660e7`  
		Last Modified: Wed, 11 Jan 2023 03:50:06 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff87a028868183f43bf60f7ec66589cc7db564a5c43989c32f882ca2ee99d4d8`  
		Last Modified: Fri, 03 Feb 2023 20:20:08 GMT  
		Size: 65.9 MB (65942153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3aa195277547c3f7d9ff37a7c6feb1d8a622e35b9a480d6cf2027e7cd7da42`  
		Last Modified: Fri, 03 Feb 2023 20:19:59 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:75aeeada68d11f4130ee5572f39867ef58f4d6e1b2cbf144b6f1cd4de82adf69
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.4 MB (91426110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:771d1a97b5fc626468184c1ec01292eb3fb63c91fcca97411350c7898154d897`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:58:28 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:58:29 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Sat, 04 Feb 2023 06:58:29 GMT
ENV EMQX_VERSION=5.0.16
# Sat, 04 Feb 2023 06:58:29 GMT
ENV AMD64_SHA256=ee95db4baeaa51ff19bb37104013d0a954be64478d02015466a2dfc8d825d19c
# Sat, 04 Feb 2023 06:58:29 GMT
ENV ARM64_SHA256=8bf96461796da3bb0640c0f7456e3bc36b68ddd1ab9c5dae950553645d4859a6
# Sat, 04 Feb 2023 06:58:29 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Sat, 04 Feb 2023 06:58:33 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Sat, 04 Feb 2023 06:58:34 GMT
WORKDIR /opt/emqx
# Sat, 04 Feb 2023 06:58:34 GMT
USER emqx
# Sat, 04 Feb 2023 06:58:34 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Sat, 04 Feb 2023 06:58:34 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Sat, 04 Feb 2023 06:58:34 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Sat, 04 Feb 2023 06:58:34 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 06:58:34 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df3b032d76ee04c762ca45c13d20cc97e3a552190bf307bb662aa8ad8a6b74f`  
		Last Modified: Sat, 04 Feb 2023 06:59:15 GMT  
		Size: 3.0 MB (3002716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc23a2f376c6744b63203db8042aed32611c322263c42d2247668e256b60ec4`  
		Last Modified: Sat, 04 Feb 2023 06:59:14 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651de4374a28919ba86a076a0c255e4fe0e94de8069906a5dea43db5c34562d5`  
		Last Modified: Sat, 04 Feb 2023 06:59:20 GMT  
		Size: 58.4 MB (58373588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3932ab6d8b453c204fa46e29e69624f4b7d516c6096902028d45c137d92c71ff`  
		Last Modified: Sat, 04 Feb 2023 06:59:14 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
