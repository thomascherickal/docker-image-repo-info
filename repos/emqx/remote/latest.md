## `emqx:latest`

```console
$ docker pull emqx@sha256:e80f75090e8dfad5cb2f8560823582120da0e97e2de688c72f139471a7d8a08e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:0da18e03ac5868e325ed9d0d8fd0bed6892398631d76771c86d416173ecb0a94
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100553813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cc71c243b1bddb2a83472b82a49d37c593e2864bcaf6ab29751490c325be5ab`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:00:12 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:00:13 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Sat, 29 Jul 2023 04:02:21 GMT
ENV EMQX_VERSION=5.1.3
# Sat, 29 Jul 2023 04:02:21 GMT
ENV AMD64_SHA256=d07916a5c8de0b9ff3ce1e34c526e037c6b3e588b83252b135548fb94a36ecd1
# Sat, 29 Jul 2023 04:02:21 GMT
ENV ARM64_SHA256=1ab925d36703c439a1af907a370198a2880bd1834d0b8def78d79008ba7a4384
# Sat, 29 Jul 2023 04:02:21 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Sat, 29 Jul 2023 04:02:28 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Sat, 29 Jul 2023 04:02:29 GMT
WORKDIR /opt/emqx
# Sat, 29 Jul 2023 04:02:29 GMT
USER emqx
# Sat, 29 Jul 2023 04:02:29 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Sat, 29 Jul 2023 04:02:29 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Sat, 29 Jul 2023 04:02:29 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Sat, 29 Jul 2023 04:02:29 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Sat, 29 Jul 2023 04:02:29 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aae0cd767678d99b5128cb9f0b9f0d533d60f80be20eeda6f6530c35a813613`  
		Last Modified: Fri, 28 Jul 2023 01:01:03 GMT  
		Size: 3.0 MB (2987830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bde007415e9cca4e319dea3b886b7d723309116b3ba73372e0de710d2b6b068`  
		Last Modified: Fri, 28 Jul 2023 01:01:02 GMT  
		Size: 4.1 KB (4111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8dd92661c4a45cd0fb46fff014736bb01b98c157d429971bc11dabca6a4dd7`  
		Last Modified: Sat, 29 Jul 2023 04:02:52 GMT  
		Size: 66.1 MB (66143367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f3cab5c206d9d11e631327d82dd828b91a5cc7e660203223422cc8ba7d6a63`  
		Last Modified: Sat, 29 Jul 2023 04:02:45 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:26bacf373108d95059b6f0d4ab962a18fca4393d5363897d471d184b0d91ce98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.9 MB (90856364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7e33dbd2197c109823ca73328f665ee4ed9ded13926b5f4a6039bff9c2e6a99`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:15 GMT
ADD file:085ecd2f941de953afe5513a41a37412d72cbafd982de581ebd2309b3772b51e in / 
# Thu, 27 Jul 2023 23:43:15 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:59:21 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:59:21 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Fri, 28 Jul 2023 23:35:32 GMT
ENV EMQX_VERSION=5.1.3
# Fri, 28 Jul 2023 23:35:32 GMT
ENV AMD64_SHA256=d07916a5c8de0b9ff3ce1e34c526e037c6b3e588b83252b135548fb94a36ecd1
# Fri, 28 Jul 2023 23:35:32 GMT
ENV ARM64_SHA256=1ab925d36703c439a1af907a370198a2880bd1834d0b8def78d79008ba7a4384
# Fri, 28 Jul 2023 23:35:33 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 28 Jul 2023 23:35:38 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Fri, 28 Jul 2023 23:35:38 GMT
WORKDIR /opt/emqx
# Fri, 28 Jul 2023 23:35:39 GMT
USER emqx
# Fri, 28 Jul 2023 23:35:39 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 28 Jul 2023 23:35:39 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 28 Jul 2023 23:35:39 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 28 Jul 2023 23:35:39 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 23:35:39 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:795b5d192ab1819e75375fead3f2f931bd86046e3308224944f16a5ec3b97424`  
		Last Modified: Thu, 27 Jul 2023 23:47:14 GMT  
		Size: 30.1 MB (30062831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf0f15215e9823dbfc2d709d9ca85f9fdb46f7665c3621f3699f4bed019d389`  
		Last Modified: Fri, 28 Jul 2023 02:00:04 GMT  
		Size: 3.0 MB (3002976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8e62bd45d0ac350812046fdc53fe9edeb5523a9bad244ef297b7eda7e76e15`  
		Last Modified: Fri, 28 Jul 2023 02:00:03 GMT  
		Size: 4.1 KB (4117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b2ff23268f19e2ecc7441d1e0afb5ded4e6bc18b623c194141e4e4b9070c78`  
		Last Modified: Fri, 28 Jul 2023 23:35:57 GMT  
		Size: 57.8 MB (57785536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41459a592ecb37b373bb52f95973709a59941b2b5c6166671a816f013b78671b`  
		Last Modified: Fri, 28 Jul 2023 23:35:52 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
