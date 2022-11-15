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
$ docker pull emqx@sha256:cb6daea8f3ec82829550982f158cf8cab692f9f4132deae6f5fb313d13e1ed7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:f356cc67a765ca1a8f061357a4f2a642972013633aa430dabb63714d27a025ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124846626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:690157a23d6d16f7a0018e067eb70e3dd47d21343f1ab306b016b698618820b8`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:14:37 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:14:37 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 15 Nov 2022 12:14:37 GMT
ENV OTP=otp24.1.5-3
# Tue, 15 Nov 2022 12:14:42 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 15 Nov 2022 12:14:47 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 15 Nov 2022 12:14:48 GMT
WORKDIR /opt/emqx
# Tue, 15 Nov 2022 12:14:48 GMT
USER emqx
# Tue, 15 Nov 2022 12:14:48 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 15 Nov 2022 12:14:48 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 15 Nov 2022 12:14:48 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 15 Nov 2022 12:14:48 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 12:14:48 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9361f46d474c278613330bf20b7b1264c2eec81c3e1f05e78b21aa201437a7`  
		Last Modified: Tue, 15 Nov 2022 12:15:15 GMT  
		Size: 2.6 MB (2571046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f847ee13842a669d2f625effb83a707e818d3cb509e2f4eed1ce3a7cd79db896`  
		Last Modified: Tue, 15 Nov 2022 12:15:20 GMT  
		Size: 45.4 MB (45424513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0fe5c47919417828878227ee16596985e496752ae09305250f4553c19fb83d`  
		Last Modified: Tue, 15 Nov 2022 12:15:20 GMT  
		Size: 45.4 MB (45437332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fb804a2f0e054f72cf8ec813e7913c1ef5fa5099d7c163aacd340aca87dd6c`  
		Last Modified: Tue, 15 Nov 2022 12:15:14 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:b96eb9baf9f59f5524f82adfbe01e9ef5c01e081bb4b7b61847de59a7ad562fb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110236571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b6eebb68d3555822f6610bc02400972790c4e0f2bae2ba0b827e1618e38ac76`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:13:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:13:29 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 15 Nov 2022 06:13:29 GMT
ENV OTP=otp24.1.5-3
# Tue, 15 Nov 2022 06:13:32 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 15 Nov 2022 06:13:36 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 15 Nov 2022 06:13:37 GMT
WORKDIR /opt/emqx
# Tue, 15 Nov 2022 06:13:37 GMT
USER emqx
# Tue, 15 Nov 2022 06:13:37 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 15 Nov 2022 06:13:37 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 15 Nov 2022 06:13:37 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 15 Nov 2022 06:13:37 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 06:13:37 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad108ef5d5673e32622aa158fbc152df7e8c340c7f4e79efffecd4c5d6c2a7be`  
		Last Modified: Tue, 15 Nov 2022 06:14:09 GMT  
		Size: 2.6 MB (2560816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96042e2ccd2609d9b280266d2cc3063aab600802b597ec18244c2761f3af513`  
		Last Modified: Tue, 15 Nov 2022 06:14:11 GMT  
		Size: 38.8 MB (38806727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432b8a52dff2f8fc12cecf2988e77261a173d791f10a1ccedb107ace30b8fdf0`  
		Last Modified: Tue, 15 Nov 2022 06:14:11 GMT  
		Size: 38.8 MB (38807317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4504a627c078e5f88f9616bd61b3f0074e95a846d4bee00e1e4f6024bb61244`  
		Last Modified: Tue, 15 Nov 2022 06:14:08 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3`

```console
$ docker pull emqx@sha256:12ab8526f35fd84a33ca2f9ce56162054a8184d4a6b9505424489159ff1d86d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.3` - linux; amd64

```console
$ docker pull emqx@sha256:5dbeffef0db52adbdfdc3175bf110ae5397765651d0ff26c6f4f1b00aab1f096
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.9 MB (103866571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dd06ed84996138dedd11b022ae9566327d16d15c9c1f191814a1461c45561df`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:14 GMT
ADD file:9461639b945ced6fb6164491a7e0131261a1b7d69264cce516e75c71e4df22d2 in / 
# Tue, 15 Nov 2022 04:05:14 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:14:14 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:14:14 GMT
ENV EMQX_VERSION=4.3.15
# Tue, 15 Nov 2022 12:14:18 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="8f44386aebf472297377d7b6b595638f323227347047d5278dce9c0cd04963bc"; fi;     if [ ${arch} = "arm64" ]; then sha256="b0094028d388684136be975c574d98295205dd5a343045f76f423a109535e016"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 15 Nov 2022 12:14:24 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 15 Nov 2022 12:14:24 GMT
WORKDIR /opt/emqx
# Tue, 15 Nov 2022 12:14:24 GMT
USER emqx
# Tue, 15 Nov 2022 12:14:24 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 15 Nov 2022 12:14:25 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 15 Nov 2022 12:14:25 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Tue, 15 Nov 2022 12:14:25 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 12:14:25 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:32820e52a00eb22dc76d70d992be7082cd24b636cfb597ff3951d29a821b46b9`  
		Last Modified: Tue, 15 Nov 2022 04:09:26 GMT  
		Size: 27.1 MB (27140332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a034d47f6faf5df0c00edec91ebcd75cc95132acb38b2ee8646b151d04075a52`  
		Last Modified: Tue, 15 Nov 2022 12:15:02 GMT  
		Size: 4.6 MB (4612387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6649304de99a4b7be85a78987d47dfcb89baac2788b2b3d38f1133fff151c61d`  
		Last Modified: Tue, 15 Nov 2022 12:15:05 GMT  
		Size: 36.1 MB (36056922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1096265ccb90946221ffb9dd0f2c8d92887a50b1c09713b9b21985f7a08932`  
		Last Modified: Tue, 15 Nov 2022 12:15:06 GMT  
		Size: 36.1 MB (36055890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9dff1d293cd0c1d668772e79461b980d6281b7a2da60ea2e9f3ca1f9069cc8`  
		Last Modified: Tue, 15 Nov 2022 12:15:01 GMT  
		Size: 1.0 KB (1040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.3` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:41d0b865a8ae856f8b872d7debd6cea5c3b88b5305741b6123aea500a084b2e4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101941144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5db10c6572b2573057a3c57cd2a00999bd57ea1cfedb02e4f4c5bb7435b3d304`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:34 GMT
ADD file:aaead8e4dd08d41c8d1692bbe76b673119289836428e1f713ca550c2468711ac in / 
# Tue, 15 Nov 2022 01:41:34 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:13:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:13:13 GMT
ENV EMQX_VERSION=4.3.15
# Tue, 15 Nov 2022 06:13:16 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="8f44386aebf472297377d7b6b595638f323227347047d5278dce9c0cd04963bc"; fi;     if [ ${arch} = "arm64" ]; then sha256="b0094028d388684136be975c574d98295205dd5a343045f76f423a109535e016"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 15 Nov 2022 06:13:20 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 15 Nov 2022 06:13:21 GMT
WORKDIR /opt/emqx
# Tue, 15 Nov 2022 06:13:21 GMT
USER emqx
# Tue, 15 Nov 2022 06:13:21 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 15 Nov 2022 06:13:21 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 15 Nov 2022 06:13:21 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Tue, 15 Nov 2022 06:13:21 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 06:13:21 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:cc457132e077d684a6cecad3331c35341d814c5d364f3cf24d698a6d8e76d0e7`  
		Last Modified: Tue, 15 Nov 2022 01:45:13 GMT  
		Size: 25.9 MB (25914924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d027abecdd5af35e9a16c44518f0617af3a9b80b03d0fac7e90d16f1de3c6100`  
		Last Modified: Tue, 15 Nov 2022 06:13:52 GMT  
		Size: 4.5 MB (4490492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35bd45a31f146e3d3b0af0147d4d492d45872372c83ebdc32e15129498c485e`  
		Last Modified: Tue, 15 Nov 2022 06:13:58 GMT  
		Size: 35.8 MB (35761772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6749b66844622561c7c7de00810191fad38032463dbd3288e9a4fdbd1323e41`  
		Last Modified: Tue, 15 Nov 2022 06:13:55 GMT  
		Size: 35.8 MB (35772916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21ae72d82eb83adc78c809979e9c1b9290e137e25e0d5bb0adb275fe6db6681`  
		Last Modified: Tue, 15 Nov 2022 06:13:51 GMT  
		Size: 1.0 KB (1040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3.15`

```console
$ docker pull emqx@sha256:12ab8526f35fd84a33ca2f9ce56162054a8184d4a6b9505424489159ff1d86d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.3.15` - linux; amd64

```console
$ docker pull emqx@sha256:5dbeffef0db52adbdfdc3175bf110ae5397765651d0ff26c6f4f1b00aab1f096
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.9 MB (103866571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dd06ed84996138dedd11b022ae9566327d16d15c9c1f191814a1461c45561df`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:14 GMT
ADD file:9461639b945ced6fb6164491a7e0131261a1b7d69264cce516e75c71e4df22d2 in / 
# Tue, 15 Nov 2022 04:05:14 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:14:14 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:14:14 GMT
ENV EMQX_VERSION=4.3.15
# Tue, 15 Nov 2022 12:14:18 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="8f44386aebf472297377d7b6b595638f323227347047d5278dce9c0cd04963bc"; fi;     if [ ${arch} = "arm64" ]; then sha256="b0094028d388684136be975c574d98295205dd5a343045f76f423a109535e016"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 15 Nov 2022 12:14:24 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 15 Nov 2022 12:14:24 GMT
WORKDIR /opt/emqx
# Tue, 15 Nov 2022 12:14:24 GMT
USER emqx
# Tue, 15 Nov 2022 12:14:24 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 15 Nov 2022 12:14:25 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 15 Nov 2022 12:14:25 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Tue, 15 Nov 2022 12:14:25 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 12:14:25 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:32820e52a00eb22dc76d70d992be7082cd24b636cfb597ff3951d29a821b46b9`  
		Last Modified: Tue, 15 Nov 2022 04:09:26 GMT  
		Size: 27.1 MB (27140332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a034d47f6faf5df0c00edec91ebcd75cc95132acb38b2ee8646b151d04075a52`  
		Last Modified: Tue, 15 Nov 2022 12:15:02 GMT  
		Size: 4.6 MB (4612387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6649304de99a4b7be85a78987d47dfcb89baac2788b2b3d38f1133fff151c61d`  
		Last Modified: Tue, 15 Nov 2022 12:15:05 GMT  
		Size: 36.1 MB (36056922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1096265ccb90946221ffb9dd0f2c8d92887a50b1c09713b9b21985f7a08932`  
		Last Modified: Tue, 15 Nov 2022 12:15:06 GMT  
		Size: 36.1 MB (36055890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9dff1d293cd0c1d668772e79461b980d6281b7a2da60ea2e9f3ca1f9069cc8`  
		Last Modified: Tue, 15 Nov 2022 12:15:01 GMT  
		Size: 1.0 KB (1040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.3.15` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:41d0b865a8ae856f8b872d7debd6cea5c3b88b5305741b6123aea500a084b2e4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101941144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5db10c6572b2573057a3c57cd2a00999bd57ea1cfedb02e4f4c5bb7435b3d304`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:34 GMT
ADD file:aaead8e4dd08d41c8d1692bbe76b673119289836428e1f713ca550c2468711ac in / 
# Tue, 15 Nov 2022 01:41:34 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:13:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:13:13 GMT
ENV EMQX_VERSION=4.3.15
# Tue, 15 Nov 2022 06:13:16 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="8f44386aebf472297377d7b6b595638f323227347047d5278dce9c0cd04963bc"; fi;     if [ ${arch} = "arm64" ]; then sha256="b0094028d388684136be975c574d98295205dd5a343045f76f423a109535e016"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 15 Nov 2022 06:13:20 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 15 Nov 2022 06:13:21 GMT
WORKDIR /opt/emqx
# Tue, 15 Nov 2022 06:13:21 GMT
USER emqx
# Tue, 15 Nov 2022 06:13:21 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 15 Nov 2022 06:13:21 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 15 Nov 2022 06:13:21 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Tue, 15 Nov 2022 06:13:21 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 06:13:21 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:cc457132e077d684a6cecad3331c35341d814c5d364f3cf24d698a6d8e76d0e7`  
		Last Modified: Tue, 15 Nov 2022 01:45:13 GMT  
		Size: 25.9 MB (25914924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d027abecdd5af35e9a16c44518f0617af3a9b80b03d0fac7e90d16f1de3c6100`  
		Last Modified: Tue, 15 Nov 2022 06:13:52 GMT  
		Size: 4.5 MB (4490492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35bd45a31f146e3d3b0af0147d4d492d45872372c83ebdc32e15129498c485e`  
		Last Modified: Tue, 15 Nov 2022 06:13:58 GMT  
		Size: 35.8 MB (35761772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6749b66844622561c7c7de00810191fad38032463dbd3288e9a4fdbd1323e41`  
		Last Modified: Tue, 15 Nov 2022 06:13:55 GMT  
		Size: 35.8 MB (35772916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21ae72d82eb83adc78c809979e9c1b9290e137e25e0d5bb0adb275fe6db6681`  
		Last Modified: Tue, 15 Nov 2022 06:13:51 GMT  
		Size: 1.0 KB (1040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:cb6daea8f3ec82829550982f158cf8cab692f9f4132deae6f5fb313d13e1ed7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:f356cc67a765ca1a8f061357a4f2a642972013633aa430dabb63714d27a025ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124846626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:690157a23d6d16f7a0018e067eb70e3dd47d21343f1ab306b016b698618820b8`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:14:37 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:14:37 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 15 Nov 2022 12:14:37 GMT
ENV OTP=otp24.1.5-3
# Tue, 15 Nov 2022 12:14:42 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 15 Nov 2022 12:14:47 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 15 Nov 2022 12:14:48 GMT
WORKDIR /opt/emqx
# Tue, 15 Nov 2022 12:14:48 GMT
USER emqx
# Tue, 15 Nov 2022 12:14:48 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 15 Nov 2022 12:14:48 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 15 Nov 2022 12:14:48 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 15 Nov 2022 12:14:48 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 12:14:48 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9361f46d474c278613330bf20b7b1264c2eec81c3e1f05e78b21aa201437a7`  
		Last Modified: Tue, 15 Nov 2022 12:15:15 GMT  
		Size: 2.6 MB (2571046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f847ee13842a669d2f625effb83a707e818d3cb509e2f4eed1ce3a7cd79db896`  
		Last Modified: Tue, 15 Nov 2022 12:15:20 GMT  
		Size: 45.4 MB (45424513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0fe5c47919417828878227ee16596985e496752ae09305250f4553c19fb83d`  
		Last Modified: Tue, 15 Nov 2022 12:15:20 GMT  
		Size: 45.4 MB (45437332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fb804a2f0e054f72cf8ec813e7913c1ef5fa5099d7c163aacd340aca87dd6c`  
		Last Modified: Tue, 15 Nov 2022 12:15:14 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:b96eb9baf9f59f5524f82adfbe01e9ef5c01e081bb4b7b61847de59a7ad562fb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110236571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b6eebb68d3555822f6610bc02400972790c4e0f2bae2ba0b827e1618e38ac76`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:13:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:13:29 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 15 Nov 2022 06:13:29 GMT
ENV OTP=otp24.1.5-3
# Tue, 15 Nov 2022 06:13:32 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 15 Nov 2022 06:13:36 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 15 Nov 2022 06:13:37 GMT
WORKDIR /opt/emqx
# Tue, 15 Nov 2022 06:13:37 GMT
USER emqx
# Tue, 15 Nov 2022 06:13:37 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 15 Nov 2022 06:13:37 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 15 Nov 2022 06:13:37 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 15 Nov 2022 06:13:37 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 06:13:37 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad108ef5d5673e32622aa158fbc152df7e8c340c7f4e79efffecd4c5d6c2a7be`  
		Last Modified: Tue, 15 Nov 2022 06:14:09 GMT  
		Size: 2.6 MB (2560816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96042e2ccd2609d9b280266d2cc3063aab600802b597ec18244c2761f3af513`  
		Last Modified: Tue, 15 Nov 2022 06:14:11 GMT  
		Size: 38.8 MB (38806727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432b8a52dff2f8fc12cecf2988e77261a173d791f10a1ccedb107ace30b8fdf0`  
		Last Modified: Tue, 15 Nov 2022 06:14:11 GMT  
		Size: 38.8 MB (38807317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4504a627c078e5f88f9616bd61b3f0074e95a846d4bee00e1e4f6024bb61244`  
		Last Modified: Tue, 15 Nov 2022 06:14:08 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.4`

```console
$ docker pull emqx@sha256:cb6daea8f3ec82829550982f158cf8cab692f9f4132deae6f5fb313d13e1ed7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4.4` - linux; amd64

```console
$ docker pull emqx@sha256:f356cc67a765ca1a8f061357a4f2a642972013633aa430dabb63714d27a025ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124846626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:690157a23d6d16f7a0018e067eb70e3dd47d21343f1ab306b016b698618820b8`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:14:37 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:14:37 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 15 Nov 2022 12:14:37 GMT
ENV OTP=otp24.1.5-3
# Tue, 15 Nov 2022 12:14:42 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 15 Nov 2022 12:14:47 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 15 Nov 2022 12:14:48 GMT
WORKDIR /opt/emqx
# Tue, 15 Nov 2022 12:14:48 GMT
USER emqx
# Tue, 15 Nov 2022 12:14:48 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 15 Nov 2022 12:14:48 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 15 Nov 2022 12:14:48 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 15 Nov 2022 12:14:48 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 12:14:48 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9361f46d474c278613330bf20b7b1264c2eec81c3e1f05e78b21aa201437a7`  
		Last Modified: Tue, 15 Nov 2022 12:15:15 GMT  
		Size: 2.6 MB (2571046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f847ee13842a669d2f625effb83a707e818d3cb509e2f4eed1ce3a7cd79db896`  
		Last Modified: Tue, 15 Nov 2022 12:15:20 GMT  
		Size: 45.4 MB (45424513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0fe5c47919417828878227ee16596985e496752ae09305250f4553c19fb83d`  
		Last Modified: Tue, 15 Nov 2022 12:15:20 GMT  
		Size: 45.4 MB (45437332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fb804a2f0e054f72cf8ec813e7913c1ef5fa5099d7c163aacd340aca87dd6c`  
		Last Modified: Tue, 15 Nov 2022 12:15:14 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:b96eb9baf9f59f5524f82adfbe01e9ef5c01e081bb4b7b61847de59a7ad562fb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110236571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b6eebb68d3555822f6610bc02400972790c4e0f2bae2ba0b827e1618e38ac76`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:13:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:13:29 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 15 Nov 2022 06:13:29 GMT
ENV OTP=otp24.1.5-3
# Tue, 15 Nov 2022 06:13:32 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 15 Nov 2022 06:13:36 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 15 Nov 2022 06:13:37 GMT
WORKDIR /opt/emqx
# Tue, 15 Nov 2022 06:13:37 GMT
USER emqx
# Tue, 15 Nov 2022 06:13:37 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 15 Nov 2022 06:13:37 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 15 Nov 2022 06:13:37 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 15 Nov 2022 06:13:37 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 06:13:37 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad108ef5d5673e32622aa158fbc152df7e8c340c7f4e79efffecd4c5d6c2a7be`  
		Last Modified: Tue, 15 Nov 2022 06:14:09 GMT  
		Size: 2.6 MB (2560816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96042e2ccd2609d9b280266d2cc3063aab600802b597ec18244c2761f3af513`  
		Last Modified: Tue, 15 Nov 2022 06:14:11 GMT  
		Size: 38.8 MB (38806727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432b8a52dff2f8fc12cecf2988e77261a173d791f10a1ccedb107ace30b8fdf0`  
		Last Modified: Tue, 15 Nov 2022 06:14:11 GMT  
		Size: 38.8 MB (38807317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4504a627c078e5f88f9616bd61b3f0074e95a846d4bee00e1e4f6024bb61244`  
		Last Modified: Tue, 15 Nov 2022 06:14:08 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:cb6daea8f3ec82829550982f158cf8cab692f9f4132deae6f5fb313d13e1ed7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:f356cc67a765ca1a8f061357a4f2a642972013633aa430dabb63714d27a025ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124846626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:690157a23d6d16f7a0018e067eb70e3dd47d21343f1ab306b016b698618820b8`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:14:37 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:14:37 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 15 Nov 2022 12:14:37 GMT
ENV OTP=otp24.1.5-3
# Tue, 15 Nov 2022 12:14:42 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 15 Nov 2022 12:14:47 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 15 Nov 2022 12:14:48 GMT
WORKDIR /opt/emqx
# Tue, 15 Nov 2022 12:14:48 GMT
USER emqx
# Tue, 15 Nov 2022 12:14:48 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 15 Nov 2022 12:14:48 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 15 Nov 2022 12:14:48 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 15 Nov 2022 12:14:48 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 12:14:48 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9361f46d474c278613330bf20b7b1264c2eec81c3e1f05e78b21aa201437a7`  
		Last Modified: Tue, 15 Nov 2022 12:15:15 GMT  
		Size: 2.6 MB (2571046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f847ee13842a669d2f625effb83a707e818d3cb509e2f4eed1ce3a7cd79db896`  
		Last Modified: Tue, 15 Nov 2022 12:15:20 GMT  
		Size: 45.4 MB (45424513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0fe5c47919417828878227ee16596985e496752ae09305250f4553c19fb83d`  
		Last Modified: Tue, 15 Nov 2022 12:15:20 GMT  
		Size: 45.4 MB (45437332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fb804a2f0e054f72cf8ec813e7913c1ef5fa5099d7c163aacd340aca87dd6c`  
		Last Modified: Tue, 15 Nov 2022 12:15:14 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:b96eb9baf9f59f5524f82adfbe01e9ef5c01e081bb4b7b61847de59a7ad562fb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110236571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b6eebb68d3555822f6610bc02400972790c4e0f2bae2ba0b827e1618e38ac76`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:13:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:13:29 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 15 Nov 2022 06:13:29 GMT
ENV OTP=otp24.1.5-3
# Tue, 15 Nov 2022 06:13:32 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 15 Nov 2022 06:13:36 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 15 Nov 2022 06:13:37 GMT
WORKDIR /opt/emqx
# Tue, 15 Nov 2022 06:13:37 GMT
USER emqx
# Tue, 15 Nov 2022 06:13:37 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 15 Nov 2022 06:13:37 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 15 Nov 2022 06:13:37 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 15 Nov 2022 06:13:37 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 06:13:37 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad108ef5d5673e32622aa158fbc152df7e8c340c7f4e79efffecd4c5d6c2a7be`  
		Last Modified: Tue, 15 Nov 2022 06:14:09 GMT  
		Size: 2.6 MB (2560816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96042e2ccd2609d9b280266d2cc3063aab600802b597ec18244c2761f3af513`  
		Last Modified: Tue, 15 Nov 2022 06:14:11 GMT  
		Size: 38.8 MB (38806727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432b8a52dff2f8fc12cecf2988e77261a173d791f10a1ccedb107ace30b8fdf0`  
		Last Modified: Tue, 15 Nov 2022 06:14:11 GMT  
		Size: 38.8 MB (38807317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4504a627c078e5f88f9616bd61b3f0074e95a846d4bee00e1e4f6024bb61244`  
		Last Modified: Tue, 15 Nov 2022 06:14:08 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
