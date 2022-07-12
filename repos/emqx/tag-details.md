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
$ docker pull emqx@sha256:103824eb37afc831d17842ac74387a443db99d151019520a07f1373662209577
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
$ docker pull emqx@sha256:946e47e6ec5e3824d1e24158a1346cd7ceeed76286adc12e632652da786427dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110226385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fadbe16099c697c0e648ef7516872ab25b0d2c92440e5d358b0450eef617534a`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:53:51 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:53:51 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 12 Jul 2022 02:53:52 GMT
ENV OTP=otp24.1.5-3
# Tue, 12 Jul 2022 02:53:57 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 12 Jul 2022 02:53:59 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 12 Jul 2022 02:53:59 GMT
WORKDIR /opt/emqx
# Tue, 12 Jul 2022 02:54:00 GMT
USER emqx
# Tue, 12 Jul 2022 02:54:01 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 12 Jul 2022 02:54:02 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 12 Jul 2022 02:54:04 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 12 Jul 2022 02:54:04 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 02:54:05 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f655b2e505c1a8b007de0d707e1d4eca7b4b2842b22189a1534abeb9459d3c44`  
		Last Modified: Tue, 12 Jul 2022 02:54:42 GMT  
		Size: 2.6 MB (2556499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d337f96eb101b6de0343aafd1d51c0151db92756ef3e3a306385bd59e1ed325`  
		Last Modified: Tue, 12 Jul 2022 02:54:46 GMT  
		Size: 38.8 MB (38806784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc27f862187de8b2c5f81f5df47896a86f5ceb566b2be89c3934ca57436fd5c9`  
		Last Modified: Tue, 12 Jul 2022 02:54:46 GMT  
		Size: 38.8 MB (38807769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0169a24f38847390df2abbab3af160e2c10462a458c790a6618ea162c05c2bd9`  
		Last Modified: Tue, 12 Jul 2022 02:54:41 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3`

```console
$ docker pull emqx@sha256:6e2dd7be3dd52e004490d0891d4bda96a1a1f93e59cbab58268c25ebf7b97706
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
$ docker pull emqx@sha256:cfaeb3aa69e8e840038f1416552faee26a36755510b7f5561e3993394c42948b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101935679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:170d6323d78024b1b5f9cfab283f9fd9d6baae8b3c2fc2f61206faa7a66dba83`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 12 Jul 2022 00:41:02 GMT
ADD file:d6b43ca12a2cc7f73a66ace962f04878f02eab9345172028d77c21d3dc94fe0c in / 
# Tue, 12 Jul 2022 00:41:03 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:53:26 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:53:26 GMT
ENV EMQX_VERSION=4.3.15
# Tue, 12 Jul 2022 02:53:31 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="8f44386aebf472297377d7b6b595638f323227347047d5278dce9c0cd04963bc"; fi;     if [ ${arch} = "arm64" ]; then sha256="b0094028d388684136be975c574d98295205dd5a343045f76f423a109535e016"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 12 Jul 2022 02:53:32 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 12 Jul 2022 02:53:33 GMT
WORKDIR /opt/emqx
# Tue, 12 Jul 2022 02:53:33 GMT
USER emqx
# Tue, 12 Jul 2022 02:53:34 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 12 Jul 2022 02:53:35 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 12 Jul 2022 02:53:37 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Tue, 12 Jul 2022 02:53:37 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 02:53:38 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:8bd5501da4f4b37ad7488bd0eafa32d8927de3bf1e32747545810f2ca65429ed`  
		Last Modified: Tue, 12 Jul 2022 00:47:14 GMT  
		Size: 25.9 MB (25914236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06bcca172041b03050fc3e47d3b1b530a124253b8e1dfab8a8c79c563b64faf`  
		Last Modified: Tue, 12 Jul 2022 02:54:27 GMT  
		Size: 4.5 MB (4485490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3fd61f596e7e568efa978a3fc177d2fd3105d7ad53be4a994de47cd433ad487`  
		Last Modified: Tue, 12 Jul 2022 02:54:30 GMT  
		Size: 35.8 MB (35761659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ead8ab9fe40a15f7b30ecf82e069bf6667ab4e999d911c46073a9024d71f3`  
		Last Modified: Tue, 12 Jul 2022 02:54:30 GMT  
		Size: 35.8 MB (35773254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e065ee88142d7c017b52f1199b9b6085abb567ade22dd107bbb997755f661ed7`  
		Last Modified: Tue, 12 Jul 2022 02:54:26 GMT  
		Size: 1.0 KB (1040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3.15`

```console
$ docker pull emqx@sha256:6e2dd7be3dd52e004490d0891d4bda96a1a1f93e59cbab58268c25ebf7b97706
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
$ docker pull emqx@sha256:cfaeb3aa69e8e840038f1416552faee26a36755510b7f5561e3993394c42948b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101935679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:170d6323d78024b1b5f9cfab283f9fd9d6baae8b3c2fc2f61206faa7a66dba83`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 12 Jul 2022 00:41:02 GMT
ADD file:d6b43ca12a2cc7f73a66ace962f04878f02eab9345172028d77c21d3dc94fe0c in / 
# Tue, 12 Jul 2022 00:41:03 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:53:26 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:53:26 GMT
ENV EMQX_VERSION=4.3.15
# Tue, 12 Jul 2022 02:53:31 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="8f44386aebf472297377d7b6b595638f323227347047d5278dce9c0cd04963bc"; fi;     if [ ${arch} = "arm64" ]; then sha256="b0094028d388684136be975c574d98295205dd5a343045f76f423a109535e016"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 12 Jul 2022 02:53:32 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 12 Jul 2022 02:53:33 GMT
WORKDIR /opt/emqx
# Tue, 12 Jul 2022 02:53:33 GMT
USER emqx
# Tue, 12 Jul 2022 02:53:34 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 12 Jul 2022 02:53:35 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 12 Jul 2022 02:53:37 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Tue, 12 Jul 2022 02:53:37 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 02:53:38 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:8bd5501da4f4b37ad7488bd0eafa32d8927de3bf1e32747545810f2ca65429ed`  
		Last Modified: Tue, 12 Jul 2022 00:47:14 GMT  
		Size: 25.9 MB (25914236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06bcca172041b03050fc3e47d3b1b530a124253b8e1dfab8a8c79c563b64faf`  
		Last Modified: Tue, 12 Jul 2022 02:54:27 GMT  
		Size: 4.5 MB (4485490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3fd61f596e7e568efa978a3fc177d2fd3105d7ad53be4a994de47cd433ad487`  
		Last Modified: Tue, 12 Jul 2022 02:54:30 GMT  
		Size: 35.8 MB (35761659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ead8ab9fe40a15f7b30ecf82e069bf6667ab4e999d911c46073a9024d71f3`  
		Last Modified: Tue, 12 Jul 2022 02:54:30 GMT  
		Size: 35.8 MB (35773254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e065ee88142d7c017b52f1199b9b6085abb567ade22dd107bbb997755f661ed7`  
		Last Modified: Tue, 12 Jul 2022 02:54:26 GMT  
		Size: 1.0 KB (1040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:103824eb37afc831d17842ac74387a443db99d151019520a07f1373662209577
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
$ docker pull emqx@sha256:946e47e6ec5e3824d1e24158a1346cd7ceeed76286adc12e632652da786427dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110226385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fadbe16099c697c0e648ef7516872ab25b0d2c92440e5d358b0450eef617534a`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:53:51 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:53:51 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 12 Jul 2022 02:53:52 GMT
ENV OTP=otp24.1.5-3
# Tue, 12 Jul 2022 02:53:57 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 12 Jul 2022 02:53:59 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 12 Jul 2022 02:53:59 GMT
WORKDIR /opt/emqx
# Tue, 12 Jul 2022 02:54:00 GMT
USER emqx
# Tue, 12 Jul 2022 02:54:01 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 12 Jul 2022 02:54:02 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 12 Jul 2022 02:54:04 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 12 Jul 2022 02:54:04 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 02:54:05 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f655b2e505c1a8b007de0d707e1d4eca7b4b2842b22189a1534abeb9459d3c44`  
		Last Modified: Tue, 12 Jul 2022 02:54:42 GMT  
		Size: 2.6 MB (2556499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d337f96eb101b6de0343aafd1d51c0151db92756ef3e3a306385bd59e1ed325`  
		Last Modified: Tue, 12 Jul 2022 02:54:46 GMT  
		Size: 38.8 MB (38806784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc27f862187de8b2c5f81f5df47896a86f5ceb566b2be89c3934ca57436fd5c9`  
		Last Modified: Tue, 12 Jul 2022 02:54:46 GMT  
		Size: 38.8 MB (38807769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0169a24f38847390df2abbab3af160e2c10462a458c790a6618ea162c05c2bd9`  
		Last Modified: Tue, 12 Jul 2022 02:54:41 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.4`

```console
$ docker pull emqx@sha256:103824eb37afc831d17842ac74387a443db99d151019520a07f1373662209577
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
$ docker pull emqx@sha256:946e47e6ec5e3824d1e24158a1346cd7ceeed76286adc12e632652da786427dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110226385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fadbe16099c697c0e648ef7516872ab25b0d2c92440e5d358b0450eef617534a`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:53:51 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:53:51 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 12 Jul 2022 02:53:52 GMT
ENV OTP=otp24.1.5-3
# Tue, 12 Jul 2022 02:53:57 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 12 Jul 2022 02:53:59 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 12 Jul 2022 02:53:59 GMT
WORKDIR /opt/emqx
# Tue, 12 Jul 2022 02:54:00 GMT
USER emqx
# Tue, 12 Jul 2022 02:54:01 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 12 Jul 2022 02:54:02 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 12 Jul 2022 02:54:04 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 12 Jul 2022 02:54:04 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 02:54:05 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f655b2e505c1a8b007de0d707e1d4eca7b4b2842b22189a1534abeb9459d3c44`  
		Last Modified: Tue, 12 Jul 2022 02:54:42 GMT  
		Size: 2.6 MB (2556499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d337f96eb101b6de0343aafd1d51c0151db92756ef3e3a306385bd59e1ed325`  
		Last Modified: Tue, 12 Jul 2022 02:54:46 GMT  
		Size: 38.8 MB (38806784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc27f862187de8b2c5f81f5df47896a86f5ceb566b2be89c3934ca57436fd5c9`  
		Last Modified: Tue, 12 Jul 2022 02:54:46 GMT  
		Size: 38.8 MB (38807769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0169a24f38847390df2abbab3af160e2c10462a458c790a6618ea162c05c2bd9`  
		Last Modified: Tue, 12 Jul 2022 02:54:41 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:103824eb37afc831d17842ac74387a443db99d151019520a07f1373662209577
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
$ docker pull emqx@sha256:946e47e6ec5e3824d1e24158a1346cd7ceeed76286adc12e632652da786427dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110226385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fadbe16099c697c0e648ef7516872ab25b0d2c92440e5d358b0450eef617534a`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:53:51 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:53:51 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 12 Jul 2022 02:53:52 GMT
ENV OTP=otp24.1.5-3
# Tue, 12 Jul 2022 02:53:57 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 12 Jul 2022 02:53:59 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 12 Jul 2022 02:53:59 GMT
WORKDIR /opt/emqx
# Tue, 12 Jul 2022 02:54:00 GMT
USER emqx
# Tue, 12 Jul 2022 02:54:01 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 12 Jul 2022 02:54:02 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 12 Jul 2022 02:54:04 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 12 Jul 2022 02:54:04 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 02:54:05 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f655b2e505c1a8b007de0d707e1d4eca7b4b2842b22189a1534abeb9459d3c44`  
		Last Modified: Tue, 12 Jul 2022 02:54:42 GMT  
		Size: 2.6 MB (2556499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d337f96eb101b6de0343aafd1d51c0151db92756ef3e3a306385bd59e1ed325`  
		Last Modified: Tue, 12 Jul 2022 02:54:46 GMT  
		Size: 38.8 MB (38806784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc27f862187de8b2c5f81f5df47896a86f5ceb566b2be89c3934ca57436fd5c9`  
		Last Modified: Tue, 12 Jul 2022 02:54:46 GMT  
		Size: 38.8 MB (38807769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0169a24f38847390df2abbab3af160e2c10462a458c790a6618ea162c05c2bd9`  
		Last Modified: Tue, 12 Jul 2022 02:54:41 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
