<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `emqx`

-	[`emqx:4`](#emqx4)
-	[`emqx:4.3`](#emqx43)
-	[`emqx:4.3.15`](#emqx4315)
-	[`emqx:4.4`](#emqx44)
-	[`emqx:4.4.4`](#emqx444)
-	[`emqx:latest`](#emqxlatest)

## `emqx:4`

```console
$ docker pull emqx@sha256:00da7d91ed80191c10bcf0ddbddb8b7cfb6b87020752505e9b8c4b950a019a1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:96aaa084ede72e2f7063825961b9d4c33c7de7070a3eda430420f1aef1705d7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124813883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e05d42000605d355acff3be7bd2e91561b4d0a782bebfabd01d3d03810209333`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:05:55 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:05:56 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 23 Aug 2022 01:05:56 GMT
ENV OTP=otp24.1.5-3
# Tue, 23 Aug 2022 01:06:01 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 23 Aug 2022 01:06:08 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 23 Aug 2022 01:06:08 GMT
WORKDIR /opt/emqx
# Tue, 23 Aug 2022 01:06:08 GMT
USER emqx
# Tue, 23 Aug 2022 01:06:08 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 23 Aug 2022 01:06:08 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 23 Aug 2022 01:06:08 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 23 Aug 2022 01:06:09 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 01:06:09 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffe4803a256fc338d2725fd4a931050eb43f5804176597d989565411f39c0ba`  
		Last Modified: Tue, 23 Aug 2022 01:06:37 GMT  
		Size: 2.6 MB (2569463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8158f546cdbbf53444243363ab3ad5ffb0d011f3609b02f3e76f388262324cf`  
		Last Modified: Tue, 23 Aug 2022 01:06:42 GMT  
		Size: 45.4 MB (45424512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573b89c93de2f74dcf9490f92cbbf4e6ce0d5cf3a36113621de60cb5f14c606d`  
		Last Modified: Tue, 23 Aug 2022 01:06:42 GMT  
		Size: 45.4 MB (45437317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efae4ef2c4c3e4f2858b9437a6dc47120ff2cd5821967db6f10e8ecb32d33cb1`  
		Last Modified: Tue, 23 Aug 2022 01:06:37 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:96b008f7a2747ff4f13160a962292dbd1ab678597a9228a76b3203f84a46bf1b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110228075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c98a17532608ae41772e2e92f9bb3d479794c37c9d9e045805c39568ce75607`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:00:31 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:00:32 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 02 Aug 2022 02:00:33 GMT
ENV OTP=otp24.1.5-3
# Tue, 02 Aug 2022 02:00:39 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 02 Aug 2022 02:00:40 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 02 Aug 2022 02:00:40 GMT
WORKDIR /opt/emqx
# Tue, 02 Aug 2022 02:00:41 GMT
USER emqx
# Tue, 02 Aug 2022 02:00:42 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 02 Aug 2022 02:00:43 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 02 Aug 2022 02:00:45 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 02 Aug 2022 02:00:45 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 02:00:46 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b8f37b5c2edc91fd1bdf8c28fd2b3da0c926ac40e82e7c59c7d03f310614f8`  
		Last Modified: Tue, 02 Aug 2022 02:01:24 GMT  
		Size: 2.6 MB (2558106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4cdc0cba9be243cb158e5751b728035148562b033d8ef1de765ca01f1a60dc`  
		Last Modified: Tue, 02 Aug 2022 02:01:28 GMT  
		Size: 38.8 MB (38806797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14c711205c5c7e4009eff2ea08ba336ac4598b6d1dfa6c1f7cf37089a5e727e`  
		Last Modified: Tue, 02 Aug 2022 02:01:28 GMT  
		Size: 38.8 MB (38807760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f05323f5f302f4d39168dba4ee48ae9ba98e3f6cd38134a5eaf7d8fe54dbc96`  
		Last Modified: Tue, 02 Aug 2022 02:01:24 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3`

```console
$ docker pull emqx@sha256:f7c938a4b47ab9b6ea6d3849832666a7d3d2f8e0cc76fafad5892fe11a15e9cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.3` - linux; amd64

```console
$ docker pull emqx@sha256:f29b7e63cad4da4acdb4a42066b107758a6be7e6e221d7e5fb6df158915ea2b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.9 MB (103862512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feced5ed4320bee6a4c980e1d7807203f0dd0bcb9f40ade339ec3eb2b6fbfeef`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:05:33 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:05:33 GMT
ENV EMQX_VERSION=4.3.15
# Tue, 23 Aug 2022 01:05:38 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="8f44386aebf472297377d7b6b595638f323227347047d5278dce9c0cd04963bc"; fi;     if [ ${arch} = "arm64" ]; then sha256="b0094028d388684136be975c574d98295205dd5a343045f76f423a109535e016"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 23 Aug 2022 01:05:44 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 23 Aug 2022 01:05:44 GMT
WORKDIR /opt/emqx
# Tue, 23 Aug 2022 01:05:44 GMT
USER emqx
# Tue, 23 Aug 2022 01:05:44 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 23 Aug 2022 01:05:45 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 23 Aug 2022 01:05:45 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Tue, 23 Aug 2022 01:05:45 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 01:05:45 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fc000e6c6f87d5970bb32934528b67bd477dd1f5b55750bacff840ca9afa16`  
		Last Modified: Tue, 23 Aug 2022 01:06:24 GMT  
		Size: 4.6 MB (4610293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dfcce166ea2a4d49761e69fa4301ac76c2ffbce971391faf1f7b3847f965d2`  
		Last Modified: Tue, 23 Aug 2022 01:06:28 GMT  
		Size: 36.1 MB (36056943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac686cd8804af39d2959b821282da48d5fcfb7b8e6338a9c689c28b5ecf22bf`  
		Last Modified: Tue, 23 Aug 2022 01:06:28 GMT  
		Size: 36.1 MB (36055904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1aa5f6638a70fdc86e8f2423e702510595c42488ffe301df20abb03590fdfb`  
		Last Modified: Tue, 23 Aug 2022 01:06:23 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.3` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:b16db7118eb58b8d4a97fb43c042cd32a1655157bc4db9f9dcae97f114624fb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101935760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b7a2a6bf2ba99e9903831293b4162a6627d0e1a53f9820d1ecbee59f9490863`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:03 GMT
ADD file:d973e057fdca9166fb9f39e73d7d5d4ca8ac2af6a55813580bf14a13cef4c159 in / 
# Tue, 02 Aug 2022 00:41:04 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:00:06 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:00:07 GMT
ENV EMQX_VERSION=4.3.15
# Tue, 02 Aug 2022 02:00:11 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="8f44386aebf472297377d7b6b595638f323227347047d5278dce9c0cd04963bc"; fi;     if [ ${arch} = "arm64" ]; then sha256="b0094028d388684136be975c574d98295205dd5a343045f76f423a109535e016"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 02 Aug 2022 02:00:13 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 02 Aug 2022 02:00:13 GMT
WORKDIR /opt/emqx
# Tue, 02 Aug 2022 02:00:14 GMT
USER emqx
# Tue, 02 Aug 2022 02:00:15 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 02 Aug 2022 02:00:16 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 02 Aug 2022 02:00:18 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Tue, 02 Aug 2022 02:00:18 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 02:00:19 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:6d588874b4737b02fc84169cf7d3d1d70f20c7f5dbd1ddfe27de4aff25e23314`  
		Last Modified: Tue, 02 Aug 2022 00:46:56 GMT  
		Size: 25.9 MB (25914363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2b2f4e619a38b8280049a873bd6f8a35e77602ef714c8d925914cfdc1d7f66`  
		Last Modified: Tue, 02 Aug 2022 02:01:08 GMT  
		Size: 4.5 MB (4485416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce39f660024cb68f4dce1c54e7144cf9f342e0153943e1f5c82ee3538c880fa`  
		Last Modified: Tue, 02 Aug 2022 02:01:12 GMT  
		Size: 35.8 MB (35761683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01a9662cbb50570188d29c50987a3a9013fb6857606ae07726533cca3e6f94f`  
		Last Modified: Tue, 02 Aug 2022 02:01:12 GMT  
		Size: 35.8 MB (35773257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1cc57c05c26773068d31086af331ff5adeb249867eeaeccfd54090deff52b6`  
		Last Modified: Tue, 02 Aug 2022 02:01:08 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3.15`

```console
$ docker pull emqx@sha256:f7c938a4b47ab9b6ea6d3849832666a7d3d2f8e0cc76fafad5892fe11a15e9cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.3.15` - linux; amd64

```console
$ docker pull emqx@sha256:f29b7e63cad4da4acdb4a42066b107758a6be7e6e221d7e5fb6df158915ea2b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.9 MB (103862512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feced5ed4320bee6a4c980e1d7807203f0dd0bcb9f40ade339ec3eb2b6fbfeef`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:05:33 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:05:33 GMT
ENV EMQX_VERSION=4.3.15
# Tue, 23 Aug 2022 01:05:38 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="8f44386aebf472297377d7b6b595638f323227347047d5278dce9c0cd04963bc"; fi;     if [ ${arch} = "arm64" ]; then sha256="b0094028d388684136be975c574d98295205dd5a343045f76f423a109535e016"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 23 Aug 2022 01:05:44 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 23 Aug 2022 01:05:44 GMT
WORKDIR /opt/emqx
# Tue, 23 Aug 2022 01:05:44 GMT
USER emqx
# Tue, 23 Aug 2022 01:05:44 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 23 Aug 2022 01:05:45 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 23 Aug 2022 01:05:45 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Tue, 23 Aug 2022 01:05:45 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 01:05:45 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fc000e6c6f87d5970bb32934528b67bd477dd1f5b55750bacff840ca9afa16`  
		Last Modified: Tue, 23 Aug 2022 01:06:24 GMT  
		Size: 4.6 MB (4610293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dfcce166ea2a4d49761e69fa4301ac76c2ffbce971391faf1f7b3847f965d2`  
		Last Modified: Tue, 23 Aug 2022 01:06:28 GMT  
		Size: 36.1 MB (36056943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac686cd8804af39d2959b821282da48d5fcfb7b8e6338a9c689c28b5ecf22bf`  
		Last Modified: Tue, 23 Aug 2022 01:06:28 GMT  
		Size: 36.1 MB (36055904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1aa5f6638a70fdc86e8f2423e702510595c42488ffe301df20abb03590fdfb`  
		Last Modified: Tue, 23 Aug 2022 01:06:23 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.3.15` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:b16db7118eb58b8d4a97fb43c042cd32a1655157bc4db9f9dcae97f114624fb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101935760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b7a2a6bf2ba99e9903831293b4162a6627d0e1a53f9820d1ecbee59f9490863`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:03 GMT
ADD file:d973e057fdca9166fb9f39e73d7d5d4ca8ac2af6a55813580bf14a13cef4c159 in / 
# Tue, 02 Aug 2022 00:41:04 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:00:06 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:00:07 GMT
ENV EMQX_VERSION=4.3.15
# Tue, 02 Aug 2022 02:00:11 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="8f44386aebf472297377d7b6b595638f323227347047d5278dce9c0cd04963bc"; fi;     if [ ${arch} = "arm64" ]; then sha256="b0094028d388684136be975c574d98295205dd5a343045f76f423a109535e016"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 02 Aug 2022 02:00:13 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 02 Aug 2022 02:00:13 GMT
WORKDIR /opt/emqx
# Tue, 02 Aug 2022 02:00:14 GMT
USER emqx
# Tue, 02 Aug 2022 02:00:15 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 02 Aug 2022 02:00:16 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 02 Aug 2022 02:00:18 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Tue, 02 Aug 2022 02:00:18 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 02:00:19 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:6d588874b4737b02fc84169cf7d3d1d70f20c7f5dbd1ddfe27de4aff25e23314`  
		Last Modified: Tue, 02 Aug 2022 00:46:56 GMT  
		Size: 25.9 MB (25914363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2b2f4e619a38b8280049a873bd6f8a35e77602ef714c8d925914cfdc1d7f66`  
		Last Modified: Tue, 02 Aug 2022 02:01:08 GMT  
		Size: 4.5 MB (4485416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce39f660024cb68f4dce1c54e7144cf9f342e0153943e1f5c82ee3538c880fa`  
		Last Modified: Tue, 02 Aug 2022 02:01:12 GMT  
		Size: 35.8 MB (35761683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01a9662cbb50570188d29c50987a3a9013fb6857606ae07726533cca3e6f94f`  
		Last Modified: Tue, 02 Aug 2022 02:01:12 GMT  
		Size: 35.8 MB (35773257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1cc57c05c26773068d31086af331ff5adeb249867eeaeccfd54090deff52b6`  
		Last Modified: Tue, 02 Aug 2022 02:01:08 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:00da7d91ed80191c10bcf0ddbddb8b7cfb6b87020752505e9b8c4b950a019a1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:96aaa084ede72e2f7063825961b9d4c33c7de7070a3eda430420f1aef1705d7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124813883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e05d42000605d355acff3be7bd2e91561b4d0a782bebfabd01d3d03810209333`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:05:55 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:05:56 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 23 Aug 2022 01:05:56 GMT
ENV OTP=otp24.1.5-3
# Tue, 23 Aug 2022 01:06:01 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 23 Aug 2022 01:06:08 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 23 Aug 2022 01:06:08 GMT
WORKDIR /opt/emqx
# Tue, 23 Aug 2022 01:06:08 GMT
USER emqx
# Tue, 23 Aug 2022 01:06:08 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 23 Aug 2022 01:06:08 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 23 Aug 2022 01:06:08 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 23 Aug 2022 01:06:09 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 01:06:09 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffe4803a256fc338d2725fd4a931050eb43f5804176597d989565411f39c0ba`  
		Last Modified: Tue, 23 Aug 2022 01:06:37 GMT  
		Size: 2.6 MB (2569463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8158f546cdbbf53444243363ab3ad5ffb0d011f3609b02f3e76f388262324cf`  
		Last Modified: Tue, 23 Aug 2022 01:06:42 GMT  
		Size: 45.4 MB (45424512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573b89c93de2f74dcf9490f92cbbf4e6ce0d5cf3a36113621de60cb5f14c606d`  
		Last Modified: Tue, 23 Aug 2022 01:06:42 GMT  
		Size: 45.4 MB (45437317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efae4ef2c4c3e4f2858b9437a6dc47120ff2cd5821967db6f10e8ecb32d33cb1`  
		Last Modified: Tue, 23 Aug 2022 01:06:37 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:96b008f7a2747ff4f13160a962292dbd1ab678597a9228a76b3203f84a46bf1b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110228075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c98a17532608ae41772e2e92f9bb3d479794c37c9d9e045805c39568ce75607`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:00:31 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:00:32 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 02 Aug 2022 02:00:33 GMT
ENV OTP=otp24.1.5-3
# Tue, 02 Aug 2022 02:00:39 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 02 Aug 2022 02:00:40 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 02 Aug 2022 02:00:40 GMT
WORKDIR /opt/emqx
# Tue, 02 Aug 2022 02:00:41 GMT
USER emqx
# Tue, 02 Aug 2022 02:00:42 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 02 Aug 2022 02:00:43 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 02 Aug 2022 02:00:45 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 02 Aug 2022 02:00:45 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 02:00:46 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b8f37b5c2edc91fd1bdf8c28fd2b3da0c926ac40e82e7c59c7d03f310614f8`  
		Last Modified: Tue, 02 Aug 2022 02:01:24 GMT  
		Size: 2.6 MB (2558106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4cdc0cba9be243cb158e5751b728035148562b033d8ef1de765ca01f1a60dc`  
		Last Modified: Tue, 02 Aug 2022 02:01:28 GMT  
		Size: 38.8 MB (38806797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14c711205c5c7e4009eff2ea08ba336ac4598b6d1dfa6c1f7cf37089a5e727e`  
		Last Modified: Tue, 02 Aug 2022 02:01:28 GMT  
		Size: 38.8 MB (38807760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f05323f5f302f4d39168dba4ee48ae9ba98e3f6cd38134a5eaf7d8fe54dbc96`  
		Last Modified: Tue, 02 Aug 2022 02:01:24 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.4`

```console
$ docker pull emqx@sha256:00da7d91ed80191c10bcf0ddbddb8b7cfb6b87020752505e9b8c4b950a019a1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4.4` - linux; amd64

```console
$ docker pull emqx@sha256:96aaa084ede72e2f7063825961b9d4c33c7de7070a3eda430420f1aef1705d7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124813883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e05d42000605d355acff3be7bd2e91561b4d0a782bebfabd01d3d03810209333`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:05:55 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:05:56 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 23 Aug 2022 01:05:56 GMT
ENV OTP=otp24.1.5-3
# Tue, 23 Aug 2022 01:06:01 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 23 Aug 2022 01:06:08 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 23 Aug 2022 01:06:08 GMT
WORKDIR /opt/emqx
# Tue, 23 Aug 2022 01:06:08 GMT
USER emqx
# Tue, 23 Aug 2022 01:06:08 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 23 Aug 2022 01:06:08 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 23 Aug 2022 01:06:08 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 23 Aug 2022 01:06:09 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 01:06:09 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffe4803a256fc338d2725fd4a931050eb43f5804176597d989565411f39c0ba`  
		Last Modified: Tue, 23 Aug 2022 01:06:37 GMT  
		Size: 2.6 MB (2569463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8158f546cdbbf53444243363ab3ad5ffb0d011f3609b02f3e76f388262324cf`  
		Last Modified: Tue, 23 Aug 2022 01:06:42 GMT  
		Size: 45.4 MB (45424512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573b89c93de2f74dcf9490f92cbbf4e6ce0d5cf3a36113621de60cb5f14c606d`  
		Last Modified: Tue, 23 Aug 2022 01:06:42 GMT  
		Size: 45.4 MB (45437317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efae4ef2c4c3e4f2858b9437a6dc47120ff2cd5821967db6f10e8ecb32d33cb1`  
		Last Modified: Tue, 23 Aug 2022 01:06:37 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:96b008f7a2747ff4f13160a962292dbd1ab678597a9228a76b3203f84a46bf1b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110228075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c98a17532608ae41772e2e92f9bb3d479794c37c9d9e045805c39568ce75607`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:00:31 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:00:32 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 02 Aug 2022 02:00:33 GMT
ENV OTP=otp24.1.5-3
# Tue, 02 Aug 2022 02:00:39 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 02 Aug 2022 02:00:40 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 02 Aug 2022 02:00:40 GMT
WORKDIR /opt/emqx
# Tue, 02 Aug 2022 02:00:41 GMT
USER emqx
# Tue, 02 Aug 2022 02:00:42 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 02 Aug 2022 02:00:43 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 02 Aug 2022 02:00:45 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 02 Aug 2022 02:00:45 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 02:00:46 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b8f37b5c2edc91fd1bdf8c28fd2b3da0c926ac40e82e7c59c7d03f310614f8`  
		Last Modified: Tue, 02 Aug 2022 02:01:24 GMT  
		Size: 2.6 MB (2558106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4cdc0cba9be243cb158e5751b728035148562b033d8ef1de765ca01f1a60dc`  
		Last Modified: Tue, 02 Aug 2022 02:01:28 GMT  
		Size: 38.8 MB (38806797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14c711205c5c7e4009eff2ea08ba336ac4598b6d1dfa6c1f7cf37089a5e727e`  
		Last Modified: Tue, 02 Aug 2022 02:01:28 GMT  
		Size: 38.8 MB (38807760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f05323f5f302f4d39168dba4ee48ae9ba98e3f6cd38134a5eaf7d8fe54dbc96`  
		Last Modified: Tue, 02 Aug 2022 02:01:24 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:00da7d91ed80191c10bcf0ddbddb8b7cfb6b87020752505e9b8c4b950a019a1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:96aaa084ede72e2f7063825961b9d4c33c7de7070a3eda430420f1aef1705d7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124813883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e05d42000605d355acff3be7bd2e91561b4d0a782bebfabd01d3d03810209333`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:05:55 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:05:56 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 23 Aug 2022 01:05:56 GMT
ENV OTP=otp24.1.5-3
# Tue, 23 Aug 2022 01:06:01 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 23 Aug 2022 01:06:08 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 23 Aug 2022 01:06:08 GMT
WORKDIR /opt/emqx
# Tue, 23 Aug 2022 01:06:08 GMT
USER emqx
# Tue, 23 Aug 2022 01:06:08 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 23 Aug 2022 01:06:08 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 23 Aug 2022 01:06:08 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 23 Aug 2022 01:06:09 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 01:06:09 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffe4803a256fc338d2725fd4a931050eb43f5804176597d989565411f39c0ba`  
		Last Modified: Tue, 23 Aug 2022 01:06:37 GMT  
		Size: 2.6 MB (2569463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8158f546cdbbf53444243363ab3ad5ffb0d011f3609b02f3e76f388262324cf`  
		Last Modified: Tue, 23 Aug 2022 01:06:42 GMT  
		Size: 45.4 MB (45424512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573b89c93de2f74dcf9490f92cbbf4e6ce0d5cf3a36113621de60cb5f14c606d`  
		Last Modified: Tue, 23 Aug 2022 01:06:42 GMT  
		Size: 45.4 MB (45437317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efae4ef2c4c3e4f2858b9437a6dc47120ff2cd5821967db6f10e8ecb32d33cb1`  
		Last Modified: Tue, 23 Aug 2022 01:06:37 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:96b008f7a2747ff4f13160a962292dbd1ab678597a9228a76b3203f84a46bf1b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110228075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c98a17532608ae41772e2e92f9bb3d479794c37c9d9e045805c39568ce75607`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:00:31 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:00:32 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 02 Aug 2022 02:00:33 GMT
ENV OTP=otp24.1.5-3
# Tue, 02 Aug 2022 02:00:39 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 02 Aug 2022 02:00:40 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 02 Aug 2022 02:00:40 GMT
WORKDIR /opt/emqx
# Tue, 02 Aug 2022 02:00:41 GMT
USER emqx
# Tue, 02 Aug 2022 02:00:42 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 02 Aug 2022 02:00:43 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 02 Aug 2022 02:00:45 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 02 Aug 2022 02:00:45 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 02:00:46 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b8f37b5c2edc91fd1bdf8c28fd2b3da0c926ac40e82e7c59c7d03f310614f8`  
		Last Modified: Tue, 02 Aug 2022 02:01:24 GMT  
		Size: 2.6 MB (2558106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4cdc0cba9be243cb158e5751b728035148562b033d8ef1de765ca01f1a60dc`  
		Last Modified: Tue, 02 Aug 2022 02:01:28 GMT  
		Size: 38.8 MB (38806797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14c711205c5c7e4009eff2ea08ba336ac4598b6d1dfa6c1f7cf37089a5e727e`  
		Last Modified: Tue, 02 Aug 2022 02:01:28 GMT  
		Size: 38.8 MB (38807760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f05323f5f302f4d39168dba4ee48ae9ba98e3f6cd38134a5eaf7d8fe54dbc96`  
		Last Modified: Tue, 02 Aug 2022 02:01:24 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
