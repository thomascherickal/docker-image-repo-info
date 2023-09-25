<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `emqx`

-	[`emqx:5`](#emqx5)
-	[`emqx:5.0`](#emqx50)
-	[`emqx:5.0.26`](#emqx5026)
-	[`emqx:5.1`](#emqx51)
-	[`emqx:5.1.6`](#emqx516)
-	[`emqx:5.2`](#emqx52)
-	[`emqx:5.2.1`](#emqx521)
-	[`emqx:latest`](#emqxlatest)

## `emqx:5`

```console
$ docker pull emqx@sha256:50c3b7243098d8ad15efa4412768034a702b610221e9f58c394ab38de9a27cb5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:c3487b29bd4cfe7064a23a92a9db5d7b05c76898d6a273f0a35650003677ae7a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101162302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:690dc4b352c18c787ead489a9ab9660cb9b59c538bbe0bb3dd0014beec5501c3`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Mon, 25 Sep 2023 19:21:09 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Mon, 25 Sep 2023 19:21:09 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Mon, 25 Sep 2023 19:21:10 GMT
ENV EMQX_VERSION=5.2.1
# Mon, 25 Sep 2023 19:21:10 GMT
ENV AMD64_SHA256=359a12811e5e6725e4269d9484abd348effdde35c0f2af1f5b63cae790c73020
# Mon, 25 Sep 2023 19:21:10 GMT
ENV ARM64_SHA256=2e0a3e0b33669c9b6da488970a2f92d08d7bd0824295822b205b83461ba4728d
# Mon, 25 Sep 2023 19:21:10 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Mon, 25 Sep 2023 19:21:23 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl;     rm -rf /var/lib/apt/lists/*;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl
# Mon, 25 Sep 2023 19:21:24 GMT
WORKDIR /opt/emqx
# Mon, 25 Sep 2023 19:21:24 GMT
USER emqx
# Mon, 25 Sep 2023 19:21:24 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Mon, 25 Sep 2023 19:21:24 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Mon, 25 Sep 2023 19:21:24 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Mon, 25 Sep 2023 19:21:24 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Mon, 25 Sep 2023 19:21:24 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc61d6b2cab9e777137dcf99de5d2130f5fc71aeaedfe9db7374372bc8fde1e`  
		Last Modified: Mon, 25 Sep 2023 19:21:39 GMT  
		Size: 1.6 MB (1629447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705f111e43d6eb1a415b0ae91899025ddc6d41c20c308e507b7d63975355be3a`  
		Last Modified: Mon, 25 Sep 2023 19:21:39 GMT  
		Size: 4.1 KB (4110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fbab83e4365361212f21e742cfea68928187e9b6f2bf0161257729e7ca27e`  
		Last Modified: Mon, 25 Sep 2023 19:21:46 GMT  
		Size: 68.1 MB (68110131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ba398fb5523476b555e788b016cbc0930eb4a33b561424782e7743aa06c901`  
		Last Modified: Mon, 25 Sep 2023 19:21:39 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:c99d83d1ff9918dfa3d0d003b4bc6312e9bf4369289cd786fdd72b4b7f8ed503
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91463122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b37f898441dd381142791cca1c675099ea0ed9f32c75bc33d9901e471a4281a`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:28 GMT
ADD file:024479be439b4ecb37c939e68673adc72955f3345ca0e809bd13e897709e59e4 in / 
# Wed, 20 Sep 2023 02:44:28 GMT
CMD ["bash"]
# Mon, 25 Sep 2023 19:39:34 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Mon, 25 Sep 2023 19:39:35 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Mon, 25 Sep 2023 19:39:35 GMT
ENV EMQX_VERSION=5.2.1
# Mon, 25 Sep 2023 19:39:35 GMT
ENV AMD64_SHA256=359a12811e5e6725e4269d9484abd348effdde35c0f2af1f5b63cae790c73020
# Mon, 25 Sep 2023 19:39:35 GMT
ENV ARM64_SHA256=2e0a3e0b33669c9b6da488970a2f92d08d7bd0824295822b205b83461ba4728d
# Mon, 25 Sep 2023 19:39:35 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Mon, 25 Sep 2023 19:39:45 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl;     rm -rf /var/lib/apt/lists/*;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl
# Mon, 25 Sep 2023 19:39:46 GMT
WORKDIR /opt/emqx
# Mon, 25 Sep 2023 19:39:46 GMT
USER emqx
# Mon, 25 Sep 2023 19:39:46 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Mon, 25 Sep 2023 19:39:46 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Mon, 25 Sep 2023 19:39:46 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Mon, 25 Sep 2023 19:39:46 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Mon, 25 Sep 2023 19:39:46 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:fc521c5b98350f6fd8c72ace1e48558bb7b53cb3db201a2a3b42095401cd02f1`  
		Last Modified: Wed, 20 Sep 2023 02:48:13 GMT  
		Size: 30.1 MB (30062869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be57ddd88e7a46ad28aa9e7adbff962cc738ade8ec137900e53038f0e7f09e0c`  
		Last Modified: Mon, 25 Sep 2023 19:39:59 GMT  
		Size: 1.6 MB (1644088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6900626db5907a9fdea38e754a64a2d3b51204f395e7aa35dc33bf0437d9f35e`  
		Last Modified: Mon, 25 Sep 2023 19:39:58 GMT  
		Size: 4.1 KB (4115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb41abb93750b931f478cbde94a8d1f7ad40512d4766cec2dbb5bab56b01559`  
		Last Modified: Mon, 25 Sep 2023 19:40:04 GMT  
		Size: 59.8 MB (59751145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57abcdf896fd209aa7f38e6d5d2d8a6461725322bcda1b9517d3eac660203b89`  
		Last Modified: Mon, 25 Sep 2023 19:39:59 GMT  
		Size: 905.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:4237d27a7fbcdebf62a97e8a0a800d9366b5291263fd55298c591d0c9318fcd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:fd961c253839b1036678b5e6df65a051e162e9755ddbc7507ec5740a8aa17cda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101982457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f34650533762a6802d20f0caeee6aae0806bf4e4a4a5bdc4fe67e3753cb2380`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 20:55:00 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 20:55:01 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 20 Sep 2023 20:55:01 GMT
ENV EMQX_VERSION=5.0.26
# Wed, 20 Sep 2023 20:55:01 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Wed, 20 Sep 2023 20:55:01 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Wed, 20 Sep 2023 20:55:01 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 20 Sep 2023 20:55:10 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 20 Sep 2023 20:55:10 GMT
WORKDIR /opt/emqx
# Wed, 20 Sep 2023 20:55:10 GMT
USER emqx
# Wed, 20 Sep 2023 20:55:10 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 20 Sep 2023 20:55:11 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 20 Sep 2023 20:55:11 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 20 Sep 2023 20:55:11 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 20:55:11 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e606b83938f5c3cab8dc3f920452e0ed598df1e6b2865415ad7758659706c8`  
		Last Modified: Wed, 20 Sep 2023 20:55:36 GMT  
		Size: 3.0 MB (2987866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa5adf986b73764f1af06edb3f4bc2467d624dc6caa4e92b396155210bad82a`  
		Last Modified: Wed, 20 Sep 2023 20:55:35 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a1c950c606944746473f7a03117a1cb857b2af80cdbb932e824b635aca357d`  
		Last Modified: Wed, 20 Sep 2023 20:55:44 GMT  
		Size: 67.6 MB (67571870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a67779c5911233149f4887afb068ad6ed9a2e15eca051c329e83cb6b36c759`  
		Last Modified: Wed, 20 Sep 2023 20:55:35 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:6f3fcc837419af3e4a64523782af643756d23996ebea645b505865c49136c450
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93060258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6859a3b8fa616e8eefef1343fecc47197d9f76168e585c33d5698a8058d6ef6`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:28 GMT
ADD file:024479be439b4ecb37c939e68673adc72955f3345ca0e809bd13e897709e59e4 in / 
# Wed, 20 Sep 2023 02:44:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:43:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:43:30 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 20 Sep 2023 09:43:30 GMT
ENV EMQX_VERSION=5.0.26
# Wed, 20 Sep 2023 09:43:30 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Wed, 20 Sep 2023 09:43:30 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Wed, 20 Sep 2023 09:43:30 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 20 Sep 2023 09:43:37 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 20 Sep 2023 09:43:38 GMT
WORKDIR /opt/emqx
# Wed, 20 Sep 2023 09:43:38 GMT
USER emqx
# Wed, 20 Sep 2023 09:43:38 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 20 Sep 2023 09:43:38 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 20 Sep 2023 09:43:38 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 20 Sep 2023 09:43:38 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 09:43:38 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:fc521c5b98350f6fd8c72ace1e48558bb7b53cb3db201a2a3b42095401cd02f1`  
		Last Modified: Wed, 20 Sep 2023 02:48:13 GMT  
		Size: 30.1 MB (30062869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad6c853d0601d84f2b531042ce064d5fb3f9aa39d30e074f5673152558f8af7`  
		Last Modified: Wed, 20 Sep 2023 09:43:59 GMT  
		Size: 3.0 MB (3002964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aaa8c587ac603c1fab64204d2a4a4d5d4d9a88f0c1da2c73f487e0605c293b`  
		Last Modified: Wed, 20 Sep 2023 09:43:59 GMT  
		Size: 4.1 KB (4118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b402ca7847b75bb32c821e62954c85f3da4a1569b3481d7cf969169f0dd1c8c3`  
		Last Modified: Wed, 20 Sep 2023 09:44:05 GMT  
		Size: 60.0 MB (59989404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2afda3e0a87072dc5c76a3bed62c82b739acf9e4114ec1152ad122a27e9abdf4`  
		Last Modified: Wed, 20 Sep 2023 09:43:59 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.26`

```console
$ docker pull emqx@sha256:4237d27a7fbcdebf62a97e8a0a800d9366b5291263fd55298c591d0c9318fcd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0.26` - linux; amd64

```console
$ docker pull emqx@sha256:fd961c253839b1036678b5e6df65a051e162e9755ddbc7507ec5740a8aa17cda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101982457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f34650533762a6802d20f0caeee6aae0806bf4e4a4a5bdc4fe67e3753cb2380`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 20:55:00 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 20:55:01 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 20 Sep 2023 20:55:01 GMT
ENV EMQX_VERSION=5.0.26
# Wed, 20 Sep 2023 20:55:01 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Wed, 20 Sep 2023 20:55:01 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Wed, 20 Sep 2023 20:55:01 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 20 Sep 2023 20:55:10 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 20 Sep 2023 20:55:10 GMT
WORKDIR /opt/emqx
# Wed, 20 Sep 2023 20:55:10 GMT
USER emqx
# Wed, 20 Sep 2023 20:55:10 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 20 Sep 2023 20:55:11 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 20 Sep 2023 20:55:11 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 20 Sep 2023 20:55:11 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 20:55:11 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e606b83938f5c3cab8dc3f920452e0ed598df1e6b2865415ad7758659706c8`  
		Last Modified: Wed, 20 Sep 2023 20:55:36 GMT  
		Size: 3.0 MB (2987866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa5adf986b73764f1af06edb3f4bc2467d624dc6caa4e92b396155210bad82a`  
		Last Modified: Wed, 20 Sep 2023 20:55:35 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a1c950c606944746473f7a03117a1cb857b2af80cdbb932e824b635aca357d`  
		Last Modified: Wed, 20 Sep 2023 20:55:44 GMT  
		Size: 67.6 MB (67571870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a67779c5911233149f4887afb068ad6ed9a2e15eca051c329e83cb6b36c759`  
		Last Modified: Wed, 20 Sep 2023 20:55:35 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0.26` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:6f3fcc837419af3e4a64523782af643756d23996ebea645b505865c49136c450
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93060258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6859a3b8fa616e8eefef1343fecc47197d9f76168e585c33d5698a8058d6ef6`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:28 GMT
ADD file:024479be439b4ecb37c939e68673adc72955f3345ca0e809bd13e897709e59e4 in / 
# Wed, 20 Sep 2023 02:44:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:43:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:43:30 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 20 Sep 2023 09:43:30 GMT
ENV EMQX_VERSION=5.0.26
# Wed, 20 Sep 2023 09:43:30 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Wed, 20 Sep 2023 09:43:30 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Wed, 20 Sep 2023 09:43:30 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 20 Sep 2023 09:43:37 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 20 Sep 2023 09:43:38 GMT
WORKDIR /opt/emqx
# Wed, 20 Sep 2023 09:43:38 GMT
USER emqx
# Wed, 20 Sep 2023 09:43:38 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 20 Sep 2023 09:43:38 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 20 Sep 2023 09:43:38 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 20 Sep 2023 09:43:38 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 09:43:38 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:fc521c5b98350f6fd8c72ace1e48558bb7b53cb3db201a2a3b42095401cd02f1`  
		Last Modified: Wed, 20 Sep 2023 02:48:13 GMT  
		Size: 30.1 MB (30062869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad6c853d0601d84f2b531042ce064d5fb3f9aa39d30e074f5673152558f8af7`  
		Last Modified: Wed, 20 Sep 2023 09:43:59 GMT  
		Size: 3.0 MB (3002964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aaa8c587ac603c1fab64204d2a4a4d5d4d9a88f0c1da2c73f487e0605c293b`  
		Last Modified: Wed, 20 Sep 2023 09:43:59 GMT  
		Size: 4.1 KB (4118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b402ca7847b75bb32c821e62954c85f3da4a1569b3481d7cf969169f0dd1c8c3`  
		Last Modified: Wed, 20 Sep 2023 09:44:05 GMT  
		Size: 60.0 MB (59989404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2afda3e0a87072dc5c76a3bed62c82b739acf9e4114ec1152ad122a27e9abdf4`  
		Last Modified: Wed, 20 Sep 2023 09:43:59 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.1`

```console
$ docker pull emqx@sha256:30f0ad94b7bcf49dc7c08c8b9b10345965583001c997183d08b4267ffa2750e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.1` - linux; amd64

```console
$ docker pull emqx@sha256:e60238af3a941939bdfcec99cf3821cf2fe9c200a995778f923456dbd58739b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.4 MB (102391844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c191db8d9c4f5e9361bc1f49cd1b4fdf7b9ce07b4913aec3f9d9e42275ff498`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 20:55:00 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 20:55:01 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 20 Sep 2023 20:55:15 GMT
ENV EMQX_VERSION=5.1.6
# Wed, 20 Sep 2023 20:55:15 GMT
ENV AMD64_SHA256=5c65f7538141e93d71d1dd7d088589339ef6a091b90f901604a2e0e004f5f4aa
# Wed, 20 Sep 2023 20:55:15 GMT
ENV ARM64_SHA256=ae832d29d6b4e7fa43f3bf04c8c9fad4c9047f079d1587d3ed2a3564d5ea8147
# Wed, 20 Sep 2023 20:55:16 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 20 Sep 2023 20:55:23 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Wed, 20 Sep 2023 20:55:24 GMT
WORKDIR /opt/emqx
# Wed, 20 Sep 2023 20:55:24 GMT
USER emqx
# Wed, 20 Sep 2023 20:55:24 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 20 Sep 2023 20:55:24 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 20 Sep 2023 20:55:24 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 20 Sep 2023 20:55:24 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 20:55:24 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e606b83938f5c3cab8dc3f920452e0ed598df1e6b2865415ad7758659706c8`  
		Last Modified: Wed, 20 Sep 2023 20:55:36 GMT  
		Size: 3.0 MB (2987866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa5adf986b73764f1af06edb3f4bc2467d624dc6caa4e92b396155210bad82a`  
		Last Modified: Wed, 20 Sep 2023 20:55:35 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456a710471aa0ea2d6c72f52a291f2e961f8545d6e46771fd494c8c67e7101b4`  
		Last Modified: Wed, 20 Sep 2023 20:56:00 GMT  
		Size: 68.0 MB (67981255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4590893df0fb1d2d42a6c80e1f9b2adfb0e96224deee7f8893933b610583f276`  
		Last Modified: Wed, 20 Sep 2023 20:55:53 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.1` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:3e2d6b1ec160923fc9a643c76529f05a2d0036edbdbe33bfb8522aa7e0ab3f4a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.7 MB (92695550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6c72fc2e6dc9c490372142a99bb0ff0b84daeb9509a94b11c63cd3f8890a667`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:28 GMT
ADD file:024479be439b4ecb37c939e68673adc72955f3345ca0e809bd13e897709e59e4 in / 
# Wed, 20 Sep 2023 02:44:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:43:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:43:30 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 20 Sep 2023 09:43:41 GMT
ENV EMQX_VERSION=5.1.6
# Wed, 20 Sep 2023 09:43:41 GMT
ENV AMD64_SHA256=5c65f7538141e93d71d1dd7d088589339ef6a091b90f901604a2e0e004f5f4aa
# Wed, 20 Sep 2023 09:43:41 GMT
ENV ARM64_SHA256=ae832d29d6b4e7fa43f3bf04c8c9fad4c9047f079d1587d3ed2a3564d5ea8147
# Wed, 20 Sep 2023 09:43:41 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 20 Sep 2023 09:43:49 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Wed, 20 Sep 2023 09:43:50 GMT
WORKDIR /opt/emqx
# Wed, 20 Sep 2023 09:43:50 GMT
USER emqx
# Wed, 20 Sep 2023 09:43:50 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 20 Sep 2023 09:43:50 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 20 Sep 2023 09:43:50 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 20 Sep 2023 09:43:50 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 09:43:50 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:fc521c5b98350f6fd8c72ace1e48558bb7b53cb3db201a2a3b42095401cd02f1`  
		Last Modified: Wed, 20 Sep 2023 02:48:13 GMT  
		Size: 30.1 MB (30062869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad6c853d0601d84f2b531042ce064d5fb3f9aa39d30e074f5673152558f8af7`  
		Last Modified: Wed, 20 Sep 2023 09:43:59 GMT  
		Size: 3.0 MB (3002964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aaa8c587ac603c1fab64204d2a4a4d5d4d9a88f0c1da2c73f487e0605c293b`  
		Last Modified: Wed, 20 Sep 2023 09:43:59 GMT  
		Size: 4.1 KB (4118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede3251ec3661ce2a030991bb4e9aeb51a3127ded8c26fb4ea678800451aa92b`  
		Last Modified: Wed, 20 Sep 2023 09:44:19 GMT  
		Size: 59.6 MB (59624697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7857c3d170ee9aa40624dde89b5a3328f7604a266360b10b52103708404916c6`  
		Last Modified: Wed, 20 Sep 2023 09:44:13 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.1.6`

```console
$ docker pull emqx@sha256:30f0ad94b7bcf49dc7c08c8b9b10345965583001c997183d08b4267ffa2750e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.1.6` - linux; amd64

```console
$ docker pull emqx@sha256:e60238af3a941939bdfcec99cf3821cf2fe9c200a995778f923456dbd58739b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.4 MB (102391844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c191db8d9c4f5e9361bc1f49cd1b4fdf7b9ce07b4913aec3f9d9e42275ff498`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 20:55:00 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 20:55:01 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 20 Sep 2023 20:55:15 GMT
ENV EMQX_VERSION=5.1.6
# Wed, 20 Sep 2023 20:55:15 GMT
ENV AMD64_SHA256=5c65f7538141e93d71d1dd7d088589339ef6a091b90f901604a2e0e004f5f4aa
# Wed, 20 Sep 2023 20:55:15 GMT
ENV ARM64_SHA256=ae832d29d6b4e7fa43f3bf04c8c9fad4c9047f079d1587d3ed2a3564d5ea8147
# Wed, 20 Sep 2023 20:55:16 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 20 Sep 2023 20:55:23 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Wed, 20 Sep 2023 20:55:24 GMT
WORKDIR /opt/emqx
# Wed, 20 Sep 2023 20:55:24 GMT
USER emqx
# Wed, 20 Sep 2023 20:55:24 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 20 Sep 2023 20:55:24 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 20 Sep 2023 20:55:24 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 20 Sep 2023 20:55:24 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 20:55:24 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e606b83938f5c3cab8dc3f920452e0ed598df1e6b2865415ad7758659706c8`  
		Last Modified: Wed, 20 Sep 2023 20:55:36 GMT  
		Size: 3.0 MB (2987866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa5adf986b73764f1af06edb3f4bc2467d624dc6caa4e92b396155210bad82a`  
		Last Modified: Wed, 20 Sep 2023 20:55:35 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456a710471aa0ea2d6c72f52a291f2e961f8545d6e46771fd494c8c67e7101b4`  
		Last Modified: Wed, 20 Sep 2023 20:56:00 GMT  
		Size: 68.0 MB (67981255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4590893df0fb1d2d42a6c80e1f9b2adfb0e96224deee7f8893933b610583f276`  
		Last Modified: Wed, 20 Sep 2023 20:55:53 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.1.6` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:3e2d6b1ec160923fc9a643c76529f05a2d0036edbdbe33bfb8522aa7e0ab3f4a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.7 MB (92695550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6c72fc2e6dc9c490372142a99bb0ff0b84daeb9509a94b11c63cd3f8890a667`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:28 GMT
ADD file:024479be439b4ecb37c939e68673adc72955f3345ca0e809bd13e897709e59e4 in / 
# Wed, 20 Sep 2023 02:44:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:43:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:43:30 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 20 Sep 2023 09:43:41 GMT
ENV EMQX_VERSION=5.1.6
# Wed, 20 Sep 2023 09:43:41 GMT
ENV AMD64_SHA256=5c65f7538141e93d71d1dd7d088589339ef6a091b90f901604a2e0e004f5f4aa
# Wed, 20 Sep 2023 09:43:41 GMT
ENV ARM64_SHA256=ae832d29d6b4e7fa43f3bf04c8c9fad4c9047f079d1587d3ed2a3564d5ea8147
# Wed, 20 Sep 2023 09:43:41 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 20 Sep 2023 09:43:49 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Wed, 20 Sep 2023 09:43:50 GMT
WORKDIR /opt/emqx
# Wed, 20 Sep 2023 09:43:50 GMT
USER emqx
# Wed, 20 Sep 2023 09:43:50 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 20 Sep 2023 09:43:50 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 20 Sep 2023 09:43:50 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 20 Sep 2023 09:43:50 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 09:43:50 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:fc521c5b98350f6fd8c72ace1e48558bb7b53cb3db201a2a3b42095401cd02f1`  
		Last Modified: Wed, 20 Sep 2023 02:48:13 GMT  
		Size: 30.1 MB (30062869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad6c853d0601d84f2b531042ce064d5fb3f9aa39d30e074f5673152558f8af7`  
		Last Modified: Wed, 20 Sep 2023 09:43:59 GMT  
		Size: 3.0 MB (3002964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aaa8c587ac603c1fab64204d2a4a4d5d4d9a88f0c1da2c73f487e0605c293b`  
		Last Modified: Wed, 20 Sep 2023 09:43:59 GMT  
		Size: 4.1 KB (4118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede3251ec3661ce2a030991bb4e9aeb51a3127ded8c26fb4ea678800451aa92b`  
		Last Modified: Wed, 20 Sep 2023 09:44:19 GMT  
		Size: 59.6 MB (59624697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7857c3d170ee9aa40624dde89b5a3328f7604a266360b10b52103708404916c6`  
		Last Modified: Wed, 20 Sep 2023 09:44:13 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.2`

```console
$ docker pull emqx@sha256:50c3b7243098d8ad15efa4412768034a702b610221e9f58c394ab38de9a27cb5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.2` - linux; amd64

```console
$ docker pull emqx@sha256:c3487b29bd4cfe7064a23a92a9db5d7b05c76898d6a273f0a35650003677ae7a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101162302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:690dc4b352c18c787ead489a9ab9660cb9b59c538bbe0bb3dd0014beec5501c3`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Mon, 25 Sep 2023 19:21:09 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Mon, 25 Sep 2023 19:21:09 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Mon, 25 Sep 2023 19:21:10 GMT
ENV EMQX_VERSION=5.2.1
# Mon, 25 Sep 2023 19:21:10 GMT
ENV AMD64_SHA256=359a12811e5e6725e4269d9484abd348effdde35c0f2af1f5b63cae790c73020
# Mon, 25 Sep 2023 19:21:10 GMT
ENV ARM64_SHA256=2e0a3e0b33669c9b6da488970a2f92d08d7bd0824295822b205b83461ba4728d
# Mon, 25 Sep 2023 19:21:10 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Mon, 25 Sep 2023 19:21:23 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl;     rm -rf /var/lib/apt/lists/*;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl
# Mon, 25 Sep 2023 19:21:24 GMT
WORKDIR /opt/emqx
# Mon, 25 Sep 2023 19:21:24 GMT
USER emqx
# Mon, 25 Sep 2023 19:21:24 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Mon, 25 Sep 2023 19:21:24 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Mon, 25 Sep 2023 19:21:24 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Mon, 25 Sep 2023 19:21:24 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Mon, 25 Sep 2023 19:21:24 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc61d6b2cab9e777137dcf99de5d2130f5fc71aeaedfe9db7374372bc8fde1e`  
		Last Modified: Mon, 25 Sep 2023 19:21:39 GMT  
		Size: 1.6 MB (1629447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705f111e43d6eb1a415b0ae91899025ddc6d41c20c308e507b7d63975355be3a`  
		Last Modified: Mon, 25 Sep 2023 19:21:39 GMT  
		Size: 4.1 KB (4110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fbab83e4365361212f21e742cfea68928187e9b6f2bf0161257729e7ca27e`  
		Last Modified: Mon, 25 Sep 2023 19:21:46 GMT  
		Size: 68.1 MB (68110131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ba398fb5523476b555e788b016cbc0930eb4a33b561424782e7743aa06c901`  
		Last Modified: Mon, 25 Sep 2023 19:21:39 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.2` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:c99d83d1ff9918dfa3d0d003b4bc6312e9bf4369289cd786fdd72b4b7f8ed503
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91463122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b37f898441dd381142791cca1c675099ea0ed9f32c75bc33d9901e471a4281a`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:28 GMT
ADD file:024479be439b4ecb37c939e68673adc72955f3345ca0e809bd13e897709e59e4 in / 
# Wed, 20 Sep 2023 02:44:28 GMT
CMD ["bash"]
# Mon, 25 Sep 2023 19:39:34 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Mon, 25 Sep 2023 19:39:35 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Mon, 25 Sep 2023 19:39:35 GMT
ENV EMQX_VERSION=5.2.1
# Mon, 25 Sep 2023 19:39:35 GMT
ENV AMD64_SHA256=359a12811e5e6725e4269d9484abd348effdde35c0f2af1f5b63cae790c73020
# Mon, 25 Sep 2023 19:39:35 GMT
ENV ARM64_SHA256=2e0a3e0b33669c9b6da488970a2f92d08d7bd0824295822b205b83461ba4728d
# Mon, 25 Sep 2023 19:39:35 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Mon, 25 Sep 2023 19:39:45 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl;     rm -rf /var/lib/apt/lists/*;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl
# Mon, 25 Sep 2023 19:39:46 GMT
WORKDIR /opt/emqx
# Mon, 25 Sep 2023 19:39:46 GMT
USER emqx
# Mon, 25 Sep 2023 19:39:46 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Mon, 25 Sep 2023 19:39:46 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Mon, 25 Sep 2023 19:39:46 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Mon, 25 Sep 2023 19:39:46 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Mon, 25 Sep 2023 19:39:46 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:fc521c5b98350f6fd8c72ace1e48558bb7b53cb3db201a2a3b42095401cd02f1`  
		Last Modified: Wed, 20 Sep 2023 02:48:13 GMT  
		Size: 30.1 MB (30062869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be57ddd88e7a46ad28aa9e7adbff962cc738ade8ec137900e53038f0e7f09e0c`  
		Last Modified: Mon, 25 Sep 2023 19:39:59 GMT  
		Size: 1.6 MB (1644088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6900626db5907a9fdea38e754a64a2d3b51204f395e7aa35dc33bf0437d9f35e`  
		Last Modified: Mon, 25 Sep 2023 19:39:58 GMT  
		Size: 4.1 KB (4115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb41abb93750b931f478cbde94a8d1f7ad40512d4766cec2dbb5bab56b01559`  
		Last Modified: Mon, 25 Sep 2023 19:40:04 GMT  
		Size: 59.8 MB (59751145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57abcdf896fd209aa7f38e6d5d2d8a6461725322bcda1b9517d3eac660203b89`  
		Last Modified: Mon, 25 Sep 2023 19:39:59 GMT  
		Size: 905.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.2.1`

```console
$ docker pull emqx@sha256:50c3b7243098d8ad15efa4412768034a702b610221e9f58c394ab38de9a27cb5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.2.1` - linux; amd64

```console
$ docker pull emqx@sha256:c3487b29bd4cfe7064a23a92a9db5d7b05c76898d6a273f0a35650003677ae7a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101162302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:690dc4b352c18c787ead489a9ab9660cb9b59c538bbe0bb3dd0014beec5501c3`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Mon, 25 Sep 2023 19:21:09 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Mon, 25 Sep 2023 19:21:09 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Mon, 25 Sep 2023 19:21:10 GMT
ENV EMQX_VERSION=5.2.1
# Mon, 25 Sep 2023 19:21:10 GMT
ENV AMD64_SHA256=359a12811e5e6725e4269d9484abd348effdde35c0f2af1f5b63cae790c73020
# Mon, 25 Sep 2023 19:21:10 GMT
ENV ARM64_SHA256=2e0a3e0b33669c9b6da488970a2f92d08d7bd0824295822b205b83461ba4728d
# Mon, 25 Sep 2023 19:21:10 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Mon, 25 Sep 2023 19:21:23 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl;     rm -rf /var/lib/apt/lists/*;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl
# Mon, 25 Sep 2023 19:21:24 GMT
WORKDIR /opt/emqx
# Mon, 25 Sep 2023 19:21:24 GMT
USER emqx
# Mon, 25 Sep 2023 19:21:24 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Mon, 25 Sep 2023 19:21:24 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Mon, 25 Sep 2023 19:21:24 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Mon, 25 Sep 2023 19:21:24 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Mon, 25 Sep 2023 19:21:24 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc61d6b2cab9e777137dcf99de5d2130f5fc71aeaedfe9db7374372bc8fde1e`  
		Last Modified: Mon, 25 Sep 2023 19:21:39 GMT  
		Size: 1.6 MB (1629447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705f111e43d6eb1a415b0ae91899025ddc6d41c20c308e507b7d63975355be3a`  
		Last Modified: Mon, 25 Sep 2023 19:21:39 GMT  
		Size: 4.1 KB (4110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fbab83e4365361212f21e742cfea68928187e9b6f2bf0161257729e7ca27e`  
		Last Modified: Mon, 25 Sep 2023 19:21:46 GMT  
		Size: 68.1 MB (68110131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ba398fb5523476b555e788b016cbc0930eb4a33b561424782e7743aa06c901`  
		Last Modified: Mon, 25 Sep 2023 19:21:39 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.2.1` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:c99d83d1ff9918dfa3d0d003b4bc6312e9bf4369289cd786fdd72b4b7f8ed503
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91463122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b37f898441dd381142791cca1c675099ea0ed9f32c75bc33d9901e471a4281a`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:28 GMT
ADD file:024479be439b4ecb37c939e68673adc72955f3345ca0e809bd13e897709e59e4 in / 
# Wed, 20 Sep 2023 02:44:28 GMT
CMD ["bash"]
# Mon, 25 Sep 2023 19:39:34 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Mon, 25 Sep 2023 19:39:35 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Mon, 25 Sep 2023 19:39:35 GMT
ENV EMQX_VERSION=5.2.1
# Mon, 25 Sep 2023 19:39:35 GMT
ENV AMD64_SHA256=359a12811e5e6725e4269d9484abd348effdde35c0f2af1f5b63cae790c73020
# Mon, 25 Sep 2023 19:39:35 GMT
ENV ARM64_SHA256=2e0a3e0b33669c9b6da488970a2f92d08d7bd0824295822b205b83461ba4728d
# Mon, 25 Sep 2023 19:39:35 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Mon, 25 Sep 2023 19:39:45 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl;     rm -rf /var/lib/apt/lists/*;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl
# Mon, 25 Sep 2023 19:39:46 GMT
WORKDIR /opt/emqx
# Mon, 25 Sep 2023 19:39:46 GMT
USER emqx
# Mon, 25 Sep 2023 19:39:46 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Mon, 25 Sep 2023 19:39:46 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Mon, 25 Sep 2023 19:39:46 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Mon, 25 Sep 2023 19:39:46 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Mon, 25 Sep 2023 19:39:46 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:fc521c5b98350f6fd8c72ace1e48558bb7b53cb3db201a2a3b42095401cd02f1`  
		Last Modified: Wed, 20 Sep 2023 02:48:13 GMT  
		Size: 30.1 MB (30062869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be57ddd88e7a46ad28aa9e7adbff962cc738ade8ec137900e53038f0e7f09e0c`  
		Last Modified: Mon, 25 Sep 2023 19:39:59 GMT  
		Size: 1.6 MB (1644088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6900626db5907a9fdea38e754a64a2d3b51204f395e7aa35dc33bf0437d9f35e`  
		Last Modified: Mon, 25 Sep 2023 19:39:58 GMT  
		Size: 4.1 KB (4115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb41abb93750b931f478cbde94a8d1f7ad40512d4766cec2dbb5bab56b01559`  
		Last Modified: Mon, 25 Sep 2023 19:40:04 GMT  
		Size: 59.8 MB (59751145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57abcdf896fd209aa7f38e6d5d2d8a6461725322bcda1b9517d3eac660203b89`  
		Last Modified: Mon, 25 Sep 2023 19:39:59 GMT  
		Size: 905.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:50c3b7243098d8ad15efa4412768034a702b610221e9f58c394ab38de9a27cb5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:c3487b29bd4cfe7064a23a92a9db5d7b05c76898d6a273f0a35650003677ae7a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101162302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:690dc4b352c18c787ead489a9ab9660cb9b59c538bbe0bb3dd0014beec5501c3`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Mon, 25 Sep 2023 19:21:09 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Mon, 25 Sep 2023 19:21:09 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Mon, 25 Sep 2023 19:21:10 GMT
ENV EMQX_VERSION=5.2.1
# Mon, 25 Sep 2023 19:21:10 GMT
ENV AMD64_SHA256=359a12811e5e6725e4269d9484abd348effdde35c0f2af1f5b63cae790c73020
# Mon, 25 Sep 2023 19:21:10 GMT
ENV ARM64_SHA256=2e0a3e0b33669c9b6da488970a2f92d08d7bd0824295822b205b83461ba4728d
# Mon, 25 Sep 2023 19:21:10 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Mon, 25 Sep 2023 19:21:23 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl;     rm -rf /var/lib/apt/lists/*;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl
# Mon, 25 Sep 2023 19:21:24 GMT
WORKDIR /opt/emqx
# Mon, 25 Sep 2023 19:21:24 GMT
USER emqx
# Mon, 25 Sep 2023 19:21:24 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Mon, 25 Sep 2023 19:21:24 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Mon, 25 Sep 2023 19:21:24 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Mon, 25 Sep 2023 19:21:24 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Mon, 25 Sep 2023 19:21:24 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc61d6b2cab9e777137dcf99de5d2130f5fc71aeaedfe9db7374372bc8fde1e`  
		Last Modified: Mon, 25 Sep 2023 19:21:39 GMT  
		Size: 1.6 MB (1629447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705f111e43d6eb1a415b0ae91899025ddc6d41c20c308e507b7d63975355be3a`  
		Last Modified: Mon, 25 Sep 2023 19:21:39 GMT  
		Size: 4.1 KB (4110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fbab83e4365361212f21e742cfea68928187e9b6f2bf0161257729e7ca27e`  
		Last Modified: Mon, 25 Sep 2023 19:21:46 GMT  
		Size: 68.1 MB (68110131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ba398fb5523476b555e788b016cbc0930eb4a33b561424782e7743aa06c901`  
		Last Modified: Mon, 25 Sep 2023 19:21:39 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:c99d83d1ff9918dfa3d0d003b4bc6312e9bf4369289cd786fdd72b4b7f8ed503
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91463122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b37f898441dd381142791cca1c675099ea0ed9f32c75bc33d9901e471a4281a`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:28 GMT
ADD file:024479be439b4ecb37c939e68673adc72955f3345ca0e809bd13e897709e59e4 in / 
# Wed, 20 Sep 2023 02:44:28 GMT
CMD ["bash"]
# Mon, 25 Sep 2023 19:39:34 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Mon, 25 Sep 2023 19:39:35 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Mon, 25 Sep 2023 19:39:35 GMT
ENV EMQX_VERSION=5.2.1
# Mon, 25 Sep 2023 19:39:35 GMT
ENV AMD64_SHA256=359a12811e5e6725e4269d9484abd348effdde35c0f2af1f5b63cae790c73020
# Mon, 25 Sep 2023 19:39:35 GMT
ENV ARM64_SHA256=2e0a3e0b33669c9b6da488970a2f92d08d7bd0824295822b205b83461ba4728d
# Mon, 25 Sep 2023 19:39:35 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Mon, 25 Sep 2023 19:39:45 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl;     rm -rf /var/lib/apt/lists/*;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl
# Mon, 25 Sep 2023 19:39:46 GMT
WORKDIR /opt/emqx
# Mon, 25 Sep 2023 19:39:46 GMT
USER emqx
# Mon, 25 Sep 2023 19:39:46 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Mon, 25 Sep 2023 19:39:46 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Mon, 25 Sep 2023 19:39:46 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Mon, 25 Sep 2023 19:39:46 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Mon, 25 Sep 2023 19:39:46 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:fc521c5b98350f6fd8c72ace1e48558bb7b53cb3db201a2a3b42095401cd02f1`  
		Last Modified: Wed, 20 Sep 2023 02:48:13 GMT  
		Size: 30.1 MB (30062869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be57ddd88e7a46ad28aa9e7adbff962cc738ade8ec137900e53038f0e7f09e0c`  
		Last Modified: Mon, 25 Sep 2023 19:39:59 GMT  
		Size: 1.6 MB (1644088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6900626db5907a9fdea38e754a64a2d3b51204f395e7aa35dc33bf0437d9f35e`  
		Last Modified: Mon, 25 Sep 2023 19:39:58 GMT  
		Size: 4.1 KB (4115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb41abb93750b931f478cbde94a8d1f7ad40512d4766cec2dbb5bab56b01559`  
		Last Modified: Mon, 25 Sep 2023 19:40:04 GMT  
		Size: 59.8 MB (59751145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57abcdf896fd209aa7f38e6d5d2d8a6461725322bcda1b9517d3eac660203b89`  
		Last Modified: Mon, 25 Sep 2023 19:39:59 GMT  
		Size: 905.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
