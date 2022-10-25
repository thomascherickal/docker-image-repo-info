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
$ docker pull emqx@sha256:7a868ed955b251f62d231b0b1b298d14b279792c84cd8c5b108becb3752fbce6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:6a14406b3709ca58cddc419ab1be3d038ec906678f59c1c8dfe0bf8a5b5d8a82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124853978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0517be0738f3f49939248c10fda1fabcccc595724959bb499b23fc6715c860f4`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:59:24 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:59:24 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 25 Oct 2022 02:59:25 GMT
ENV OTP=otp24.1.5-3
# Tue, 25 Oct 2022 02:59:29 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 25 Oct 2022 02:59:35 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 25 Oct 2022 02:59:35 GMT
WORKDIR /opt/emqx
# Tue, 25 Oct 2022 02:59:36 GMT
USER emqx
# Tue, 25 Oct 2022 02:59:36 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 25 Oct 2022 02:59:36 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 25 Oct 2022 02:59:36 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 25 Oct 2022 02:59:36 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 25 Oct 2022 02:59:36 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d74aaf56efa5133b3013772f289a177e4ca77677fa3a9c47129df9accb5c5b`  
		Last Modified: Tue, 25 Oct 2022 03:00:04 GMT  
		Size: 2.6 MB (2570980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e31e444f54589c1eb9f22aeeb8be2a989c01b19cae5b441e2e3fff82afb395`  
		Last Modified: Tue, 25 Oct 2022 03:00:08 GMT  
		Size: 45.4 MB (45424512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed69e4861c423a1a2dd9d103a29c0b06cd85611aec57ed628beb7ebf2a7a3dae`  
		Last Modified: Tue, 25 Oct 2022 03:00:08 GMT  
		Size: 45.4 MB (45437341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d71dc161d50458f0bb157d8141a0de75894e359e2d0ce9d5b2ecdb7cc0c85e0`  
		Last Modified: Tue, 25 Oct 2022 03:00:03 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:cd4145dc7a3e5b6419dc4f7df1ac35999469ffc613ccfeb4402e64a709115d6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110033511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262b1fa4217f1bbadbe5d83379ddb4f55744afa84619dd6dc1fff205e060c8a2`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:24:14 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:24:14 GMT
ENV EMQX_VERSION=4.4.4
# Wed, 05 Oct 2022 03:24:15 GMT
ENV OTP=otp24.1.5-3
# Wed, 05 Oct 2022 03:24:19 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 05 Oct 2022 03:24:21 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 05 Oct 2022 03:24:21 GMT
WORKDIR /opt/emqx
# Wed, 05 Oct 2022 03:24:22 GMT
USER emqx
# Wed, 05 Oct 2022 03:24:23 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 05 Oct 2022 03:24:24 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 05 Oct 2022 03:24:26 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 05 Oct 2022 03:24:26 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 03:24:27 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75a1f5842b76ca0e80f51010d3a1751158f2fc5fe23e1379771d0eaa6699578`  
		Last Modified: Wed, 05 Oct 2022 03:25:05 GMT  
		Size: 2.4 MB (2353586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57e83ab7e0975fc6638b0b73b6a4c987acb1d1d95e0f8e1add7128836462d10`  
		Last Modified: Wed, 05 Oct 2022 03:25:10 GMT  
		Size: 38.8 MB (38806775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7121b78d29f52bb06f1b85015074e8c415262eac1bf16060359de7f43a76cf28`  
		Last Modified: Wed, 05 Oct 2022 03:25:09 GMT  
		Size: 38.8 MB (38807649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5587cdfa385c41c68799ea99e489a5bf6927d31ebd5206f070b0423466c790bf`  
		Last Modified: Wed, 05 Oct 2022 03:25:05 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3`

```console
$ docker pull emqx@sha256:2fc53ec14276df6f1e73e8f51855fbe597ef5af000f3035e494f43a0f8dc304d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.3` - linux; amd64

```console
$ docker pull emqx@sha256:43536a67d4429cc8aa867fdf41039dd7e396f9f56490715fe3f32b0f806aa4dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.9 MB (103867129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7241d89833d419874337271105f686b7f2e2c5d430a0900ee3cb8c7e2dee6256`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:59:03 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:59:03 GMT
ENV EMQX_VERSION=4.3.15
# Tue, 25 Oct 2022 02:59:07 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="8f44386aebf472297377d7b6b595638f323227347047d5278dce9c0cd04963bc"; fi;     if [ ${arch} = "arm64" ]; then sha256="b0094028d388684136be975c574d98295205dd5a343045f76f423a109535e016"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 25 Oct 2022 02:59:13 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 25 Oct 2022 02:59:13 GMT
WORKDIR /opt/emqx
# Tue, 25 Oct 2022 02:59:13 GMT
USER emqx
# Tue, 25 Oct 2022 02:59:13 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 25 Oct 2022 02:59:13 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 25 Oct 2022 02:59:13 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Tue, 25 Oct 2022 02:59:14 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 25 Oct 2022 02:59:14 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d619d62981391eba9cb8cf0c1de3e78ac9ec4eedd35f96f0842ae7598cc0880e`  
		Last Modified: Tue, 25 Oct 2022 02:59:49 GMT  
		Size: 4.6 MB (4612444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4f47eed4e4a2bece4b248f586388f8687f4f52184f3c70d0f20a284792e1bc`  
		Last Modified: Tue, 25 Oct 2022 02:59:52 GMT  
		Size: 36.1 MB (36056918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f8f173e104425373e2486c3f79eeca40ed850bae442d1e77c97d6551af0932`  
		Last Modified: Tue, 25 Oct 2022 02:59:53 GMT  
		Size: 36.1 MB (36055894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656e85600df981c2fbcc419979c0d583783a62cb8fd4f90aa11c64a60101aed0`  
		Last Modified: Tue, 25 Oct 2022 02:59:48 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.3` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:629b441d39b7a142a51d728a9187c5c6ea9f9284d32a9791915e9c1e90c012aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101934737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6913d186f709b0af9442dc82a46b72c2b5757a1632414cd9058ff6526b6cbf02`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 04 Oct 2022 23:45:10 GMT
ADD file:5395cc8536f80a7cce6fbae552f35b892b152e1db2fce6274fc514d8fc77d7c9 in / 
# Tue, 04 Oct 2022 23:45:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:23:44 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:23:44 GMT
ENV EMQX_VERSION=4.3.15
# Wed, 05 Oct 2022 03:23:54 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="8f44386aebf472297377d7b6b595638f323227347047d5278dce9c0cd04963bc"; fi;     if [ ${arch} = "arm64" ]; then sha256="b0094028d388684136be975c574d98295205dd5a343045f76f423a109535e016"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 05 Oct 2022 03:23:55 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 05 Oct 2022 03:23:56 GMT
WORKDIR /opt/emqx
# Wed, 05 Oct 2022 03:23:57 GMT
USER emqx
# Wed, 05 Oct 2022 03:23:58 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 05 Oct 2022 03:23:59 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 05 Oct 2022 03:24:01 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Wed, 05 Oct 2022 03:24:01 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 03:24:02 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:2c1ba50780a9bc2b2a8f3d639ceca4285c97f51fd1c51c783fe34e150ff35e60`  
		Last Modified: Tue, 04 Oct 2022 23:51:14 GMT  
		Size: 25.9 MB (25911903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19384defea5c4645ab0afd2e7408e4759ae66eec0a2b17c00ace6a108caa8990`  
		Last Modified: Wed, 05 Oct 2022 03:24:50 GMT  
		Size: 4.5 MB (4486821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15fba364be2e196f73b5425d10f5650b0a4f1ef00a7ba6fcccb398c4d65433c3`  
		Last Modified: Wed, 05 Oct 2022 03:24:54 GMT  
		Size: 35.8 MB (35761705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f04abf011d985213ffc2959224310c3fc3724c4c9a9278ca9f69c07d1d9f4fa`  
		Last Modified: Wed, 05 Oct 2022 03:24:54 GMT  
		Size: 35.8 MB (35773267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda6f697ffba6940a292b9ce4651f69662e4ce567d945c1c4228dc4f70afc65d`  
		Last Modified: Wed, 05 Oct 2022 03:24:49 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3.15`

```console
$ docker pull emqx@sha256:2fc53ec14276df6f1e73e8f51855fbe597ef5af000f3035e494f43a0f8dc304d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.3.15` - linux; amd64

```console
$ docker pull emqx@sha256:43536a67d4429cc8aa867fdf41039dd7e396f9f56490715fe3f32b0f806aa4dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.9 MB (103867129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7241d89833d419874337271105f686b7f2e2c5d430a0900ee3cb8c7e2dee6256`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:59:03 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:59:03 GMT
ENV EMQX_VERSION=4.3.15
# Tue, 25 Oct 2022 02:59:07 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="8f44386aebf472297377d7b6b595638f323227347047d5278dce9c0cd04963bc"; fi;     if [ ${arch} = "arm64" ]; then sha256="b0094028d388684136be975c574d98295205dd5a343045f76f423a109535e016"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 25 Oct 2022 02:59:13 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 25 Oct 2022 02:59:13 GMT
WORKDIR /opt/emqx
# Tue, 25 Oct 2022 02:59:13 GMT
USER emqx
# Tue, 25 Oct 2022 02:59:13 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 25 Oct 2022 02:59:13 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 25 Oct 2022 02:59:13 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Tue, 25 Oct 2022 02:59:14 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 25 Oct 2022 02:59:14 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d619d62981391eba9cb8cf0c1de3e78ac9ec4eedd35f96f0842ae7598cc0880e`  
		Last Modified: Tue, 25 Oct 2022 02:59:49 GMT  
		Size: 4.6 MB (4612444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4f47eed4e4a2bece4b248f586388f8687f4f52184f3c70d0f20a284792e1bc`  
		Last Modified: Tue, 25 Oct 2022 02:59:52 GMT  
		Size: 36.1 MB (36056918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f8f173e104425373e2486c3f79eeca40ed850bae442d1e77c97d6551af0932`  
		Last Modified: Tue, 25 Oct 2022 02:59:53 GMT  
		Size: 36.1 MB (36055894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656e85600df981c2fbcc419979c0d583783a62cb8fd4f90aa11c64a60101aed0`  
		Last Modified: Tue, 25 Oct 2022 02:59:48 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.3.15` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:629b441d39b7a142a51d728a9187c5c6ea9f9284d32a9791915e9c1e90c012aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101934737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6913d186f709b0af9442dc82a46b72c2b5757a1632414cd9058ff6526b6cbf02`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 04 Oct 2022 23:45:10 GMT
ADD file:5395cc8536f80a7cce6fbae552f35b892b152e1db2fce6274fc514d8fc77d7c9 in / 
# Tue, 04 Oct 2022 23:45:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:23:44 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:23:44 GMT
ENV EMQX_VERSION=4.3.15
# Wed, 05 Oct 2022 03:23:54 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="8f44386aebf472297377d7b6b595638f323227347047d5278dce9c0cd04963bc"; fi;     if [ ${arch} = "arm64" ]; then sha256="b0094028d388684136be975c574d98295205dd5a343045f76f423a109535e016"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 05 Oct 2022 03:23:55 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 05 Oct 2022 03:23:56 GMT
WORKDIR /opt/emqx
# Wed, 05 Oct 2022 03:23:57 GMT
USER emqx
# Wed, 05 Oct 2022 03:23:58 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 05 Oct 2022 03:23:59 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 05 Oct 2022 03:24:01 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Wed, 05 Oct 2022 03:24:01 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 03:24:02 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:2c1ba50780a9bc2b2a8f3d639ceca4285c97f51fd1c51c783fe34e150ff35e60`  
		Last Modified: Tue, 04 Oct 2022 23:51:14 GMT  
		Size: 25.9 MB (25911903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19384defea5c4645ab0afd2e7408e4759ae66eec0a2b17c00ace6a108caa8990`  
		Last Modified: Wed, 05 Oct 2022 03:24:50 GMT  
		Size: 4.5 MB (4486821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15fba364be2e196f73b5425d10f5650b0a4f1ef00a7ba6fcccb398c4d65433c3`  
		Last Modified: Wed, 05 Oct 2022 03:24:54 GMT  
		Size: 35.8 MB (35761705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f04abf011d985213ffc2959224310c3fc3724c4c9a9278ca9f69c07d1d9f4fa`  
		Last Modified: Wed, 05 Oct 2022 03:24:54 GMT  
		Size: 35.8 MB (35773267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda6f697ffba6940a292b9ce4651f69662e4ce567d945c1c4228dc4f70afc65d`  
		Last Modified: Wed, 05 Oct 2022 03:24:49 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:7a868ed955b251f62d231b0b1b298d14b279792c84cd8c5b108becb3752fbce6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:6a14406b3709ca58cddc419ab1be3d038ec906678f59c1c8dfe0bf8a5b5d8a82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124853978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0517be0738f3f49939248c10fda1fabcccc595724959bb499b23fc6715c860f4`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:59:24 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:59:24 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 25 Oct 2022 02:59:25 GMT
ENV OTP=otp24.1.5-3
# Tue, 25 Oct 2022 02:59:29 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 25 Oct 2022 02:59:35 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 25 Oct 2022 02:59:35 GMT
WORKDIR /opt/emqx
# Tue, 25 Oct 2022 02:59:36 GMT
USER emqx
# Tue, 25 Oct 2022 02:59:36 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 25 Oct 2022 02:59:36 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 25 Oct 2022 02:59:36 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 25 Oct 2022 02:59:36 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 25 Oct 2022 02:59:36 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d74aaf56efa5133b3013772f289a177e4ca77677fa3a9c47129df9accb5c5b`  
		Last Modified: Tue, 25 Oct 2022 03:00:04 GMT  
		Size: 2.6 MB (2570980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e31e444f54589c1eb9f22aeeb8be2a989c01b19cae5b441e2e3fff82afb395`  
		Last Modified: Tue, 25 Oct 2022 03:00:08 GMT  
		Size: 45.4 MB (45424512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed69e4861c423a1a2dd9d103a29c0b06cd85611aec57ed628beb7ebf2a7a3dae`  
		Last Modified: Tue, 25 Oct 2022 03:00:08 GMT  
		Size: 45.4 MB (45437341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d71dc161d50458f0bb157d8141a0de75894e359e2d0ce9d5b2ecdb7cc0c85e0`  
		Last Modified: Tue, 25 Oct 2022 03:00:03 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:cd4145dc7a3e5b6419dc4f7df1ac35999469ffc613ccfeb4402e64a709115d6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110033511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262b1fa4217f1bbadbe5d83379ddb4f55744afa84619dd6dc1fff205e060c8a2`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:24:14 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:24:14 GMT
ENV EMQX_VERSION=4.4.4
# Wed, 05 Oct 2022 03:24:15 GMT
ENV OTP=otp24.1.5-3
# Wed, 05 Oct 2022 03:24:19 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 05 Oct 2022 03:24:21 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 05 Oct 2022 03:24:21 GMT
WORKDIR /opt/emqx
# Wed, 05 Oct 2022 03:24:22 GMT
USER emqx
# Wed, 05 Oct 2022 03:24:23 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 05 Oct 2022 03:24:24 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 05 Oct 2022 03:24:26 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 05 Oct 2022 03:24:26 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 03:24:27 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75a1f5842b76ca0e80f51010d3a1751158f2fc5fe23e1379771d0eaa6699578`  
		Last Modified: Wed, 05 Oct 2022 03:25:05 GMT  
		Size: 2.4 MB (2353586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57e83ab7e0975fc6638b0b73b6a4c987acb1d1d95e0f8e1add7128836462d10`  
		Last Modified: Wed, 05 Oct 2022 03:25:10 GMT  
		Size: 38.8 MB (38806775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7121b78d29f52bb06f1b85015074e8c415262eac1bf16060359de7f43a76cf28`  
		Last Modified: Wed, 05 Oct 2022 03:25:09 GMT  
		Size: 38.8 MB (38807649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5587cdfa385c41c68799ea99e489a5bf6927d31ebd5206f070b0423466c790bf`  
		Last Modified: Wed, 05 Oct 2022 03:25:05 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.4`

```console
$ docker pull emqx@sha256:7a868ed955b251f62d231b0b1b298d14b279792c84cd8c5b108becb3752fbce6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4.4` - linux; amd64

```console
$ docker pull emqx@sha256:6a14406b3709ca58cddc419ab1be3d038ec906678f59c1c8dfe0bf8a5b5d8a82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124853978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0517be0738f3f49939248c10fda1fabcccc595724959bb499b23fc6715c860f4`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:59:24 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:59:24 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 25 Oct 2022 02:59:25 GMT
ENV OTP=otp24.1.5-3
# Tue, 25 Oct 2022 02:59:29 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 25 Oct 2022 02:59:35 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 25 Oct 2022 02:59:35 GMT
WORKDIR /opt/emqx
# Tue, 25 Oct 2022 02:59:36 GMT
USER emqx
# Tue, 25 Oct 2022 02:59:36 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 25 Oct 2022 02:59:36 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 25 Oct 2022 02:59:36 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 25 Oct 2022 02:59:36 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 25 Oct 2022 02:59:36 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d74aaf56efa5133b3013772f289a177e4ca77677fa3a9c47129df9accb5c5b`  
		Last Modified: Tue, 25 Oct 2022 03:00:04 GMT  
		Size: 2.6 MB (2570980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e31e444f54589c1eb9f22aeeb8be2a989c01b19cae5b441e2e3fff82afb395`  
		Last Modified: Tue, 25 Oct 2022 03:00:08 GMT  
		Size: 45.4 MB (45424512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed69e4861c423a1a2dd9d103a29c0b06cd85611aec57ed628beb7ebf2a7a3dae`  
		Last Modified: Tue, 25 Oct 2022 03:00:08 GMT  
		Size: 45.4 MB (45437341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d71dc161d50458f0bb157d8141a0de75894e359e2d0ce9d5b2ecdb7cc0c85e0`  
		Last Modified: Tue, 25 Oct 2022 03:00:03 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:cd4145dc7a3e5b6419dc4f7df1ac35999469ffc613ccfeb4402e64a709115d6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110033511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262b1fa4217f1bbadbe5d83379ddb4f55744afa84619dd6dc1fff205e060c8a2`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:24:14 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:24:14 GMT
ENV EMQX_VERSION=4.4.4
# Wed, 05 Oct 2022 03:24:15 GMT
ENV OTP=otp24.1.5-3
# Wed, 05 Oct 2022 03:24:19 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 05 Oct 2022 03:24:21 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 05 Oct 2022 03:24:21 GMT
WORKDIR /opt/emqx
# Wed, 05 Oct 2022 03:24:22 GMT
USER emqx
# Wed, 05 Oct 2022 03:24:23 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 05 Oct 2022 03:24:24 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 05 Oct 2022 03:24:26 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 05 Oct 2022 03:24:26 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 03:24:27 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75a1f5842b76ca0e80f51010d3a1751158f2fc5fe23e1379771d0eaa6699578`  
		Last Modified: Wed, 05 Oct 2022 03:25:05 GMT  
		Size: 2.4 MB (2353586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57e83ab7e0975fc6638b0b73b6a4c987acb1d1d95e0f8e1add7128836462d10`  
		Last Modified: Wed, 05 Oct 2022 03:25:10 GMT  
		Size: 38.8 MB (38806775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7121b78d29f52bb06f1b85015074e8c415262eac1bf16060359de7f43a76cf28`  
		Last Modified: Wed, 05 Oct 2022 03:25:09 GMT  
		Size: 38.8 MB (38807649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5587cdfa385c41c68799ea99e489a5bf6927d31ebd5206f070b0423466c790bf`  
		Last Modified: Wed, 05 Oct 2022 03:25:05 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:7a868ed955b251f62d231b0b1b298d14b279792c84cd8c5b108becb3752fbce6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:6a14406b3709ca58cddc419ab1be3d038ec906678f59c1c8dfe0bf8a5b5d8a82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124853978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0517be0738f3f49939248c10fda1fabcccc595724959bb499b23fc6715c860f4`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:59:24 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:59:24 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 25 Oct 2022 02:59:25 GMT
ENV OTP=otp24.1.5-3
# Tue, 25 Oct 2022 02:59:29 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 25 Oct 2022 02:59:35 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 25 Oct 2022 02:59:35 GMT
WORKDIR /opt/emqx
# Tue, 25 Oct 2022 02:59:36 GMT
USER emqx
# Tue, 25 Oct 2022 02:59:36 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 25 Oct 2022 02:59:36 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 25 Oct 2022 02:59:36 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 25 Oct 2022 02:59:36 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 25 Oct 2022 02:59:36 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d74aaf56efa5133b3013772f289a177e4ca77677fa3a9c47129df9accb5c5b`  
		Last Modified: Tue, 25 Oct 2022 03:00:04 GMT  
		Size: 2.6 MB (2570980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e31e444f54589c1eb9f22aeeb8be2a989c01b19cae5b441e2e3fff82afb395`  
		Last Modified: Tue, 25 Oct 2022 03:00:08 GMT  
		Size: 45.4 MB (45424512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed69e4861c423a1a2dd9d103a29c0b06cd85611aec57ed628beb7ebf2a7a3dae`  
		Last Modified: Tue, 25 Oct 2022 03:00:08 GMT  
		Size: 45.4 MB (45437341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d71dc161d50458f0bb157d8141a0de75894e359e2d0ce9d5b2ecdb7cc0c85e0`  
		Last Modified: Tue, 25 Oct 2022 03:00:03 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:cd4145dc7a3e5b6419dc4f7df1ac35999469ffc613ccfeb4402e64a709115d6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110033511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262b1fa4217f1bbadbe5d83379ddb4f55744afa84619dd6dc1fff205e060c8a2`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:24:14 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:24:14 GMT
ENV EMQX_VERSION=4.4.4
# Wed, 05 Oct 2022 03:24:15 GMT
ENV OTP=otp24.1.5-3
# Wed, 05 Oct 2022 03:24:19 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 05 Oct 2022 03:24:21 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 05 Oct 2022 03:24:21 GMT
WORKDIR /opt/emqx
# Wed, 05 Oct 2022 03:24:22 GMT
USER emqx
# Wed, 05 Oct 2022 03:24:23 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 05 Oct 2022 03:24:24 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 05 Oct 2022 03:24:26 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 05 Oct 2022 03:24:26 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 03:24:27 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75a1f5842b76ca0e80f51010d3a1751158f2fc5fe23e1379771d0eaa6699578`  
		Last Modified: Wed, 05 Oct 2022 03:25:05 GMT  
		Size: 2.4 MB (2353586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57e83ab7e0975fc6638b0b73b6a4c987acb1d1d95e0f8e1add7128836462d10`  
		Last Modified: Wed, 05 Oct 2022 03:25:10 GMT  
		Size: 38.8 MB (38806775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7121b78d29f52bb06f1b85015074e8c415262eac1bf16060359de7f43a76cf28`  
		Last Modified: Wed, 05 Oct 2022 03:25:09 GMT  
		Size: 38.8 MB (38807649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5587cdfa385c41c68799ea99e489a5bf6927d31ebd5206f070b0423466c790bf`  
		Last Modified: Wed, 05 Oct 2022 03:25:05 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
