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
-	[`chronograf:1.8.9`](#chronograf189)
-	[`chronograf:1.8.9-alpine`](#chronograf189-alpine)
-	[`chronograf:alpine`](#chronografalpine)
-	[`chronograf:latest`](#chronograflatest)

## `chronograf:1.6`

```console
$ docker pull chronograf@sha256:3290a7886028860931a6afb455544abdbd06abe67568278dfa6b8708b978a26f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6` - linux; amd64

```console
$ docker pull chronograf@sha256:b9a28ad04b89eba6fc7a7fc0b2f8977a04a2cd217bf66c47dadfd76e30caf36a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49357074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bb4c08628bb4f54c66f6d09dbccb16bcbcf759fad51f8d8b811eb5c7c9c734b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:17 GMT
ADD file:55a25b93e8f2940a796f3cbf1e78bddf5f49c46b1b89b63b9b5673cbed9483ca in / 
# Thu, 22 Jul 2021 00:47:17 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:24:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 22 Jul 2021 01:24:09 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Thu, 22 Jul 2021 01:24:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 01:24:17 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 22 Jul 2021 01:24:17 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 22 Jul 2021 01:24:17 GMT
EXPOSE 8888
# Thu, 22 Jul 2021 01:24:17 GMT
VOLUME [/var/lib/chronograf]
# Thu, 22 Jul 2021 01:24:18 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 22 Jul 2021 01:24:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jul 2021 01:24:18 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:778066204fb734c2fb80cb8127cb35d67d742806a4eaf1aba0b5393c4ae6f2a4`  
		Last Modified: Thu, 22 Jul 2021 00:53:22 GMT  
		Size: 22.5 MB (22527428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ff0af07da1ef7cf177b743e7ad0a7624265bf35374bcd2570af99c1be4eea9`  
		Last Modified: Thu, 22 Jul 2021 01:25:27 GMT  
		Size: 6.8 MB (6760219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f26b17e6da793ff8da6f077c69557203f88fe77ecc7042e8e2918d18554ebd`  
		Last Modified: Thu, 22 Jul 2021 01:25:30 GMT  
		Size: 20.0 MB (20045037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7cc06c5d3c492373713f56a60d75c1eae4eac3a8545069df1425737bbbbe7b`  
		Last Modified: Thu, 22 Jul 2021 01:25:26 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68abf45cb5ee116aea013f36d6cd0cb9e6ea531acb41876612911a02769043c8`  
		Last Modified: Thu, 22 Jul 2021 01:25:26 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a255c248d9b5e418f5bcd58db1fdbf5f1b639b6723448990cbf670097a862edf`  
		Last Modified: Thu, 22 Jul 2021 01:25:26 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:937f347d13b519066ca1ae2249c195c1299fc329a9ba8709436fb43e2ff81974
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43940050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ed3e4e95860aad998ffa6095b118d4bcbe0933cc2c4c3b8879bb0a481d744a3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 02:07:27 GMT
ADD file:86bd875241ca751f2f50a9c3504cfca4ce772411fed23fe6893299a271c275e3 in / 
# Thu, 22 Jul 2021 02:07:28 GMT
CMD ["bash"]
# Tue, 10 Aug 2021 23:00:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 10 Aug 2021 23:00:20 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 10 Aug 2021 23:00:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 10 Aug 2021 23:00:39 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 10 Aug 2021 23:00:39 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 10 Aug 2021 23:00:40 GMT
EXPOSE 8888
# Tue, 10 Aug 2021 23:00:40 GMT
VOLUME [/var/lib/chronograf]
# Tue, 10 Aug 2021 23:00:41 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 10 Aug 2021 23:00:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Aug 2021 23:00:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:37325b08023150a9e16c0c8d98d10daa998ce21ec3b9226cc6f0148a245a8a57`  
		Last Modified: Thu, 22 Jul 2021 02:21:16 GMT  
		Size: 19.3 MB (19315955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84236a4145013894eb753d54367ba39e700f41448379d11fb8acf79e2100e630`  
		Last Modified: Tue, 10 Aug 2021 23:03:14 GMT  
		Size: 5.8 MB (5779562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a1dc89d74b7c5071acf919f530b85ed228e090e9cdccc9afea8caf0f30200f`  
		Last Modified: Tue, 10 Aug 2021 23:03:25 GMT  
		Size: 18.8 MB (18820143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99343d22bd6913d879353af2a2174afdea899e9dc0a06db34b78037c0ddccd45`  
		Last Modified: Tue, 10 Aug 2021 23:03:11 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ead756033b31ea26f45491b0a1053f06560360ab82603e4c36052a0a6cdd076`  
		Last Modified: Tue, 10 Aug 2021 23:03:12 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f774ca5cc026dd5d49d1d4894048be0935c16ddb91e0bed0fa054c7d2f4e317`  
		Last Modified: Tue, 10 Aug 2021 23:03:12 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:afa0840b17f84a700c0deb52cb501377580e19c35dff926b5fd39e793e2e7212
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45422986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef285484a7ffd8e6a5a9e4402ed62feddef421d98005777802a6b794a02c33b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:40 GMT
ADD file:b39a01b3af7a531df3592571b7f6eaa7efd20919858f7f0cd2ddf1c1eceb078d in / 
# Thu, 22 Jul 2021 00:41:40 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:11:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 22 Jul 2021 01:11:45 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Thu, 22 Jul 2021 01:11:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 01:11:52 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 22 Jul 2021 01:11:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 22 Jul 2021 01:11:53 GMT
EXPOSE 8888
# Thu, 22 Jul 2021 01:11:53 GMT
VOLUME [/var/lib/chronograf]
# Thu, 22 Jul 2021 01:11:53 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 22 Jul 2021 01:11:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jul 2021 01:11:53 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9e7a560784c85cb9624bff5b6e479fbb95d5e265873987014f8aec75d509a530`  
		Last Modified: Thu, 22 Jul 2021 00:48:50 GMT  
		Size: 20.4 MB (20389427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58364f3e37bf6b8fd81d518b8f7e5a5c8b7e7ac6f79faf0c99101ffcef189204`  
		Last Modified: Thu, 22 Jul 2021 01:12:56 GMT  
		Size: 6.0 MB (6047477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34735440a1709a73691c1c574ac41c981fa36b3b95d3b2bba5cf49fa7868d1f`  
		Last Modified: Thu, 22 Jul 2021 01:12:58 GMT  
		Size: 19.0 MB (18961699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc731438f8ce8524d8b69426f1334bba5456c937316755b4406e99aac85bc8c`  
		Last Modified: Thu, 22 Jul 2021 01:12:55 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19d64e854a5d99474e0d5416fcfd7b67f69fa0cb037fbe64639c799774d162f`  
		Last Modified: Thu, 22 Jul 2021 01:12:55 GMT  
		Size: 11.9 KB (11900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2c77130bfd89d37c59e03ad8a63d38b68d3b61b93bfb4fe5a791d69b235356`  
		Last Modified: Thu, 22 Jul 2021 01:12:55 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6-alpine`

```console
$ docker pull chronograf@sha256:96255563a0f40d99b020410ebe817af3bfd5d8cf6bdde976cbb99129a6f6d652
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.6-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:7882fe897350c28398fa7147fc558a59d0e5d6cd57fb7fce6fa5c6ec734ca121
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14842739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dd57435798267753c1c67ff5ab33958f8504bf1fb341f30d6f9447ccb4c45fb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:12:40 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 14 Apr 2021 20:12:40 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 14 Apr 2021 20:12:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 20:12:45 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Wed, 14 Apr 2021 20:12:45 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 14 Apr 2021 20:12:45 GMT
EXPOSE 8888
# Wed, 14 Apr 2021 20:12:45 GMT
VOLUME [/var/lib/chronograf]
# Wed, 14 Apr 2021 20:12:46 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 14 Apr 2021 20:12:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 20:12:46 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9162e7666a3906b38fdfed2592cc2e4df967e365a3fcf17c8d6320caed7fd960`  
		Last Modified: Wed, 14 Apr 2021 20:13:33 GMT  
		Size: 280.9 KB (280875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4bc3cd9677b698574efa7718020ef698ba2fb4cf0c14e6b0ba97c34d32ce38`  
		Last Modified: Wed, 14 Apr 2021 20:13:35 GMT  
		Size: 11.7 MB (11736738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f050b1c3c0b5b5196a500b823d74fc3c18ea97d495b27d4869d652380b38af`  
		Last Modified: Wed, 14 Apr 2021 20:13:33 GMT  
		Size: 12.3 KB (12269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46702cb5f5ea894d168f763b18f46e526d677c70a6a672c8f6788cccd454d623`  
		Last Modified: Wed, 14 Apr 2021 20:13:33 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b426d5459c453e17fafb96f0187741ab25d8af8d5455df2a731ecebaf2b6b0c8`  
		Last Modified: Wed, 14 Apr 2021 20:13:33 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2`

```console
$ docker pull chronograf@sha256:3290a7886028860931a6afb455544abdbd06abe67568278dfa6b8708b978a26f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6.2` - linux; amd64

```console
$ docker pull chronograf@sha256:b9a28ad04b89eba6fc7a7fc0b2f8977a04a2cd217bf66c47dadfd76e30caf36a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49357074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bb4c08628bb4f54c66f6d09dbccb16bcbcf759fad51f8d8b811eb5c7c9c734b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:17 GMT
ADD file:55a25b93e8f2940a796f3cbf1e78bddf5f49c46b1b89b63b9b5673cbed9483ca in / 
# Thu, 22 Jul 2021 00:47:17 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:24:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 22 Jul 2021 01:24:09 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Thu, 22 Jul 2021 01:24:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 01:24:17 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 22 Jul 2021 01:24:17 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 22 Jul 2021 01:24:17 GMT
EXPOSE 8888
# Thu, 22 Jul 2021 01:24:17 GMT
VOLUME [/var/lib/chronograf]
# Thu, 22 Jul 2021 01:24:18 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 22 Jul 2021 01:24:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jul 2021 01:24:18 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:778066204fb734c2fb80cb8127cb35d67d742806a4eaf1aba0b5393c4ae6f2a4`  
		Last Modified: Thu, 22 Jul 2021 00:53:22 GMT  
		Size: 22.5 MB (22527428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ff0af07da1ef7cf177b743e7ad0a7624265bf35374bcd2570af99c1be4eea9`  
		Last Modified: Thu, 22 Jul 2021 01:25:27 GMT  
		Size: 6.8 MB (6760219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f26b17e6da793ff8da6f077c69557203f88fe77ecc7042e8e2918d18554ebd`  
		Last Modified: Thu, 22 Jul 2021 01:25:30 GMT  
		Size: 20.0 MB (20045037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7cc06c5d3c492373713f56a60d75c1eae4eac3a8545069df1425737bbbbe7b`  
		Last Modified: Thu, 22 Jul 2021 01:25:26 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68abf45cb5ee116aea013f36d6cd0cb9e6ea531acb41876612911a02769043c8`  
		Last Modified: Thu, 22 Jul 2021 01:25:26 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a255c248d9b5e418f5bcd58db1fdbf5f1b639b6723448990cbf670097a862edf`  
		Last Modified: Thu, 22 Jul 2021 01:25:26 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:937f347d13b519066ca1ae2249c195c1299fc329a9ba8709436fb43e2ff81974
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43940050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ed3e4e95860aad998ffa6095b118d4bcbe0933cc2c4c3b8879bb0a481d744a3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 02:07:27 GMT
ADD file:86bd875241ca751f2f50a9c3504cfca4ce772411fed23fe6893299a271c275e3 in / 
# Thu, 22 Jul 2021 02:07:28 GMT
CMD ["bash"]
# Tue, 10 Aug 2021 23:00:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 10 Aug 2021 23:00:20 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 10 Aug 2021 23:00:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 10 Aug 2021 23:00:39 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 10 Aug 2021 23:00:39 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 10 Aug 2021 23:00:40 GMT
EXPOSE 8888
# Tue, 10 Aug 2021 23:00:40 GMT
VOLUME [/var/lib/chronograf]
# Tue, 10 Aug 2021 23:00:41 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 10 Aug 2021 23:00:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Aug 2021 23:00:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:37325b08023150a9e16c0c8d98d10daa998ce21ec3b9226cc6f0148a245a8a57`  
		Last Modified: Thu, 22 Jul 2021 02:21:16 GMT  
		Size: 19.3 MB (19315955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84236a4145013894eb753d54367ba39e700f41448379d11fb8acf79e2100e630`  
		Last Modified: Tue, 10 Aug 2021 23:03:14 GMT  
		Size: 5.8 MB (5779562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a1dc89d74b7c5071acf919f530b85ed228e090e9cdccc9afea8caf0f30200f`  
		Last Modified: Tue, 10 Aug 2021 23:03:25 GMT  
		Size: 18.8 MB (18820143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99343d22bd6913d879353af2a2174afdea899e9dc0a06db34b78037c0ddccd45`  
		Last Modified: Tue, 10 Aug 2021 23:03:11 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ead756033b31ea26f45491b0a1053f06560360ab82603e4c36052a0a6cdd076`  
		Last Modified: Tue, 10 Aug 2021 23:03:12 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f774ca5cc026dd5d49d1d4894048be0935c16ddb91e0bed0fa054c7d2f4e317`  
		Last Modified: Tue, 10 Aug 2021 23:03:12 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:afa0840b17f84a700c0deb52cb501377580e19c35dff926b5fd39e793e2e7212
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45422986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef285484a7ffd8e6a5a9e4402ed62feddef421d98005777802a6b794a02c33b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:40 GMT
ADD file:b39a01b3af7a531df3592571b7f6eaa7efd20919858f7f0cd2ddf1c1eceb078d in / 
# Thu, 22 Jul 2021 00:41:40 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:11:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 22 Jul 2021 01:11:45 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Thu, 22 Jul 2021 01:11:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 01:11:52 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 22 Jul 2021 01:11:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 22 Jul 2021 01:11:53 GMT
EXPOSE 8888
# Thu, 22 Jul 2021 01:11:53 GMT
VOLUME [/var/lib/chronograf]
# Thu, 22 Jul 2021 01:11:53 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 22 Jul 2021 01:11:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jul 2021 01:11:53 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9e7a560784c85cb9624bff5b6e479fbb95d5e265873987014f8aec75d509a530`  
		Last Modified: Thu, 22 Jul 2021 00:48:50 GMT  
		Size: 20.4 MB (20389427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58364f3e37bf6b8fd81d518b8f7e5a5c8b7e7ac6f79faf0c99101ffcef189204`  
		Last Modified: Thu, 22 Jul 2021 01:12:56 GMT  
		Size: 6.0 MB (6047477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34735440a1709a73691c1c574ac41c981fa36b3b95d3b2bba5cf49fa7868d1f`  
		Last Modified: Thu, 22 Jul 2021 01:12:58 GMT  
		Size: 19.0 MB (18961699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc731438f8ce8524d8b69426f1334bba5456c937316755b4406e99aac85bc8c`  
		Last Modified: Thu, 22 Jul 2021 01:12:55 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19d64e854a5d99474e0d5416fcfd7b67f69fa0cb037fbe64639c799774d162f`  
		Last Modified: Thu, 22 Jul 2021 01:12:55 GMT  
		Size: 11.9 KB (11900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2c77130bfd89d37c59e03ad8a63d38b68d3b61b93bfb4fe5a791d69b235356`  
		Last Modified: Thu, 22 Jul 2021 01:12:55 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2-alpine`

```console
$ docker pull chronograf@sha256:96255563a0f40d99b020410ebe817af3bfd5d8cf6bdde976cbb99129a6f6d652
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.6.2-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:7882fe897350c28398fa7147fc558a59d0e5d6cd57fb7fce6fa5c6ec734ca121
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14842739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dd57435798267753c1c67ff5ab33958f8504bf1fb341f30d6f9447ccb4c45fb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:12:40 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 14 Apr 2021 20:12:40 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 14 Apr 2021 20:12:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 20:12:45 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Wed, 14 Apr 2021 20:12:45 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 14 Apr 2021 20:12:45 GMT
EXPOSE 8888
# Wed, 14 Apr 2021 20:12:45 GMT
VOLUME [/var/lib/chronograf]
# Wed, 14 Apr 2021 20:12:46 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 14 Apr 2021 20:12:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 20:12:46 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9162e7666a3906b38fdfed2592cc2e4df967e365a3fcf17c8d6320caed7fd960`  
		Last Modified: Wed, 14 Apr 2021 20:13:33 GMT  
		Size: 280.9 KB (280875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4bc3cd9677b698574efa7718020ef698ba2fb4cf0c14e6b0ba97c34d32ce38`  
		Last Modified: Wed, 14 Apr 2021 20:13:35 GMT  
		Size: 11.7 MB (11736738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f050b1c3c0b5b5196a500b823d74fc3c18ea97d495b27d4869d652380b38af`  
		Last Modified: Wed, 14 Apr 2021 20:13:33 GMT  
		Size: 12.3 KB (12269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46702cb5f5ea894d168f763b18f46e526d677c70a6a672c8f6788cccd454d623`  
		Last Modified: Wed, 14 Apr 2021 20:13:33 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b426d5459c453e17fafb96f0187741ab25d8af8d5455df2a731ecebaf2b6b0c8`  
		Last Modified: Wed, 14 Apr 2021 20:13:33 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7`

```console
$ docker pull chronograf@sha256:dacc73a23295385e695210de4710b45a8a4c2e9215fd96635dd60adff840d82d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7` - linux; amd64

```console
$ docker pull chronograf@sha256:f07b93ede6a49cf298713ec9dca2c0322b3860b8f15e4ec4c1597f7781e0d933
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65385719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b290d786e3b64aee3327b5d428870b0c402d44262232aa2f78a537f562ccac1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:17 GMT
ADD file:55a25b93e8f2940a796f3cbf1e78bddf5f49c46b1b89b63b9b5673cbed9483ca in / 
# Thu, 22 Jul 2021 00:47:17 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:24:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 22 Jul 2021 01:24:33 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 22 Jul 2021 01:24:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 01:24:44 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 22 Jul 2021 01:24:45 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 22 Jul 2021 01:24:45 GMT
EXPOSE 8888
# Thu, 22 Jul 2021 01:24:45 GMT
VOLUME [/var/lib/chronograf]
# Thu, 22 Jul 2021 01:24:45 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 22 Jul 2021 01:24:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jul 2021 01:24:46 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:778066204fb734c2fb80cb8127cb35d67d742806a4eaf1aba0b5393c4ae6f2a4`  
		Last Modified: Thu, 22 Jul 2021 00:53:22 GMT  
		Size: 22.5 MB (22527428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af046676142b8cb38f06f16544407e732c72ccb1c7f61dfd528ffa48bcb515f8`  
		Last Modified: Thu, 22 Jul 2021 01:25:42 GMT  
		Size: 4.5 MB (4506056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547bd60780ecc304a0d507bb744d0511bb46f343bbd1c08b0fa36411794a7f55`  
		Last Modified: Thu, 22 Jul 2021 01:25:47 GMT  
		Size: 38.3 MB (38327856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36734290af47c9748907e5573610cfb215df4f03bf3314f6ce99240b246ad58a`  
		Last Modified: Thu, 22 Jul 2021 01:25:42 GMT  
		Size: 12.2 KB (12238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b150b43be4bc8353e2064d76ca9f39dd114cbf639c9330f8ba8566a33a9f967`  
		Last Modified: Thu, 22 Jul 2021 01:25:41 GMT  
		Size: 11.9 KB (11902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e94b39fe315a6b08dbb3f1e100273a11051ece6da5e4896e1b6833d60eb979`  
		Last Modified: Thu, 22 Jul 2021 01:25:41 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:1d6a2a47d1a53e5add56f3a4f85656b5bb195938af16da1267302f76d0a01c2c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (59002287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea4a884bbcf9a9acedb85ede6e9d279c7f056db4f991ce6eb96da82f1583cfdf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 02:07:27 GMT
ADD file:86bd875241ca751f2f50a9c3504cfca4ce772411fed23fe6893299a271c275e3 in / 
# Thu, 22 Jul 2021 02:07:28 GMT
CMD ["bash"]
# Tue, 10 Aug 2021 23:01:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 10 Aug 2021 23:01:12 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 10 Aug 2021 23:01:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 10 Aug 2021 23:01:48 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 10 Aug 2021 23:01:48 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 10 Aug 2021 23:01:49 GMT
EXPOSE 8888
# Tue, 10 Aug 2021 23:01:49 GMT
VOLUME [/var/lib/chronograf]
# Tue, 10 Aug 2021 23:01:50 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 10 Aug 2021 23:01:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Aug 2021 23:01:51 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:37325b08023150a9e16c0c8d98d10daa998ce21ec3b9226cc6f0148a245a8a57`  
		Last Modified: Thu, 22 Jul 2021 02:21:16 GMT  
		Size: 19.3 MB (19315955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed63205ee5bbe64765ff2ec58aad56001ae3eb0d545702e6c05108dd001961bf`  
		Last Modified: Tue, 10 Aug 2021 23:03:39 GMT  
		Size: 3.9 MB (3879523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdd12b4164662e89f773859a94b34fd08b538d249f2bd05dccda3f989e69ac4`  
		Last Modified: Tue, 10 Aug 2021 23:03:57 GMT  
		Size: 35.8 MB (35782417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b74f5599148ea9c1fd6af2a42de0465c64fc60e12be00b443792137b69e7801`  
		Last Modified: Tue, 10 Aug 2021 23:03:37 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9c1c0540b45b54cfb793cc3bbfc8443ba363ffd2c0d5d009e3cc346566b622`  
		Last Modified: Tue, 10 Aug 2021 23:03:37 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a09074b078251844942abc895a5007d7db5ebcec7036ed6b056e0a636212f5a`  
		Last Modified: Tue, 10 Aug 2021 23:03:37 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:4dbb76305faec27c609871c2f96a39a0ae9298340777afa6aaf6167e1ea51a51
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60481706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e4defb43f22947064bfb2173c71904b0642253b9155c2ad5f5fab9e692fb3d1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:40 GMT
ADD file:b39a01b3af7a531df3592571b7f6eaa7efd20919858f7f0cd2ddf1c1eceb078d in / 
# Thu, 22 Jul 2021 00:41:40 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:07 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 22 Jul 2021 01:12:07 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 22 Jul 2021 01:12:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 01:12:17 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 22 Jul 2021 01:12:17 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 22 Jul 2021 01:12:17 GMT
EXPOSE 8888
# Thu, 22 Jul 2021 01:12:17 GMT
VOLUME [/var/lib/chronograf]
# Thu, 22 Jul 2021 01:12:18 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 22 Jul 2021 01:12:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jul 2021 01:12:18 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9e7a560784c85cb9624bff5b6e479fbb95d5e265873987014f8aec75d509a530`  
		Last Modified: Thu, 22 Jul 2021 00:48:50 GMT  
		Size: 20.4 MB (20389427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84d271af61d403095e160eaa7a08c7145947112444ea42d8e236650e8aa845f`  
		Last Modified: Thu, 22 Jul 2021 01:13:14 GMT  
		Size: 4.1 MB (4082168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672d4e6c5320fcd575044df66639ac14555c933eecaae0d0a52abfb702c90fa6`  
		Last Modified: Thu, 22 Jul 2021 01:13:18 GMT  
		Size: 36.0 MB (35985725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3e588a82833a04c0b6a45c8910a33f1d4b09dd115ecdf4c25c0321b3f78cdd`  
		Last Modified: Thu, 22 Jul 2021 01:13:13 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0a76bc763944f38422c274fcb2760c3a6c186d9ce465f35d5cdbb3590a8a72`  
		Last Modified: Thu, 22 Jul 2021 01:13:13 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0bdd9d30749d198987730ca6cc4401f09eb37887c287fc412038ad17cfe03a`  
		Last Modified: Thu, 22 Jul 2021 01:13:14 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7-alpine`

```console
$ docker pull chronograf@sha256:2a506b16f05ed98563f442490f072e41c2c728b3bc2b22af0ff1ed102ce4f847
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.7-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:76887aca3d47afe98e527aa93ff1987f915add234c37a5bc4fd04a9966d0c408
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22661245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2499d4b53fa9ffbb4438cd1c565ae78d7bcddcafc81006370d72472c67bf550`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:12:40 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 14 Apr 2021 20:12:52 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 14 Apr 2021 20:12:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 20:12:57 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 14 Apr 2021 20:12:57 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 14 Apr 2021 20:12:57 GMT
EXPOSE 8888
# Wed, 14 Apr 2021 20:12:57 GMT
VOLUME [/var/lib/chronograf]
# Wed, 14 Apr 2021 20:12:58 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 14 Apr 2021 20:12:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 20:12:58 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9162e7666a3906b38fdfed2592cc2e4df967e365a3fcf17c8d6320caed7fd960`  
		Last Modified: Wed, 14 Apr 2021 20:13:33 GMT  
		Size: 280.9 KB (280875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f4b124c6a1aaaba55eb52f4a702a3971446fc3c69d0ec8dc0c709c3aeb0b74`  
		Last Modified: Wed, 14 Apr 2021 20:13:53 GMT  
		Size: 19.6 MB (19555245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f14586d69b49961d9119ce5688addaa07197accd543400d095567b621d98a1`  
		Last Modified: Wed, 14 Apr 2021 20:13:49 GMT  
		Size: 12.3 KB (12267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e58bc88a957e5e32c8aea21d2f8e9602ff838e51f4efe63621be77fd73ea659`  
		Last Modified: Wed, 14 Apr 2021 20:13:49 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0271a6755ddede52dd80e1a68a5fbdf1a42276d30efd901cfd04ec0ebf5d92`  
		Last Modified: Wed, 14 Apr 2021 20:13:49 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17`

```console
$ docker pull chronograf@sha256:dacc73a23295385e695210de4710b45a8a4c2e9215fd96635dd60adff840d82d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7.17` - linux; amd64

```console
$ docker pull chronograf@sha256:f07b93ede6a49cf298713ec9dca2c0322b3860b8f15e4ec4c1597f7781e0d933
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65385719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b290d786e3b64aee3327b5d428870b0c402d44262232aa2f78a537f562ccac1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:17 GMT
ADD file:55a25b93e8f2940a796f3cbf1e78bddf5f49c46b1b89b63b9b5673cbed9483ca in / 
# Thu, 22 Jul 2021 00:47:17 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:24:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 22 Jul 2021 01:24:33 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 22 Jul 2021 01:24:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 01:24:44 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 22 Jul 2021 01:24:45 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 22 Jul 2021 01:24:45 GMT
EXPOSE 8888
# Thu, 22 Jul 2021 01:24:45 GMT
VOLUME [/var/lib/chronograf]
# Thu, 22 Jul 2021 01:24:45 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 22 Jul 2021 01:24:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jul 2021 01:24:46 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:778066204fb734c2fb80cb8127cb35d67d742806a4eaf1aba0b5393c4ae6f2a4`  
		Last Modified: Thu, 22 Jul 2021 00:53:22 GMT  
		Size: 22.5 MB (22527428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af046676142b8cb38f06f16544407e732c72ccb1c7f61dfd528ffa48bcb515f8`  
		Last Modified: Thu, 22 Jul 2021 01:25:42 GMT  
		Size: 4.5 MB (4506056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547bd60780ecc304a0d507bb744d0511bb46f343bbd1c08b0fa36411794a7f55`  
		Last Modified: Thu, 22 Jul 2021 01:25:47 GMT  
		Size: 38.3 MB (38327856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36734290af47c9748907e5573610cfb215df4f03bf3314f6ce99240b246ad58a`  
		Last Modified: Thu, 22 Jul 2021 01:25:42 GMT  
		Size: 12.2 KB (12238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b150b43be4bc8353e2064d76ca9f39dd114cbf639c9330f8ba8566a33a9f967`  
		Last Modified: Thu, 22 Jul 2021 01:25:41 GMT  
		Size: 11.9 KB (11902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e94b39fe315a6b08dbb3f1e100273a11051ece6da5e4896e1b6833d60eb979`  
		Last Modified: Thu, 22 Jul 2021 01:25:41 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:1d6a2a47d1a53e5add56f3a4f85656b5bb195938af16da1267302f76d0a01c2c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (59002287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea4a884bbcf9a9acedb85ede6e9d279c7f056db4f991ce6eb96da82f1583cfdf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 02:07:27 GMT
ADD file:86bd875241ca751f2f50a9c3504cfca4ce772411fed23fe6893299a271c275e3 in / 
# Thu, 22 Jul 2021 02:07:28 GMT
CMD ["bash"]
# Tue, 10 Aug 2021 23:01:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 10 Aug 2021 23:01:12 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 10 Aug 2021 23:01:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 10 Aug 2021 23:01:48 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 10 Aug 2021 23:01:48 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 10 Aug 2021 23:01:49 GMT
EXPOSE 8888
# Tue, 10 Aug 2021 23:01:49 GMT
VOLUME [/var/lib/chronograf]
# Tue, 10 Aug 2021 23:01:50 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 10 Aug 2021 23:01:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Aug 2021 23:01:51 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:37325b08023150a9e16c0c8d98d10daa998ce21ec3b9226cc6f0148a245a8a57`  
		Last Modified: Thu, 22 Jul 2021 02:21:16 GMT  
		Size: 19.3 MB (19315955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed63205ee5bbe64765ff2ec58aad56001ae3eb0d545702e6c05108dd001961bf`  
		Last Modified: Tue, 10 Aug 2021 23:03:39 GMT  
		Size: 3.9 MB (3879523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdd12b4164662e89f773859a94b34fd08b538d249f2bd05dccda3f989e69ac4`  
		Last Modified: Tue, 10 Aug 2021 23:03:57 GMT  
		Size: 35.8 MB (35782417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b74f5599148ea9c1fd6af2a42de0465c64fc60e12be00b443792137b69e7801`  
		Last Modified: Tue, 10 Aug 2021 23:03:37 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9c1c0540b45b54cfb793cc3bbfc8443ba363ffd2c0d5d009e3cc346566b622`  
		Last Modified: Tue, 10 Aug 2021 23:03:37 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a09074b078251844942abc895a5007d7db5ebcec7036ed6b056e0a636212f5a`  
		Last Modified: Tue, 10 Aug 2021 23:03:37 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:4dbb76305faec27c609871c2f96a39a0ae9298340777afa6aaf6167e1ea51a51
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60481706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e4defb43f22947064bfb2173c71904b0642253b9155c2ad5f5fab9e692fb3d1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:40 GMT
ADD file:b39a01b3af7a531df3592571b7f6eaa7efd20919858f7f0cd2ddf1c1eceb078d in / 
# Thu, 22 Jul 2021 00:41:40 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:07 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 22 Jul 2021 01:12:07 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 22 Jul 2021 01:12:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 01:12:17 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 22 Jul 2021 01:12:17 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 22 Jul 2021 01:12:17 GMT
EXPOSE 8888
# Thu, 22 Jul 2021 01:12:17 GMT
VOLUME [/var/lib/chronograf]
# Thu, 22 Jul 2021 01:12:18 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 22 Jul 2021 01:12:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jul 2021 01:12:18 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9e7a560784c85cb9624bff5b6e479fbb95d5e265873987014f8aec75d509a530`  
		Last Modified: Thu, 22 Jul 2021 00:48:50 GMT  
		Size: 20.4 MB (20389427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84d271af61d403095e160eaa7a08c7145947112444ea42d8e236650e8aa845f`  
		Last Modified: Thu, 22 Jul 2021 01:13:14 GMT  
		Size: 4.1 MB (4082168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672d4e6c5320fcd575044df66639ac14555c933eecaae0d0a52abfb702c90fa6`  
		Last Modified: Thu, 22 Jul 2021 01:13:18 GMT  
		Size: 36.0 MB (35985725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3e588a82833a04c0b6a45c8910a33f1d4b09dd115ecdf4c25c0321b3f78cdd`  
		Last Modified: Thu, 22 Jul 2021 01:13:13 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0a76bc763944f38422c274fcb2760c3a6c186d9ce465f35d5cdbb3590a8a72`  
		Last Modified: Thu, 22 Jul 2021 01:13:13 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0bdd9d30749d198987730ca6cc4401f09eb37887c287fc412038ad17cfe03a`  
		Last Modified: Thu, 22 Jul 2021 01:13:14 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17-alpine`

```console
$ docker pull chronograf@sha256:2a506b16f05ed98563f442490f072e41c2c728b3bc2b22af0ff1ed102ce4f847
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.7.17-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:76887aca3d47afe98e527aa93ff1987f915add234c37a5bc4fd04a9966d0c408
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22661245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2499d4b53fa9ffbb4438cd1c565ae78d7bcddcafc81006370d72472c67bf550`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:12:40 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 14 Apr 2021 20:12:52 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 14 Apr 2021 20:12:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 20:12:57 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 14 Apr 2021 20:12:57 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 14 Apr 2021 20:12:57 GMT
EXPOSE 8888
# Wed, 14 Apr 2021 20:12:57 GMT
VOLUME [/var/lib/chronograf]
# Wed, 14 Apr 2021 20:12:58 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 14 Apr 2021 20:12:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 20:12:58 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9162e7666a3906b38fdfed2592cc2e4df967e365a3fcf17c8d6320caed7fd960`  
		Last Modified: Wed, 14 Apr 2021 20:13:33 GMT  
		Size: 280.9 KB (280875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f4b124c6a1aaaba55eb52f4a702a3971446fc3c69d0ec8dc0c709c3aeb0b74`  
		Last Modified: Wed, 14 Apr 2021 20:13:53 GMT  
		Size: 19.6 MB (19555245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f14586d69b49961d9119ce5688addaa07197accd543400d095567b621d98a1`  
		Last Modified: Wed, 14 Apr 2021 20:13:49 GMT  
		Size: 12.3 KB (12267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e58bc88a957e5e32c8aea21d2f8e9602ff838e51f4efe63621be77fd73ea659`  
		Last Modified: Wed, 14 Apr 2021 20:13:49 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0271a6755ddede52dd80e1a68a5fbdf1a42276d30efd901cfd04ec0ebf5d92`  
		Last Modified: Wed, 14 Apr 2021 20:13:49 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8`

```console
$ docker pull chronograf@sha256:750ca1c63b4c3ef1acc99d4a2cf8320f78b19c653403c4f69ec3a3bc5e67ecb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8` - linux; amd64

```console
$ docker pull chronograf@sha256:dbc2c61a84e72db77fa9f2da381c0268db8dc74dbb6820b76d08b10b1988db1e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70443794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f07c735db5e077a7ae57f6216fec094bc3b975979ab304a059604dc5f145faf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:17 GMT
ADD file:55a25b93e8f2940a796f3cbf1e78bddf5f49c46b1b89b63b9b5673cbed9483ca in / 
# Thu, 22 Jul 2021 00:47:17 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:24:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 22 Jul 2021 01:24:53 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Thu, 22 Jul 2021 01:25:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 01:25:01 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 22 Jul 2021 01:25:02 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 22 Jul 2021 01:25:02 GMT
EXPOSE 8888
# Thu, 22 Jul 2021 01:25:02 GMT
VOLUME [/var/lib/chronograf]
# Thu, 22 Jul 2021 01:25:02 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 22 Jul 2021 01:25:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jul 2021 01:25:03 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:778066204fb734c2fb80cb8127cb35d67d742806a4eaf1aba0b5393c4ae6f2a4`  
		Last Modified: Thu, 22 Jul 2021 00:53:22 GMT  
		Size: 22.5 MB (22527428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ff0af07da1ef7cf177b743e7ad0a7624265bf35374bcd2570af99c1be4eea9`  
		Last Modified: Thu, 22 Jul 2021 01:25:27 GMT  
		Size: 6.8 MB (6760219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f0c0740080eb1beb0bafc38e6302c80ab58a56cd623d417c394b231d55d2a9`  
		Last Modified: Thu, 22 Jul 2021 01:26:04 GMT  
		Size: 41.1 MB (41131759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87cfa89e6cb17bd471dd756aad021cff94fe738e0b8908ebedaeb2496916554`  
		Last Modified: Thu, 22 Jul 2021 01:25:58 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bfeee62a671086588e9c04f66c454fb68ecee8c66dbe508743ef70e5974b66`  
		Last Modified: Thu, 22 Jul 2021 01:25:59 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d1ef1a0aa9a111a5fd29bfab71dae1eb2f860cdb6745adbca31962564a9d08`  
		Last Modified: Thu, 22 Jul 2021 01:25:58 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:aaa12f3421fbcc2da74abf990ee7e7515ef96f85710f3361d890a52991d3d8d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59617640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065f7eaeabb6ce83c6ac6cb1cfe4e40568460463aa8b45664a6797fbec021dee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 02:07:27 GMT
ADD file:86bd875241ca751f2f50a9c3504cfca4ce772411fed23fe6893299a271c275e3 in / 
# Thu, 22 Jul 2021 02:07:28 GMT
CMD ["bash"]
# Tue, 10 Aug 2021 23:00:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 10 Aug 2021 23:02:02 GMT
ENV CHRONOGRAF_VERSION=1.8.9
# Tue, 10 Aug 2021 23:02:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 10 Aug 2021 23:02:22 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 10 Aug 2021 23:02:23 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 10 Aug 2021 23:02:23 GMT
EXPOSE 8888
# Tue, 10 Aug 2021 23:02:24 GMT
VOLUME [/var/lib/chronograf]
# Tue, 10 Aug 2021 23:02:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 10 Aug 2021 23:02:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Aug 2021 23:02:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:37325b08023150a9e16c0c8d98d10daa998ce21ec3b9226cc6f0148a245a8a57`  
		Last Modified: Thu, 22 Jul 2021 02:21:16 GMT  
		Size: 19.3 MB (19315955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84236a4145013894eb753d54367ba39e700f41448379d11fb8acf79e2100e630`  
		Last Modified: Tue, 10 Aug 2021 23:03:14 GMT  
		Size: 5.8 MB (5779562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563aa1050ffeff783f5c0ace0c0d4c26bf42c55be8a64652b976ba2242844480`  
		Last Modified: Tue, 10 Aug 2021 23:04:29 GMT  
		Size: 34.5 MB (34497735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33390c7d3a170ef269b4e0664ab92012f5e8a0be393ea68452543bc3805dd86`  
		Last Modified: Tue, 10 Aug 2021 23:04:10 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63513570675210dbda0283a576386daa6c1305131230de9124c5a42c5b9ede1`  
		Last Modified: Tue, 10 Aug 2021 23:04:11 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001f573921c3e4fda4891864bdc68ad985bbec2316df915bf5b962fb9cc9cced`  
		Last Modified: Tue, 10 Aug 2021 23:04:10 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:f16a60124e199840257f215b25bf2347840a341f56c2b50eb6ccfb47740c6c47
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64970233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7e052aba53be0451400f0ec90d1cbd1cf089dfe6b31480453fcc5f21a74d8d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:40 GMT
ADD file:b39a01b3af7a531df3592571b7f6eaa7efd20919858f7f0cd2ddf1c1eceb078d in / 
# Thu, 22 Jul 2021 00:41:40 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:11:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 22 Jul 2021 01:12:23 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Thu, 22 Jul 2021 01:12:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 01:12:31 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 22 Jul 2021 01:12:31 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 22 Jul 2021 01:12:31 GMT
EXPOSE 8888
# Thu, 22 Jul 2021 01:12:31 GMT
VOLUME [/var/lib/chronograf]
# Thu, 22 Jul 2021 01:12:31 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 22 Jul 2021 01:12:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jul 2021 01:12:32 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9e7a560784c85cb9624bff5b6e479fbb95d5e265873987014f8aec75d509a530`  
		Last Modified: Thu, 22 Jul 2021 00:48:50 GMT  
		Size: 20.4 MB (20389427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58364f3e37bf6b8fd81d518b8f7e5a5c8b7e7ac6f79faf0c99101ffcef189204`  
		Last Modified: Thu, 22 Jul 2021 01:12:56 GMT  
		Size: 6.0 MB (6047477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4b587acd1b705f40e13a6f37bde0255703ed113b71c608ddd2f398cbe2f40e`  
		Last Modified: Thu, 22 Jul 2021 01:13:36 GMT  
		Size: 38.5 MB (38508940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2161d973333f7691e631e2063f505a6e800edf211cca030fd5cf083eeb62ed5`  
		Last Modified: Thu, 22 Jul 2021 01:13:30 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0bf9aa56a41dfc971d38fa9b8c9fdcacbe80ea7f7bed40138fc47a30072709`  
		Last Modified: Thu, 22 Jul 2021 01:13:30 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145897592d2b460b30d22c92b220ab150f0af94c742f79505897d3c5c386124d`  
		Last Modified: Thu, 22 Jul 2021 01:13:31 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8-alpine`

```console
$ docker pull chronograf@sha256:a5cbcfd2bfc1c933986ccca221a0d540377ce3c034476353415125e083ae5e38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:6a22d2aa10b70b8b5cde2994229c5c586e371e24f31d5180fd4e44814710d89a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25351611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8f8be3a981be5d1db8847952e656de841d06af31f8aaf6389ede18a35878a09`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:12:40 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 14 Apr 2021 20:13:04 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Wed, 14 Apr 2021 20:13:10 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 20:13:10 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 14 Apr 2021 20:13:10 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 14 Apr 2021 20:13:11 GMT
EXPOSE 8888
# Wed, 14 Apr 2021 20:13:11 GMT
VOLUME [/var/lib/chronograf]
# Wed, 14 Apr 2021 20:13:11 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 14 Apr 2021 20:13:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 20:13:11 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9162e7666a3906b38fdfed2592cc2e4df967e365a3fcf17c8d6320caed7fd960`  
		Last Modified: Wed, 14 Apr 2021 20:13:33 GMT  
		Size: 280.9 KB (280875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba38a1f02c9de9fb4aaffaca80c92ad2fecaabbf0afe54b81331fb3bab94e36`  
		Last Modified: Wed, 14 Apr 2021 20:14:10 GMT  
		Size: 22.2 MB (22245617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911ddedf41d4e2c1c792681fdb37a8cdc228aacce7bc520c0155a8abdef24867`  
		Last Modified: Wed, 14 Apr 2021 20:14:05 GMT  
		Size: 12.3 KB (12262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4896f07f3bdcc32cc856a2f9ef4169f64096b1b8566ae4d50983a9a3ad3d485`  
		Last Modified: Wed, 14 Apr 2021 20:14:05 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736cbd00b8d9ec9952f27cc06af1eff2a238e8d06ddff183157196dfc82cb962`  
		Last Modified: Wed, 14 Apr 2021 20:14:06 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.9`

```console
$ docker pull chronograf@sha256:0b1f595b21a65a23328e0a6391e2ce8ca5dbd219d3c0d1d2c73522bcf0d8b02e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v7

### `chronograf:1.8.9` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:aaa12f3421fbcc2da74abf990ee7e7515ef96f85710f3361d890a52991d3d8d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59617640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065f7eaeabb6ce83c6ac6cb1cfe4e40568460463aa8b45664a6797fbec021dee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 02:07:27 GMT
ADD file:86bd875241ca751f2f50a9c3504cfca4ce772411fed23fe6893299a271c275e3 in / 
# Thu, 22 Jul 2021 02:07:28 GMT
CMD ["bash"]
# Tue, 10 Aug 2021 23:00:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 10 Aug 2021 23:02:02 GMT
ENV CHRONOGRAF_VERSION=1.8.9
# Tue, 10 Aug 2021 23:02:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 10 Aug 2021 23:02:22 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 10 Aug 2021 23:02:23 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 10 Aug 2021 23:02:23 GMT
EXPOSE 8888
# Tue, 10 Aug 2021 23:02:24 GMT
VOLUME [/var/lib/chronograf]
# Tue, 10 Aug 2021 23:02:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 10 Aug 2021 23:02:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Aug 2021 23:02:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:37325b08023150a9e16c0c8d98d10daa998ce21ec3b9226cc6f0148a245a8a57`  
		Last Modified: Thu, 22 Jul 2021 02:21:16 GMT  
		Size: 19.3 MB (19315955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84236a4145013894eb753d54367ba39e700f41448379d11fb8acf79e2100e630`  
		Last Modified: Tue, 10 Aug 2021 23:03:14 GMT  
		Size: 5.8 MB (5779562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563aa1050ffeff783f5c0ace0c0d4c26bf42c55be8a64652b976ba2242844480`  
		Last Modified: Tue, 10 Aug 2021 23:04:29 GMT  
		Size: 34.5 MB (34497735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33390c7d3a170ef269b4e0664ab92012f5e8a0be393ea68452543bc3805dd86`  
		Last Modified: Tue, 10 Aug 2021 23:04:10 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63513570675210dbda0283a576386daa6c1305131230de9124c5a42c5b9ede1`  
		Last Modified: Tue, 10 Aug 2021 23:04:11 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001f573921c3e4fda4891864bdc68ad985bbec2316df915bf5b962fb9cc9cced`  
		Last Modified: Tue, 10 Aug 2021 23:04:10 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.9-alpine`

```console
$ docker pull chronograf@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `chronograf:alpine`

```console
$ docker pull chronograf@sha256:a5cbcfd2bfc1c933986ccca221a0d540377ce3c034476353415125e083ae5e38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:6a22d2aa10b70b8b5cde2994229c5c586e371e24f31d5180fd4e44814710d89a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25351611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8f8be3a981be5d1db8847952e656de841d06af31f8aaf6389ede18a35878a09`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:12:40 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 14 Apr 2021 20:13:04 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Wed, 14 Apr 2021 20:13:10 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 20:13:10 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 14 Apr 2021 20:13:10 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 14 Apr 2021 20:13:11 GMT
EXPOSE 8888
# Wed, 14 Apr 2021 20:13:11 GMT
VOLUME [/var/lib/chronograf]
# Wed, 14 Apr 2021 20:13:11 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 14 Apr 2021 20:13:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 20:13:11 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9162e7666a3906b38fdfed2592cc2e4df967e365a3fcf17c8d6320caed7fd960`  
		Last Modified: Wed, 14 Apr 2021 20:13:33 GMT  
		Size: 280.9 KB (280875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba38a1f02c9de9fb4aaffaca80c92ad2fecaabbf0afe54b81331fb3bab94e36`  
		Last Modified: Wed, 14 Apr 2021 20:14:10 GMT  
		Size: 22.2 MB (22245617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911ddedf41d4e2c1c792681fdb37a8cdc228aacce7bc520c0155a8abdef24867`  
		Last Modified: Wed, 14 Apr 2021 20:14:05 GMT  
		Size: 12.3 KB (12262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4896f07f3bdcc32cc856a2f9ef4169f64096b1b8566ae4d50983a9a3ad3d485`  
		Last Modified: Wed, 14 Apr 2021 20:14:05 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736cbd00b8d9ec9952f27cc06af1eff2a238e8d06ddff183157196dfc82cb962`  
		Last Modified: Wed, 14 Apr 2021 20:14:06 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:latest`

```console
$ docker pull chronograf@sha256:750ca1c63b4c3ef1acc99d4a2cf8320f78b19c653403c4f69ec3a3bc5e67ecb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:dbc2c61a84e72db77fa9f2da381c0268db8dc74dbb6820b76d08b10b1988db1e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70443794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f07c735db5e077a7ae57f6216fec094bc3b975979ab304a059604dc5f145faf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:17 GMT
ADD file:55a25b93e8f2940a796f3cbf1e78bddf5f49c46b1b89b63b9b5673cbed9483ca in / 
# Thu, 22 Jul 2021 00:47:17 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:24:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 22 Jul 2021 01:24:53 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Thu, 22 Jul 2021 01:25:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 01:25:01 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 22 Jul 2021 01:25:02 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 22 Jul 2021 01:25:02 GMT
EXPOSE 8888
# Thu, 22 Jul 2021 01:25:02 GMT
VOLUME [/var/lib/chronograf]
# Thu, 22 Jul 2021 01:25:02 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 22 Jul 2021 01:25:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jul 2021 01:25:03 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:778066204fb734c2fb80cb8127cb35d67d742806a4eaf1aba0b5393c4ae6f2a4`  
		Last Modified: Thu, 22 Jul 2021 00:53:22 GMT  
		Size: 22.5 MB (22527428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ff0af07da1ef7cf177b743e7ad0a7624265bf35374bcd2570af99c1be4eea9`  
		Last Modified: Thu, 22 Jul 2021 01:25:27 GMT  
		Size: 6.8 MB (6760219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f0c0740080eb1beb0bafc38e6302c80ab58a56cd623d417c394b231d55d2a9`  
		Last Modified: Thu, 22 Jul 2021 01:26:04 GMT  
		Size: 41.1 MB (41131759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87cfa89e6cb17bd471dd756aad021cff94fe738e0b8908ebedaeb2496916554`  
		Last Modified: Thu, 22 Jul 2021 01:25:58 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bfeee62a671086588e9c04f66c454fb68ecee8c66dbe508743ef70e5974b66`  
		Last Modified: Thu, 22 Jul 2021 01:25:59 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d1ef1a0aa9a111a5fd29bfab71dae1eb2f860cdb6745adbca31962564a9d08`  
		Last Modified: Thu, 22 Jul 2021 01:25:58 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:aaa12f3421fbcc2da74abf990ee7e7515ef96f85710f3361d890a52991d3d8d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59617640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065f7eaeabb6ce83c6ac6cb1cfe4e40568460463aa8b45664a6797fbec021dee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 02:07:27 GMT
ADD file:86bd875241ca751f2f50a9c3504cfca4ce772411fed23fe6893299a271c275e3 in / 
# Thu, 22 Jul 2021 02:07:28 GMT
CMD ["bash"]
# Tue, 10 Aug 2021 23:00:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 10 Aug 2021 23:02:02 GMT
ENV CHRONOGRAF_VERSION=1.8.9
# Tue, 10 Aug 2021 23:02:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 10 Aug 2021 23:02:22 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 10 Aug 2021 23:02:23 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 10 Aug 2021 23:02:23 GMT
EXPOSE 8888
# Tue, 10 Aug 2021 23:02:24 GMT
VOLUME [/var/lib/chronograf]
# Tue, 10 Aug 2021 23:02:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 10 Aug 2021 23:02:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Aug 2021 23:02:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:37325b08023150a9e16c0c8d98d10daa998ce21ec3b9226cc6f0148a245a8a57`  
		Last Modified: Thu, 22 Jul 2021 02:21:16 GMT  
		Size: 19.3 MB (19315955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84236a4145013894eb753d54367ba39e700f41448379d11fb8acf79e2100e630`  
		Last Modified: Tue, 10 Aug 2021 23:03:14 GMT  
		Size: 5.8 MB (5779562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563aa1050ffeff783f5c0ace0c0d4c26bf42c55be8a64652b976ba2242844480`  
		Last Modified: Tue, 10 Aug 2021 23:04:29 GMT  
		Size: 34.5 MB (34497735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33390c7d3a170ef269b4e0664ab92012f5e8a0be393ea68452543bc3805dd86`  
		Last Modified: Tue, 10 Aug 2021 23:04:10 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63513570675210dbda0283a576386daa6c1305131230de9124c5a42c5b9ede1`  
		Last Modified: Tue, 10 Aug 2021 23:04:11 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001f573921c3e4fda4891864bdc68ad985bbec2316df915bf5b962fb9cc9cced`  
		Last Modified: Tue, 10 Aug 2021 23:04:10 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:f16a60124e199840257f215b25bf2347840a341f56c2b50eb6ccfb47740c6c47
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64970233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7e052aba53be0451400f0ec90d1cbd1cf089dfe6b31480453fcc5f21a74d8d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:40 GMT
ADD file:b39a01b3af7a531df3592571b7f6eaa7efd20919858f7f0cd2ddf1c1eceb078d in / 
# Thu, 22 Jul 2021 00:41:40 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:11:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 22 Jul 2021 01:12:23 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Thu, 22 Jul 2021 01:12:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 01:12:31 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 22 Jul 2021 01:12:31 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 22 Jul 2021 01:12:31 GMT
EXPOSE 8888
# Thu, 22 Jul 2021 01:12:31 GMT
VOLUME [/var/lib/chronograf]
# Thu, 22 Jul 2021 01:12:31 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 22 Jul 2021 01:12:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jul 2021 01:12:32 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9e7a560784c85cb9624bff5b6e479fbb95d5e265873987014f8aec75d509a530`  
		Last Modified: Thu, 22 Jul 2021 00:48:50 GMT  
		Size: 20.4 MB (20389427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58364f3e37bf6b8fd81d518b8f7e5a5c8b7e7ac6f79faf0c99101ffcef189204`  
		Last Modified: Thu, 22 Jul 2021 01:12:56 GMT  
		Size: 6.0 MB (6047477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4b587acd1b705f40e13a6f37bde0255703ed113b71c608ddd2f398cbe2f40e`  
		Last Modified: Thu, 22 Jul 2021 01:13:36 GMT  
		Size: 38.5 MB (38508940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2161d973333f7691e631e2063f505a6e800edf211cca030fd5cf083eeb62ed5`  
		Last Modified: Thu, 22 Jul 2021 01:13:30 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0bf9aa56a41dfc971d38fa9b8c9fdcacbe80ea7f7bed40138fc47a30072709`  
		Last Modified: Thu, 22 Jul 2021 01:13:30 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145897592d2b460b30d22c92b220ab150f0af94c742f79505897d3c5c386124d`  
		Last Modified: Thu, 22 Jul 2021 01:13:31 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
