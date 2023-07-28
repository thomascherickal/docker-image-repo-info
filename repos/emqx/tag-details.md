<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `emqx`

-	[`emqx:4`](#emqx4)
-	[`emqx:4.4`](#emqx44)
-	[`emqx:4.4.19`](#emqx4419)
-	[`emqx:5`](#emqx5)
-	[`emqx:5.0`](#emqx50)
-	[`emqx:5.0.26`](#emqx5026)
-	[`emqx:5.1`](#emqx51)
-	[`emqx:5.1.2`](#emqx512)
-	[`emqx:latest`](#emqxlatest)

## `emqx:4`

```console
$ docker pull emqx@sha256:d725d5f22bacc08925f2985a6331322920913c4996f8505493013ac052ee23c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:fc50beecaa7b5c1e46d8f8bfc8cbbb488338b66aa4bcebc668db86420c66a274
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.4 MB (81431006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc3bcc2f5087e2da0565a5db36c800051b3cfad79f834da16862329e41b4a2b7`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:59:58 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:59:58 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Fri, 28 Jul 2023 00:59:58 GMT
ENV EMQX_VERSION=4.4.19
# Fri, 28 Jul 2023 00:59:58 GMT
ENV OTP=otp24.3.4.2-1
# Fri, 28 Jul 2023 01:00:04 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="bf4192c64c9006733b30f96fe99506a0a3af115c7073995a044cc0e60230675e"; fi;     if [ ${arch} = "arm64" ]; then sha256="7cd27d5112380fd4d81029b10ba862a050b0bba8af1eb90aac669189fc3053c0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$(sha256sum $pkg)";     echo "$sha256 *$pkg" | sha256sum -c;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Fri, 28 Jul 2023 01:00:04 GMT
WORKDIR /opt/emqx
# Fri, 28 Jul 2023 01:00:04 GMT
USER emqx
# Fri, 28 Jul 2023 01:00:04 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 28 Jul 2023 01:00:04 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Fri, 28 Jul 2023 01:00:05 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Fri, 28 Jul 2023 01:00:05 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:00:05 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e690ff3367f4d3d3d39a37f40fdf863ae19ae3695fd90f42378f95d7c177305`  
		Last Modified: Fri, 28 Jul 2023 01:00:47 GMT  
		Size: 2.6 MB (2569629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39372de4932c8edd554c7282e088f4a7dbe87e9c95f62bb6ae7e40f16629a6b6`  
		Last Modified: Fri, 28 Jul 2023 01:00:47 GMT  
		Size: 4.1 KB (4111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6238515153ee9a756e508b5fdbe8e7f35bfd039c91baedba8531a446c9ad71c7`  
		Last Modified: Fri, 28 Jul 2023 01:00:52 GMT  
		Size: 47.4 MB (47438555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f7909d008f4712e46f7ab113b9632d2c4831fd5fe2816b2395320738625d04`  
		Last Modified: Fri, 28 Jul 2023 01:00:47 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:bd9a13fefeaa141317d829c013ab43caf2b68d5c83d530d01b94830e714fdae5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.8 MB (72845146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc477ef5340781063780f5d0603c5cd6d1976bbfad58e3880fce76e1abddfe7`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:15 GMT
ADD file:085ecd2f941de953afe5513a41a37412d72cbafd982de581ebd2309b3772b51e in / 
# Thu, 27 Jul 2023 23:43:15 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:59:09 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:59:10 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Fri, 28 Jul 2023 01:59:10 GMT
ENV EMQX_VERSION=4.4.19
# Fri, 28 Jul 2023 01:59:10 GMT
ENV OTP=otp24.3.4.2-1
# Fri, 28 Jul 2023 01:59:14 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="bf4192c64c9006733b30f96fe99506a0a3af115c7073995a044cc0e60230675e"; fi;     if [ ${arch} = "arm64" ]; then sha256="7cd27d5112380fd4d81029b10ba862a050b0bba8af1eb90aac669189fc3053c0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$(sha256sum $pkg)";     echo "$sha256 *$pkg" | sha256sum -c;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Fri, 28 Jul 2023 01:59:14 GMT
WORKDIR /opt/emqx
# Fri, 28 Jul 2023 01:59:14 GMT
USER emqx
# Fri, 28 Jul 2023 01:59:14 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 28 Jul 2023 01:59:14 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Fri, 28 Jul 2023 01:59:15 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Fri, 28 Jul 2023 01:59:15 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:59:15 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:795b5d192ab1819e75375fead3f2f931bd86046e3308224944f16a5ec3b97424`  
		Last Modified: Thu, 27 Jul 2023 23:47:14 GMT  
		Size: 30.1 MB (30062831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d974c15af0511d2e80822a01aff4c9ab7cf452adb0ead23b34c473ba53e7800`  
		Last Modified: Fri, 28 Jul 2023 01:59:49 GMT  
		Size: 2.6 MB (2559432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7001284e1b299bea800aafb75ca8535248fd87caa04afcf274c5285de7afa141`  
		Last Modified: Fri, 28 Jul 2023 01:59:48 GMT  
		Size: 4.1 KB (4116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54059c3a431f1767b6da30b1d0abae98736402c42de24eff3e080ed5ab9034e`  
		Last Modified: Fri, 28 Jul 2023 01:59:52 GMT  
		Size: 40.2 MB (40217658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff013677fafb7f4521f32804e4798d73220eab570eda7213b7a09c1627323f8e`  
		Last Modified: Fri, 28 Jul 2023 01:59:48 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:d725d5f22bacc08925f2985a6331322920913c4996f8505493013ac052ee23c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:fc50beecaa7b5c1e46d8f8bfc8cbbb488338b66aa4bcebc668db86420c66a274
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.4 MB (81431006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc3bcc2f5087e2da0565a5db36c800051b3cfad79f834da16862329e41b4a2b7`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:59:58 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:59:58 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Fri, 28 Jul 2023 00:59:58 GMT
ENV EMQX_VERSION=4.4.19
# Fri, 28 Jul 2023 00:59:58 GMT
ENV OTP=otp24.3.4.2-1
# Fri, 28 Jul 2023 01:00:04 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="bf4192c64c9006733b30f96fe99506a0a3af115c7073995a044cc0e60230675e"; fi;     if [ ${arch} = "arm64" ]; then sha256="7cd27d5112380fd4d81029b10ba862a050b0bba8af1eb90aac669189fc3053c0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$(sha256sum $pkg)";     echo "$sha256 *$pkg" | sha256sum -c;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Fri, 28 Jul 2023 01:00:04 GMT
WORKDIR /opt/emqx
# Fri, 28 Jul 2023 01:00:04 GMT
USER emqx
# Fri, 28 Jul 2023 01:00:04 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 28 Jul 2023 01:00:04 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Fri, 28 Jul 2023 01:00:05 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Fri, 28 Jul 2023 01:00:05 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:00:05 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e690ff3367f4d3d3d39a37f40fdf863ae19ae3695fd90f42378f95d7c177305`  
		Last Modified: Fri, 28 Jul 2023 01:00:47 GMT  
		Size: 2.6 MB (2569629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39372de4932c8edd554c7282e088f4a7dbe87e9c95f62bb6ae7e40f16629a6b6`  
		Last Modified: Fri, 28 Jul 2023 01:00:47 GMT  
		Size: 4.1 KB (4111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6238515153ee9a756e508b5fdbe8e7f35bfd039c91baedba8531a446c9ad71c7`  
		Last Modified: Fri, 28 Jul 2023 01:00:52 GMT  
		Size: 47.4 MB (47438555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f7909d008f4712e46f7ab113b9632d2c4831fd5fe2816b2395320738625d04`  
		Last Modified: Fri, 28 Jul 2023 01:00:47 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:bd9a13fefeaa141317d829c013ab43caf2b68d5c83d530d01b94830e714fdae5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.8 MB (72845146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc477ef5340781063780f5d0603c5cd6d1976bbfad58e3880fce76e1abddfe7`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:15 GMT
ADD file:085ecd2f941de953afe5513a41a37412d72cbafd982de581ebd2309b3772b51e in / 
# Thu, 27 Jul 2023 23:43:15 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:59:09 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:59:10 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Fri, 28 Jul 2023 01:59:10 GMT
ENV EMQX_VERSION=4.4.19
# Fri, 28 Jul 2023 01:59:10 GMT
ENV OTP=otp24.3.4.2-1
# Fri, 28 Jul 2023 01:59:14 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="bf4192c64c9006733b30f96fe99506a0a3af115c7073995a044cc0e60230675e"; fi;     if [ ${arch} = "arm64" ]; then sha256="7cd27d5112380fd4d81029b10ba862a050b0bba8af1eb90aac669189fc3053c0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$(sha256sum $pkg)";     echo "$sha256 *$pkg" | sha256sum -c;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Fri, 28 Jul 2023 01:59:14 GMT
WORKDIR /opt/emqx
# Fri, 28 Jul 2023 01:59:14 GMT
USER emqx
# Fri, 28 Jul 2023 01:59:14 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 28 Jul 2023 01:59:14 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Fri, 28 Jul 2023 01:59:15 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Fri, 28 Jul 2023 01:59:15 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:59:15 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:795b5d192ab1819e75375fead3f2f931bd86046e3308224944f16a5ec3b97424`  
		Last Modified: Thu, 27 Jul 2023 23:47:14 GMT  
		Size: 30.1 MB (30062831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d974c15af0511d2e80822a01aff4c9ab7cf452adb0ead23b34c473ba53e7800`  
		Last Modified: Fri, 28 Jul 2023 01:59:49 GMT  
		Size: 2.6 MB (2559432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7001284e1b299bea800aafb75ca8535248fd87caa04afcf274c5285de7afa141`  
		Last Modified: Fri, 28 Jul 2023 01:59:48 GMT  
		Size: 4.1 KB (4116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54059c3a431f1767b6da30b1d0abae98736402c42de24eff3e080ed5ab9034e`  
		Last Modified: Fri, 28 Jul 2023 01:59:52 GMT  
		Size: 40.2 MB (40217658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff013677fafb7f4521f32804e4798d73220eab570eda7213b7a09c1627323f8e`  
		Last Modified: Fri, 28 Jul 2023 01:59:48 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.19`

```console
$ docker pull emqx@sha256:d725d5f22bacc08925f2985a6331322920913c4996f8505493013ac052ee23c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4.19` - linux; amd64

```console
$ docker pull emqx@sha256:fc50beecaa7b5c1e46d8f8bfc8cbbb488338b66aa4bcebc668db86420c66a274
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.4 MB (81431006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc3bcc2f5087e2da0565a5db36c800051b3cfad79f834da16862329e41b4a2b7`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:59:58 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:59:58 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Fri, 28 Jul 2023 00:59:58 GMT
ENV EMQX_VERSION=4.4.19
# Fri, 28 Jul 2023 00:59:58 GMT
ENV OTP=otp24.3.4.2-1
# Fri, 28 Jul 2023 01:00:04 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="bf4192c64c9006733b30f96fe99506a0a3af115c7073995a044cc0e60230675e"; fi;     if [ ${arch} = "arm64" ]; then sha256="7cd27d5112380fd4d81029b10ba862a050b0bba8af1eb90aac669189fc3053c0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$(sha256sum $pkg)";     echo "$sha256 *$pkg" | sha256sum -c;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Fri, 28 Jul 2023 01:00:04 GMT
WORKDIR /opt/emqx
# Fri, 28 Jul 2023 01:00:04 GMT
USER emqx
# Fri, 28 Jul 2023 01:00:04 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 28 Jul 2023 01:00:04 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Fri, 28 Jul 2023 01:00:05 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Fri, 28 Jul 2023 01:00:05 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:00:05 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e690ff3367f4d3d3d39a37f40fdf863ae19ae3695fd90f42378f95d7c177305`  
		Last Modified: Fri, 28 Jul 2023 01:00:47 GMT  
		Size: 2.6 MB (2569629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39372de4932c8edd554c7282e088f4a7dbe87e9c95f62bb6ae7e40f16629a6b6`  
		Last Modified: Fri, 28 Jul 2023 01:00:47 GMT  
		Size: 4.1 KB (4111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6238515153ee9a756e508b5fdbe8e7f35bfd039c91baedba8531a446c9ad71c7`  
		Last Modified: Fri, 28 Jul 2023 01:00:52 GMT  
		Size: 47.4 MB (47438555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f7909d008f4712e46f7ab113b9632d2c4831fd5fe2816b2395320738625d04`  
		Last Modified: Fri, 28 Jul 2023 01:00:47 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4.19` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:bd9a13fefeaa141317d829c013ab43caf2b68d5c83d530d01b94830e714fdae5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.8 MB (72845146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc477ef5340781063780f5d0603c5cd6d1976bbfad58e3880fce76e1abddfe7`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:15 GMT
ADD file:085ecd2f941de953afe5513a41a37412d72cbafd982de581ebd2309b3772b51e in / 
# Thu, 27 Jul 2023 23:43:15 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:59:09 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:59:10 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Fri, 28 Jul 2023 01:59:10 GMT
ENV EMQX_VERSION=4.4.19
# Fri, 28 Jul 2023 01:59:10 GMT
ENV OTP=otp24.3.4.2-1
# Fri, 28 Jul 2023 01:59:14 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="bf4192c64c9006733b30f96fe99506a0a3af115c7073995a044cc0e60230675e"; fi;     if [ ${arch} = "arm64" ]; then sha256="7cd27d5112380fd4d81029b10ba862a050b0bba8af1eb90aac669189fc3053c0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$(sha256sum $pkg)";     echo "$sha256 *$pkg" | sha256sum -c;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Fri, 28 Jul 2023 01:59:14 GMT
WORKDIR /opt/emqx
# Fri, 28 Jul 2023 01:59:14 GMT
USER emqx
# Fri, 28 Jul 2023 01:59:14 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 28 Jul 2023 01:59:14 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Fri, 28 Jul 2023 01:59:15 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Fri, 28 Jul 2023 01:59:15 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:59:15 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:795b5d192ab1819e75375fead3f2f931bd86046e3308224944f16a5ec3b97424`  
		Last Modified: Thu, 27 Jul 2023 23:47:14 GMT  
		Size: 30.1 MB (30062831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d974c15af0511d2e80822a01aff4c9ab7cf452adb0ead23b34c473ba53e7800`  
		Last Modified: Fri, 28 Jul 2023 01:59:49 GMT  
		Size: 2.6 MB (2559432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7001284e1b299bea800aafb75ca8535248fd87caa04afcf274c5285de7afa141`  
		Last Modified: Fri, 28 Jul 2023 01:59:48 GMT  
		Size: 4.1 KB (4116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54059c3a431f1767b6da30b1d0abae98736402c42de24eff3e080ed5ab9034e`  
		Last Modified: Fri, 28 Jul 2023 01:59:52 GMT  
		Size: 40.2 MB (40217658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff013677fafb7f4521f32804e4798d73220eab570eda7213b7a09c1627323f8e`  
		Last Modified: Fri, 28 Jul 2023 01:59:48 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5`

```console
$ docker pull emqx@sha256:da87e3be9e81fa4503ac5e3f6f1d2b6323e4cda5fcf80a8251ab5e748c538667
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:22c80fc187af5e905971c228f5249c7e890bf33c0226671b097b25699a67b147
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.5 MB (100541550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6dd13511aef47b4507981a841ff223065fc6ba8d475a51bd3bf7aa566309d66`
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
# Fri, 28 Jul 2023 01:00:24 GMT
ENV EMQX_VERSION=5.1.2
# Fri, 28 Jul 2023 01:00:24 GMT
ENV AMD64_SHA256=bd34a8cfcd816305b4fc8bfb67fb8a0a29dcf7bd2e391e79534bf7d94d62ffcd
# Fri, 28 Jul 2023 01:00:25 GMT
ENV ARM64_SHA256=02d281020403f55f9d5eac5a2ffbdaebc888aa8e4b92fce847f23541f2b0eae5
# Fri, 28 Jul 2023 01:00:25 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 28 Jul 2023 01:00:32 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Fri, 28 Jul 2023 01:00:32 GMT
WORKDIR /opt/emqx
# Fri, 28 Jul 2023 01:00:32 GMT
USER emqx
# Fri, 28 Jul 2023 01:00:32 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 28 Jul 2023 01:00:32 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 28 Jul 2023 01:00:32 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 28 Jul 2023 01:00:33 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:00:33 GMT
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
	-	`sha256:653821671e5a185406df546f8943340f6769ab3efa9290fe421be10b1fc764f8`  
		Last Modified: Fri, 28 Jul 2023 01:01:27 GMT  
		Size: 66.1 MB (66131105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cd8f9966de08a13a3fdf9adac440a9019f879b9bede5c9ae0b5725ff410c26`  
		Last Modified: Fri, 28 Jul 2023 01:01:20 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:324691e5bc117de5bdf517fc988eb4b406c5e513f03f27d5c55a5cee421e75bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.8 MB (90839082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67b5546346cd38a0abdcf26e1113a3b4173a6602e6703d84e337ae356d8ffb2d`
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
# Fri, 28 Jul 2023 01:59:30 GMT
ENV EMQX_VERSION=5.1.2
# Fri, 28 Jul 2023 01:59:30 GMT
ENV AMD64_SHA256=bd34a8cfcd816305b4fc8bfb67fb8a0a29dcf7bd2e391e79534bf7d94d62ffcd
# Fri, 28 Jul 2023 01:59:30 GMT
ENV ARM64_SHA256=02d281020403f55f9d5eac5a2ffbdaebc888aa8e4b92fce847f23541f2b0eae5
# Fri, 28 Jul 2023 01:59:30 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 28 Jul 2023 01:59:36 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Fri, 28 Jul 2023 01:59:37 GMT
WORKDIR /opt/emqx
# Fri, 28 Jul 2023 01:59:37 GMT
USER emqx
# Fri, 28 Jul 2023 01:59:37 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 28 Jul 2023 01:59:37 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 28 Jul 2023 01:59:37 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 28 Jul 2023 01:59:37 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:59:37 GMT
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
	-	`sha256:48cf3bb4a948e6cd9c7d7b52bfa8de530a27fc7848c8f419ae1122ced59359e2`  
		Last Modified: Fri, 28 Jul 2023 02:00:25 GMT  
		Size: 57.8 MB (57768254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8a5ca4e496448073b25fd4a99ac622d77eb43ddcaa206f53d89d8a15b31033`  
		Last Modified: Fri, 28 Jul 2023 02:00:19 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:d4d70c329b04edb06ea817d450a8a5dd7769e7b220e2bb6510c8452098977c0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:fc52de5e495b2127918496f4279ce1175fa131ce3dd3f104ee6589565a02dd34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101982317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1dd67ffa630f220137ee6f5f73b65717f8a54256a8e063c705ffcfc115aed6c`
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
# Fri, 28 Jul 2023 01:00:13 GMT
ENV EMQX_VERSION=5.0.26
# Fri, 28 Jul 2023 01:00:13 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Fri, 28 Jul 2023 01:00:13 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Fri, 28 Jul 2023 01:00:13 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 28 Jul 2023 01:00:19 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Fri, 28 Jul 2023 01:00:20 GMT
WORKDIR /opt/emqx
# Fri, 28 Jul 2023 01:00:20 GMT
USER emqx
# Fri, 28 Jul 2023 01:00:20 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 28 Jul 2023 01:00:20 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 28 Jul 2023 01:00:20 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 28 Jul 2023 01:00:20 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:00:20 GMT
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
	-	`sha256:6788aa6e14f2bb644a8ea6308bc63a5293c7100c1cf56c89d166f0fbafc7f452`  
		Last Modified: Fri, 28 Jul 2023 01:01:11 GMT  
		Size: 67.6 MB (67571870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0def11967b7af57de71d52d148a123356502d2957e2fa39a551edd11526ae9dc`  
		Last Modified: Fri, 28 Jul 2023 01:01:02 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:fdf8d4f3160ccdf8a671edb7b858d164d8e069efe540feaac01ed1804f568b5e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93060205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87b2f145a7f6051f04edf50bee594cf3982ccf34d7a6f48eed72df2e29e17d76`
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
# Fri, 28 Jul 2023 01:59:21 GMT
ENV EMQX_VERSION=5.0.26
# Fri, 28 Jul 2023 01:59:22 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Fri, 28 Jul 2023 01:59:22 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Fri, 28 Jul 2023 01:59:22 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 28 Jul 2023 01:59:27 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Fri, 28 Jul 2023 01:59:27 GMT
WORKDIR /opt/emqx
# Fri, 28 Jul 2023 01:59:27 GMT
USER emqx
# Fri, 28 Jul 2023 01:59:27 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 28 Jul 2023 01:59:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 28 Jul 2023 01:59:28 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 28 Jul 2023 01:59:28 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:59:28 GMT
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
	-	`sha256:6e8cdb006975f3f3bedcc48175067ce996aa06aea26cf338f1c454ae06fb1e02`  
		Last Modified: Fri, 28 Jul 2023 02:00:09 GMT  
		Size: 60.0 MB (59989378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c6e5fa84728761e69e7cd1a741d97796a168b35b7903fb1e864b7753e98b75`  
		Last Modified: Fri, 28 Jul 2023 02:00:03 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.26`

```console
$ docker pull emqx@sha256:d4d70c329b04edb06ea817d450a8a5dd7769e7b220e2bb6510c8452098977c0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0.26` - linux; amd64

```console
$ docker pull emqx@sha256:fc52de5e495b2127918496f4279ce1175fa131ce3dd3f104ee6589565a02dd34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101982317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1dd67ffa630f220137ee6f5f73b65717f8a54256a8e063c705ffcfc115aed6c`
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
# Fri, 28 Jul 2023 01:00:13 GMT
ENV EMQX_VERSION=5.0.26
# Fri, 28 Jul 2023 01:00:13 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Fri, 28 Jul 2023 01:00:13 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Fri, 28 Jul 2023 01:00:13 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 28 Jul 2023 01:00:19 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Fri, 28 Jul 2023 01:00:20 GMT
WORKDIR /opt/emqx
# Fri, 28 Jul 2023 01:00:20 GMT
USER emqx
# Fri, 28 Jul 2023 01:00:20 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 28 Jul 2023 01:00:20 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 28 Jul 2023 01:00:20 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 28 Jul 2023 01:00:20 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:00:20 GMT
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
	-	`sha256:6788aa6e14f2bb644a8ea6308bc63a5293c7100c1cf56c89d166f0fbafc7f452`  
		Last Modified: Fri, 28 Jul 2023 01:01:11 GMT  
		Size: 67.6 MB (67571870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0def11967b7af57de71d52d148a123356502d2957e2fa39a551edd11526ae9dc`  
		Last Modified: Fri, 28 Jul 2023 01:01:02 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0.26` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:fdf8d4f3160ccdf8a671edb7b858d164d8e069efe540feaac01ed1804f568b5e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93060205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87b2f145a7f6051f04edf50bee594cf3982ccf34d7a6f48eed72df2e29e17d76`
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
# Fri, 28 Jul 2023 01:59:21 GMT
ENV EMQX_VERSION=5.0.26
# Fri, 28 Jul 2023 01:59:22 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Fri, 28 Jul 2023 01:59:22 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Fri, 28 Jul 2023 01:59:22 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 28 Jul 2023 01:59:27 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Fri, 28 Jul 2023 01:59:27 GMT
WORKDIR /opt/emqx
# Fri, 28 Jul 2023 01:59:27 GMT
USER emqx
# Fri, 28 Jul 2023 01:59:27 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 28 Jul 2023 01:59:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 28 Jul 2023 01:59:28 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 28 Jul 2023 01:59:28 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:59:28 GMT
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
	-	`sha256:6e8cdb006975f3f3bedcc48175067ce996aa06aea26cf338f1c454ae06fb1e02`  
		Last Modified: Fri, 28 Jul 2023 02:00:09 GMT  
		Size: 60.0 MB (59989378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c6e5fa84728761e69e7cd1a741d97796a168b35b7903fb1e864b7753e98b75`  
		Last Modified: Fri, 28 Jul 2023 02:00:03 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.1`

```console
$ docker pull emqx@sha256:da87e3be9e81fa4503ac5e3f6f1d2b6323e4cda5fcf80a8251ab5e748c538667
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.1` - linux; amd64

```console
$ docker pull emqx@sha256:22c80fc187af5e905971c228f5249c7e890bf33c0226671b097b25699a67b147
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.5 MB (100541550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6dd13511aef47b4507981a841ff223065fc6ba8d475a51bd3bf7aa566309d66`
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
# Fri, 28 Jul 2023 01:00:24 GMT
ENV EMQX_VERSION=5.1.2
# Fri, 28 Jul 2023 01:00:24 GMT
ENV AMD64_SHA256=bd34a8cfcd816305b4fc8bfb67fb8a0a29dcf7bd2e391e79534bf7d94d62ffcd
# Fri, 28 Jul 2023 01:00:25 GMT
ENV ARM64_SHA256=02d281020403f55f9d5eac5a2ffbdaebc888aa8e4b92fce847f23541f2b0eae5
# Fri, 28 Jul 2023 01:00:25 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 28 Jul 2023 01:00:32 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Fri, 28 Jul 2023 01:00:32 GMT
WORKDIR /opt/emqx
# Fri, 28 Jul 2023 01:00:32 GMT
USER emqx
# Fri, 28 Jul 2023 01:00:32 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 28 Jul 2023 01:00:32 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 28 Jul 2023 01:00:32 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 28 Jul 2023 01:00:33 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:00:33 GMT
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
	-	`sha256:653821671e5a185406df546f8943340f6769ab3efa9290fe421be10b1fc764f8`  
		Last Modified: Fri, 28 Jul 2023 01:01:27 GMT  
		Size: 66.1 MB (66131105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cd8f9966de08a13a3fdf9adac440a9019f879b9bede5c9ae0b5725ff410c26`  
		Last Modified: Fri, 28 Jul 2023 01:01:20 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.1` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:324691e5bc117de5bdf517fc988eb4b406c5e513f03f27d5c55a5cee421e75bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.8 MB (90839082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67b5546346cd38a0abdcf26e1113a3b4173a6602e6703d84e337ae356d8ffb2d`
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
# Fri, 28 Jul 2023 01:59:30 GMT
ENV EMQX_VERSION=5.1.2
# Fri, 28 Jul 2023 01:59:30 GMT
ENV AMD64_SHA256=bd34a8cfcd816305b4fc8bfb67fb8a0a29dcf7bd2e391e79534bf7d94d62ffcd
# Fri, 28 Jul 2023 01:59:30 GMT
ENV ARM64_SHA256=02d281020403f55f9d5eac5a2ffbdaebc888aa8e4b92fce847f23541f2b0eae5
# Fri, 28 Jul 2023 01:59:30 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 28 Jul 2023 01:59:36 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Fri, 28 Jul 2023 01:59:37 GMT
WORKDIR /opt/emqx
# Fri, 28 Jul 2023 01:59:37 GMT
USER emqx
# Fri, 28 Jul 2023 01:59:37 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 28 Jul 2023 01:59:37 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 28 Jul 2023 01:59:37 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 28 Jul 2023 01:59:37 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:59:37 GMT
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
	-	`sha256:48cf3bb4a948e6cd9c7d7b52bfa8de530a27fc7848c8f419ae1122ced59359e2`  
		Last Modified: Fri, 28 Jul 2023 02:00:25 GMT  
		Size: 57.8 MB (57768254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8a5ca4e496448073b25fd4a99ac622d77eb43ddcaa206f53d89d8a15b31033`  
		Last Modified: Fri, 28 Jul 2023 02:00:19 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.1.2`

```console
$ docker pull emqx@sha256:da87e3be9e81fa4503ac5e3f6f1d2b6323e4cda5fcf80a8251ab5e748c538667
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.1.2` - linux; amd64

```console
$ docker pull emqx@sha256:22c80fc187af5e905971c228f5249c7e890bf33c0226671b097b25699a67b147
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.5 MB (100541550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6dd13511aef47b4507981a841ff223065fc6ba8d475a51bd3bf7aa566309d66`
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
# Fri, 28 Jul 2023 01:00:24 GMT
ENV EMQX_VERSION=5.1.2
# Fri, 28 Jul 2023 01:00:24 GMT
ENV AMD64_SHA256=bd34a8cfcd816305b4fc8bfb67fb8a0a29dcf7bd2e391e79534bf7d94d62ffcd
# Fri, 28 Jul 2023 01:00:25 GMT
ENV ARM64_SHA256=02d281020403f55f9d5eac5a2ffbdaebc888aa8e4b92fce847f23541f2b0eae5
# Fri, 28 Jul 2023 01:00:25 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 28 Jul 2023 01:00:32 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Fri, 28 Jul 2023 01:00:32 GMT
WORKDIR /opt/emqx
# Fri, 28 Jul 2023 01:00:32 GMT
USER emqx
# Fri, 28 Jul 2023 01:00:32 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 28 Jul 2023 01:00:32 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 28 Jul 2023 01:00:32 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 28 Jul 2023 01:00:33 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:00:33 GMT
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
	-	`sha256:653821671e5a185406df546f8943340f6769ab3efa9290fe421be10b1fc764f8`  
		Last Modified: Fri, 28 Jul 2023 01:01:27 GMT  
		Size: 66.1 MB (66131105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cd8f9966de08a13a3fdf9adac440a9019f879b9bede5c9ae0b5725ff410c26`  
		Last Modified: Fri, 28 Jul 2023 01:01:20 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.1.2` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:324691e5bc117de5bdf517fc988eb4b406c5e513f03f27d5c55a5cee421e75bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.8 MB (90839082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67b5546346cd38a0abdcf26e1113a3b4173a6602e6703d84e337ae356d8ffb2d`
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
# Fri, 28 Jul 2023 01:59:30 GMT
ENV EMQX_VERSION=5.1.2
# Fri, 28 Jul 2023 01:59:30 GMT
ENV AMD64_SHA256=bd34a8cfcd816305b4fc8bfb67fb8a0a29dcf7bd2e391e79534bf7d94d62ffcd
# Fri, 28 Jul 2023 01:59:30 GMT
ENV ARM64_SHA256=02d281020403f55f9d5eac5a2ffbdaebc888aa8e4b92fce847f23541f2b0eae5
# Fri, 28 Jul 2023 01:59:30 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 28 Jul 2023 01:59:36 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Fri, 28 Jul 2023 01:59:37 GMT
WORKDIR /opt/emqx
# Fri, 28 Jul 2023 01:59:37 GMT
USER emqx
# Fri, 28 Jul 2023 01:59:37 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 28 Jul 2023 01:59:37 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 28 Jul 2023 01:59:37 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 28 Jul 2023 01:59:37 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:59:37 GMT
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
	-	`sha256:48cf3bb4a948e6cd9c7d7b52bfa8de530a27fc7848c8f419ae1122ced59359e2`  
		Last Modified: Fri, 28 Jul 2023 02:00:25 GMT  
		Size: 57.8 MB (57768254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8a5ca4e496448073b25fd4a99ac622d77eb43ddcaa206f53d89d8a15b31033`  
		Last Modified: Fri, 28 Jul 2023 02:00:19 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:da87e3be9e81fa4503ac5e3f6f1d2b6323e4cda5fcf80a8251ab5e748c538667
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:22c80fc187af5e905971c228f5249c7e890bf33c0226671b097b25699a67b147
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.5 MB (100541550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6dd13511aef47b4507981a841ff223065fc6ba8d475a51bd3bf7aa566309d66`
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
# Fri, 28 Jul 2023 01:00:24 GMT
ENV EMQX_VERSION=5.1.2
# Fri, 28 Jul 2023 01:00:24 GMT
ENV AMD64_SHA256=bd34a8cfcd816305b4fc8bfb67fb8a0a29dcf7bd2e391e79534bf7d94d62ffcd
# Fri, 28 Jul 2023 01:00:25 GMT
ENV ARM64_SHA256=02d281020403f55f9d5eac5a2ffbdaebc888aa8e4b92fce847f23541f2b0eae5
# Fri, 28 Jul 2023 01:00:25 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 28 Jul 2023 01:00:32 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Fri, 28 Jul 2023 01:00:32 GMT
WORKDIR /opt/emqx
# Fri, 28 Jul 2023 01:00:32 GMT
USER emqx
# Fri, 28 Jul 2023 01:00:32 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 28 Jul 2023 01:00:32 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 28 Jul 2023 01:00:32 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 28 Jul 2023 01:00:33 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:00:33 GMT
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
	-	`sha256:653821671e5a185406df546f8943340f6769ab3efa9290fe421be10b1fc764f8`  
		Last Modified: Fri, 28 Jul 2023 01:01:27 GMT  
		Size: 66.1 MB (66131105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cd8f9966de08a13a3fdf9adac440a9019f879b9bede5c9ae0b5725ff410c26`  
		Last Modified: Fri, 28 Jul 2023 01:01:20 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:324691e5bc117de5bdf517fc988eb4b406c5e513f03f27d5c55a5cee421e75bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.8 MB (90839082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67b5546346cd38a0abdcf26e1113a3b4173a6602e6703d84e337ae356d8ffb2d`
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
# Fri, 28 Jul 2023 01:59:30 GMT
ENV EMQX_VERSION=5.1.2
# Fri, 28 Jul 2023 01:59:30 GMT
ENV AMD64_SHA256=bd34a8cfcd816305b4fc8bfb67fb8a0a29dcf7bd2e391e79534bf7d94d62ffcd
# Fri, 28 Jul 2023 01:59:30 GMT
ENV ARM64_SHA256=02d281020403f55f9d5eac5a2ffbdaebc888aa8e4b92fce847f23541f2b0eae5
# Fri, 28 Jul 2023 01:59:30 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 28 Jul 2023 01:59:36 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Fri, 28 Jul 2023 01:59:37 GMT
WORKDIR /opt/emqx
# Fri, 28 Jul 2023 01:59:37 GMT
USER emqx
# Fri, 28 Jul 2023 01:59:37 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 28 Jul 2023 01:59:37 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 28 Jul 2023 01:59:37 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 28 Jul 2023 01:59:37 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:59:37 GMT
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
	-	`sha256:48cf3bb4a948e6cd9c7d7b52bfa8de530a27fc7848c8f419ae1122ced59359e2`  
		Last Modified: Fri, 28 Jul 2023 02:00:25 GMT  
		Size: 57.8 MB (57768254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8a5ca4e496448073b25fd4a99ac622d77eb43ddcaa206f53d89d8a15b31033`  
		Last Modified: Fri, 28 Jul 2023 02:00:19 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
