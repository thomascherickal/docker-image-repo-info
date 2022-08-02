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
$ docker pull emqx@sha256:38ab55573eca4013d9f61a6ad551712e7b8368245dc0d4eddb042a580f1b663f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:f9fec4a8fdcfbea5d1e206c6f6f93821c1f75be0acacdba0e9d47d768ba9b19f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124797693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8813118ffe0271a3b1808813a2f915fa7187a256af89f71ca5722a16601a26a7`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 03:02:11 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 03:02:12 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 12 Jul 2022 03:02:12 GMT
ENV OTP=otp24.1.5-3
# Tue, 12 Jul 2022 03:02:16 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 12 Jul 2022 03:02:22 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 12 Jul 2022 03:02:22 GMT
WORKDIR /opt/emqx
# Tue, 12 Jul 2022 03:02:22 GMT
USER emqx
# Tue, 12 Jul 2022 03:02:22 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 12 Jul 2022 03:02:22 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 12 Jul 2022 03:02:23 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 12 Jul 2022 03:02:23 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 03:02:23 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cff3eb396acb2fd5e98bdc798f91771dd05a046ea2628d4ca2a9d51eb3582e`  
		Last Modified: Tue, 12 Jul 2022 03:02:50 GMT  
		Size: 2.6 MB (2568127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b62cb68dba5bbabb0dff2d83fa346466b4b515edcb327e52a510f3cc6f4b6c`  
		Last Modified: Tue, 12 Jul 2022 03:02:55 GMT  
		Size: 45.4 MB (45424520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651b218fc74ff466641a9ebd7b9ad25a5badaff2f34ce6a038d7ebc1d8cdc1f6`  
		Last Modified: Tue, 12 Jul 2022 03:02:55 GMT  
		Size: 45.4 MB (45437330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60b97afe5179ead8b01aa526bf6b0b82ef9d3ba3750b58b77276d984eea4858`  
		Last Modified: Tue, 12 Jul 2022 03:02:49 GMT  
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
$ docker pull emqx@sha256:6c9b2b378b268094d212149a0e1eafc62d84c19d416b2a52bd15a6f8cc0e998b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.3` - linux; amd64

```console
$ docker pull emqx@sha256:ad0fd8ce97334b5cd06d604dd3cf1f7d6d48d0d2b108ba5ce3f8401e11ec29b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.9 MB (103864023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e1ed557cd0e426acb9577f04fcd6768c58f81da74de0ae24403306a0c77351b`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:32 GMT
ADD file:7f2320197e75c5169402827ce0c47d93629331875d76b9f0ddd389244747eccd in / 
# Tue, 12 Jul 2022 01:20:33 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 03:01:52 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 03:01:53 GMT
ENV EMQX_VERSION=4.3.15
# Tue, 12 Jul 2022 03:01:57 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="8f44386aebf472297377d7b6b595638f323227347047d5278dce9c0cd04963bc"; fi;     if [ ${arch} = "arm64" ]; then sha256="b0094028d388684136be975c574d98295205dd5a343045f76f423a109535e016"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 12 Jul 2022 03:02:02 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 12 Jul 2022 03:02:03 GMT
WORKDIR /opt/emqx
# Tue, 12 Jul 2022 03:02:03 GMT
USER emqx
# Tue, 12 Jul 2022 03:02:03 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 12 Jul 2022 03:02:03 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 12 Jul 2022 03:02:03 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Tue, 12 Jul 2022 03:02:03 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 03:02:03 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:ac2fb615420c18b61e0693f2569a3d38e3b9b58456b691bac44405e08389a591`  
		Last Modified: Tue, 12 Jul 2022 01:25:22 GMT  
		Size: 27.1 MB (27139850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b683e15c025523a4658ede5f1e88796aed7e4d630cf5fd9c537b59aa22f4cc14`  
		Last Modified: Tue, 12 Jul 2022 03:02:36 GMT  
		Size: 4.6 MB (4610285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408f6001682030162facb14d46f989f9e2b891a4a1fb73227932cb8806a73f42`  
		Last Modified: Tue, 12 Jul 2022 03:02:40 GMT  
		Size: 36.1 MB (36056949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62be2af98cb33331adf8eea1e326858ae79ce5c5d4f59521ad09066b57c2fdd2`  
		Last Modified: Tue, 12 Jul 2022 03:02:40 GMT  
		Size: 36.1 MB (36055899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7731a73654ac7e5570dac219d712a3d316b4d3cc3f15ea0204d0763b1811bd`  
		Last Modified: Tue, 12 Jul 2022 03:02:36 GMT  
		Size: 1.0 KB (1040 bytes)  
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
$ docker pull emqx@sha256:6c9b2b378b268094d212149a0e1eafc62d84c19d416b2a52bd15a6f8cc0e998b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.3.15` - linux; amd64

```console
$ docker pull emqx@sha256:ad0fd8ce97334b5cd06d604dd3cf1f7d6d48d0d2b108ba5ce3f8401e11ec29b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.9 MB (103864023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e1ed557cd0e426acb9577f04fcd6768c58f81da74de0ae24403306a0c77351b`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:32 GMT
ADD file:7f2320197e75c5169402827ce0c47d93629331875d76b9f0ddd389244747eccd in / 
# Tue, 12 Jul 2022 01:20:33 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 03:01:52 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 03:01:53 GMT
ENV EMQX_VERSION=4.3.15
# Tue, 12 Jul 2022 03:01:57 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="8f44386aebf472297377d7b6b595638f323227347047d5278dce9c0cd04963bc"; fi;     if [ ${arch} = "arm64" ]; then sha256="b0094028d388684136be975c574d98295205dd5a343045f76f423a109535e016"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 12 Jul 2022 03:02:02 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 12 Jul 2022 03:02:03 GMT
WORKDIR /opt/emqx
# Tue, 12 Jul 2022 03:02:03 GMT
USER emqx
# Tue, 12 Jul 2022 03:02:03 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 12 Jul 2022 03:02:03 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 12 Jul 2022 03:02:03 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Tue, 12 Jul 2022 03:02:03 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 03:02:03 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:ac2fb615420c18b61e0693f2569a3d38e3b9b58456b691bac44405e08389a591`  
		Last Modified: Tue, 12 Jul 2022 01:25:22 GMT  
		Size: 27.1 MB (27139850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b683e15c025523a4658ede5f1e88796aed7e4d630cf5fd9c537b59aa22f4cc14`  
		Last Modified: Tue, 12 Jul 2022 03:02:36 GMT  
		Size: 4.6 MB (4610285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408f6001682030162facb14d46f989f9e2b891a4a1fb73227932cb8806a73f42`  
		Last Modified: Tue, 12 Jul 2022 03:02:40 GMT  
		Size: 36.1 MB (36056949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62be2af98cb33331adf8eea1e326858ae79ce5c5d4f59521ad09066b57c2fdd2`  
		Last Modified: Tue, 12 Jul 2022 03:02:40 GMT  
		Size: 36.1 MB (36055899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7731a73654ac7e5570dac219d712a3d316b4d3cc3f15ea0204d0763b1811bd`  
		Last Modified: Tue, 12 Jul 2022 03:02:36 GMT  
		Size: 1.0 KB (1040 bytes)  
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
$ docker pull emqx@sha256:38ab55573eca4013d9f61a6ad551712e7b8368245dc0d4eddb042a580f1b663f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:f9fec4a8fdcfbea5d1e206c6f6f93821c1f75be0acacdba0e9d47d768ba9b19f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124797693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8813118ffe0271a3b1808813a2f915fa7187a256af89f71ca5722a16601a26a7`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 03:02:11 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 03:02:12 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 12 Jul 2022 03:02:12 GMT
ENV OTP=otp24.1.5-3
# Tue, 12 Jul 2022 03:02:16 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 12 Jul 2022 03:02:22 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 12 Jul 2022 03:02:22 GMT
WORKDIR /opt/emqx
# Tue, 12 Jul 2022 03:02:22 GMT
USER emqx
# Tue, 12 Jul 2022 03:02:22 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 12 Jul 2022 03:02:22 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 12 Jul 2022 03:02:23 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 12 Jul 2022 03:02:23 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 03:02:23 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cff3eb396acb2fd5e98bdc798f91771dd05a046ea2628d4ca2a9d51eb3582e`  
		Last Modified: Tue, 12 Jul 2022 03:02:50 GMT  
		Size: 2.6 MB (2568127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b62cb68dba5bbabb0dff2d83fa346466b4b515edcb327e52a510f3cc6f4b6c`  
		Last Modified: Tue, 12 Jul 2022 03:02:55 GMT  
		Size: 45.4 MB (45424520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651b218fc74ff466641a9ebd7b9ad25a5badaff2f34ce6a038d7ebc1d8cdc1f6`  
		Last Modified: Tue, 12 Jul 2022 03:02:55 GMT  
		Size: 45.4 MB (45437330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60b97afe5179ead8b01aa526bf6b0b82ef9d3ba3750b58b77276d984eea4858`  
		Last Modified: Tue, 12 Jul 2022 03:02:49 GMT  
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
$ docker pull emqx@sha256:38ab55573eca4013d9f61a6ad551712e7b8368245dc0d4eddb042a580f1b663f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4.4` - linux; amd64

```console
$ docker pull emqx@sha256:f9fec4a8fdcfbea5d1e206c6f6f93821c1f75be0acacdba0e9d47d768ba9b19f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124797693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8813118ffe0271a3b1808813a2f915fa7187a256af89f71ca5722a16601a26a7`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 03:02:11 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 03:02:12 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 12 Jul 2022 03:02:12 GMT
ENV OTP=otp24.1.5-3
# Tue, 12 Jul 2022 03:02:16 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 12 Jul 2022 03:02:22 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 12 Jul 2022 03:02:22 GMT
WORKDIR /opt/emqx
# Tue, 12 Jul 2022 03:02:22 GMT
USER emqx
# Tue, 12 Jul 2022 03:02:22 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 12 Jul 2022 03:02:22 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 12 Jul 2022 03:02:23 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 12 Jul 2022 03:02:23 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 03:02:23 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cff3eb396acb2fd5e98bdc798f91771dd05a046ea2628d4ca2a9d51eb3582e`  
		Last Modified: Tue, 12 Jul 2022 03:02:50 GMT  
		Size: 2.6 MB (2568127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b62cb68dba5bbabb0dff2d83fa346466b4b515edcb327e52a510f3cc6f4b6c`  
		Last Modified: Tue, 12 Jul 2022 03:02:55 GMT  
		Size: 45.4 MB (45424520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651b218fc74ff466641a9ebd7b9ad25a5badaff2f34ce6a038d7ebc1d8cdc1f6`  
		Last Modified: Tue, 12 Jul 2022 03:02:55 GMT  
		Size: 45.4 MB (45437330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60b97afe5179ead8b01aa526bf6b0b82ef9d3ba3750b58b77276d984eea4858`  
		Last Modified: Tue, 12 Jul 2022 03:02:49 GMT  
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
$ docker pull emqx@sha256:38ab55573eca4013d9f61a6ad551712e7b8368245dc0d4eddb042a580f1b663f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:f9fec4a8fdcfbea5d1e206c6f6f93821c1f75be0acacdba0e9d47d768ba9b19f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124797693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8813118ffe0271a3b1808813a2f915fa7187a256af89f71ca5722a16601a26a7`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 03:02:11 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 03:02:12 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 12 Jul 2022 03:02:12 GMT
ENV OTP=otp24.1.5-3
# Tue, 12 Jul 2022 03:02:16 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 12 Jul 2022 03:02:22 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 12 Jul 2022 03:02:22 GMT
WORKDIR /opt/emqx
# Tue, 12 Jul 2022 03:02:22 GMT
USER emqx
# Tue, 12 Jul 2022 03:02:22 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 12 Jul 2022 03:02:22 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 12 Jul 2022 03:02:23 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 12 Jul 2022 03:02:23 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 03:02:23 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cff3eb396acb2fd5e98bdc798f91771dd05a046ea2628d4ca2a9d51eb3582e`  
		Last Modified: Tue, 12 Jul 2022 03:02:50 GMT  
		Size: 2.6 MB (2568127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b62cb68dba5bbabb0dff2d83fa346466b4b515edcb327e52a510f3cc6f4b6c`  
		Last Modified: Tue, 12 Jul 2022 03:02:55 GMT  
		Size: 45.4 MB (45424520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651b218fc74ff466641a9ebd7b9ad25a5badaff2f34ce6a038d7ebc1d8cdc1f6`  
		Last Modified: Tue, 12 Jul 2022 03:02:55 GMT  
		Size: 45.4 MB (45437330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60b97afe5179ead8b01aa526bf6b0b82ef9d3ba3750b58b77276d984eea4858`  
		Last Modified: Tue, 12 Jul 2022 03:02:49 GMT  
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
