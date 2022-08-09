<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `chronograf`

-	[`chronograf:1.6`](#chronograf16)
-	[`chronograf:1.6-alpine`](#chronograf16-alpine)
-	[`chronograf:1.6.2`](#chronograf162)
-	[`chronograf:1.6.2-alpine`](#chronograf162-alpine)
-	[`chronograf:1.7`](#chronograf17)
-	[`chronograf:1.7-alpine`](#chronograf17-alpine)
-	[`chronograf:1.7.17`](#chronograf1717)
-	[`chronograf:1.7.17-alpine`](#chronograf1717-alpine)
-	[`chronograf:1.8`](#chronograf18)
-	[`chronograf:1.8-alpine`](#chronograf18-alpine)
-	[`chronograf:1.8.10`](#chronograf1810)
-	[`chronograf:1.8.10-alpine`](#chronograf1810-alpine)
-	[`chronograf:1.9`](#chronograf19)
-	[`chronograf:1.9-alpine`](#chronograf19-alpine)
-	[`chronograf:1.9.4`](#chronograf194)
-	[`chronograf:1.9.4-alpine`](#chronograf194-alpine)
-	[`chronograf:alpine`](#chronografalpine)
-	[`chronograf:latest`](#chronograflatest)

## `chronograf:1.6`

```console
$ docker pull chronograf@sha256:967a9e71143492aaddcd9d6acc37363abd513761a4ef09ec5573ad5c8f950944
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6` - linux; amd64

```console
$ docker pull chronograf@sha256:70b667a17282f4759e22ccb3d92f003469ca1bf9b43e41cf8c6b88dc1ef43880
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49397889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fd6c0f131d65571e79b70365992fc8bc78244fd1534cffeb16aa85db58fcddb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:20 GMT
ADD file:cfad5912b6dd7590713979e5a5e231b1b6873200fde725cb7baf75110d7fa138 in / 
# Thu, 23 Jun 2022 00:22:20 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:03:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 01:03:40 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Thu, 23 Jun 2022 01:03:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 01:03:48 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 01:03:48 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 01:03:48 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 01:03:49 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 01:03:49 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 01:03:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 01:03:49 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bff3e048017eab8adaed886bad4b3c5c81f7d952b65b056dca8d6dbc198222dd`  
		Last Modified: Thu, 23 Jun 2022 00:30:01 GMT  
		Size: 22.6 MB (22567461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b5498e1d3acd0f9ff62393ea37f571882a0eec6680617ecb40142cd977a4d4`  
		Last Modified: Thu, 23 Jun 2022 01:05:10 GMT  
		Size: 6.8 MB (6760409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e53ac4f7c306dbbff3ed6070a3e4bb1064345503f79625f8ba1fe206dd2cd3`  
		Last Modified: Thu, 23 Jun 2022 01:05:12 GMT  
		Size: 20.0 MB (20045624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d48cfd8d3ee5e2efa84bf652c47c516de588fb29f36a835a7b082dbcb905f7`  
		Last Modified: Thu, 23 Jun 2022 01:05:09 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f3849f106bcba131de9e8cd92bccedf13183beeb78ffa565ce73ffca7197fd`  
		Last Modified: Thu, 23 Jun 2022 01:05:09 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412be8bc5cfad025ac058cc8ab54533a4d0b6c7057c7453000a98fd19a4c3380`  
		Last Modified: Thu, 23 Jun 2022 01:05:10 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:eaea119494f4817d97489359ff72b559c5d8000fcf3a200a37fa488124685d49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43986225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11d685c8050f3162df21624c33af34810dd59950e192bb2baf5f551900602f30`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 01:05:38 GMT
ADD file:fc42adb3b30bf8dda0909ae6f3c3754d78c642e1a1d739bedf21934b7e7da3dd in / 
# Thu, 23 Jun 2022 01:05:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 02:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 02:26:01 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Thu, 23 Jun 2022 02:26:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 02:26:21 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 02:26:21 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 02:26:21 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 02:26:22 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 02:26:22 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 02:26:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 02:26:23 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a259ad5a4933979a4df4eb948f8761dde9b9f3d710259da588afee9fa00f1fef`  
		Last Modified: Thu, 23 Jun 2022 01:22:42 GMT  
		Size: 19.4 MB (19359846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0f7a736acf205407547109d49c141be814413fe2e704f167f154beb4a64bf8`  
		Last Modified: Thu, 23 Jun 2022 02:29:36 GMT  
		Size: 5.8 MB (5781003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7649b91c7a87f39cfdd15ace81a5708e29d5736187ad5688c99eba98516d5070`  
		Last Modified: Thu, 23 Jun 2022 02:29:46 GMT  
		Size: 18.8 MB (18820980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd56b47fbeef69f45c8e6d719bb49c0d4dab06ebbef98e2ba5d5d37162657f2`  
		Last Modified: Thu, 23 Jun 2022 02:29:33 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f7cde79be7f011bb4c5bae2d46e45602b9ac5b9ce48424681281a56ded6330`  
		Last Modified: Thu, 23 Jun 2022 02:29:33 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b06a1994052cfff81d2ec208c570bbcc19843129b0457fde09dbab875c752ef`  
		Last Modified: Thu, 23 Jun 2022 02:29:33 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:f52ed2f2fab6d8f1293176b446884075d4a539f6f3d837d3f134b0b725d026d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45457259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17eca1164e22f0f5463188aeff9909238f9b12fa2e561a988003a9aff00c388b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 00:42:59 GMT
ADD file:c1bdac846ff41ceb56a44de5da778cfb7c3db7ccf4d689b7c1c22c0b80381c49 in / 
# Thu, 23 Jun 2022 00:42:59 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:27:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 01:27:20 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Thu, 23 Jun 2022 01:27:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 01:27:29 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 01:27:30 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 01:27:30 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 01:27:31 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 01:27:33 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 01:27:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 01:27:34 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:45f14b91a40fe8177f16f6b6526ada782d0d63a7958757d4e07c543e574ea7a8`  
		Last Modified: Thu, 23 Jun 2022 00:51:46 GMT  
		Size: 20.4 MB (20423990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba5c15f7bd5dfe32b1718aade52f008519a7ffa497114d413766119a3dbd4f8`  
		Last Modified: Thu, 23 Jun 2022 01:29:14 GMT  
		Size: 6.0 MB (6047312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2fe174fded1e6bbab973e46933621989f01d511bf87a681fdacb11bc0c6550`  
		Last Modified: Thu, 23 Jun 2022 01:29:16 GMT  
		Size: 19.0 MB (18961565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542933e37201dabb5bbe1daefc6274ffcf5b391a1e01ee8ba9b669b2b49acc16`  
		Last Modified: Thu, 23 Jun 2022 01:29:13 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c46645c7e500a2c98d858dae361ab37fb202595a64a3381f9101696d1cff8c`  
		Last Modified: Thu, 23 Jun 2022 01:29:13 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb68906a3c40e5c62b26804b2712777dd64b3276632378430815e626dbd09a5`  
		Last Modified: Thu, 23 Jun 2022 01:29:13 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6-alpine`

```console
$ docker pull chronograf@sha256:0980feb5cd4beab335f5dc2eb79d4e9588b47e7b4fa44803588828ce579445d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.6-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:a12fa36731d388128a24d8c6bae42c7d135a48b6b94d7535e7eb4bd9a66f7ec2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14875047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a8f13512cb9539b5f180281961b0271bad20862a4e4ea7f56bbc58964423f8d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:17:07 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:17:08 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 09 Aug 2022 18:17:08 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 09 Aug 2022 18:17:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 09 Aug 2022 18:17:12 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Tue, 09 Aug 2022 18:17:12 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Aug 2022 18:17:12 GMT
EXPOSE 8888
# Tue, 09 Aug 2022 18:17:12 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Aug 2022 18:17:12 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Tue, 09 Aug 2022 18:17:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Aug 2022 18:17:13 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b667f667e0d162df357cbdea46ee3457fd45395b451ccad50381f4665f8149`  
		Last Modified: Tue, 09 Aug 2022 18:18:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86aedf0b86f2f672427bd99edb4d53285ee3f072fdd5e4ea92fd315f1f9d2bb8`  
		Last Modified: Tue, 09 Aug 2022 18:18:07 GMT  
		Size: 284.6 KB (284571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f1df9899b6ebf1d7df5d628d46580ccbb0e5f130f92a62fa0e6f5e940fe4fc`  
		Last Modified: Tue, 09 Aug 2022 18:18:09 GMT  
		Size: 11.7 MB (11738425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8791b6fe87b776babbb1a953ade5de230b9240678f38258cd21e37a5927ae136`  
		Last Modified: Tue, 09 Aug 2022 18:18:07 GMT  
		Size: 12.3 KB (12273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0086db28ed5d9a6f65ea6988dd5457188e01632dcb02c1d0fd446f660d9d351`  
		Last Modified: Tue, 09 Aug 2022 18:18:07 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c686c318fdda143bca0bfaa2fca999e7547916b852d9fbaa7b4dc38409b40b`  
		Last Modified: Tue, 09 Aug 2022 18:18:07 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2`

```console
$ docker pull chronograf@sha256:967a9e71143492aaddcd9d6acc37363abd513761a4ef09ec5573ad5c8f950944
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6.2` - linux; amd64

```console
$ docker pull chronograf@sha256:70b667a17282f4759e22ccb3d92f003469ca1bf9b43e41cf8c6b88dc1ef43880
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49397889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fd6c0f131d65571e79b70365992fc8bc78244fd1534cffeb16aa85db58fcddb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:20 GMT
ADD file:cfad5912b6dd7590713979e5a5e231b1b6873200fde725cb7baf75110d7fa138 in / 
# Thu, 23 Jun 2022 00:22:20 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:03:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 01:03:40 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Thu, 23 Jun 2022 01:03:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 01:03:48 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 01:03:48 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 01:03:48 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 01:03:49 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 01:03:49 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 01:03:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 01:03:49 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bff3e048017eab8adaed886bad4b3c5c81f7d952b65b056dca8d6dbc198222dd`  
		Last Modified: Thu, 23 Jun 2022 00:30:01 GMT  
		Size: 22.6 MB (22567461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b5498e1d3acd0f9ff62393ea37f571882a0eec6680617ecb40142cd977a4d4`  
		Last Modified: Thu, 23 Jun 2022 01:05:10 GMT  
		Size: 6.8 MB (6760409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e53ac4f7c306dbbff3ed6070a3e4bb1064345503f79625f8ba1fe206dd2cd3`  
		Last Modified: Thu, 23 Jun 2022 01:05:12 GMT  
		Size: 20.0 MB (20045624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d48cfd8d3ee5e2efa84bf652c47c516de588fb29f36a835a7b082dbcb905f7`  
		Last Modified: Thu, 23 Jun 2022 01:05:09 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f3849f106bcba131de9e8cd92bccedf13183beeb78ffa565ce73ffca7197fd`  
		Last Modified: Thu, 23 Jun 2022 01:05:09 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412be8bc5cfad025ac058cc8ab54533a4d0b6c7057c7453000a98fd19a4c3380`  
		Last Modified: Thu, 23 Jun 2022 01:05:10 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:eaea119494f4817d97489359ff72b559c5d8000fcf3a200a37fa488124685d49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43986225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11d685c8050f3162df21624c33af34810dd59950e192bb2baf5f551900602f30`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 01:05:38 GMT
ADD file:fc42adb3b30bf8dda0909ae6f3c3754d78c642e1a1d739bedf21934b7e7da3dd in / 
# Thu, 23 Jun 2022 01:05:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 02:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 02:26:01 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Thu, 23 Jun 2022 02:26:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 02:26:21 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 02:26:21 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 02:26:21 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 02:26:22 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 02:26:22 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 02:26:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 02:26:23 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a259ad5a4933979a4df4eb948f8761dde9b9f3d710259da588afee9fa00f1fef`  
		Last Modified: Thu, 23 Jun 2022 01:22:42 GMT  
		Size: 19.4 MB (19359846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0f7a736acf205407547109d49c141be814413fe2e704f167f154beb4a64bf8`  
		Last Modified: Thu, 23 Jun 2022 02:29:36 GMT  
		Size: 5.8 MB (5781003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7649b91c7a87f39cfdd15ace81a5708e29d5736187ad5688c99eba98516d5070`  
		Last Modified: Thu, 23 Jun 2022 02:29:46 GMT  
		Size: 18.8 MB (18820980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd56b47fbeef69f45c8e6d719bb49c0d4dab06ebbef98e2ba5d5d37162657f2`  
		Last Modified: Thu, 23 Jun 2022 02:29:33 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f7cde79be7f011bb4c5bae2d46e45602b9ac5b9ce48424681281a56ded6330`  
		Last Modified: Thu, 23 Jun 2022 02:29:33 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b06a1994052cfff81d2ec208c570bbcc19843129b0457fde09dbab875c752ef`  
		Last Modified: Thu, 23 Jun 2022 02:29:33 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:f52ed2f2fab6d8f1293176b446884075d4a539f6f3d837d3f134b0b725d026d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45457259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17eca1164e22f0f5463188aeff9909238f9b12fa2e561a988003a9aff00c388b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 00:42:59 GMT
ADD file:c1bdac846ff41ceb56a44de5da778cfb7c3db7ccf4d689b7c1c22c0b80381c49 in / 
# Thu, 23 Jun 2022 00:42:59 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:27:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 01:27:20 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Thu, 23 Jun 2022 01:27:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 01:27:29 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 01:27:30 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 01:27:30 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 01:27:31 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 01:27:33 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 01:27:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 01:27:34 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:45f14b91a40fe8177f16f6b6526ada782d0d63a7958757d4e07c543e574ea7a8`  
		Last Modified: Thu, 23 Jun 2022 00:51:46 GMT  
		Size: 20.4 MB (20423990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba5c15f7bd5dfe32b1718aade52f008519a7ffa497114d413766119a3dbd4f8`  
		Last Modified: Thu, 23 Jun 2022 01:29:14 GMT  
		Size: 6.0 MB (6047312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2fe174fded1e6bbab973e46933621989f01d511bf87a681fdacb11bc0c6550`  
		Last Modified: Thu, 23 Jun 2022 01:29:16 GMT  
		Size: 19.0 MB (18961565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542933e37201dabb5bbe1daefc6274ffcf5b391a1e01ee8ba9b669b2b49acc16`  
		Last Modified: Thu, 23 Jun 2022 01:29:13 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c46645c7e500a2c98d858dae361ab37fb202595a64a3381f9101696d1cff8c`  
		Last Modified: Thu, 23 Jun 2022 01:29:13 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb68906a3c40e5c62b26804b2712777dd64b3276632378430815e626dbd09a5`  
		Last Modified: Thu, 23 Jun 2022 01:29:13 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2-alpine`

```console
$ docker pull chronograf@sha256:0980feb5cd4beab335f5dc2eb79d4e9588b47e7b4fa44803588828ce579445d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.6.2-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:a12fa36731d388128a24d8c6bae42c7d135a48b6b94d7535e7eb4bd9a66f7ec2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14875047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a8f13512cb9539b5f180281961b0271bad20862a4e4ea7f56bbc58964423f8d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:17:07 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:17:08 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 09 Aug 2022 18:17:08 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 09 Aug 2022 18:17:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 09 Aug 2022 18:17:12 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Tue, 09 Aug 2022 18:17:12 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Aug 2022 18:17:12 GMT
EXPOSE 8888
# Tue, 09 Aug 2022 18:17:12 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Aug 2022 18:17:12 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Tue, 09 Aug 2022 18:17:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Aug 2022 18:17:13 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b667f667e0d162df357cbdea46ee3457fd45395b451ccad50381f4665f8149`  
		Last Modified: Tue, 09 Aug 2022 18:18:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86aedf0b86f2f672427bd99edb4d53285ee3f072fdd5e4ea92fd315f1f9d2bb8`  
		Last Modified: Tue, 09 Aug 2022 18:18:07 GMT  
		Size: 284.6 KB (284571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f1df9899b6ebf1d7df5d628d46580ccbb0e5f130f92a62fa0e6f5e940fe4fc`  
		Last Modified: Tue, 09 Aug 2022 18:18:09 GMT  
		Size: 11.7 MB (11738425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8791b6fe87b776babbb1a953ade5de230b9240678f38258cd21e37a5927ae136`  
		Last Modified: Tue, 09 Aug 2022 18:18:07 GMT  
		Size: 12.3 KB (12273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0086db28ed5d9a6f65ea6988dd5457188e01632dcb02c1d0fd446f660d9d351`  
		Last Modified: Tue, 09 Aug 2022 18:18:07 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c686c318fdda143bca0bfaa2fca999e7547916b852d9fbaa7b4dc38409b40b`  
		Last Modified: Tue, 09 Aug 2022 18:18:07 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7`

```console
$ docker pull chronograf@sha256:64d62de26959222c34f80f59b803d6819a76a4f15ce162e2b8c98a409e065854
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7` - linux; amd64

```console
$ docker pull chronograf@sha256:c5cae25dce4df401c1c8f91b16c4caab3fc4fa19f6620b716e4d9fe8fed4e99f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65427090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f420e13fb6cec22c8d940263fcc76f69cf0f114af1998d310630ed38034f21b5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:20 GMT
ADD file:cfad5912b6dd7590713979e5a5e231b1b6873200fde725cb7baf75110d7fa138 in / 
# Thu, 23 Jun 2022 00:22:20 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:04:03 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 01:04:03 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 23 Jun 2022 01:04:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 01:04:14 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 01:04:14 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 01:04:14 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 01:04:14 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 01:04:15 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 01:04:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 01:04:15 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bff3e048017eab8adaed886bad4b3c5c81f7d952b65b056dca8d6dbc198222dd`  
		Last Modified: Thu, 23 Jun 2022 00:30:01 GMT  
		Size: 22.6 MB (22567461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f498f06d4ed9111864f2ab866f548535967b7a27356e24751b496239c5cd48`  
		Last Modified: Thu, 23 Jun 2022 01:05:23 GMT  
		Size: 4.5 MB (4506747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcdfa28a81d1b8e1e01f3559e494476d77efa27b677497075efea8937251e40`  
		Last Modified: Thu, 23 Jun 2022 01:05:28 GMT  
		Size: 38.3 MB (38328483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08cc1b0dfc1406fbf7318d2c168494aa8dd06ecde735e45faff3a9cf7836294`  
		Last Modified: Thu, 23 Jun 2022 01:05:22 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8995808b815f6b1ac983ee510f22df4c6edfc8521de517d0850234ba2d25a486`  
		Last Modified: Thu, 23 Jun 2022 01:05:23 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2be6170b31a796c94d1f4c620cd8e03aed67489d41ef7bc7737d118ed303078`  
		Last Modified: Thu, 23 Jun 2022 01:05:22 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:9c5742d8c18c067052a12cf2a72ae66e91beede8710b3330ed344cb17e70c453
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (59047810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60f79ccb7d5eb6978bfbe5498017f01d15afae9f2ae7d28b146ceb6baab6dd71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 01:05:38 GMT
ADD file:fc42adb3b30bf8dda0909ae6f3c3754d78c642e1a1d739bedf21934b7e7da3dd in / 
# Thu, 23 Jun 2022 01:05:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 02:26:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 02:26:50 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 23 Jun 2022 02:27:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 02:27:23 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 02:27:24 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 02:27:24 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 02:27:25 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 02:27:25 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 02:27:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 02:27:26 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a259ad5a4933979a4df4eb948f8761dde9b9f3d710259da588afee9fa00f1fef`  
		Last Modified: Thu, 23 Jun 2022 01:22:42 GMT  
		Size: 19.4 MB (19359846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1151ce28350c58d0281452a2f6816ba23bba0fb059a87dce3d58571b33f8703d`  
		Last Modified: Thu, 23 Jun 2022 02:30:00 GMT  
		Size: 3.9 MB (3880137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640ce7e7a0a82d6cabb233df34c4f83a2866f50e05fcefd53f2be4664ea99a9b`  
		Last Modified: Thu, 23 Jun 2022 02:30:17 GMT  
		Size: 35.8 MB (35783434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2982946af9b0db1e6f252d6efd539f6e760b58591c707b020ce1dbaaa5b42a`  
		Last Modified: Thu, 23 Jun 2022 02:29:58 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d107aea611fc0fba41c5be29ad3b8f9b4930eaa60002ee0b2d1240d9c1d4a2ce`  
		Last Modified: Thu, 23 Jun 2022 02:29:58 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4c3656080bec74f2510192d1b056c08c27aba9ea76f287cbfbcd23025dc2d6`  
		Last Modified: Thu, 23 Jun 2022 02:29:58 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:8d166be109cff4bf91830a92c5f923c96adbaafa124065f43ef32ffee0fd1eb2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60329104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d8e02065a47aeb30163b563e0c4c31efe9a9ee4e060dd635f83029f757b1b8f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 00:42:59 GMT
ADD file:c1bdac846ff41ceb56a44de5da778cfb7c3db7ccf4d689b7c1c22c0b80381c49 in / 
# Thu, 23 Jun 2022 00:42:59 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:27:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 01:27:47 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 23 Jun 2022 01:27:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 01:28:00 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 01:28:01 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 01:28:01 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 01:28:02 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 01:28:04 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 01:28:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 01:28:05 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:45f14b91a40fe8177f16f6b6526ada782d0d63a7958757d4e07c543e574ea7a8`  
		Last Modified: Thu, 23 Jun 2022 00:51:46 GMT  
		Size: 20.4 MB (20423990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac8b9598caa4b3c56f37f213c384246bc7d1f7af45b3322d773660d9bf5de4f`  
		Last Modified: Thu, 23 Jun 2022 01:29:28 GMT  
		Size: 3.9 MB (3893941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5426d04d01602e2f8b696af6b30401fb6fd4138203bf457189063bcdb3c733`  
		Last Modified: Thu, 23 Jun 2022 01:29:32 GMT  
		Size: 36.0 MB (35986784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67971835240decaa81a59fa355c46e2788fe76785c7acbea4f72ca41d65414f1`  
		Last Modified: Thu, 23 Jun 2022 01:29:28 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdcb2163bc786a80e47d18b390e3bff9bd2abb60b9957002a2048ce6cd36ef67`  
		Last Modified: Thu, 23 Jun 2022 01:29:28 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef11897af2ff779b380dc88b7350055a885ef55b11dd72b504f87d627c1b7e2`  
		Last Modified: Thu, 23 Jun 2022 01:29:28 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7-alpine`

```console
$ docker pull chronograf@sha256:fea4948a9d212c423a391a04a0fa1a744bab2201b04f25d28a664324916f2166
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.7-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:6e99be2a7bac5d79785429c530f776f1b9c4962f98ca89eba9da3accc2e0149b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22693411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:613fc9f1aee33747b3623b95a2c4e433e694a02bf99b2603842cad9cd95350eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:17:07 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:17:08 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 09 Aug 2022 18:17:18 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 09 Aug 2022 18:17:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 09 Aug 2022 18:17:23 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Aug 2022 18:17:23 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Aug 2022 18:17:23 GMT
EXPOSE 8888
# Tue, 09 Aug 2022 18:17:23 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Aug 2022 18:17:23 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Tue, 09 Aug 2022 18:17:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Aug 2022 18:17:23 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b667f667e0d162df357cbdea46ee3457fd45395b451ccad50381f4665f8149`  
		Last Modified: Tue, 09 Aug 2022 18:18:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86aedf0b86f2f672427bd99edb4d53285ee3f072fdd5e4ea92fd315f1f9d2bb8`  
		Last Modified: Tue, 09 Aug 2022 18:18:07 GMT  
		Size: 284.6 KB (284571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d588c7a740f6a0231b7e4eef9c215c7d86c3ee2c7629f86608c0da729d296b4`  
		Last Modified: Tue, 09 Aug 2022 18:18:23 GMT  
		Size: 19.6 MB (19556805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2285853c8534cea7724c2b4e7c863c0ca3077cea5440d2ab2a1057b3b2ae40`  
		Last Modified: Tue, 09 Aug 2022 18:18:20 GMT  
		Size: 12.3 KB (12261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5295b9363991edc0b91ca76c2202f61857fa2130afd1918b477a969afba18311`  
		Last Modified: Tue, 09 Aug 2022 18:18:20 GMT  
		Size: 11.9 KB (11894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961531905b194ca826eec578c91b790b266e5c429a5969e7afb0a17a674fee7c`  
		Last Modified: Tue, 09 Aug 2022 18:18:20 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17`

```console
$ docker pull chronograf@sha256:64d62de26959222c34f80f59b803d6819a76a4f15ce162e2b8c98a409e065854
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7.17` - linux; amd64

```console
$ docker pull chronograf@sha256:c5cae25dce4df401c1c8f91b16c4caab3fc4fa19f6620b716e4d9fe8fed4e99f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65427090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f420e13fb6cec22c8d940263fcc76f69cf0f114af1998d310630ed38034f21b5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:20 GMT
ADD file:cfad5912b6dd7590713979e5a5e231b1b6873200fde725cb7baf75110d7fa138 in / 
# Thu, 23 Jun 2022 00:22:20 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:04:03 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 01:04:03 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 23 Jun 2022 01:04:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 01:04:14 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 01:04:14 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 01:04:14 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 01:04:14 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 01:04:15 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 01:04:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 01:04:15 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bff3e048017eab8adaed886bad4b3c5c81f7d952b65b056dca8d6dbc198222dd`  
		Last Modified: Thu, 23 Jun 2022 00:30:01 GMT  
		Size: 22.6 MB (22567461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f498f06d4ed9111864f2ab866f548535967b7a27356e24751b496239c5cd48`  
		Last Modified: Thu, 23 Jun 2022 01:05:23 GMT  
		Size: 4.5 MB (4506747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcdfa28a81d1b8e1e01f3559e494476d77efa27b677497075efea8937251e40`  
		Last Modified: Thu, 23 Jun 2022 01:05:28 GMT  
		Size: 38.3 MB (38328483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08cc1b0dfc1406fbf7318d2c168494aa8dd06ecde735e45faff3a9cf7836294`  
		Last Modified: Thu, 23 Jun 2022 01:05:22 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8995808b815f6b1ac983ee510f22df4c6edfc8521de517d0850234ba2d25a486`  
		Last Modified: Thu, 23 Jun 2022 01:05:23 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2be6170b31a796c94d1f4c620cd8e03aed67489d41ef7bc7737d118ed303078`  
		Last Modified: Thu, 23 Jun 2022 01:05:22 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:9c5742d8c18c067052a12cf2a72ae66e91beede8710b3330ed344cb17e70c453
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (59047810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60f79ccb7d5eb6978bfbe5498017f01d15afae9f2ae7d28b146ceb6baab6dd71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 01:05:38 GMT
ADD file:fc42adb3b30bf8dda0909ae6f3c3754d78c642e1a1d739bedf21934b7e7da3dd in / 
# Thu, 23 Jun 2022 01:05:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 02:26:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 02:26:50 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 23 Jun 2022 02:27:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 02:27:23 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 02:27:24 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 02:27:24 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 02:27:25 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 02:27:25 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 02:27:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 02:27:26 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a259ad5a4933979a4df4eb948f8761dde9b9f3d710259da588afee9fa00f1fef`  
		Last Modified: Thu, 23 Jun 2022 01:22:42 GMT  
		Size: 19.4 MB (19359846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1151ce28350c58d0281452a2f6816ba23bba0fb059a87dce3d58571b33f8703d`  
		Last Modified: Thu, 23 Jun 2022 02:30:00 GMT  
		Size: 3.9 MB (3880137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640ce7e7a0a82d6cabb233df34c4f83a2866f50e05fcefd53f2be4664ea99a9b`  
		Last Modified: Thu, 23 Jun 2022 02:30:17 GMT  
		Size: 35.8 MB (35783434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2982946af9b0db1e6f252d6efd539f6e760b58591c707b020ce1dbaaa5b42a`  
		Last Modified: Thu, 23 Jun 2022 02:29:58 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d107aea611fc0fba41c5be29ad3b8f9b4930eaa60002ee0b2d1240d9c1d4a2ce`  
		Last Modified: Thu, 23 Jun 2022 02:29:58 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4c3656080bec74f2510192d1b056c08c27aba9ea76f287cbfbcd23025dc2d6`  
		Last Modified: Thu, 23 Jun 2022 02:29:58 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:8d166be109cff4bf91830a92c5f923c96adbaafa124065f43ef32ffee0fd1eb2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60329104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d8e02065a47aeb30163b563e0c4c31efe9a9ee4e060dd635f83029f757b1b8f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 00:42:59 GMT
ADD file:c1bdac846ff41ceb56a44de5da778cfb7c3db7ccf4d689b7c1c22c0b80381c49 in / 
# Thu, 23 Jun 2022 00:42:59 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:27:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 01:27:47 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 23 Jun 2022 01:27:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 01:28:00 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 01:28:01 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 01:28:01 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 01:28:02 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 01:28:04 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 01:28:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 01:28:05 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:45f14b91a40fe8177f16f6b6526ada782d0d63a7958757d4e07c543e574ea7a8`  
		Last Modified: Thu, 23 Jun 2022 00:51:46 GMT  
		Size: 20.4 MB (20423990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac8b9598caa4b3c56f37f213c384246bc7d1f7af45b3322d773660d9bf5de4f`  
		Last Modified: Thu, 23 Jun 2022 01:29:28 GMT  
		Size: 3.9 MB (3893941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5426d04d01602e2f8b696af6b30401fb6fd4138203bf457189063bcdb3c733`  
		Last Modified: Thu, 23 Jun 2022 01:29:32 GMT  
		Size: 36.0 MB (35986784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67971835240decaa81a59fa355c46e2788fe76785c7acbea4f72ca41d65414f1`  
		Last Modified: Thu, 23 Jun 2022 01:29:28 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdcb2163bc786a80e47d18b390e3bff9bd2abb60b9957002a2048ce6cd36ef67`  
		Last Modified: Thu, 23 Jun 2022 01:29:28 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef11897af2ff779b380dc88b7350055a885ef55b11dd72b504f87d627c1b7e2`  
		Last Modified: Thu, 23 Jun 2022 01:29:28 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17-alpine`

```console
$ docker pull chronograf@sha256:fea4948a9d212c423a391a04a0fa1a744bab2201b04f25d28a664324916f2166
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.7.17-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:6e99be2a7bac5d79785429c530f776f1b9c4962f98ca89eba9da3accc2e0149b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22693411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:613fc9f1aee33747b3623b95a2c4e433e694a02bf99b2603842cad9cd95350eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:17:07 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:17:08 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 09 Aug 2022 18:17:18 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 09 Aug 2022 18:17:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 09 Aug 2022 18:17:23 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Aug 2022 18:17:23 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Aug 2022 18:17:23 GMT
EXPOSE 8888
# Tue, 09 Aug 2022 18:17:23 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Aug 2022 18:17:23 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Tue, 09 Aug 2022 18:17:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Aug 2022 18:17:23 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b667f667e0d162df357cbdea46ee3457fd45395b451ccad50381f4665f8149`  
		Last Modified: Tue, 09 Aug 2022 18:18:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86aedf0b86f2f672427bd99edb4d53285ee3f072fdd5e4ea92fd315f1f9d2bb8`  
		Last Modified: Tue, 09 Aug 2022 18:18:07 GMT  
		Size: 284.6 KB (284571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d588c7a740f6a0231b7e4eef9c215c7d86c3ee2c7629f86608c0da729d296b4`  
		Last Modified: Tue, 09 Aug 2022 18:18:23 GMT  
		Size: 19.6 MB (19556805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2285853c8534cea7724c2b4e7c863c0ca3077cea5440d2ab2a1057b3b2ae40`  
		Last Modified: Tue, 09 Aug 2022 18:18:20 GMT  
		Size: 12.3 KB (12261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5295b9363991edc0b91ca76c2202f61857fa2130afd1918b477a969afba18311`  
		Last Modified: Tue, 09 Aug 2022 18:18:20 GMT  
		Size: 11.9 KB (11894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961531905b194ca826eec578c91b790b266e5c429a5969e7afb0a17a674fee7c`  
		Last Modified: Tue, 09 Aug 2022 18:18:20 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8`

```console
$ docker pull chronograf@sha256:fc5d7eb0310653a77792b53dab0bb5e4b8c4f98ad049b7215440c7e1dbe2c514
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8` - linux; amd64

```console
$ docker pull chronograf@sha256:63caf9f0f528e26b71300621aaf5e006d1db4320f0611c9de314deef1b29da7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66278888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd374f64eac84b9357bda804cee1d8c976d03532a09dbaed36744c6bb58dba11`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:20 GMT
ADD file:cfad5912b6dd7590713979e5a5e231b1b6873200fde725cb7baf75110d7fa138 in / 
# Thu, 23 Jun 2022 00:22:20 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:03:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 01:04:21 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Thu, 23 Jun 2022 01:04:29 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 01:04:30 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 01:04:30 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 01:04:30 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 01:04:30 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 01:04:30 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 01:04:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 01:04:30 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bff3e048017eab8adaed886bad4b3c5c81f7d952b65b056dca8d6dbc198222dd`  
		Last Modified: Thu, 23 Jun 2022 00:30:01 GMT  
		Size: 22.6 MB (22567461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b5498e1d3acd0f9ff62393ea37f571882a0eec6680617ecb40142cd977a4d4`  
		Last Modified: Thu, 23 Jun 2022 01:05:10 GMT  
		Size: 6.8 MB (6760409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3571224894ea1d72616a619e9884699ec937cf0611294c58271749705282eb42`  
		Last Modified: Thu, 23 Jun 2022 01:05:44 GMT  
		Size: 36.9 MB (36926628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80abaef4bc317c3286ed790449ac193fc9593858ba90d3172992d734f8868f2f`  
		Last Modified: Thu, 23 Jun 2022 01:05:39 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d28eeb4e3f820fa4c1809d2bdb2ef78bdef4edf847c63dbfeaef74592f70799`  
		Last Modified: Thu, 23 Jun 2022 01:05:39 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e36896bec5c1d1566f204be387023e292e163d8abe950865c11a8e8fb6870aa`  
		Last Modified: Thu, 23 Jun 2022 01:05:39 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:ae095e81b5493e1f535f270877a68ab596fe2062f24feeb625b620e683cf4d74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.7 MB (59677249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904cadb37b2b12e77e43bc74e32946098fa3e05da140b6398a0601123411b46f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 01:05:38 GMT
ADD file:fc42adb3b30bf8dda0909ae6f3c3754d78c642e1a1d739bedf21934b7e7da3dd in / 
# Thu, 23 Jun 2022 01:05:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 02:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 02:27:43 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Thu, 23 Jun 2022 02:28:04 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 02:28:05 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 02:28:05 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 02:28:05 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 02:28:06 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 02:28:06 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 02:28:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 02:28:07 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a259ad5a4933979a4df4eb948f8761dde9b9f3d710259da588afee9fa00f1fef`  
		Last Modified: Thu, 23 Jun 2022 01:22:42 GMT  
		Size: 19.4 MB (19359846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0f7a736acf205407547109d49c141be814413fe2e704f167f154beb4a64bf8`  
		Last Modified: Thu, 23 Jun 2022 02:29:36 GMT  
		Size: 5.8 MB (5781003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd9fdb3bbbe22d909cf6075be0c42a4cd2829be933bdf2f57f0e7eeaeded65c`  
		Last Modified: Thu, 23 Jun 2022 02:30:48 GMT  
		Size: 34.5 MB (34512017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26d510940d20bcb9aa24c28848269aaa33dafa3a4b08a920cfa0d65790005c4`  
		Last Modified: Thu, 23 Jun 2022 02:30:29 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9196dc934b24b3b98dadc8a27af109a4d423b526cc9ca51bf2507026fe15d05`  
		Last Modified: Thu, 23 Jun 2022 02:30:34 GMT  
		Size: 11.9 KB (11900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e59dcb7e40fd82416224258887b3c2cb96806ff1324096c7d294b3c0c49bf1`  
		Last Modified: Thu, 23 Jun 2022 02:30:29 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:c604e20e46ed81d4e09f3138a1e5558ae6df6eda8e5d1ff0b89d62f116e9b7b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.9 MB (60927292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2eceadb48d0f5d4f735bc6a8c9573e4414903782ef6d731d7b1598c4ab2a56d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 00:42:59 GMT
ADD file:c1bdac846ff41ceb56a44de5da778cfb7c3db7ccf4d689b7c1c22c0b80381c49 in / 
# Thu, 23 Jun 2022 00:42:59 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:27:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 01:28:10 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Thu, 23 Jun 2022 01:28:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 01:28:20 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 01:28:21 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 01:28:21 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 01:28:22 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 01:28:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 01:28:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 01:28:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:45f14b91a40fe8177f16f6b6526ada782d0d63a7958757d4e07c543e574ea7a8`  
		Last Modified: Thu, 23 Jun 2022 00:51:46 GMT  
		Size: 20.4 MB (20423990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba5c15f7bd5dfe32b1718aade52f008519a7ffa497114d413766119a3dbd4f8`  
		Last Modified: Thu, 23 Jun 2022 01:29:14 GMT  
		Size: 6.0 MB (6047312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c1a8cb2336b85ea9a994dbce5e4a24a55bf674f2f99de4d6ace760d7500e69`  
		Last Modified: Thu, 23 Jun 2022 01:29:48 GMT  
		Size: 34.4 MB (34431598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c15f181ea0049ba7b848851ca06b65650fd20f80fe36b50d2539cdc744d8386`  
		Last Modified: Thu, 23 Jun 2022 01:29:43 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbaa4b067e7757a8dfbd975c1a6e477396433d160f700e17652803c8c50fc2b`  
		Last Modified: Thu, 23 Jun 2022 01:29:43 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdbab753cfbe0ef9907ea289d72732370b4ca5cd6b650c1a85f992af3ef56bd9`  
		Last Modified: Thu, 23 Jun 2022 01:29:43 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8-alpine`

```console
$ docker pull chronograf@sha256:e21c2df83074058f591e400db598e2f2e0db991c065b382002f19a57036d65b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:4fbff7c953dd88ff517c74a639c8fab663fe9365b302d1e6414bea67cb3a79a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22340814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e17e2be70c7462109bc2188a05c987ba18caac5fdbe12032d9b157b5e466809`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:17:07 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:17:08 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 09 Aug 2022 18:17:28 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 09 Aug 2022 18:17:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 09 Aug 2022 18:17:33 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Aug 2022 18:17:33 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Aug 2022 18:17:33 GMT
EXPOSE 8888
# Tue, 09 Aug 2022 18:17:33 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Aug 2022 18:17:33 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Tue, 09 Aug 2022 18:17:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Aug 2022 18:17:34 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b667f667e0d162df357cbdea46ee3457fd45395b451ccad50381f4665f8149`  
		Last Modified: Tue, 09 Aug 2022 18:18:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86aedf0b86f2f672427bd99edb4d53285ee3f072fdd5e4ea92fd315f1f9d2bb8`  
		Last Modified: Tue, 09 Aug 2022 18:18:07 GMT  
		Size: 284.6 KB (284571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf91dd373292f741fe4469ec76e73a80420fbc2da4bdc8d4d3e2f14c4cca7607`  
		Last Modified: Tue, 09 Aug 2022 18:18:37 GMT  
		Size: 19.2 MB (19204195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686071ec84727f65defe0a32dc8401552bc4e3d88c84a6e35829f0da6fb5db30`  
		Last Modified: Tue, 09 Aug 2022 18:18:33 GMT  
		Size: 12.3 KB (12268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a1a0c949f66345474da08be2eb9ad15e11a935b421d5d4d52e509861a46bf7`  
		Last Modified: Tue, 09 Aug 2022 18:18:33 GMT  
		Size: 11.9 KB (11900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae01956999004409f2013989dc7bc0d92b2ca8b9079486ad1eb081d55e5b6ae7`  
		Last Modified: Tue, 09 Aug 2022 18:18:33 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.10`

```console
$ docker pull chronograf@sha256:fc5d7eb0310653a77792b53dab0bb5e4b8c4f98ad049b7215440c7e1dbe2c514
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8.10` - linux; amd64

```console
$ docker pull chronograf@sha256:63caf9f0f528e26b71300621aaf5e006d1db4320f0611c9de314deef1b29da7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66278888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd374f64eac84b9357bda804cee1d8c976d03532a09dbaed36744c6bb58dba11`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:20 GMT
ADD file:cfad5912b6dd7590713979e5a5e231b1b6873200fde725cb7baf75110d7fa138 in / 
# Thu, 23 Jun 2022 00:22:20 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:03:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 01:04:21 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Thu, 23 Jun 2022 01:04:29 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 01:04:30 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 01:04:30 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 01:04:30 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 01:04:30 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 01:04:30 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 01:04:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 01:04:30 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bff3e048017eab8adaed886bad4b3c5c81f7d952b65b056dca8d6dbc198222dd`  
		Last Modified: Thu, 23 Jun 2022 00:30:01 GMT  
		Size: 22.6 MB (22567461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b5498e1d3acd0f9ff62393ea37f571882a0eec6680617ecb40142cd977a4d4`  
		Last Modified: Thu, 23 Jun 2022 01:05:10 GMT  
		Size: 6.8 MB (6760409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3571224894ea1d72616a619e9884699ec937cf0611294c58271749705282eb42`  
		Last Modified: Thu, 23 Jun 2022 01:05:44 GMT  
		Size: 36.9 MB (36926628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80abaef4bc317c3286ed790449ac193fc9593858ba90d3172992d734f8868f2f`  
		Last Modified: Thu, 23 Jun 2022 01:05:39 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d28eeb4e3f820fa4c1809d2bdb2ef78bdef4edf847c63dbfeaef74592f70799`  
		Last Modified: Thu, 23 Jun 2022 01:05:39 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e36896bec5c1d1566f204be387023e292e163d8abe950865c11a8e8fb6870aa`  
		Last Modified: Thu, 23 Jun 2022 01:05:39 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.10` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:ae095e81b5493e1f535f270877a68ab596fe2062f24feeb625b620e683cf4d74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.7 MB (59677249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904cadb37b2b12e77e43bc74e32946098fa3e05da140b6398a0601123411b46f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 01:05:38 GMT
ADD file:fc42adb3b30bf8dda0909ae6f3c3754d78c642e1a1d739bedf21934b7e7da3dd in / 
# Thu, 23 Jun 2022 01:05:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 02:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 02:27:43 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Thu, 23 Jun 2022 02:28:04 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 02:28:05 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 02:28:05 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 02:28:05 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 02:28:06 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 02:28:06 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 02:28:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 02:28:07 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a259ad5a4933979a4df4eb948f8761dde9b9f3d710259da588afee9fa00f1fef`  
		Last Modified: Thu, 23 Jun 2022 01:22:42 GMT  
		Size: 19.4 MB (19359846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0f7a736acf205407547109d49c141be814413fe2e704f167f154beb4a64bf8`  
		Last Modified: Thu, 23 Jun 2022 02:29:36 GMT  
		Size: 5.8 MB (5781003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd9fdb3bbbe22d909cf6075be0c42a4cd2829be933bdf2f57f0e7eeaeded65c`  
		Last Modified: Thu, 23 Jun 2022 02:30:48 GMT  
		Size: 34.5 MB (34512017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26d510940d20bcb9aa24c28848269aaa33dafa3a4b08a920cfa0d65790005c4`  
		Last Modified: Thu, 23 Jun 2022 02:30:29 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9196dc934b24b3b98dadc8a27af109a4d423b526cc9ca51bf2507026fe15d05`  
		Last Modified: Thu, 23 Jun 2022 02:30:34 GMT  
		Size: 11.9 KB (11900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e59dcb7e40fd82416224258887b3c2cb96806ff1324096c7d294b3c0c49bf1`  
		Last Modified: Thu, 23 Jun 2022 02:30:29 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.10` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:c604e20e46ed81d4e09f3138a1e5558ae6df6eda8e5d1ff0b89d62f116e9b7b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.9 MB (60927292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2eceadb48d0f5d4f735bc6a8c9573e4414903782ef6d731d7b1598c4ab2a56d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 00:42:59 GMT
ADD file:c1bdac846ff41ceb56a44de5da778cfb7c3db7ccf4d689b7c1c22c0b80381c49 in / 
# Thu, 23 Jun 2022 00:42:59 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:27:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 01:28:10 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Thu, 23 Jun 2022 01:28:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 01:28:20 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 01:28:21 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 01:28:21 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 01:28:22 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 01:28:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 01:28:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 01:28:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:45f14b91a40fe8177f16f6b6526ada782d0d63a7958757d4e07c543e574ea7a8`  
		Last Modified: Thu, 23 Jun 2022 00:51:46 GMT  
		Size: 20.4 MB (20423990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba5c15f7bd5dfe32b1718aade52f008519a7ffa497114d413766119a3dbd4f8`  
		Last Modified: Thu, 23 Jun 2022 01:29:14 GMT  
		Size: 6.0 MB (6047312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c1a8cb2336b85ea9a994dbce5e4a24a55bf674f2f99de4d6ace760d7500e69`  
		Last Modified: Thu, 23 Jun 2022 01:29:48 GMT  
		Size: 34.4 MB (34431598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c15f181ea0049ba7b848851ca06b65650fd20f80fe36b50d2539cdc744d8386`  
		Last Modified: Thu, 23 Jun 2022 01:29:43 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbaa4b067e7757a8dfbd975c1a6e477396433d160f700e17652803c8c50fc2b`  
		Last Modified: Thu, 23 Jun 2022 01:29:43 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdbab753cfbe0ef9907ea289d72732370b4ca5cd6b650c1a85f992af3ef56bd9`  
		Last Modified: Thu, 23 Jun 2022 01:29:43 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.10-alpine`

```console
$ docker pull chronograf@sha256:e21c2df83074058f591e400db598e2f2e0db991c065b382002f19a57036d65b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.8.10-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:4fbff7c953dd88ff517c74a639c8fab663fe9365b302d1e6414bea67cb3a79a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22340814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e17e2be70c7462109bc2188a05c987ba18caac5fdbe12032d9b157b5e466809`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:17:07 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:17:08 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 09 Aug 2022 18:17:28 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 09 Aug 2022 18:17:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 09 Aug 2022 18:17:33 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Aug 2022 18:17:33 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Aug 2022 18:17:33 GMT
EXPOSE 8888
# Tue, 09 Aug 2022 18:17:33 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Aug 2022 18:17:33 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Tue, 09 Aug 2022 18:17:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Aug 2022 18:17:34 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b667f667e0d162df357cbdea46ee3457fd45395b451ccad50381f4665f8149`  
		Last Modified: Tue, 09 Aug 2022 18:18:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86aedf0b86f2f672427bd99edb4d53285ee3f072fdd5e4ea92fd315f1f9d2bb8`  
		Last Modified: Tue, 09 Aug 2022 18:18:07 GMT  
		Size: 284.6 KB (284571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf91dd373292f741fe4469ec76e73a80420fbc2da4bdc8d4d3e2f14c4cca7607`  
		Last Modified: Tue, 09 Aug 2022 18:18:37 GMT  
		Size: 19.2 MB (19204195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686071ec84727f65defe0a32dc8401552bc4e3d88c84a6e35829f0da6fb5db30`  
		Last Modified: Tue, 09 Aug 2022 18:18:33 GMT  
		Size: 12.3 KB (12268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a1a0c949f66345474da08be2eb9ad15e11a935b421d5d4d52e509861a46bf7`  
		Last Modified: Tue, 09 Aug 2022 18:18:33 GMT  
		Size: 11.9 KB (11900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae01956999004409f2013989dc7bc0d92b2ca8b9079486ad1eb081d55e5b6ae7`  
		Last Modified: Tue, 09 Aug 2022 18:18:33 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9`

```console
$ docker pull chronograf@sha256:4d4f645349b61c6a8de0310a62b065fc599c6cc10b4a8b8144fcb2d16f0d797f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.9` - linux; amd64

```console
$ docker pull chronograf@sha256:f17e9512b8d3019b3e7304a27104b93e804ca748b4b7ae6bf70fe6e8eb670dbd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66922675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cfe22ae70d4b13903558a6a9361bb8987c312e7ffb6eff9b993a83bfc1fa29c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:20 GMT
ADD file:cfad5912b6dd7590713979e5a5e231b1b6873200fde725cb7baf75110d7fa138 in / 
# Thu, 23 Jun 2022 00:22:20 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:03:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 01:04:34 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Thu, 23 Jun 2022 01:04:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 01:04:43 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 01:04:43 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 01:04:44 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 01:04:44 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 01:04:44 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 01:04:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 01:04:44 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bff3e048017eab8adaed886bad4b3c5c81f7d952b65b056dca8d6dbc198222dd`  
		Last Modified: Thu, 23 Jun 2022 00:30:01 GMT  
		Size: 22.6 MB (22567461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b5498e1d3acd0f9ff62393ea37f571882a0eec6680617ecb40142cd977a4d4`  
		Last Modified: Thu, 23 Jun 2022 01:05:10 GMT  
		Size: 6.8 MB (6760409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa682df4ed7265161d790b536e4d0c183299a4d68fb350df760037392c48cae`  
		Last Modified: Thu, 23 Jun 2022 01:05:59 GMT  
		Size: 37.6 MB (37570412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64122926f1c38ece9730eb059c7a59bfbf86dca2e952162b527012d9b3ed7f1`  
		Last Modified: Thu, 23 Jun 2022 01:05:54 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e912b66168d1ebc8e41b42c475e211579caa5bcb17cc5bb033fb89b6d2a77c4b`  
		Last Modified: Thu, 23 Jun 2022 01:05:54 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059c52a2c8401210a0c468e477ad83f5a23cea31ea7fb6064ab631ab296af992`  
		Last Modified: Thu, 23 Jun 2022 01:05:54 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:ccdedcdf7a13cb6ecc4921006cf8e2e9b8f9e2cfbe7ccb04106368c2462fa426
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60456724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdbcbee07e5932907088936b99acefe742302fa27dadd8a2ebb44666f34ed58b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 01:05:38 GMT
ADD file:fc42adb3b30bf8dda0909ae6f3c3754d78c642e1a1d739bedf21934b7e7da3dd in / 
# Thu, 23 Jun 2022 01:05:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 02:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 02:28:19 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Thu, 23 Jun 2022 02:28:39 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 02:28:40 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 02:28:40 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 02:28:41 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 02:28:41 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 02:28:42 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 02:28:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 02:28:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a259ad5a4933979a4df4eb948f8761dde9b9f3d710259da588afee9fa00f1fef`  
		Last Modified: Thu, 23 Jun 2022 01:22:42 GMT  
		Size: 19.4 MB (19359846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0f7a736acf205407547109d49c141be814413fe2e704f167f154beb4a64bf8`  
		Last Modified: Thu, 23 Jun 2022 02:29:36 GMT  
		Size: 5.8 MB (5781003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec49c5d35def6ec8c590f209f60abf43ea871d2d35302760bbb0357a98f43b26`  
		Last Modified: Thu, 23 Jun 2022 02:31:18 GMT  
		Size: 35.3 MB (35291489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f657baa3f44759dd9b58b6460a04ffd0dc57bc7278218447b9de83ccd7d023`  
		Last Modified: Thu, 23 Jun 2022 02:30:59 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8dbc5d31121e03f9d916e8276728d4a02d649e1e57746561430adcb65350008`  
		Last Modified: Thu, 23 Jun 2022 02:30:59 GMT  
		Size: 11.9 KB (11902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0086f50118a0d8b418649e9fd989d5eb5c94e7c14506b6980ca0ba840a75c1`  
		Last Modified: Thu, 23 Jun 2022 02:30:59 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:d5dfa6b4fc06d5183c2fffc72832fe0aeadecb2fac2a02adb08592f924fe47d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61669706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6515bd8a31c397aec3531e07859da02f7b6e487896be7f6c2e0af789d214eaf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 00:42:59 GMT
ADD file:c1bdac846ff41ceb56a44de5da778cfb7c3db7ccf4d689b7c1c22c0b80381c49 in / 
# Thu, 23 Jun 2022 00:42:59 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:27:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 01:28:32 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Thu, 23 Jun 2022 01:28:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 01:28:42 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 01:28:43 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 01:28:43 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 01:28:44 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 01:28:46 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 01:28:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 01:28:47 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:45f14b91a40fe8177f16f6b6526ada782d0d63a7958757d4e07c543e574ea7a8`  
		Last Modified: Thu, 23 Jun 2022 00:51:46 GMT  
		Size: 20.4 MB (20423990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba5c15f7bd5dfe32b1718aade52f008519a7ffa497114d413766119a3dbd4f8`  
		Last Modified: Thu, 23 Jun 2022 01:29:14 GMT  
		Size: 6.0 MB (6047312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35008848465d6270ff38da08a7514053d62632985429e2326581b33946d6761b`  
		Last Modified: Thu, 23 Jun 2022 01:30:04 GMT  
		Size: 35.2 MB (35174017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75069e610add6e199c1abfd85f6596a3f7e15bc912230ddb1e0cdab0b41d71d`  
		Last Modified: Thu, 23 Jun 2022 01:29:59 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cdbd4a0e6503bdb63b1ce28ad92eeb99798ed8df1d1cf91cf4b53eabb8b192`  
		Last Modified: Thu, 23 Jun 2022 01:29:59 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6cb9709f043f81dc4d6f60f562a1d82615eb06ff08d1d6ed5544c34ad0fea3`  
		Last Modified: Thu, 23 Jun 2022 01:29:59 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9-alpine`

```console
$ docker pull chronograf@sha256:cf92fc3cc4691bd74be8d509e1daca31c444deeda4f588d763a6dbf938b01403
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.9-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:38373234e15d1c93f102793597e9bf12e862d1c6aa7585a0bcba9c07ebc77621
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.8 MB (22808785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ced3757bcaca9904d45cc79b6978e0aa53759fa9d16a4fb13fa24be010091f25`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:17:07 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:17:08 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 09 Aug 2022 18:17:38 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 09 Aug 2022 18:17:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 09 Aug 2022 18:17:43 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Aug 2022 18:17:43 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Aug 2022 18:17:43 GMT
EXPOSE 8888
# Tue, 09 Aug 2022 18:17:43 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Aug 2022 18:17:43 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Tue, 09 Aug 2022 18:17:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Aug 2022 18:17:43 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b667f667e0d162df357cbdea46ee3457fd45395b451ccad50381f4665f8149`  
		Last Modified: Tue, 09 Aug 2022 18:18:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86aedf0b86f2f672427bd99edb4d53285ee3f072fdd5e4ea92fd315f1f9d2bb8`  
		Last Modified: Tue, 09 Aug 2022 18:18:07 GMT  
		Size: 284.6 KB (284571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63ea984c81d9a176e87bff3e349d81ffb7375a5fbb71f461b755a13a4e2ab17`  
		Last Modified: Tue, 09 Aug 2022 18:18:51 GMT  
		Size: 19.7 MB (19672179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8828c26e16c48e93e2262d948136dc8b4f87b0a28d6a7b29b71e7a18844c1a34`  
		Last Modified: Tue, 09 Aug 2022 18:18:47 GMT  
		Size: 12.3 KB (12263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015194f0f71e31bae9c869e9a3a8d1ceca19267c54f9cc06ac3e2a9236a89f57`  
		Last Modified: Tue, 09 Aug 2022 18:18:47 GMT  
		Size: 11.9 KB (11893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0585391111ba79d1f1c74c4c722494c1e3378ab7694b9df14300c55ff270fe0`  
		Last Modified: Tue, 09 Aug 2022 18:18:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9.4`

```console
$ docker pull chronograf@sha256:4d4f645349b61c6a8de0310a62b065fc599c6cc10b4a8b8144fcb2d16f0d797f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.9.4` - linux; amd64

```console
$ docker pull chronograf@sha256:f17e9512b8d3019b3e7304a27104b93e804ca748b4b7ae6bf70fe6e8eb670dbd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66922675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cfe22ae70d4b13903558a6a9361bb8987c312e7ffb6eff9b993a83bfc1fa29c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:20 GMT
ADD file:cfad5912b6dd7590713979e5a5e231b1b6873200fde725cb7baf75110d7fa138 in / 
# Thu, 23 Jun 2022 00:22:20 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:03:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 01:04:34 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Thu, 23 Jun 2022 01:04:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 01:04:43 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 01:04:43 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 01:04:44 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 01:04:44 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 01:04:44 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 01:04:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 01:04:44 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bff3e048017eab8adaed886bad4b3c5c81f7d952b65b056dca8d6dbc198222dd`  
		Last Modified: Thu, 23 Jun 2022 00:30:01 GMT  
		Size: 22.6 MB (22567461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b5498e1d3acd0f9ff62393ea37f571882a0eec6680617ecb40142cd977a4d4`  
		Last Modified: Thu, 23 Jun 2022 01:05:10 GMT  
		Size: 6.8 MB (6760409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa682df4ed7265161d790b536e4d0c183299a4d68fb350df760037392c48cae`  
		Last Modified: Thu, 23 Jun 2022 01:05:59 GMT  
		Size: 37.6 MB (37570412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64122926f1c38ece9730eb059c7a59bfbf86dca2e952162b527012d9b3ed7f1`  
		Last Modified: Thu, 23 Jun 2022 01:05:54 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e912b66168d1ebc8e41b42c475e211579caa5bcb17cc5bb033fb89b6d2a77c4b`  
		Last Modified: Thu, 23 Jun 2022 01:05:54 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059c52a2c8401210a0c468e477ad83f5a23cea31ea7fb6064ab631ab296af992`  
		Last Modified: Thu, 23 Jun 2022 01:05:54 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9.4` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:ccdedcdf7a13cb6ecc4921006cf8e2e9b8f9e2cfbe7ccb04106368c2462fa426
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60456724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdbcbee07e5932907088936b99acefe742302fa27dadd8a2ebb44666f34ed58b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 01:05:38 GMT
ADD file:fc42adb3b30bf8dda0909ae6f3c3754d78c642e1a1d739bedf21934b7e7da3dd in / 
# Thu, 23 Jun 2022 01:05:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 02:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 02:28:19 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Thu, 23 Jun 2022 02:28:39 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 02:28:40 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 02:28:40 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 02:28:41 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 02:28:41 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 02:28:42 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 02:28:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 02:28:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a259ad5a4933979a4df4eb948f8761dde9b9f3d710259da588afee9fa00f1fef`  
		Last Modified: Thu, 23 Jun 2022 01:22:42 GMT  
		Size: 19.4 MB (19359846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0f7a736acf205407547109d49c141be814413fe2e704f167f154beb4a64bf8`  
		Last Modified: Thu, 23 Jun 2022 02:29:36 GMT  
		Size: 5.8 MB (5781003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec49c5d35def6ec8c590f209f60abf43ea871d2d35302760bbb0357a98f43b26`  
		Last Modified: Thu, 23 Jun 2022 02:31:18 GMT  
		Size: 35.3 MB (35291489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f657baa3f44759dd9b58b6460a04ffd0dc57bc7278218447b9de83ccd7d023`  
		Last Modified: Thu, 23 Jun 2022 02:30:59 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8dbc5d31121e03f9d916e8276728d4a02d649e1e57746561430adcb65350008`  
		Last Modified: Thu, 23 Jun 2022 02:30:59 GMT  
		Size: 11.9 KB (11902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0086f50118a0d8b418649e9fd989d5eb5c94e7c14506b6980ca0ba840a75c1`  
		Last Modified: Thu, 23 Jun 2022 02:30:59 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9.4` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:d5dfa6b4fc06d5183c2fffc72832fe0aeadecb2fac2a02adb08592f924fe47d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61669706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6515bd8a31c397aec3531e07859da02f7b6e487896be7f6c2e0af789d214eaf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 00:42:59 GMT
ADD file:c1bdac846ff41ceb56a44de5da778cfb7c3db7ccf4d689b7c1c22c0b80381c49 in / 
# Thu, 23 Jun 2022 00:42:59 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:27:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 01:28:32 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Thu, 23 Jun 2022 01:28:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 01:28:42 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 01:28:43 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 01:28:43 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 01:28:44 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 01:28:46 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 01:28:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 01:28:47 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:45f14b91a40fe8177f16f6b6526ada782d0d63a7958757d4e07c543e574ea7a8`  
		Last Modified: Thu, 23 Jun 2022 00:51:46 GMT  
		Size: 20.4 MB (20423990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba5c15f7bd5dfe32b1718aade52f008519a7ffa497114d413766119a3dbd4f8`  
		Last Modified: Thu, 23 Jun 2022 01:29:14 GMT  
		Size: 6.0 MB (6047312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35008848465d6270ff38da08a7514053d62632985429e2326581b33946d6761b`  
		Last Modified: Thu, 23 Jun 2022 01:30:04 GMT  
		Size: 35.2 MB (35174017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75069e610add6e199c1abfd85f6596a3f7e15bc912230ddb1e0cdab0b41d71d`  
		Last Modified: Thu, 23 Jun 2022 01:29:59 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cdbd4a0e6503bdb63b1ce28ad92eeb99798ed8df1d1cf91cf4b53eabb8b192`  
		Last Modified: Thu, 23 Jun 2022 01:29:59 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6cb9709f043f81dc4d6f60f562a1d82615eb06ff08d1d6ed5544c34ad0fea3`  
		Last Modified: Thu, 23 Jun 2022 01:29:59 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9.4-alpine`

```console
$ docker pull chronograf@sha256:cf92fc3cc4691bd74be8d509e1daca31c444deeda4f588d763a6dbf938b01403
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.9.4-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:38373234e15d1c93f102793597e9bf12e862d1c6aa7585a0bcba9c07ebc77621
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.8 MB (22808785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ced3757bcaca9904d45cc79b6978e0aa53759fa9d16a4fb13fa24be010091f25`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:17:07 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:17:08 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 09 Aug 2022 18:17:38 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 09 Aug 2022 18:17:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 09 Aug 2022 18:17:43 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Aug 2022 18:17:43 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Aug 2022 18:17:43 GMT
EXPOSE 8888
# Tue, 09 Aug 2022 18:17:43 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Aug 2022 18:17:43 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Tue, 09 Aug 2022 18:17:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Aug 2022 18:17:43 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b667f667e0d162df357cbdea46ee3457fd45395b451ccad50381f4665f8149`  
		Last Modified: Tue, 09 Aug 2022 18:18:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86aedf0b86f2f672427bd99edb4d53285ee3f072fdd5e4ea92fd315f1f9d2bb8`  
		Last Modified: Tue, 09 Aug 2022 18:18:07 GMT  
		Size: 284.6 KB (284571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63ea984c81d9a176e87bff3e349d81ffb7375a5fbb71f461b755a13a4e2ab17`  
		Last Modified: Tue, 09 Aug 2022 18:18:51 GMT  
		Size: 19.7 MB (19672179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8828c26e16c48e93e2262d948136dc8b4f87b0a28d6a7b29b71e7a18844c1a34`  
		Last Modified: Tue, 09 Aug 2022 18:18:47 GMT  
		Size: 12.3 KB (12263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015194f0f71e31bae9c869e9a3a8d1ceca19267c54f9cc06ac3e2a9236a89f57`  
		Last Modified: Tue, 09 Aug 2022 18:18:47 GMT  
		Size: 11.9 KB (11893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0585391111ba79d1f1c74c4c722494c1e3378ab7694b9df14300c55ff270fe0`  
		Last Modified: Tue, 09 Aug 2022 18:18:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:alpine`

```console
$ docker pull chronograf@sha256:cf92fc3cc4691bd74be8d509e1daca31c444deeda4f588d763a6dbf938b01403
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:38373234e15d1c93f102793597e9bf12e862d1c6aa7585a0bcba9c07ebc77621
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.8 MB (22808785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ced3757bcaca9904d45cc79b6978e0aa53759fa9d16a4fb13fa24be010091f25`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:17:07 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:17:08 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 09 Aug 2022 18:17:38 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 09 Aug 2022 18:17:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 09 Aug 2022 18:17:43 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Aug 2022 18:17:43 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Aug 2022 18:17:43 GMT
EXPOSE 8888
# Tue, 09 Aug 2022 18:17:43 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Aug 2022 18:17:43 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Tue, 09 Aug 2022 18:17:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Aug 2022 18:17:43 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b667f667e0d162df357cbdea46ee3457fd45395b451ccad50381f4665f8149`  
		Last Modified: Tue, 09 Aug 2022 18:18:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86aedf0b86f2f672427bd99edb4d53285ee3f072fdd5e4ea92fd315f1f9d2bb8`  
		Last Modified: Tue, 09 Aug 2022 18:18:07 GMT  
		Size: 284.6 KB (284571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63ea984c81d9a176e87bff3e349d81ffb7375a5fbb71f461b755a13a4e2ab17`  
		Last Modified: Tue, 09 Aug 2022 18:18:51 GMT  
		Size: 19.7 MB (19672179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8828c26e16c48e93e2262d948136dc8b4f87b0a28d6a7b29b71e7a18844c1a34`  
		Last Modified: Tue, 09 Aug 2022 18:18:47 GMT  
		Size: 12.3 KB (12263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015194f0f71e31bae9c869e9a3a8d1ceca19267c54f9cc06ac3e2a9236a89f57`  
		Last Modified: Tue, 09 Aug 2022 18:18:47 GMT  
		Size: 11.9 KB (11893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0585391111ba79d1f1c74c4c722494c1e3378ab7694b9df14300c55ff270fe0`  
		Last Modified: Tue, 09 Aug 2022 18:18:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:latest`

```console
$ docker pull chronograf@sha256:4d4f645349b61c6a8de0310a62b065fc599c6cc10b4a8b8144fcb2d16f0d797f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:f17e9512b8d3019b3e7304a27104b93e804ca748b4b7ae6bf70fe6e8eb670dbd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66922675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cfe22ae70d4b13903558a6a9361bb8987c312e7ffb6eff9b993a83bfc1fa29c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:20 GMT
ADD file:cfad5912b6dd7590713979e5a5e231b1b6873200fde725cb7baf75110d7fa138 in / 
# Thu, 23 Jun 2022 00:22:20 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:03:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 01:04:34 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Thu, 23 Jun 2022 01:04:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 01:04:43 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 01:04:43 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 01:04:44 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 01:04:44 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 01:04:44 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 01:04:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 01:04:44 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bff3e048017eab8adaed886bad4b3c5c81f7d952b65b056dca8d6dbc198222dd`  
		Last Modified: Thu, 23 Jun 2022 00:30:01 GMT  
		Size: 22.6 MB (22567461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b5498e1d3acd0f9ff62393ea37f571882a0eec6680617ecb40142cd977a4d4`  
		Last Modified: Thu, 23 Jun 2022 01:05:10 GMT  
		Size: 6.8 MB (6760409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa682df4ed7265161d790b536e4d0c183299a4d68fb350df760037392c48cae`  
		Last Modified: Thu, 23 Jun 2022 01:05:59 GMT  
		Size: 37.6 MB (37570412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64122926f1c38ece9730eb059c7a59bfbf86dca2e952162b527012d9b3ed7f1`  
		Last Modified: Thu, 23 Jun 2022 01:05:54 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e912b66168d1ebc8e41b42c475e211579caa5bcb17cc5bb033fb89b6d2a77c4b`  
		Last Modified: Thu, 23 Jun 2022 01:05:54 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059c52a2c8401210a0c468e477ad83f5a23cea31ea7fb6064ab631ab296af992`  
		Last Modified: Thu, 23 Jun 2022 01:05:54 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:ccdedcdf7a13cb6ecc4921006cf8e2e9b8f9e2cfbe7ccb04106368c2462fa426
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60456724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdbcbee07e5932907088936b99acefe742302fa27dadd8a2ebb44666f34ed58b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 01:05:38 GMT
ADD file:fc42adb3b30bf8dda0909ae6f3c3754d78c642e1a1d739bedf21934b7e7da3dd in / 
# Thu, 23 Jun 2022 01:05:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 02:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 02:28:19 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Thu, 23 Jun 2022 02:28:39 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 02:28:40 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 02:28:40 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 02:28:41 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 02:28:41 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 02:28:42 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 02:28:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 02:28:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a259ad5a4933979a4df4eb948f8761dde9b9f3d710259da588afee9fa00f1fef`  
		Last Modified: Thu, 23 Jun 2022 01:22:42 GMT  
		Size: 19.4 MB (19359846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0f7a736acf205407547109d49c141be814413fe2e704f167f154beb4a64bf8`  
		Last Modified: Thu, 23 Jun 2022 02:29:36 GMT  
		Size: 5.8 MB (5781003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec49c5d35def6ec8c590f209f60abf43ea871d2d35302760bbb0357a98f43b26`  
		Last Modified: Thu, 23 Jun 2022 02:31:18 GMT  
		Size: 35.3 MB (35291489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f657baa3f44759dd9b58b6460a04ffd0dc57bc7278218447b9de83ccd7d023`  
		Last Modified: Thu, 23 Jun 2022 02:30:59 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8dbc5d31121e03f9d916e8276728d4a02d649e1e57746561430adcb65350008`  
		Last Modified: Thu, 23 Jun 2022 02:30:59 GMT  
		Size: 11.9 KB (11902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0086f50118a0d8b418649e9fd989d5eb5c94e7c14506b6980ca0ba840a75c1`  
		Last Modified: Thu, 23 Jun 2022 02:30:59 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:d5dfa6b4fc06d5183c2fffc72832fe0aeadecb2fac2a02adb08592f924fe47d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61669706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6515bd8a31c397aec3531e07859da02f7b6e487896be7f6c2e0af789d214eaf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jun 2022 00:42:59 GMT
ADD file:c1bdac846ff41ceb56a44de5da778cfb7c3db7ccf4d689b7c1c22c0b80381c49 in / 
# Thu, 23 Jun 2022 00:42:59 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:27:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 01:28:32 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Thu, 23 Jun 2022 01:28:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 01:28:42 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Jun 2022 01:28:43 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Jun 2022 01:28:43 GMT
EXPOSE 8888
# Thu, 23 Jun 2022 01:28:44 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Jun 2022 01:28:46 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Jun 2022 01:28:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 01:28:47 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:45f14b91a40fe8177f16f6b6526ada782d0d63a7958757d4e07c543e574ea7a8`  
		Last Modified: Thu, 23 Jun 2022 00:51:46 GMT  
		Size: 20.4 MB (20423990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba5c15f7bd5dfe32b1718aade52f008519a7ffa497114d413766119a3dbd4f8`  
		Last Modified: Thu, 23 Jun 2022 01:29:14 GMT  
		Size: 6.0 MB (6047312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35008848465d6270ff38da08a7514053d62632985429e2326581b33946d6761b`  
		Last Modified: Thu, 23 Jun 2022 01:30:04 GMT  
		Size: 35.2 MB (35174017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75069e610add6e199c1abfd85f6596a3f7e15bc912230ddb1e0cdab0b41d71d`  
		Last Modified: Thu, 23 Jun 2022 01:29:59 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cdbd4a0e6503bdb63b1ce28ad92eeb99798ed8df1d1cf91cf4b53eabb8b192`  
		Last Modified: Thu, 23 Jun 2022 01:29:59 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6cb9709f043f81dc4d6f60f562a1d82615eb06ff08d1d6ed5544c34ad0fea3`  
		Last Modified: Thu, 23 Jun 2022 01:29:59 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
