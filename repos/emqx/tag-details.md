<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `emqx`

-	[`emqx:4`](#emqx4)
-	[`emqx:4.4`](#emqx44)
-	[`emqx:4.4.16`](#emqx4416)
-	[`emqx:5`](#emqx5)
-	[`emqx:5.0`](#emqx50)
-	[`emqx:5.0.20`](#emqx5020)
-	[`emqx:latest`](#emqxlatest)

## `emqx:4`

```console
$ docker pull emqx@sha256:66006f642cc3215583a30c2d15ad386a2fcc1f006aa66a14539c16565a76b7d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:5e552b0687cfef125a11ed39c2e3fe3748922102cb321ed3aac5dbdcc443939e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81269970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57afe9a5c7943aae009fe747656549ce2a26eb2351bbc86e38b3d6fe1c7a9136`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:03:11 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:03:11 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Fri, 10 Mar 2023 20:19:30 GMT
ENV EMQX_VERSION=4.4.15
# Fri, 10 Mar 2023 20:19:30 GMT
ENV OTP=otp24.3.4.2-1
# Fri, 10 Mar 2023 20:19:35 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="14aef227fc0a0e7cb16bfd42cea40ec4670f37f8d0e5242611c7ee642020d653"; fi;     if [ ${arch} = "arm64" ]; then sha256="9904da703e022cc04d5f31a27e802cab6a5a2a395d20314d8a8bd79b018d7458"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Fri, 10 Mar 2023 20:19:36 GMT
WORKDIR /opt/emqx
# Fri, 10 Mar 2023 20:19:36 GMT
USER emqx
# Fri, 10 Mar 2023 20:19:36 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 10 Mar 2023 20:19:36 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Fri, 10 Mar 2023 20:19:36 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Fri, 10 Mar 2023 20:19:36 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 10 Mar 2023 20:19:36 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396ee3d6a271f9fce1d0b1fd4fc0bd3a54cd9c9139a819de5351b130046fea9d`  
		Last Modified: Wed, 01 Mar 2023 05:04:03 GMT  
		Size: 2.6 MB (2569541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79aa88ad721c3aad2bd0e2aaccdbb555263a96f1e69f9f9e7e2e698cbd61acf`  
		Last Modified: Wed, 01 Mar 2023 05:04:02 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070d315b7bbe1b667bcbf292eb0e9b5ae6624ff881e709da5f49b4ee70258429`  
		Last Modified: Fri, 10 Mar 2023 20:20:07 GMT  
		Size: 47.3 MB (47283808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5d5f12478a669f22b1c76437d5156d06c87dd7fbb215e3032c5aaa07bdeb60`  
		Last Modified: Fri, 10 Mar 2023 20:20:02 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:302d388fec6952b4d508bee70da2f2f4edf454e439f0f50873ec4b7be92ec5b8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72692924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:548af17ae2f25781112f862a431310434a58097853c09c32d44e0903ae8f57ab`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:21:03 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:21:03 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Fri, 10 Mar 2023 21:48:16 GMT
ENV EMQX_VERSION=4.4.15
# Fri, 10 Mar 2023 21:48:16 GMT
ENV OTP=otp24.3.4.2-1
# Fri, 10 Mar 2023 21:48:19 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="14aef227fc0a0e7cb16bfd42cea40ec4670f37f8d0e5242611c7ee642020d653"; fi;     if [ ${arch} = "arm64" ]; then sha256="9904da703e022cc04d5f31a27e802cab6a5a2a395d20314d8a8bd79b018d7458"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Fri, 10 Mar 2023 21:48:20 GMT
WORKDIR /opt/emqx
# Fri, 10 Mar 2023 21:48:20 GMT
USER emqx
# Fri, 10 Mar 2023 21:48:20 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 10 Mar 2023 21:48:20 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Fri, 10 Mar 2023 21:48:20 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Fri, 10 Mar 2023 21:48:20 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 10 Mar 2023 21:48:20 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ea117f9b26bad2c79fea1dafb19b2ccbfb0e0744061d7743a5aea0c0e38af7`  
		Last Modified: Wed, 01 Mar 2023 03:21:50 GMT  
		Size: 2.6 MB (2559230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fde159950f1c178189d5f614a5405bd1df5caabc1ebd2bfc1e35376f9bd0e19`  
		Last Modified: Wed, 01 Mar 2023 03:21:50 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c707ab042a290342eb2f3e6ca94316ccbbb85fd1dc124c1492dc5a38dad21c4`  
		Last Modified: Fri, 10 Mar 2023 21:48:46 GMT  
		Size: 40.1 MB (40065658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bb60b18003a6c900ed899cad52f70b16202937acc544953166bb024b35dbdb`  
		Last Modified: Fri, 10 Mar 2023 21:48:43 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:66006f642cc3215583a30c2d15ad386a2fcc1f006aa66a14539c16565a76b7d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:5e552b0687cfef125a11ed39c2e3fe3748922102cb321ed3aac5dbdcc443939e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81269970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57afe9a5c7943aae009fe747656549ce2a26eb2351bbc86e38b3d6fe1c7a9136`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:03:11 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:03:11 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Fri, 10 Mar 2023 20:19:30 GMT
ENV EMQX_VERSION=4.4.15
# Fri, 10 Mar 2023 20:19:30 GMT
ENV OTP=otp24.3.4.2-1
# Fri, 10 Mar 2023 20:19:35 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="14aef227fc0a0e7cb16bfd42cea40ec4670f37f8d0e5242611c7ee642020d653"; fi;     if [ ${arch} = "arm64" ]; then sha256="9904da703e022cc04d5f31a27e802cab6a5a2a395d20314d8a8bd79b018d7458"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Fri, 10 Mar 2023 20:19:36 GMT
WORKDIR /opt/emqx
# Fri, 10 Mar 2023 20:19:36 GMT
USER emqx
# Fri, 10 Mar 2023 20:19:36 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 10 Mar 2023 20:19:36 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Fri, 10 Mar 2023 20:19:36 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Fri, 10 Mar 2023 20:19:36 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 10 Mar 2023 20:19:36 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396ee3d6a271f9fce1d0b1fd4fc0bd3a54cd9c9139a819de5351b130046fea9d`  
		Last Modified: Wed, 01 Mar 2023 05:04:03 GMT  
		Size: 2.6 MB (2569541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79aa88ad721c3aad2bd0e2aaccdbb555263a96f1e69f9f9e7e2e698cbd61acf`  
		Last Modified: Wed, 01 Mar 2023 05:04:02 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070d315b7bbe1b667bcbf292eb0e9b5ae6624ff881e709da5f49b4ee70258429`  
		Last Modified: Fri, 10 Mar 2023 20:20:07 GMT  
		Size: 47.3 MB (47283808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5d5f12478a669f22b1c76437d5156d06c87dd7fbb215e3032c5aaa07bdeb60`  
		Last Modified: Fri, 10 Mar 2023 20:20:02 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:302d388fec6952b4d508bee70da2f2f4edf454e439f0f50873ec4b7be92ec5b8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72692924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:548af17ae2f25781112f862a431310434a58097853c09c32d44e0903ae8f57ab`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:21:03 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:21:03 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Fri, 10 Mar 2023 21:48:16 GMT
ENV EMQX_VERSION=4.4.15
# Fri, 10 Mar 2023 21:48:16 GMT
ENV OTP=otp24.3.4.2-1
# Fri, 10 Mar 2023 21:48:19 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="14aef227fc0a0e7cb16bfd42cea40ec4670f37f8d0e5242611c7ee642020d653"; fi;     if [ ${arch} = "arm64" ]; then sha256="9904da703e022cc04d5f31a27e802cab6a5a2a395d20314d8a8bd79b018d7458"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Fri, 10 Mar 2023 21:48:20 GMT
WORKDIR /opt/emqx
# Fri, 10 Mar 2023 21:48:20 GMT
USER emqx
# Fri, 10 Mar 2023 21:48:20 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 10 Mar 2023 21:48:20 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Fri, 10 Mar 2023 21:48:20 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Fri, 10 Mar 2023 21:48:20 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 10 Mar 2023 21:48:20 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ea117f9b26bad2c79fea1dafb19b2ccbfb0e0744061d7743a5aea0c0e38af7`  
		Last Modified: Wed, 01 Mar 2023 03:21:50 GMT  
		Size: 2.6 MB (2559230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fde159950f1c178189d5f614a5405bd1df5caabc1ebd2bfc1e35376f9bd0e19`  
		Last Modified: Wed, 01 Mar 2023 03:21:50 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c707ab042a290342eb2f3e6ca94316ccbbb85fd1dc124c1492dc5a38dad21c4`  
		Last Modified: Fri, 10 Mar 2023 21:48:46 GMT  
		Size: 40.1 MB (40065658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bb60b18003a6c900ed899cad52f70b16202937acc544953166bb024b35dbdb`  
		Last Modified: Fri, 10 Mar 2023 21:48:43 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.16`

**does not exist** (yet?)

## `emqx:5`

```console
$ docker pull emqx@sha256:46717cea11e956cb8edeb6b900efb34ead650e8ea5e34128b2f266a1dccb5a2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:419cacf6195600e119273142f75802a43aa3345067a905da93afa3c6ef6352ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101213576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d3da61ba7da85ea7d8a71e7377117d6f7e23f7c7a05787bf28600e87334a614`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:03:25 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:03:26 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Fri, 10 Mar 2023 20:19:39 GMT
ENV EMQX_VERSION=5.0.20
# Fri, 10 Mar 2023 20:19:39 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Fri, 10 Mar 2023 20:19:39 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Fri, 10 Mar 2023 20:19:39 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 10 Mar 2023 20:19:44 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Fri, 10 Mar 2023 20:19:45 GMT
WORKDIR /opt/emqx
# Fri, 10 Mar 2023 20:19:45 GMT
USER emqx
# Fri, 10 Mar 2023 20:19:45 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 10 Mar 2023 20:19:45 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 10 Mar 2023 20:19:45 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 10 Mar 2023 20:19:45 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 10 Mar 2023 20:19:46 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a35a595ef04513102e76624112833df5aee4f5e7a95b61fa5eddc304211ab3`  
		Last Modified: Wed, 01 Mar 2023 05:04:19 GMT  
		Size: 3.0 MB (2987679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e798ac719c7147c6c2faada408a48221abe27042dbc139527a475289fd20c98a`  
		Last Modified: Wed, 01 Mar 2023 05:04:19 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eafb9c8208d3bccc697ced82005883b641d02d97977cba3529a803fe07f6df9`  
		Last Modified: Fri, 10 Mar 2023 20:20:26 GMT  
		Size: 66.8 MB (66809481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ede4f97a9c6b64ff913490d403d30cc16ce0befeb510b05b022918bae24e753`  
		Last Modified: Fri, 10 Mar 2023 20:20:18 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:13e95e2fef6dbd597b66a357807ceb71cba9ee2526562f9e3a1c1b8ccd84c33b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92303842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e912e5f1bdce506ce56157f5a78282b230d9c95b6700df96645f9f25e4dce4b5`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:21:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:21:17 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Fri, 10 Mar 2023 21:48:23 GMT
ENV EMQX_VERSION=5.0.20
# Fri, 10 Mar 2023 21:48:23 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Fri, 10 Mar 2023 21:48:23 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Fri, 10 Mar 2023 21:48:23 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 10 Mar 2023 21:48:27 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Fri, 10 Mar 2023 21:48:28 GMT
WORKDIR /opt/emqx
# Fri, 10 Mar 2023 21:48:28 GMT
USER emqx
# Fri, 10 Mar 2023 21:48:28 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 10 Mar 2023 21:48:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 10 Mar 2023 21:48:28 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 10 Mar 2023 21:48:28 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 10 Mar 2023 21:48:28 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38086ab7a191a5da95fb6158c384014d022c21f7e3615ad8b0cdd460c25f9035`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 3.0 MB (3002759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54eeac58f385f878614093545595a71c10cb909203557c85c1b5ef5defba64d`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b403af0a79322aefc651ac609b98935d96017c8baa135e28307c6e9cc0691aff`  
		Last Modified: Fri, 10 Mar 2023 21:49:03 GMT  
		Size: 59.2 MB (59233251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f7b75ab2328825c25f602efb49a16223ab44d99a65a2e8a15856390f623199`  
		Last Modified: Fri, 10 Mar 2023 21:48:57 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:46717cea11e956cb8edeb6b900efb34ead650e8ea5e34128b2f266a1dccb5a2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:419cacf6195600e119273142f75802a43aa3345067a905da93afa3c6ef6352ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101213576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d3da61ba7da85ea7d8a71e7377117d6f7e23f7c7a05787bf28600e87334a614`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:03:25 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:03:26 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Fri, 10 Mar 2023 20:19:39 GMT
ENV EMQX_VERSION=5.0.20
# Fri, 10 Mar 2023 20:19:39 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Fri, 10 Mar 2023 20:19:39 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Fri, 10 Mar 2023 20:19:39 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 10 Mar 2023 20:19:44 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Fri, 10 Mar 2023 20:19:45 GMT
WORKDIR /opt/emqx
# Fri, 10 Mar 2023 20:19:45 GMT
USER emqx
# Fri, 10 Mar 2023 20:19:45 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 10 Mar 2023 20:19:45 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 10 Mar 2023 20:19:45 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 10 Mar 2023 20:19:45 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 10 Mar 2023 20:19:46 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a35a595ef04513102e76624112833df5aee4f5e7a95b61fa5eddc304211ab3`  
		Last Modified: Wed, 01 Mar 2023 05:04:19 GMT  
		Size: 3.0 MB (2987679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e798ac719c7147c6c2faada408a48221abe27042dbc139527a475289fd20c98a`  
		Last Modified: Wed, 01 Mar 2023 05:04:19 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eafb9c8208d3bccc697ced82005883b641d02d97977cba3529a803fe07f6df9`  
		Last Modified: Fri, 10 Mar 2023 20:20:26 GMT  
		Size: 66.8 MB (66809481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ede4f97a9c6b64ff913490d403d30cc16ce0befeb510b05b022918bae24e753`  
		Last Modified: Fri, 10 Mar 2023 20:20:18 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:13e95e2fef6dbd597b66a357807ceb71cba9ee2526562f9e3a1c1b8ccd84c33b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92303842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e912e5f1bdce506ce56157f5a78282b230d9c95b6700df96645f9f25e4dce4b5`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:21:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:21:17 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Fri, 10 Mar 2023 21:48:23 GMT
ENV EMQX_VERSION=5.0.20
# Fri, 10 Mar 2023 21:48:23 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Fri, 10 Mar 2023 21:48:23 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Fri, 10 Mar 2023 21:48:23 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 10 Mar 2023 21:48:27 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Fri, 10 Mar 2023 21:48:28 GMT
WORKDIR /opt/emqx
# Fri, 10 Mar 2023 21:48:28 GMT
USER emqx
# Fri, 10 Mar 2023 21:48:28 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 10 Mar 2023 21:48:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 10 Mar 2023 21:48:28 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 10 Mar 2023 21:48:28 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 10 Mar 2023 21:48:28 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38086ab7a191a5da95fb6158c384014d022c21f7e3615ad8b0cdd460c25f9035`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 3.0 MB (3002759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54eeac58f385f878614093545595a71c10cb909203557c85c1b5ef5defba64d`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b403af0a79322aefc651ac609b98935d96017c8baa135e28307c6e9cc0691aff`  
		Last Modified: Fri, 10 Mar 2023 21:49:03 GMT  
		Size: 59.2 MB (59233251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f7b75ab2328825c25f602efb49a16223ab44d99a65a2e8a15856390f623199`  
		Last Modified: Fri, 10 Mar 2023 21:48:57 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.20`

```console
$ docker pull emqx@sha256:46717cea11e956cb8edeb6b900efb34ead650e8ea5e34128b2f266a1dccb5a2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0.20` - linux; amd64

```console
$ docker pull emqx@sha256:419cacf6195600e119273142f75802a43aa3345067a905da93afa3c6ef6352ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101213576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d3da61ba7da85ea7d8a71e7377117d6f7e23f7c7a05787bf28600e87334a614`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:03:25 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:03:26 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Fri, 10 Mar 2023 20:19:39 GMT
ENV EMQX_VERSION=5.0.20
# Fri, 10 Mar 2023 20:19:39 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Fri, 10 Mar 2023 20:19:39 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Fri, 10 Mar 2023 20:19:39 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 10 Mar 2023 20:19:44 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Fri, 10 Mar 2023 20:19:45 GMT
WORKDIR /opt/emqx
# Fri, 10 Mar 2023 20:19:45 GMT
USER emqx
# Fri, 10 Mar 2023 20:19:45 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 10 Mar 2023 20:19:45 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 10 Mar 2023 20:19:45 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 10 Mar 2023 20:19:45 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 10 Mar 2023 20:19:46 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a35a595ef04513102e76624112833df5aee4f5e7a95b61fa5eddc304211ab3`  
		Last Modified: Wed, 01 Mar 2023 05:04:19 GMT  
		Size: 3.0 MB (2987679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e798ac719c7147c6c2faada408a48221abe27042dbc139527a475289fd20c98a`  
		Last Modified: Wed, 01 Mar 2023 05:04:19 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eafb9c8208d3bccc697ced82005883b641d02d97977cba3529a803fe07f6df9`  
		Last Modified: Fri, 10 Mar 2023 20:20:26 GMT  
		Size: 66.8 MB (66809481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ede4f97a9c6b64ff913490d403d30cc16ce0befeb510b05b022918bae24e753`  
		Last Modified: Fri, 10 Mar 2023 20:20:18 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0.20` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:13e95e2fef6dbd597b66a357807ceb71cba9ee2526562f9e3a1c1b8ccd84c33b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92303842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e912e5f1bdce506ce56157f5a78282b230d9c95b6700df96645f9f25e4dce4b5`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:21:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:21:17 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Fri, 10 Mar 2023 21:48:23 GMT
ENV EMQX_VERSION=5.0.20
# Fri, 10 Mar 2023 21:48:23 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Fri, 10 Mar 2023 21:48:23 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Fri, 10 Mar 2023 21:48:23 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 10 Mar 2023 21:48:27 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Fri, 10 Mar 2023 21:48:28 GMT
WORKDIR /opt/emqx
# Fri, 10 Mar 2023 21:48:28 GMT
USER emqx
# Fri, 10 Mar 2023 21:48:28 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 10 Mar 2023 21:48:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 10 Mar 2023 21:48:28 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 10 Mar 2023 21:48:28 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 10 Mar 2023 21:48:28 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38086ab7a191a5da95fb6158c384014d022c21f7e3615ad8b0cdd460c25f9035`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 3.0 MB (3002759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54eeac58f385f878614093545595a71c10cb909203557c85c1b5ef5defba64d`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b403af0a79322aefc651ac609b98935d96017c8baa135e28307c6e9cc0691aff`  
		Last Modified: Fri, 10 Mar 2023 21:49:03 GMT  
		Size: 59.2 MB (59233251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f7b75ab2328825c25f602efb49a16223ab44d99a65a2e8a15856390f623199`  
		Last Modified: Fri, 10 Mar 2023 21:48:57 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:46717cea11e956cb8edeb6b900efb34ead650e8ea5e34128b2f266a1dccb5a2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:419cacf6195600e119273142f75802a43aa3345067a905da93afa3c6ef6352ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101213576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d3da61ba7da85ea7d8a71e7377117d6f7e23f7c7a05787bf28600e87334a614`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:03:25 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:03:26 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Fri, 10 Mar 2023 20:19:39 GMT
ENV EMQX_VERSION=5.0.20
# Fri, 10 Mar 2023 20:19:39 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Fri, 10 Mar 2023 20:19:39 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Fri, 10 Mar 2023 20:19:39 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 10 Mar 2023 20:19:44 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Fri, 10 Mar 2023 20:19:45 GMT
WORKDIR /opt/emqx
# Fri, 10 Mar 2023 20:19:45 GMT
USER emqx
# Fri, 10 Mar 2023 20:19:45 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 10 Mar 2023 20:19:45 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 10 Mar 2023 20:19:45 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 10 Mar 2023 20:19:45 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 10 Mar 2023 20:19:46 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a35a595ef04513102e76624112833df5aee4f5e7a95b61fa5eddc304211ab3`  
		Last Modified: Wed, 01 Mar 2023 05:04:19 GMT  
		Size: 3.0 MB (2987679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e798ac719c7147c6c2faada408a48221abe27042dbc139527a475289fd20c98a`  
		Last Modified: Wed, 01 Mar 2023 05:04:19 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eafb9c8208d3bccc697ced82005883b641d02d97977cba3529a803fe07f6df9`  
		Last Modified: Fri, 10 Mar 2023 20:20:26 GMT  
		Size: 66.8 MB (66809481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ede4f97a9c6b64ff913490d403d30cc16ce0befeb510b05b022918bae24e753`  
		Last Modified: Fri, 10 Mar 2023 20:20:18 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:13e95e2fef6dbd597b66a357807ceb71cba9ee2526562f9e3a1c1b8ccd84c33b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92303842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e912e5f1bdce506ce56157f5a78282b230d9c95b6700df96645f9f25e4dce4b5`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:21:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:21:17 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Fri, 10 Mar 2023 21:48:23 GMT
ENV EMQX_VERSION=5.0.20
# Fri, 10 Mar 2023 21:48:23 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Fri, 10 Mar 2023 21:48:23 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Fri, 10 Mar 2023 21:48:23 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 10 Mar 2023 21:48:27 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Fri, 10 Mar 2023 21:48:28 GMT
WORKDIR /opt/emqx
# Fri, 10 Mar 2023 21:48:28 GMT
USER emqx
# Fri, 10 Mar 2023 21:48:28 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 10 Mar 2023 21:48:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 10 Mar 2023 21:48:28 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 10 Mar 2023 21:48:28 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 10 Mar 2023 21:48:28 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38086ab7a191a5da95fb6158c384014d022c21f7e3615ad8b0cdd460c25f9035`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 3.0 MB (3002759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54eeac58f385f878614093545595a71c10cb909203557c85c1b5ef5defba64d`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b403af0a79322aefc651ac609b98935d96017c8baa135e28307c6e9cc0691aff`  
		Last Modified: Fri, 10 Mar 2023 21:49:03 GMT  
		Size: 59.2 MB (59233251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f7b75ab2328825c25f602efb49a16223ab44d99a65a2e8a15856390f623199`  
		Last Modified: Fri, 10 Mar 2023 21:48:57 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
