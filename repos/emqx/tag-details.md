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
$ docker pull emqx@sha256:cbf46ed51100ee15b0c6b1de766e8984b4498b5188c18b5e512bc629ba826786
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:8929d62efa266a08e7c665db0c81aa803e05980e4433ef506f061b3c3c7a8631
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.4 MB (81430755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:037a3374dcd2c4f3d5a435a0631966fc78aea064862754af6baeeaa60bdb92d5`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:20:58 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:20:58 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 06 Jul 2023 21:53:08 GMT
ENV EMQX_VERSION=4.4.19
# Thu, 06 Jul 2023 21:53:08 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 06 Jul 2023 21:53:13 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="bf4192c64c9006733b30f96fe99506a0a3af115c7073995a044cc0e60230675e"; fi;     if [ ${arch} = "arm64" ]; then sha256="7cd27d5112380fd4d81029b10ba862a050b0bba8af1eb90aac669189fc3053c0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$(sha256sum $pkg)";     echo "$sha256 *$pkg" | sha256sum -c;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 06 Jul 2023 21:53:13 GMT
WORKDIR /opt/emqx
# Thu, 06 Jul 2023 21:53:13 GMT
USER emqx
# Thu, 06 Jul 2023 21:53:13 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 06 Jul 2023 21:53:13 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 06 Jul 2023 21:53:13 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 06 Jul 2023 21:53:13 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 06 Jul 2023 21:53:13 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ef462373a136b96c0a554f87fe5b08b7c8461aba1e112745b996eaa7b98a7d`  
		Last Modified: Tue, 04 Jul 2023 04:21:43 GMT  
		Size: 2.6 MB (2569640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ad23a7d23aef4b144a14d30ac52f4568fb6adbc5c43bebc8041add65f9d8bd`  
		Last Modified: Tue, 04 Jul 2023 04:21:42 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c36bb7323c2eb0e14462dbce129fc49067f4eac2171e2b7b4f165958d09e05`  
		Last Modified: Thu, 06 Jul 2023 21:53:45 GMT  
		Size: 47.4 MB (47438517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0011782548631d09e3b4f48191bbf40f019da085cf7b9857ab6d23f361bff316`  
		Last Modified: Thu, 06 Jul 2023 21:53:40 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:a9248efad561f6b833ebacbedf28b5e25430d7246a906d41861cafd1e1ec68ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.8 MB (72845253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e80069bbe8b69c53f5008a9f33affb0176c3d902fa45759b92bb8c8a23036632`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:03:08 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:03:08 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 06 Jul 2023 21:39:26 GMT
ENV EMQX_VERSION=4.4.19
# Thu, 06 Jul 2023 21:39:26 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 06 Jul 2023 21:39:29 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="bf4192c64c9006733b30f96fe99506a0a3af115c7073995a044cc0e60230675e"; fi;     if [ ${arch} = "arm64" ]; then sha256="7cd27d5112380fd4d81029b10ba862a050b0bba8af1eb90aac669189fc3053c0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$(sha256sum $pkg)";     echo "$sha256 *$pkg" | sha256sum -c;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 06 Jul 2023 21:39:30 GMT
WORKDIR /opt/emqx
# Thu, 06 Jul 2023 21:39:30 GMT
USER emqx
# Thu, 06 Jul 2023 21:39:31 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 06 Jul 2023 21:39:31 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 06 Jul 2023 21:39:31 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 06 Jul 2023 21:39:31 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 06 Jul 2023 21:39:31 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a1428b80937a0eb55c8466779cec4bcf7e31bdcc4fc66b763448cf9d131563`  
		Last Modified: Tue, 04 Jul 2023 03:03:50 GMT  
		Size: 2.6 MB (2559426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa00861c721843ae490a68a90f1db04218b5131cb6b2d6d39618973618f3da3`  
		Last Modified: Tue, 04 Jul 2023 03:03:49 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92be73299f3fbd6f630b7fd29adb355fe1bd1b77557870a88683610b34c7a8ff`  
		Last Modified: Thu, 06 Jul 2023 21:39:55 GMT  
		Size: 40.2 MB (40217654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c555c2079b356e8e46973c42652cd100382b54e914992c25f297321ad15d659`  
		Last Modified: Thu, 06 Jul 2023 21:39:52 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:cbf46ed51100ee15b0c6b1de766e8984b4498b5188c18b5e512bc629ba826786
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:8929d62efa266a08e7c665db0c81aa803e05980e4433ef506f061b3c3c7a8631
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.4 MB (81430755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:037a3374dcd2c4f3d5a435a0631966fc78aea064862754af6baeeaa60bdb92d5`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:20:58 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:20:58 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 06 Jul 2023 21:53:08 GMT
ENV EMQX_VERSION=4.4.19
# Thu, 06 Jul 2023 21:53:08 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 06 Jul 2023 21:53:13 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="bf4192c64c9006733b30f96fe99506a0a3af115c7073995a044cc0e60230675e"; fi;     if [ ${arch} = "arm64" ]; then sha256="7cd27d5112380fd4d81029b10ba862a050b0bba8af1eb90aac669189fc3053c0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$(sha256sum $pkg)";     echo "$sha256 *$pkg" | sha256sum -c;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 06 Jul 2023 21:53:13 GMT
WORKDIR /opt/emqx
# Thu, 06 Jul 2023 21:53:13 GMT
USER emqx
# Thu, 06 Jul 2023 21:53:13 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 06 Jul 2023 21:53:13 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 06 Jul 2023 21:53:13 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 06 Jul 2023 21:53:13 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 06 Jul 2023 21:53:13 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ef462373a136b96c0a554f87fe5b08b7c8461aba1e112745b996eaa7b98a7d`  
		Last Modified: Tue, 04 Jul 2023 04:21:43 GMT  
		Size: 2.6 MB (2569640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ad23a7d23aef4b144a14d30ac52f4568fb6adbc5c43bebc8041add65f9d8bd`  
		Last Modified: Tue, 04 Jul 2023 04:21:42 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c36bb7323c2eb0e14462dbce129fc49067f4eac2171e2b7b4f165958d09e05`  
		Last Modified: Thu, 06 Jul 2023 21:53:45 GMT  
		Size: 47.4 MB (47438517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0011782548631d09e3b4f48191bbf40f019da085cf7b9857ab6d23f361bff316`  
		Last Modified: Thu, 06 Jul 2023 21:53:40 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:a9248efad561f6b833ebacbedf28b5e25430d7246a906d41861cafd1e1ec68ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.8 MB (72845253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e80069bbe8b69c53f5008a9f33affb0176c3d902fa45759b92bb8c8a23036632`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:03:08 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:03:08 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 06 Jul 2023 21:39:26 GMT
ENV EMQX_VERSION=4.4.19
# Thu, 06 Jul 2023 21:39:26 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 06 Jul 2023 21:39:29 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="bf4192c64c9006733b30f96fe99506a0a3af115c7073995a044cc0e60230675e"; fi;     if [ ${arch} = "arm64" ]; then sha256="7cd27d5112380fd4d81029b10ba862a050b0bba8af1eb90aac669189fc3053c0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$(sha256sum $pkg)";     echo "$sha256 *$pkg" | sha256sum -c;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 06 Jul 2023 21:39:30 GMT
WORKDIR /opt/emqx
# Thu, 06 Jul 2023 21:39:30 GMT
USER emqx
# Thu, 06 Jul 2023 21:39:31 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 06 Jul 2023 21:39:31 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 06 Jul 2023 21:39:31 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 06 Jul 2023 21:39:31 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 06 Jul 2023 21:39:31 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a1428b80937a0eb55c8466779cec4bcf7e31bdcc4fc66b763448cf9d131563`  
		Last Modified: Tue, 04 Jul 2023 03:03:50 GMT  
		Size: 2.6 MB (2559426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa00861c721843ae490a68a90f1db04218b5131cb6b2d6d39618973618f3da3`  
		Last Modified: Tue, 04 Jul 2023 03:03:49 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92be73299f3fbd6f630b7fd29adb355fe1bd1b77557870a88683610b34c7a8ff`  
		Last Modified: Thu, 06 Jul 2023 21:39:55 GMT  
		Size: 40.2 MB (40217654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c555c2079b356e8e46973c42652cd100382b54e914992c25f297321ad15d659`  
		Last Modified: Thu, 06 Jul 2023 21:39:52 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.19`

```console
$ docker pull emqx@sha256:cbf46ed51100ee15b0c6b1de766e8984b4498b5188c18b5e512bc629ba826786
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4.19` - linux; amd64

```console
$ docker pull emqx@sha256:8929d62efa266a08e7c665db0c81aa803e05980e4433ef506f061b3c3c7a8631
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.4 MB (81430755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:037a3374dcd2c4f3d5a435a0631966fc78aea064862754af6baeeaa60bdb92d5`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:20:58 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:20:58 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 06 Jul 2023 21:53:08 GMT
ENV EMQX_VERSION=4.4.19
# Thu, 06 Jul 2023 21:53:08 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 06 Jul 2023 21:53:13 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="bf4192c64c9006733b30f96fe99506a0a3af115c7073995a044cc0e60230675e"; fi;     if [ ${arch} = "arm64" ]; then sha256="7cd27d5112380fd4d81029b10ba862a050b0bba8af1eb90aac669189fc3053c0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$(sha256sum $pkg)";     echo "$sha256 *$pkg" | sha256sum -c;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 06 Jul 2023 21:53:13 GMT
WORKDIR /opt/emqx
# Thu, 06 Jul 2023 21:53:13 GMT
USER emqx
# Thu, 06 Jul 2023 21:53:13 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 06 Jul 2023 21:53:13 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 06 Jul 2023 21:53:13 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 06 Jul 2023 21:53:13 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 06 Jul 2023 21:53:13 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ef462373a136b96c0a554f87fe5b08b7c8461aba1e112745b996eaa7b98a7d`  
		Last Modified: Tue, 04 Jul 2023 04:21:43 GMT  
		Size: 2.6 MB (2569640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ad23a7d23aef4b144a14d30ac52f4568fb6adbc5c43bebc8041add65f9d8bd`  
		Last Modified: Tue, 04 Jul 2023 04:21:42 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c36bb7323c2eb0e14462dbce129fc49067f4eac2171e2b7b4f165958d09e05`  
		Last Modified: Thu, 06 Jul 2023 21:53:45 GMT  
		Size: 47.4 MB (47438517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0011782548631d09e3b4f48191bbf40f019da085cf7b9857ab6d23f361bff316`  
		Last Modified: Thu, 06 Jul 2023 21:53:40 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4.19` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:a9248efad561f6b833ebacbedf28b5e25430d7246a906d41861cafd1e1ec68ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.8 MB (72845253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e80069bbe8b69c53f5008a9f33affb0176c3d902fa45759b92bb8c8a23036632`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:03:08 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:03:08 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 06 Jul 2023 21:39:26 GMT
ENV EMQX_VERSION=4.4.19
# Thu, 06 Jul 2023 21:39:26 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 06 Jul 2023 21:39:29 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="bf4192c64c9006733b30f96fe99506a0a3af115c7073995a044cc0e60230675e"; fi;     if [ ${arch} = "arm64" ]; then sha256="7cd27d5112380fd4d81029b10ba862a050b0bba8af1eb90aac669189fc3053c0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$(sha256sum $pkg)";     echo "$sha256 *$pkg" | sha256sum -c;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 06 Jul 2023 21:39:30 GMT
WORKDIR /opt/emqx
# Thu, 06 Jul 2023 21:39:30 GMT
USER emqx
# Thu, 06 Jul 2023 21:39:31 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 06 Jul 2023 21:39:31 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 06 Jul 2023 21:39:31 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 06 Jul 2023 21:39:31 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 06 Jul 2023 21:39:31 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a1428b80937a0eb55c8466779cec4bcf7e31bdcc4fc66b763448cf9d131563`  
		Last Modified: Tue, 04 Jul 2023 03:03:50 GMT  
		Size: 2.6 MB (2559426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa00861c721843ae490a68a90f1db04218b5131cb6b2d6d39618973618f3da3`  
		Last Modified: Tue, 04 Jul 2023 03:03:49 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92be73299f3fbd6f630b7fd29adb355fe1bd1b77557870a88683610b34c7a8ff`  
		Last Modified: Thu, 06 Jul 2023 21:39:55 GMT  
		Size: 40.2 MB (40217654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c555c2079b356e8e46973c42652cd100382b54e914992c25f297321ad15d659`  
		Last Modified: Thu, 06 Jul 2023 21:39:52 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5`

```console
$ docker pull emqx@sha256:65b6dfff8cc152d298758dc9c62466629bb5bb970e7a9961d9286b82514be5d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:6b8ea57b47e38c57fa6597f26e35fb7493ef9165e471b2dcbc144ea7439e2916
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.5 MB (100541327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb2b8d67a44854e750ace49e347dcb28f571a32639702aec3936b610f59b33f0`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:21:14 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Mon, 24 Jul 2023 22:33:42 GMT
ENV EMQX_VERSION=5.1.2
# Mon, 24 Jul 2023 22:33:42 GMT
ENV AMD64_SHA256=bd34a8cfcd816305b4fc8bfb67fb8a0a29dcf7bd2e391e79534bf7d94d62ffcd
# Mon, 24 Jul 2023 22:33:42 GMT
ENV ARM64_SHA256=02d281020403f55f9d5eac5a2ffbdaebc888aa8e4b92fce847f23541f2b0eae5
# Mon, 24 Jul 2023 22:33:42 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Mon, 24 Jul 2023 22:33:49 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Mon, 24 Jul 2023 22:33:50 GMT
WORKDIR /opt/emqx
# Mon, 24 Jul 2023 22:33:50 GMT
USER emqx
# Mon, 24 Jul 2023 22:33:50 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Mon, 24 Jul 2023 22:33:50 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Mon, 24 Jul 2023 22:33:50 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Mon, 24 Jul 2023 22:33:50 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Mon, 24 Jul 2023 22:33:50 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a63034914a435ac7d89264c48bbfd001cc80603c14d21f4eb9895099fa4e31a`  
		Last Modified: Tue, 04 Jul 2023 04:21:58 GMT  
		Size: 3.0 MB (2987794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc27d1c79ae1ac7fb241e52deb948fc9ef459a4cc65b366dcc7911393421f4d4`  
		Last Modified: Tue, 04 Jul 2023 04:21:57 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c89d881523eb76f242112fb48acca139fddf664fbcb6dd43bbc36e387dad1a`  
		Last Modified: Mon, 24 Jul 2023 22:34:12 GMT  
		Size: 66.1 MB (66131139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df43d2229a62ed0b8e76ec604b518e1a137ac31ca1fc82339ce2ede160f6bcee`  
		Last Modified: Mon, 24 Jul 2023 22:34:05 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:b79f2f728a453fa3ca78f59039c28fc4c90b254b15b94168cf6ccc9e0b289814
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.8 MB (90839289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b25387bf3eaec5fbcdda3aa151b52358ebbe68464fc98222b11dd19097cb5e0`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:03:21 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:03:22 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Mon, 24 Jul 2023 22:46:08 GMT
ENV EMQX_VERSION=5.1.2
# Mon, 24 Jul 2023 22:46:08 GMT
ENV AMD64_SHA256=bd34a8cfcd816305b4fc8bfb67fb8a0a29dcf7bd2e391e79534bf7d94d62ffcd
# Mon, 24 Jul 2023 22:46:08 GMT
ENV ARM64_SHA256=02d281020403f55f9d5eac5a2ffbdaebc888aa8e4b92fce847f23541f2b0eae5
# Mon, 24 Jul 2023 22:46:08 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Mon, 24 Jul 2023 22:46:15 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Mon, 24 Jul 2023 22:46:15 GMT
WORKDIR /opt/emqx
# Mon, 24 Jul 2023 22:46:15 GMT
USER emqx
# Mon, 24 Jul 2023 22:46:15 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Mon, 24 Jul 2023 22:46:15 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Mon, 24 Jul 2023 22:46:16 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Mon, 24 Jul 2023 22:46:16 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Mon, 24 Jul 2023 22:46:16 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc212c7c7d61e498e2041ef1be251acbca34483d513266fc40c2b0d41721f61`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 3.0 MB (3003072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94aca2cf657bb3bfb3bf3c6675087076999f1bd3e64ffbe99a129c8475d7795`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3359f1269332e2bb900bcac8dfcdd7e02d8ad7aaa28811e10b1b939f673a9a6`  
		Last Modified: Mon, 24 Jul 2023 22:46:34 GMT  
		Size: 57.8 MB (57768247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd7972d2bafd3d78b2df6f58a44aa6d8846b547fa161ac6c05099df4da81c25`  
		Last Modified: Mon, 24 Jul 2023 22:46:29 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:ed48aca55fd8df1845e9f6b8bab7a234667f82ee54ae3c883e7a390be9fec1b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:af206b512e1993e2ec001139a2f953cd371d9384fdc405b8119a6ebbac8540cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101982049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef0cfed032bdaa77c77d68bbd4278426f4ed54fedc2ac0f37bc22f2e87ca2219`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:21:14 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 04 Jul 2023 04:21:14 GMT
ENV EMQX_VERSION=5.0.26
# Tue, 04 Jul 2023 04:21:14 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Tue, 04 Jul 2023 04:21:14 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Tue, 04 Jul 2023 04:21:14 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 04 Jul 2023 04:21:20 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 04 Jul 2023 04:21:21 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 04:21:21 GMT
USER emqx
# Tue, 04 Jul 2023 04:21:21 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 04:21:21 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 04 Jul 2023 04:21:21 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 04 Jul 2023 04:21:21 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 04:21:21 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a63034914a435ac7d89264c48bbfd001cc80603c14d21f4eb9895099fa4e31a`  
		Last Modified: Tue, 04 Jul 2023 04:21:58 GMT  
		Size: 3.0 MB (2987794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc27d1c79ae1ac7fb241e52deb948fc9ef459a4cc65b366dcc7911393421f4d4`  
		Last Modified: Tue, 04 Jul 2023 04:21:57 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62baa3e39a567ab3fb2ef18688452d5a8e863961248234dc567d41b0d6bd798a`  
		Last Modified: Tue, 04 Jul 2023 04:22:05 GMT  
		Size: 67.6 MB (67571860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8c5ab9c1f57c1002a6b3251c5f524eb0c22290720ea5fe523cc649471a1084`  
		Last Modified: Tue, 04 Jul 2023 04:21:57 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:0abdd21e8a6b3206455cb733eca21c22695b7dc06a98d3a4de5eb999537b0195
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93060437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db90f1f3fab83ce999d6472a64971ca463afb82097d6b4cdb5da98a3c2f28c0d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:03:21 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:03:22 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 04 Jul 2023 03:03:22 GMT
ENV EMQX_VERSION=5.0.26
# Tue, 04 Jul 2023 03:03:22 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Tue, 04 Jul 2023 03:03:22 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Tue, 04 Jul 2023 03:03:22 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 04 Jul 2023 03:03:28 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 04 Jul 2023 03:03:28 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 03:03:28 GMT
USER emqx
# Tue, 04 Jul 2023 03:03:28 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 03:03:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 04 Jul 2023 03:03:29 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 04 Jul 2023 03:03:29 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:03:29 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc212c7c7d61e498e2041ef1be251acbca34483d513266fc40c2b0d41721f61`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 3.0 MB (3003072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94aca2cf657bb3bfb3bf3c6675087076999f1bd3e64ffbe99a129c8475d7795`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf20fcfbb7660480c1e5425d2d670e3fc48e00264da9d9a5b0eb282e2472df6`  
		Last Modified: Tue, 04 Jul 2023 03:04:08 GMT  
		Size: 60.0 MB (59989394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03deeecf9242891f89e9ebbde2e0197c04be91ee39569bfcd63a6a3336b20801`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.26`

```console
$ docker pull emqx@sha256:ed48aca55fd8df1845e9f6b8bab7a234667f82ee54ae3c883e7a390be9fec1b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0.26` - linux; amd64

```console
$ docker pull emqx@sha256:af206b512e1993e2ec001139a2f953cd371d9384fdc405b8119a6ebbac8540cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101982049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef0cfed032bdaa77c77d68bbd4278426f4ed54fedc2ac0f37bc22f2e87ca2219`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:21:14 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 04 Jul 2023 04:21:14 GMT
ENV EMQX_VERSION=5.0.26
# Tue, 04 Jul 2023 04:21:14 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Tue, 04 Jul 2023 04:21:14 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Tue, 04 Jul 2023 04:21:14 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 04 Jul 2023 04:21:20 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 04 Jul 2023 04:21:21 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 04:21:21 GMT
USER emqx
# Tue, 04 Jul 2023 04:21:21 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 04:21:21 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 04 Jul 2023 04:21:21 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 04 Jul 2023 04:21:21 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 04:21:21 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a63034914a435ac7d89264c48bbfd001cc80603c14d21f4eb9895099fa4e31a`  
		Last Modified: Tue, 04 Jul 2023 04:21:58 GMT  
		Size: 3.0 MB (2987794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc27d1c79ae1ac7fb241e52deb948fc9ef459a4cc65b366dcc7911393421f4d4`  
		Last Modified: Tue, 04 Jul 2023 04:21:57 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62baa3e39a567ab3fb2ef18688452d5a8e863961248234dc567d41b0d6bd798a`  
		Last Modified: Tue, 04 Jul 2023 04:22:05 GMT  
		Size: 67.6 MB (67571860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8c5ab9c1f57c1002a6b3251c5f524eb0c22290720ea5fe523cc649471a1084`  
		Last Modified: Tue, 04 Jul 2023 04:21:57 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0.26` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:0abdd21e8a6b3206455cb733eca21c22695b7dc06a98d3a4de5eb999537b0195
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93060437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db90f1f3fab83ce999d6472a64971ca463afb82097d6b4cdb5da98a3c2f28c0d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:03:21 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:03:22 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 04 Jul 2023 03:03:22 GMT
ENV EMQX_VERSION=5.0.26
# Tue, 04 Jul 2023 03:03:22 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Tue, 04 Jul 2023 03:03:22 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Tue, 04 Jul 2023 03:03:22 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 04 Jul 2023 03:03:28 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 04 Jul 2023 03:03:28 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 03:03:28 GMT
USER emqx
# Tue, 04 Jul 2023 03:03:28 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 03:03:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 04 Jul 2023 03:03:29 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 04 Jul 2023 03:03:29 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:03:29 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc212c7c7d61e498e2041ef1be251acbca34483d513266fc40c2b0d41721f61`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 3.0 MB (3003072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94aca2cf657bb3bfb3bf3c6675087076999f1bd3e64ffbe99a129c8475d7795`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf20fcfbb7660480c1e5425d2d670e3fc48e00264da9d9a5b0eb282e2472df6`  
		Last Modified: Tue, 04 Jul 2023 03:04:08 GMT  
		Size: 60.0 MB (59989394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03deeecf9242891f89e9ebbde2e0197c04be91ee39569bfcd63a6a3336b20801`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.1`

```console
$ docker pull emqx@sha256:65b6dfff8cc152d298758dc9c62466629bb5bb970e7a9961d9286b82514be5d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.1` - linux; amd64

```console
$ docker pull emqx@sha256:6b8ea57b47e38c57fa6597f26e35fb7493ef9165e471b2dcbc144ea7439e2916
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.5 MB (100541327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb2b8d67a44854e750ace49e347dcb28f571a32639702aec3936b610f59b33f0`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:21:14 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Mon, 24 Jul 2023 22:33:42 GMT
ENV EMQX_VERSION=5.1.2
# Mon, 24 Jul 2023 22:33:42 GMT
ENV AMD64_SHA256=bd34a8cfcd816305b4fc8bfb67fb8a0a29dcf7bd2e391e79534bf7d94d62ffcd
# Mon, 24 Jul 2023 22:33:42 GMT
ENV ARM64_SHA256=02d281020403f55f9d5eac5a2ffbdaebc888aa8e4b92fce847f23541f2b0eae5
# Mon, 24 Jul 2023 22:33:42 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Mon, 24 Jul 2023 22:33:49 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Mon, 24 Jul 2023 22:33:50 GMT
WORKDIR /opt/emqx
# Mon, 24 Jul 2023 22:33:50 GMT
USER emqx
# Mon, 24 Jul 2023 22:33:50 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Mon, 24 Jul 2023 22:33:50 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Mon, 24 Jul 2023 22:33:50 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Mon, 24 Jul 2023 22:33:50 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Mon, 24 Jul 2023 22:33:50 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a63034914a435ac7d89264c48bbfd001cc80603c14d21f4eb9895099fa4e31a`  
		Last Modified: Tue, 04 Jul 2023 04:21:58 GMT  
		Size: 3.0 MB (2987794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc27d1c79ae1ac7fb241e52deb948fc9ef459a4cc65b366dcc7911393421f4d4`  
		Last Modified: Tue, 04 Jul 2023 04:21:57 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c89d881523eb76f242112fb48acca139fddf664fbcb6dd43bbc36e387dad1a`  
		Last Modified: Mon, 24 Jul 2023 22:34:12 GMT  
		Size: 66.1 MB (66131139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df43d2229a62ed0b8e76ec604b518e1a137ac31ca1fc82339ce2ede160f6bcee`  
		Last Modified: Mon, 24 Jul 2023 22:34:05 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.1` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:b79f2f728a453fa3ca78f59039c28fc4c90b254b15b94168cf6ccc9e0b289814
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.8 MB (90839289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b25387bf3eaec5fbcdda3aa151b52358ebbe68464fc98222b11dd19097cb5e0`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:03:21 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:03:22 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Mon, 24 Jul 2023 22:46:08 GMT
ENV EMQX_VERSION=5.1.2
# Mon, 24 Jul 2023 22:46:08 GMT
ENV AMD64_SHA256=bd34a8cfcd816305b4fc8bfb67fb8a0a29dcf7bd2e391e79534bf7d94d62ffcd
# Mon, 24 Jul 2023 22:46:08 GMT
ENV ARM64_SHA256=02d281020403f55f9d5eac5a2ffbdaebc888aa8e4b92fce847f23541f2b0eae5
# Mon, 24 Jul 2023 22:46:08 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Mon, 24 Jul 2023 22:46:15 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Mon, 24 Jul 2023 22:46:15 GMT
WORKDIR /opt/emqx
# Mon, 24 Jul 2023 22:46:15 GMT
USER emqx
# Mon, 24 Jul 2023 22:46:15 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Mon, 24 Jul 2023 22:46:15 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Mon, 24 Jul 2023 22:46:16 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Mon, 24 Jul 2023 22:46:16 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Mon, 24 Jul 2023 22:46:16 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc212c7c7d61e498e2041ef1be251acbca34483d513266fc40c2b0d41721f61`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 3.0 MB (3003072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94aca2cf657bb3bfb3bf3c6675087076999f1bd3e64ffbe99a129c8475d7795`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3359f1269332e2bb900bcac8dfcdd7e02d8ad7aaa28811e10b1b939f673a9a6`  
		Last Modified: Mon, 24 Jul 2023 22:46:34 GMT  
		Size: 57.8 MB (57768247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd7972d2bafd3d78b2df6f58a44aa6d8846b547fa161ac6c05099df4da81c25`  
		Last Modified: Mon, 24 Jul 2023 22:46:29 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.1.2`

```console
$ docker pull emqx@sha256:65b6dfff8cc152d298758dc9c62466629bb5bb970e7a9961d9286b82514be5d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.1.2` - linux; amd64

```console
$ docker pull emqx@sha256:6b8ea57b47e38c57fa6597f26e35fb7493ef9165e471b2dcbc144ea7439e2916
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.5 MB (100541327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb2b8d67a44854e750ace49e347dcb28f571a32639702aec3936b610f59b33f0`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:21:14 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Mon, 24 Jul 2023 22:33:42 GMT
ENV EMQX_VERSION=5.1.2
# Mon, 24 Jul 2023 22:33:42 GMT
ENV AMD64_SHA256=bd34a8cfcd816305b4fc8bfb67fb8a0a29dcf7bd2e391e79534bf7d94d62ffcd
# Mon, 24 Jul 2023 22:33:42 GMT
ENV ARM64_SHA256=02d281020403f55f9d5eac5a2ffbdaebc888aa8e4b92fce847f23541f2b0eae5
# Mon, 24 Jul 2023 22:33:42 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Mon, 24 Jul 2023 22:33:49 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Mon, 24 Jul 2023 22:33:50 GMT
WORKDIR /opt/emqx
# Mon, 24 Jul 2023 22:33:50 GMT
USER emqx
# Mon, 24 Jul 2023 22:33:50 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Mon, 24 Jul 2023 22:33:50 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Mon, 24 Jul 2023 22:33:50 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Mon, 24 Jul 2023 22:33:50 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Mon, 24 Jul 2023 22:33:50 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a63034914a435ac7d89264c48bbfd001cc80603c14d21f4eb9895099fa4e31a`  
		Last Modified: Tue, 04 Jul 2023 04:21:58 GMT  
		Size: 3.0 MB (2987794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc27d1c79ae1ac7fb241e52deb948fc9ef459a4cc65b366dcc7911393421f4d4`  
		Last Modified: Tue, 04 Jul 2023 04:21:57 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c89d881523eb76f242112fb48acca139fddf664fbcb6dd43bbc36e387dad1a`  
		Last Modified: Mon, 24 Jul 2023 22:34:12 GMT  
		Size: 66.1 MB (66131139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df43d2229a62ed0b8e76ec604b518e1a137ac31ca1fc82339ce2ede160f6bcee`  
		Last Modified: Mon, 24 Jul 2023 22:34:05 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.1.2` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:b79f2f728a453fa3ca78f59039c28fc4c90b254b15b94168cf6ccc9e0b289814
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.8 MB (90839289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b25387bf3eaec5fbcdda3aa151b52358ebbe68464fc98222b11dd19097cb5e0`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:03:21 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:03:22 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Mon, 24 Jul 2023 22:46:08 GMT
ENV EMQX_VERSION=5.1.2
# Mon, 24 Jul 2023 22:46:08 GMT
ENV AMD64_SHA256=bd34a8cfcd816305b4fc8bfb67fb8a0a29dcf7bd2e391e79534bf7d94d62ffcd
# Mon, 24 Jul 2023 22:46:08 GMT
ENV ARM64_SHA256=02d281020403f55f9d5eac5a2ffbdaebc888aa8e4b92fce847f23541f2b0eae5
# Mon, 24 Jul 2023 22:46:08 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Mon, 24 Jul 2023 22:46:15 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Mon, 24 Jul 2023 22:46:15 GMT
WORKDIR /opt/emqx
# Mon, 24 Jul 2023 22:46:15 GMT
USER emqx
# Mon, 24 Jul 2023 22:46:15 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Mon, 24 Jul 2023 22:46:15 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Mon, 24 Jul 2023 22:46:16 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Mon, 24 Jul 2023 22:46:16 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Mon, 24 Jul 2023 22:46:16 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc212c7c7d61e498e2041ef1be251acbca34483d513266fc40c2b0d41721f61`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 3.0 MB (3003072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94aca2cf657bb3bfb3bf3c6675087076999f1bd3e64ffbe99a129c8475d7795`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3359f1269332e2bb900bcac8dfcdd7e02d8ad7aaa28811e10b1b939f673a9a6`  
		Last Modified: Mon, 24 Jul 2023 22:46:34 GMT  
		Size: 57.8 MB (57768247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd7972d2bafd3d78b2df6f58a44aa6d8846b547fa161ac6c05099df4da81c25`  
		Last Modified: Mon, 24 Jul 2023 22:46:29 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:65b6dfff8cc152d298758dc9c62466629bb5bb970e7a9961d9286b82514be5d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:6b8ea57b47e38c57fa6597f26e35fb7493ef9165e471b2dcbc144ea7439e2916
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.5 MB (100541327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb2b8d67a44854e750ace49e347dcb28f571a32639702aec3936b610f59b33f0`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:21:14 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Mon, 24 Jul 2023 22:33:42 GMT
ENV EMQX_VERSION=5.1.2
# Mon, 24 Jul 2023 22:33:42 GMT
ENV AMD64_SHA256=bd34a8cfcd816305b4fc8bfb67fb8a0a29dcf7bd2e391e79534bf7d94d62ffcd
# Mon, 24 Jul 2023 22:33:42 GMT
ENV ARM64_SHA256=02d281020403f55f9d5eac5a2ffbdaebc888aa8e4b92fce847f23541f2b0eae5
# Mon, 24 Jul 2023 22:33:42 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Mon, 24 Jul 2023 22:33:49 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Mon, 24 Jul 2023 22:33:50 GMT
WORKDIR /opt/emqx
# Mon, 24 Jul 2023 22:33:50 GMT
USER emqx
# Mon, 24 Jul 2023 22:33:50 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Mon, 24 Jul 2023 22:33:50 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Mon, 24 Jul 2023 22:33:50 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Mon, 24 Jul 2023 22:33:50 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Mon, 24 Jul 2023 22:33:50 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a63034914a435ac7d89264c48bbfd001cc80603c14d21f4eb9895099fa4e31a`  
		Last Modified: Tue, 04 Jul 2023 04:21:58 GMT  
		Size: 3.0 MB (2987794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc27d1c79ae1ac7fb241e52deb948fc9ef459a4cc65b366dcc7911393421f4d4`  
		Last Modified: Tue, 04 Jul 2023 04:21:57 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c89d881523eb76f242112fb48acca139fddf664fbcb6dd43bbc36e387dad1a`  
		Last Modified: Mon, 24 Jul 2023 22:34:12 GMT  
		Size: 66.1 MB (66131139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df43d2229a62ed0b8e76ec604b518e1a137ac31ca1fc82339ce2ede160f6bcee`  
		Last Modified: Mon, 24 Jul 2023 22:34:05 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:b79f2f728a453fa3ca78f59039c28fc4c90b254b15b94168cf6ccc9e0b289814
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.8 MB (90839289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b25387bf3eaec5fbcdda3aa151b52358ebbe68464fc98222b11dd19097cb5e0`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:03:21 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:03:22 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Mon, 24 Jul 2023 22:46:08 GMT
ENV EMQX_VERSION=5.1.2
# Mon, 24 Jul 2023 22:46:08 GMT
ENV AMD64_SHA256=bd34a8cfcd816305b4fc8bfb67fb8a0a29dcf7bd2e391e79534bf7d94d62ffcd
# Mon, 24 Jul 2023 22:46:08 GMT
ENV ARM64_SHA256=02d281020403f55f9d5eac5a2ffbdaebc888aa8e4b92fce847f23541f2b0eae5
# Mon, 24 Jul 2023 22:46:08 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Mon, 24 Jul 2023 22:46:15 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Mon, 24 Jul 2023 22:46:15 GMT
WORKDIR /opt/emqx
# Mon, 24 Jul 2023 22:46:15 GMT
USER emqx
# Mon, 24 Jul 2023 22:46:15 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Mon, 24 Jul 2023 22:46:15 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Mon, 24 Jul 2023 22:46:16 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Mon, 24 Jul 2023 22:46:16 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Mon, 24 Jul 2023 22:46:16 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc212c7c7d61e498e2041ef1be251acbca34483d513266fc40c2b0d41721f61`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 3.0 MB (3003072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94aca2cf657bb3bfb3bf3c6675087076999f1bd3e64ffbe99a129c8475d7795`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3359f1269332e2bb900bcac8dfcdd7e02d8ad7aaa28811e10b1b939f673a9a6`  
		Last Modified: Mon, 24 Jul 2023 22:46:34 GMT  
		Size: 57.8 MB (57768247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd7972d2bafd3d78b2df6f58a44aa6d8846b547fa161ac6c05099df4da81c25`  
		Last Modified: Mon, 24 Jul 2023 22:46:29 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
