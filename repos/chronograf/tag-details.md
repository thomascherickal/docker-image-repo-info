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
-	[`chronograf:1.8.8`](#chronograf188)
-	[`chronograf:1.8.8-alpine`](#chronograf188-alpine)
-	[`chronograf:alpine`](#chronografalpine)
-	[`chronograf:latest`](#chronograflatest)

## `chronograf:1.6`

```console
$ docker pull chronograf@sha256:3c19429c7fcd24b55b98761b46a6e5115d7ba9348fbe48f8e4f5632f606c6158
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6` - linux; amd64

```console
$ docker pull chronograf@sha256:81b3114bd62e3273c2725e47f7622471825c365c0bc67b54b295f6326ea0fe6c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49357749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40f0001c8f58787597e7040693ecbc58fe6a8db5430b59cec7fd7a542d591981`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 23 Jun 2021 00:22:13 GMT
ADD file:a63c6cc73701d6cb7195338c446b9e92ef6b7a0f9321f6cc1bf8738e3da57c66 in / 
# Wed, 23 Jun 2021 00:22:14 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:45:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 00:45:53 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 23 Jun 2021 00:46:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 00:46:03 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 00:46:03 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 00:46:04 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 00:46:04 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 00:46:04 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 00:46:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 00:46:04 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:aed007321795cdc03a0ba9b238567ffa299459e9b0322a3d835a04d06afc2500`  
		Last Modified: Wed, 23 Jun 2021 00:28:29 GMT  
		Size: 22.5 MB (22528174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f79a7dfde4ccc83615833679b158e7945fdb95a30849b2a027d580b5fa77cfd`  
		Last Modified: Wed, 23 Jun 2021 00:47:35 GMT  
		Size: 6.8 MB (6760154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d77d0daf0c5c73cd9b35fe4d8c4cf91563bb783c31a4d3380198a731c26000`  
		Last Modified: Wed, 23 Jun 2021 00:47:38 GMT  
		Size: 20.0 MB (20045030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3f6fe7d1ef3041b8c69b8c55ca807e0ebde1afc31d4710ae1d6559eb2f4bdc`  
		Last Modified: Wed, 23 Jun 2021 00:47:34 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e997943f70fea462a02d594ee6a46f0a73abeff9c850b7816424e701ccee4d69`  
		Last Modified: Wed, 23 Jun 2021 00:47:34 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb04feff8e7da6801e958391feb36da7acf97ea396fb2348c380210b0ffe0f2`  
		Last Modified: Wed, 23 Jun 2021 00:47:34 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:8737c4f7d573730830f5fd31a3bab22096b60d7945811f5a893b0e197e64ece8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43940595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a84a99d2b217c226f5e3ff995edcb890a09249e7f2e4c2bd0d761d136f2d4efe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 23 Jun 2021 00:23:36 GMT
ADD file:ffc5b643ebc5e4f3704b189af88d436975d60fe871dda953a3baa7bddc561512 in / 
# Wed, 23 Jun 2021 00:23:37 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 01:28:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 01:28:01 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 23 Jun 2021 01:28:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 01:28:19 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 01:28:20 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 01:28:20 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 01:28:20 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 01:28:21 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 01:28:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 01:28:22 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e53ed7a03b01895e35731de5c93cd7a3e826dc1ea9e08b7f35824394302d5c8c`  
		Last Modified: Wed, 23 Jun 2021 00:36:49 GMT  
		Size: 19.3 MB (19316486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edf3d3a63d2680ca0a8661d3182ee5a434352782d0f8f1ce868bfae18481d0d`  
		Last Modified: Wed, 23 Jun 2021 01:30:58 GMT  
		Size: 5.8 MB (5779598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c29384c533b4ff2e3616a7543164ef3713b5f0ff1a9b342d1203932c217a75a`  
		Last Modified: Wed, 23 Jun 2021 01:31:09 GMT  
		Size: 18.8 MB (18820122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3203b8c4936aa1d8fa96cf4807a4a6f41d9f8be9fc7baeea89a8b768e57b115`  
		Last Modified: Wed, 23 Jun 2021 01:30:55 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1655b5af0129ab746830f8d259a1a1fb316814b74600a918cb9d467f504c9c84`  
		Last Modified: Wed, 23 Jun 2021 01:30:55 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815640a9f0fee3e03109917f52987ec9cf7743f6d66c94371d1ac89118217a47`  
		Last Modified: Wed, 23 Jun 2021 01:30:55 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:2f3df66be56cb2247ffb9bb0ef72843a6cd55146535796f35ce4c10f7c40f9eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45422850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f607819633f0a3c90ec26587f19d6d6d56c2db6d19b5de11d9bd8acb6199f0a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 22 Jun 2021 23:51:10 GMT
ADD file:0124cb1e13f08e2df3878b9faa69d962ba2b9c7d5afdf72fff8b1e22201ce065 in / 
# Tue, 22 Jun 2021 23:51:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:15:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 00:15:48 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 23 Jun 2021 00:15:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 00:15:55 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 00:15:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 00:15:55 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 00:15:55 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 00:15:56 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 00:15:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 00:15:56 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:3ac59e1f301a0b03211a0a7f10a84730165b09211c4a8ef9636673101bf1220f`  
		Last Modified: Tue, 22 Jun 2021 23:58:21 GMT  
		Size: 20.4 MB (20389316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d993398ba1c7b159c102a03973e704ab0adc4f058b6750f1a526c6b95a7d5719`  
		Last Modified: Wed, 23 Jun 2021 00:17:01 GMT  
		Size: 6.0 MB (6047480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ecef16c55f94a7eaecebf58ffb360cfe5d780971f7b92c56d4bba092f5a687`  
		Last Modified: Wed, 23 Jun 2021 00:17:04 GMT  
		Size: 19.0 MB (18961666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1f5894367281b926f0335f1506a2051a2eea8cba8f3343a2965d9b07524812`  
		Last Modified: Wed, 23 Jun 2021 00:17:00 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed17f626805dd5915ee70d500c8f53974b8fcb2ef8dd67931b072850fc643a2`  
		Last Modified: Wed, 23 Jun 2021 00:17:00 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a9bc204fad3d1cb1e9cfda651d0fda8b9a58d2f7ce43512a5c693ced2a6c8a`  
		Last Modified: Wed, 23 Jun 2021 00:17:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6-alpine`

```console
$ docker pull chronograf@sha256:96255563a0f40d99b020410ebe817af3bfd5d8cf6bdde976cbb99129a6f6d652
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull chronograf@sha256:3c19429c7fcd24b55b98761b46a6e5115d7ba9348fbe48f8e4f5632f606c6158
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6.2` - linux; amd64

```console
$ docker pull chronograf@sha256:81b3114bd62e3273c2725e47f7622471825c365c0bc67b54b295f6326ea0fe6c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49357749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40f0001c8f58787597e7040693ecbc58fe6a8db5430b59cec7fd7a542d591981`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 23 Jun 2021 00:22:13 GMT
ADD file:a63c6cc73701d6cb7195338c446b9e92ef6b7a0f9321f6cc1bf8738e3da57c66 in / 
# Wed, 23 Jun 2021 00:22:14 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:45:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 00:45:53 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 23 Jun 2021 00:46:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 00:46:03 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 00:46:03 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 00:46:04 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 00:46:04 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 00:46:04 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 00:46:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 00:46:04 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:aed007321795cdc03a0ba9b238567ffa299459e9b0322a3d835a04d06afc2500`  
		Last Modified: Wed, 23 Jun 2021 00:28:29 GMT  
		Size: 22.5 MB (22528174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f79a7dfde4ccc83615833679b158e7945fdb95a30849b2a027d580b5fa77cfd`  
		Last Modified: Wed, 23 Jun 2021 00:47:35 GMT  
		Size: 6.8 MB (6760154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d77d0daf0c5c73cd9b35fe4d8c4cf91563bb783c31a4d3380198a731c26000`  
		Last Modified: Wed, 23 Jun 2021 00:47:38 GMT  
		Size: 20.0 MB (20045030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3f6fe7d1ef3041b8c69b8c55ca807e0ebde1afc31d4710ae1d6559eb2f4bdc`  
		Last Modified: Wed, 23 Jun 2021 00:47:34 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e997943f70fea462a02d594ee6a46f0a73abeff9c850b7816424e701ccee4d69`  
		Last Modified: Wed, 23 Jun 2021 00:47:34 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb04feff8e7da6801e958391feb36da7acf97ea396fb2348c380210b0ffe0f2`  
		Last Modified: Wed, 23 Jun 2021 00:47:34 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:8737c4f7d573730830f5fd31a3bab22096b60d7945811f5a893b0e197e64ece8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43940595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a84a99d2b217c226f5e3ff995edcb890a09249e7f2e4c2bd0d761d136f2d4efe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 23 Jun 2021 00:23:36 GMT
ADD file:ffc5b643ebc5e4f3704b189af88d436975d60fe871dda953a3baa7bddc561512 in / 
# Wed, 23 Jun 2021 00:23:37 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 01:28:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 01:28:01 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 23 Jun 2021 01:28:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 01:28:19 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 01:28:20 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 01:28:20 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 01:28:20 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 01:28:21 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 01:28:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 01:28:22 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e53ed7a03b01895e35731de5c93cd7a3e826dc1ea9e08b7f35824394302d5c8c`  
		Last Modified: Wed, 23 Jun 2021 00:36:49 GMT  
		Size: 19.3 MB (19316486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edf3d3a63d2680ca0a8661d3182ee5a434352782d0f8f1ce868bfae18481d0d`  
		Last Modified: Wed, 23 Jun 2021 01:30:58 GMT  
		Size: 5.8 MB (5779598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c29384c533b4ff2e3616a7543164ef3713b5f0ff1a9b342d1203932c217a75a`  
		Last Modified: Wed, 23 Jun 2021 01:31:09 GMT  
		Size: 18.8 MB (18820122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3203b8c4936aa1d8fa96cf4807a4a6f41d9f8be9fc7baeea89a8b768e57b115`  
		Last Modified: Wed, 23 Jun 2021 01:30:55 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1655b5af0129ab746830f8d259a1a1fb316814b74600a918cb9d467f504c9c84`  
		Last Modified: Wed, 23 Jun 2021 01:30:55 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815640a9f0fee3e03109917f52987ec9cf7743f6d66c94371d1ac89118217a47`  
		Last Modified: Wed, 23 Jun 2021 01:30:55 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:2f3df66be56cb2247ffb9bb0ef72843a6cd55146535796f35ce4c10f7c40f9eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45422850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f607819633f0a3c90ec26587f19d6d6d56c2db6d19b5de11d9bd8acb6199f0a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 22 Jun 2021 23:51:10 GMT
ADD file:0124cb1e13f08e2df3878b9faa69d962ba2b9c7d5afdf72fff8b1e22201ce065 in / 
# Tue, 22 Jun 2021 23:51:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:15:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 00:15:48 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 23 Jun 2021 00:15:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 00:15:55 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 00:15:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 00:15:55 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 00:15:55 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 00:15:56 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 00:15:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 00:15:56 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:3ac59e1f301a0b03211a0a7f10a84730165b09211c4a8ef9636673101bf1220f`  
		Last Modified: Tue, 22 Jun 2021 23:58:21 GMT  
		Size: 20.4 MB (20389316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d993398ba1c7b159c102a03973e704ab0adc4f058b6750f1a526c6b95a7d5719`  
		Last Modified: Wed, 23 Jun 2021 00:17:01 GMT  
		Size: 6.0 MB (6047480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ecef16c55f94a7eaecebf58ffb360cfe5d780971f7b92c56d4bba092f5a687`  
		Last Modified: Wed, 23 Jun 2021 00:17:04 GMT  
		Size: 19.0 MB (18961666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1f5894367281b926f0335f1506a2051a2eea8cba8f3343a2965d9b07524812`  
		Last Modified: Wed, 23 Jun 2021 00:17:00 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed17f626805dd5915ee70d500c8f53974b8fcb2ef8dd67931b072850fc643a2`  
		Last Modified: Wed, 23 Jun 2021 00:17:00 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a9bc204fad3d1cb1e9cfda651d0fda8b9a58d2f7ce43512a5c693ced2a6c8a`  
		Last Modified: Wed, 23 Jun 2021 00:17:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2-alpine`

```console
$ docker pull chronograf@sha256:96255563a0f40d99b020410ebe817af3bfd5d8cf6bdde976cbb99129a6f6d652
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull chronograf@sha256:d99e6350737fa7a4ef92e8fe153e11a8e55f113851c76325e76e6dc7b9c73871
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7` - linux; amd64

```console
$ docker pull chronograf@sha256:9b0a11d4597799ce85a86037766208588fb46cfd10ba6fbe1a366ec18e91eafa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65386201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f3d7f50e25bf03f7480f735f375e007604a78c12dce069354e276d17c5d0f2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 23 Jun 2021 00:22:13 GMT
ADD file:a63c6cc73701d6cb7195338c446b9e92ef6b7a0f9321f6cc1bf8738e3da57c66 in / 
# Wed, 23 Jun 2021 00:22:14 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:46:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 00:46:23 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 23 Jun 2021 00:46:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 00:46:34 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 00:46:34 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 00:46:34 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 00:46:34 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 00:46:35 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 00:46:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 00:46:35 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:aed007321795cdc03a0ba9b238567ffa299459e9b0322a3d835a04d06afc2500`  
		Last Modified: Wed, 23 Jun 2021 00:28:29 GMT  
		Size: 22.5 MB (22528174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fccbc2a8ee90b00ef8440e97c7ae468827c90a5c31569bfccaec1060731e76ea`  
		Last Modified: Wed, 23 Jun 2021 00:47:50 GMT  
		Size: 4.5 MB (4506080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71b5bf010331ef116642e0ad1d42a7f14e7d58ce3167b65832c587644485dbe`  
		Last Modified: Wed, 23 Jun 2021 00:47:56 GMT  
		Size: 38.3 MB (38327556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0d59b20fa183f068e0ebdeabc575eca82335069b94a97731f324b2405cc68b`  
		Last Modified: Wed, 23 Jun 2021 00:47:50 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c1b192f4d46e67684574ca124e988bfb6ffbe15b15bd960f331feb81ad932a`  
		Last Modified: Wed, 23 Jun 2021 00:47:49 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2124136a8f578aaba828ba9f974c40767aa40783e2bd7ee354bb25d98e551525`  
		Last Modified: Wed, 23 Jun 2021 00:47:49 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:1858ddfdff44684e7df6ae27818977ceff8213ebcb85acd6dd0880387474441e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (59002904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d171aaad1f93946b0119594a47c33f9478be157d0b944f35473fed6efe484db`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 23 Jun 2021 00:23:36 GMT
ADD file:ffc5b643ebc5e4f3704b189af88d436975d60fe871dda953a3baa7bddc561512 in / 
# Wed, 23 Jun 2021 00:23:37 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 01:28:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 01:28:53 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 23 Jun 2021 01:29:25 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 01:29:26 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 01:29:26 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 01:29:27 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 01:29:27 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 01:29:27 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 01:29:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 01:29:28 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e53ed7a03b01895e35731de5c93cd7a3e826dc1ea9e08b7f35824394302d5c8c`  
		Last Modified: Wed, 23 Jun 2021 00:36:49 GMT  
		Size: 19.3 MB (19316486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0468465c00d186c9afbb616105d9c74708324b366f930166abfcbd3e7776bcfb`  
		Last Modified: Wed, 23 Jun 2021 01:31:23 GMT  
		Size: 3.9 MB (3879558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e932879d08f6af0fb1a34d7daf3dcd4f5afe4f39da2f8baf51d71beeafc594cf`  
		Last Modified: Wed, 23 Jun 2021 01:31:42 GMT  
		Size: 35.8 MB (35782465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbcfbb4f54cf72ed9cb91346ce510a1b51772fe18805624c2e7367e3eb0fc5c5`  
		Last Modified: Wed, 23 Jun 2021 01:31:21 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fddbd8cf85bdc04233294e4500595e71964e6b50ac4fcf1f1843434c29ff6e`  
		Last Modified: Wed, 23 Jun 2021 01:31:21 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a719d6fccdadf208f9d556bf83c2d7f7430236e1e380b9113a5e27947ae8121c`  
		Last Modified: Wed, 23 Jun 2021 01:31:21 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:117f5cad70a2df1b12a5ee8aa688d6d2f88df9519fbbcf9e4a553e717f8bfc50
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60481619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7431cfe83c4ed82ec155ba823a8509c985c63fc59ad25a651a5e30454c6b5601`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 22 Jun 2021 23:51:10 GMT
ADD file:0124cb1e13f08e2df3878b9faa69d962ba2b9c7d5afdf72fff8b1e22201ce065 in / 
# Tue, 22 Jun 2021 23:51:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:16:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 00:16:11 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 23 Jun 2021 00:16:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 00:16:21 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 00:16:21 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 00:16:21 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 00:16:21 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 00:16:22 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 00:16:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 00:16:22 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:3ac59e1f301a0b03211a0a7f10a84730165b09211c4a8ef9636673101bf1220f`  
		Last Modified: Tue, 22 Jun 2021 23:58:21 GMT  
		Size: 20.4 MB (20389316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d1aad6d1a039d1c942f240839e4f4d2e0ce9f4ead3fc0bf3d25f62b84a7026`  
		Last Modified: Wed, 23 Jun 2021 00:17:17 GMT  
		Size: 4.1 MB (4082095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e467e5c88ba27b047439637909fd755d9003d3d63fdbb4ac9f0df98f95b60785`  
		Last Modified: Wed, 23 Jun 2021 00:17:21 GMT  
		Size: 36.0 MB (35985812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4af99f1ef45f486c87b40ae1f5d8d7d590ec05489257e2b7d74742cc109cde`  
		Last Modified: Wed, 23 Jun 2021 00:17:16 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4614495f3c2973d3f8c3a7e35de77ba38371e9e5cc2998958b559353025a1027`  
		Last Modified: Wed, 23 Jun 2021 00:17:16 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b241a0e39c6ca0e7901004b8fe2148f6f1b0571bc5b5d1b18a016e2e7e80d86`  
		Last Modified: Wed, 23 Jun 2021 00:17:16 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7-alpine`

```console
$ docker pull chronograf@sha256:2a506b16f05ed98563f442490f072e41c2c728b3bc2b22af0ff1ed102ce4f847
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull chronograf@sha256:d99e6350737fa7a4ef92e8fe153e11a8e55f113851c76325e76e6dc7b9c73871
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7.17` - linux; amd64

```console
$ docker pull chronograf@sha256:9b0a11d4597799ce85a86037766208588fb46cfd10ba6fbe1a366ec18e91eafa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65386201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f3d7f50e25bf03f7480f735f375e007604a78c12dce069354e276d17c5d0f2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 23 Jun 2021 00:22:13 GMT
ADD file:a63c6cc73701d6cb7195338c446b9e92ef6b7a0f9321f6cc1bf8738e3da57c66 in / 
# Wed, 23 Jun 2021 00:22:14 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:46:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 00:46:23 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 23 Jun 2021 00:46:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 00:46:34 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 00:46:34 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 00:46:34 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 00:46:34 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 00:46:35 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 00:46:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 00:46:35 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:aed007321795cdc03a0ba9b238567ffa299459e9b0322a3d835a04d06afc2500`  
		Last Modified: Wed, 23 Jun 2021 00:28:29 GMT  
		Size: 22.5 MB (22528174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fccbc2a8ee90b00ef8440e97c7ae468827c90a5c31569bfccaec1060731e76ea`  
		Last Modified: Wed, 23 Jun 2021 00:47:50 GMT  
		Size: 4.5 MB (4506080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71b5bf010331ef116642e0ad1d42a7f14e7d58ce3167b65832c587644485dbe`  
		Last Modified: Wed, 23 Jun 2021 00:47:56 GMT  
		Size: 38.3 MB (38327556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0d59b20fa183f068e0ebdeabc575eca82335069b94a97731f324b2405cc68b`  
		Last Modified: Wed, 23 Jun 2021 00:47:50 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c1b192f4d46e67684574ca124e988bfb6ffbe15b15bd960f331feb81ad932a`  
		Last Modified: Wed, 23 Jun 2021 00:47:49 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2124136a8f578aaba828ba9f974c40767aa40783e2bd7ee354bb25d98e551525`  
		Last Modified: Wed, 23 Jun 2021 00:47:49 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:1858ddfdff44684e7df6ae27818977ceff8213ebcb85acd6dd0880387474441e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (59002904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d171aaad1f93946b0119594a47c33f9478be157d0b944f35473fed6efe484db`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 23 Jun 2021 00:23:36 GMT
ADD file:ffc5b643ebc5e4f3704b189af88d436975d60fe871dda953a3baa7bddc561512 in / 
# Wed, 23 Jun 2021 00:23:37 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 01:28:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 01:28:53 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 23 Jun 2021 01:29:25 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 01:29:26 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 01:29:26 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 01:29:27 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 01:29:27 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 01:29:27 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 01:29:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 01:29:28 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e53ed7a03b01895e35731de5c93cd7a3e826dc1ea9e08b7f35824394302d5c8c`  
		Last Modified: Wed, 23 Jun 2021 00:36:49 GMT  
		Size: 19.3 MB (19316486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0468465c00d186c9afbb616105d9c74708324b366f930166abfcbd3e7776bcfb`  
		Last Modified: Wed, 23 Jun 2021 01:31:23 GMT  
		Size: 3.9 MB (3879558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e932879d08f6af0fb1a34d7daf3dcd4f5afe4f39da2f8baf51d71beeafc594cf`  
		Last Modified: Wed, 23 Jun 2021 01:31:42 GMT  
		Size: 35.8 MB (35782465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbcfbb4f54cf72ed9cb91346ce510a1b51772fe18805624c2e7367e3eb0fc5c5`  
		Last Modified: Wed, 23 Jun 2021 01:31:21 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fddbd8cf85bdc04233294e4500595e71964e6b50ac4fcf1f1843434c29ff6e`  
		Last Modified: Wed, 23 Jun 2021 01:31:21 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a719d6fccdadf208f9d556bf83c2d7f7430236e1e380b9113a5e27947ae8121c`  
		Last Modified: Wed, 23 Jun 2021 01:31:21 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:117f5cad70a2df1b12a5ee8aa688d6d2f88df9519fbbcf9e4a553e717f8bfc50
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60481619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7431cfe83c4ed82ec155ba823a8509c985c63fc59ad25a651a5e30454c6b5601`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 22 Jun 2021 23:51:10 GMT
ADD file:0124cb1e13f08e2df3878b9faa69d962ba2b9c7d5afdf72fff8b1e22201ce065 in / 
# Tue, 22 Jun 2021 23:51:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:16:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 00:16:11 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 23 Jun 2021 00:16:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 00:16:21 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 00:16:21 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 00:16:21 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 00:16:21 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 00:16:22 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 00:16:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 00:16:22 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:3ac59e1f301a0b03211a0a7f10a84730165b09211c4a8ef9636673101bf1220f`  
		Last Modified: Tue, 22 Jun 2021 23:58:21 GMT  
		Size: 20.4 MB (20389316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d1aad6d1a039d1c942f240839e4f4d2e0ce9f4ead3fc0bf3d25f62b84a7026`  
		Last Modified: Wed, 23 Jun 2021 00:17:17 GMT  
		Size: 4.1 MB (4082095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e467e5c88ba27b047439637909fd755d9003d3d63fdbb4ac9f0df98f95b60785`  
		Last Modified: Wed, 23 Jun 2021 00:17:21 GMT  
		Size: 36.0 MB (35985812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4af99f1ef45f486c87b40ae1f5d8d7d590ec05489257e2b7d74742cc109cde`  
		Last Modified: Wed, 23 Jun 2021 00:17:16 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4614495f3c2973d3f8c3a7e35de77ba38371e9e5cc2998958b559353025a1027`  
		Last Modified: Wed, 23 Jun 2021 00:17:16 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b241a0e39c6ca0e7901004b8fe2148f6f1b0571bc5b5d1b18a016e2e7e80d86`  
		Last Modified: Wed, 23 Jun 2021 00:17:16 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17-alpine`

```console
$ docker pull chronograf@sha256:2a506b16f05ed98563f442490f072e41c2c728b3bc2b22af0ff1ed102ce4f847
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull chronograf@sha256:5fcaa81ff0c52dfd8d025d6ba7a25bc9b0623a40d7178598a02fc9b96191f10d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8` - linux; amd64

```console
$ docker pull chronograf@sha256:38614022fba1c9334b2cccc9cb3b8a0c1dccd3e98982e6594b0c8ab910f06d0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70444472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61fa3316ab73148e6f0da45f19a43bf50505932421bccd4afcdb3e012dc48f16`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 23 Jun 2021 00:22:13 GMT
ADD file:a63c6cc73701d6cb7195338c446b9e92ef6b7a0f9321f6cc1bf8738e3da57c66 in / 
# Wed, 23 Jun 2021 00:22:14 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:45:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 00:46:43 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Wed, 23 Jun 2021 00:46:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 00:46:58 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 00:46:58 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 00:46:59 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 00:46:59 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 00:47:00 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 00:47:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 00:47:00 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:aed007321795cdc03a0ba9b238567ffa299459e9b0322a3d835a04d06afc2500`  
		Last Modified: Wed, 23 Jun 2021 00:28:29 GMT  
		Size: 22.5 MB (22528174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f79a7dfde4ccc83615833679b158e7945fdb95a30849b2a027d580b5fa77cfd`  
		Last Modified: Wed, 23 Jun 2021 00:47:35 GMT  
		Size: 6.8 MB (6760154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89004b1bc5bdfd4b82ca33279fb11cdd3e223dc7bc8c4fffcc63abed3f122e77`  
		Last Modified: Wed, 23 Jun 2021 00:48:17 GMT  
		Size: 41.1 MB (41131747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e370825ab42cd719f75ebbf595b21d8611269702039494db5bc073a478e42a49`  
		Last Modified: Wed, 23 Jun 2021 00:48:10 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837e2f126187214c723bd654248ff89b83c0135a5b8e81b5b22563f1ca08d4a0`  
		Last Modified: Wed, 23 Jun 2021 00:48:11 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b9f4dc233e9c1e4d5959c15bfae2bfa39e2ea901642b6c2103b456e33ad88b`  
		Last Modified: Wed, 23 Jun 2021 00:48:10 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:b2b4eed3db8a79112d754a80bcc88e57ff8fe54d288180b810b26bdcf941655c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63858812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:366ddee59ce36eff752d729afa6836460ecb4602cbb4301f9f7a08cad3ec10d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 23 Jun 2021 00:23:36 GMT
ADD file:ffc5b643ebc5e4f3704b189af88d436975d60fe871dda953a3baa7bddc561512 in / 
# Wed, 23 Jun 2021 00:23:37 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 01:28:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 01:29:44 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Wed, 23 Jun 2021 01:30:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 01:30:07 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 01:30:07 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 01:30:08 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 01:30:08 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 01:30:09 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 01:30:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 01:30:10 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e53ed7a03b01895e35731de5c93cd7a3e826dc1ea9e08b7f35824394302d5c8c`  
		Last Modified: Wed, 23 Jun 2021 00:36:49 GMT  
		Size: 19.3 MB (19316486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edf3d3a63d2680ca0a8661d3182ee5a434352782d0f8f1ce868bfae18481d0d`  
		Last Modified: Wed, 23 Jun 2021 01:30:58 GMT  
		Size: 5.8 MB (5779598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c030513d035ab03fe6d9f56e9b9ad755000a9ef12ac9289afa802830d3db820`  
		Last Modified: Wed, 23 Jun 2021 01:32:17 GMT  
		Size: 38.7 MB (38738340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dccbc91868f398e34c1b9ab0584b10330c4900831553fa7a1a7d8c37b82e656b`  
		Last Modified: Wed, 23 Jun 2021 01:31:54 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b7d320fbcf8c5d3ada1230ad24b76895e82f9c64aab24c7b1277089b407495`  
		Last Modified: Wed, 23 Jun 2021 01:31:54 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3671d38ac3973369e633dad1b6c65dbf5c6647b751fdfc473136e8b58a51d6ce`  
		Last Modified: Wed, 23 Jun 2021 01:31:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:ee7de64ec82beb5599ea42440c207022371cea7dd70154c531d0dd204f0fe1ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64970066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:497dfb6049e215ad094fedd8fb7353d3853fd9f6b6c048c7394b5343eb2b2a74`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 22 Jun 2021 23:51:10 GMT
ADD file:0124cb1e13f08e2df3878b9faa69d962ba2b9c7d5afdf72fff8b1e22201ce065 in / 
# Tue, 22 Jun 2021 23:51:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:15:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 00:16:27 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Wed, 23 Jun 2021 00:16:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 00:16:35 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 00:16:35 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 00:16:35 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 00:16:35 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 00:16:36 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 00:16:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 00:16:36 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:3ac59e1f301a0b03211a0a7f10a84730165b09211c4a8ef9636673101bf1220f`  
		Last Modified: Tue, 22 Jun 2021 23:58:21 GMT  
		Size: 20.4 MB (20389316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d993398ba1c7b159c102a03973e704ab0adc4f058b6750f1a526c6b95a7d5719`  
		Last Modified: Wed, 23 Jun 2021 00:17:01 GMT  
		Size: 6.0 MB (6047480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a5953512166f332b9f8db7b08c0d0a01687b815852ea6195c1c92dd1dfa85`  
		Last Modified: Wed, 23 Jun 2021 00:17:40 GMT  
		Size: 38.5 MB (38508873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48773f0f24739d12b881bd49de70c3cfb42fd31fa646a1cffc1430340f933359`  
		Last Modified: Wed, 23 Jun 2021 00:17:34 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac60121b4e9702f1640a18c8df67572ba9a84608747d1e71d5cc4c8ccbdbc6b`  
		Last Modified: Wed, 23 Jun 2021 00:17:34 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e8305b24a21d8df9c1039af388229008c6dccd68e91011c08ce1544299484d`  
		Last Modified: Wed, 23 Jun 2021 00:17:34 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8-alpine`

```console
$ docker pull chronograf@sha256:a5cbcfd2bfc1c933986ccca221a0d540377ce3c034476353415125e083ae5e38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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

## `chronograf:1.8.8`

```console
$ docker pull chronograf@sha256:5fcaa81ff0c52dfd8d025d6ba7a25bc9b0623a40d7178598a02fc9b96191f10d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8.8` - linux; amd64

```console
$ docker pull chronograf@sha256:38614022fba1c9334b2cccc9cb3b8a0c1dccd3e98982e6594b0c8ab910f06d0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70444472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61fa3316ab73148e6f0da45f19a43bf50505932421bccd4afcdb3e012dc48f16`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 23 Jun 2021 00:22:13 GMT
ADD file:a63c6cc73701d6cb7195338c446b9e92ef6b7a0f9321f6cc1bf8738e3da57c66 in / 
# Wed, 23 Jun 2021 00:22:14 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:45:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 00:46:43 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Wed, 23 Jun 2021 00:46:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 00:46:58 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 00:46:58 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 00:46:59 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 00:46:59 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 00:47:00 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 00:47:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 00:47:00 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:aed007321795cdc03a0ba9b238567ffa299459e9b0322a3d835a04d06afc2500`  
		Last Modified: Wed, 23 Jun 2021 00:28:29 GMT  
		Size: 22.5 MB (22528174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f79a7dfde4ccc83615833679b158e7945fdb95a30849b2a027d580b5fa77cfd`  
		Last Modified: Wed, 23 Jun 2021 00:47:35 GMT  
		Size: 6.8 MB (6760154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89004b1bc5bdfd4b82ca33279fb11cdd3e223dc7bc8c4fffcc63abed3f122e77`  
		Last Modified: Wed, 23 Jun 2021 00:48:17 GMT  
		Size: 41.1 MB (41131747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e370825ab42cd719f75ebbf595b21d8611269702039494db5bc073a478e42a49`  
		Last Modified: Wed, 23 Jun 2021 00:48:10 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837e2f126187214c723bd654248ff89b83c0135a5b8e81b5b22563f1ca08d4a0`  
		Last Modified: Wed, 23 Jun 2021 00:48:11 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b9f4dc233e9c1e4d5959c15bfae2bfa39e2ea901642b6c2103b456e33ad88b`  
		Last Modified: Wed, 23 Jun 2021 00:48:10 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:b2b4eed3db8a79112d754a80bcc88e57ff8fe54d288180b810b26bdcf941655c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63858812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:366ddee59ce36eff752d729afa6836460ecb4602cbb4301f9f7a08cad3ec10d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 23 Jun 2021 00:23:36 GMT
ADD file:ffc5b643ebc5e4f3704b189af88d436975d60fe871dda953a3baa7bddc561512 in / 
# Wed, 23 Jun 2021 00:23:37 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 01:28:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 01:29:44 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Wed, 23 Jun 2021 01:30:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 01:30:07 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 01:30:07 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 01:30:08 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 01:30:08 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 01:30:09 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 01:30:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 01:30:10 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e53ed7a03b01895e35731de5c93cd7a3e826dc1ea9e08b7f35824394302d5c8c`  
		Last Modified: Wed, 23 Jun 2021 00:36:49 GMT  
		Size: 19.3 MB (19316486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edf3d3a63d2680ca0a8661d3182ee5a434352782d0f8f1ce868bfae18481d0d`  
		Last Modified: Wed, 23 Jun 2021 01:30:58 GMT  
		Size: 5.8 MB (5779598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c030513d035ab03fe6d9f56e9b9ad755000a9ef12ac9289afa802830d3db820`  
		Last Modified: Wed, 23 Jun 2021 01:32:17 GMT  
		Size: 38.7 MB (38738340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dccbc91868f398e34c1b9ab0584b10330c4900831553fa7a1a7d8c37b82e656b`  
		Last Modified: Wed, 23 Jun 2021 01:31:54 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b7d320fbcf8c5d3ada1230ad24b76895e82f9c64aab24c7b1277089b407495`  
		Last Modified: Wed, 23 Jun 2021 01:31:54 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3671d38ac3973369e633dad1b6c65dbf5c6647b751fdfc473136e8b58a51d6ce`  
		Last Modified: Wed, 23 Jun 2021 01:31:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:ee7de64ec82beb5599ea42440c207022371cea7dd70154c531d0dd204f0fe1ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64970066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:497dfb6049e215ad094fedd8fb7353d3853fd9f6b6c048c7394b5343eb2b2a74`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 22 Jun 2021 23:51:10 GMT
ADD file:0124cb1e13f08e2df3878b9faa69d962ba2b9c7d5afdf72fff8b1e22201ce065 in / 
# Tue, 22 Jun 2021 23:51:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:15:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 00:16:27 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Wed, 23 Jun 2021 00:16:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 00:16:35 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 00:16:35 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 00:16:35 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 00:16:35 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 00:16:36 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 00:16:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 00:16:36 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:3ac59e1f301a0b03211a0a7f10a84730165b09211c4a8ef9636673101bf1220f`  
		Last Modified: Tue, 22 Jun 2021 23:58:21 GMT  
		Size: 20.4 MB (20389316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d993398ba1c7b159c102a03973e704ab0adc4f058b6750f1a526c6b95a7d5719`  
		Last Modified: Wed, 23 Jun 2021 00:17:01 GMT  
		Size: 6.0 MB (6047480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a5953512166f332b9f8db7b08c0d0a01687b815852ea6195c1c92dd1dfa85`  
		Last Modified: Wed, 23 Jun 2021 00:17:40 GMT  
		Size: 38.5 MB (38508873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48773f0f24739d12b881bd49de70c3cfb42fd31fa646a1cffc1430340f933359`  
		Last Modified: Wed, 23 Jun 2021 00:17:34 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac60121b4e9702f1640a18c8df67572ba9a84608747d1e71d5cc4c8ccbdbc6b`  
		Last Modified: Wed, 23 Jun 2021 00:17:34 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e8305b24a21d8df9c1039af388229008c6dccd68e91011c08ce1544299484d`  
		Last Modified: Wed, 23 Jun 2021 00:17:34 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.8-alpine`

```console
$ docker pull chronograf@sha256:a5cbcfd2bfc1c933986ccca221a0d540377ce3c034476353415125e083ae5e38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.8.8-alpine` - linux; amd64

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

## `chronograf:alpine`

```console
$ docker pull chronograf@sha256:a5cbcfd2bfc1c933986ccca221a0d540377ce3c034476353415125e083ae5e38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull chronograf@sha256:5fcaa81ff0c52dfd8d025d6ba7a25bc9b0623a40d7178598a02fc9b96191f10d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:38614022fba1c9334b2cccc9cb3b8a0c1dccd3e98982e6594b0c8ab910f06d0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70444472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61fa3316ab73148e6f0da45f19a43bf50505932421bccd4afcdb3e012dc48f16`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 23 Jun 2021 00:22:13 GMT
ADD file:a63c6cc73701d6cb7195338c446b9e92ef6b7a0f9321f6cc1bf8738e3da57c66 in / 
# Wed, 23 Jun 2021 00:22:14 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:45:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 00:46:43 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Wed, 23 Jun 2021 00:46:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 00:46:58 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 00:46:58 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 00:46:59 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 00:46:59 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 00:47:00 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 00:47:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 00:47:00 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:aed007321795cdc03a0ba9b238567ffa299459e9b0322a3d835a04d06afc2500`  
		Last Modified: Wed, 23 Jun 2021 00:28:29 GMT  
		Size: 22.5 MB (22528174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f79a7dfde4ccc83615833679b158e7945fdb95a30849b2a027d580b5fa77cfd`  
		Last Modified: Wed, 23 Jun 2021 00:47:35 GMT  
		Size: 6.8 MB (6760154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89004b1bc5bdfd4b82ca33279fb11cdd3e223dc7bc8c4fffcc63abed3f122e77`  
		Last Modified: Wed, 23 Jun 2021 00:48:17 GMT  
		Size: 41.1 MB (41131747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e370825ab42cd719f75ebbf595b21d8611269702039494db5bc073a478e42a49`  
		Last Modified: Wed, 23 Jun 2021 00:48:10 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837e2f126187214c723bd654248ff89b83c0135a5b8e81b5b22563f1ca08d4a0`  
		Last Modified: Wed, 23 Jun 2021 00:48:11 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b9f4dc233e9c1e4d5959c15bfae2bfa39e2ea901642b6c2103b456e33ad88b`  
		Last Modified: Wed, 23 Jun 2021 00:48:10 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:b2b4eed3db8a79112d754a80bcc88e57ff8fe54d288180b810b26bdcf941655c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63858812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:366ddee59ce36eff752d729afa6836460ecb4602cbb4301f9f7a08cad3ec10d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 23 Jun 2021 00:23:36 GMT
ADD file:ffc5b643ebc5e4f3704b189af88d436975d60fe871dda953a3baa7bddc561512 in / 
# Wed, 23 Jun 2021 00:23:37 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 01:28:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 01:29:44 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Wed, 23 Jun 2021 01:30:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 01:30:07 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 01:30:07 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 01:30:08 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 01:30:08 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 01:30:09 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 01:30:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 01:30:10 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e53ed7a03b01895e35731de5c93cd7a3e826dc1ea9e08b7f35824394302d5c8c`  
		Last Modified: Wed, 23 Jun 2021 00:36:49 GMT  
		Size: 19.3 MB (19316486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edf3d3a63d2680ca0a8661d3182ee5a434352782d0f8f1ce868bfae18481d0d`  
		Last Modified: Wed, 23 Jun 2021 01:30:58 GMT  
		Size: 5.8 MB (5779598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c030513d035ab03fe6d9f56e9b9ad755000a9ef12ac9289afa802830d3db820`  
		Last Modified: Wed, 23 Jun 2021 01:32:17 GMT  
		Size: 38.7 MB (38738340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dccbc91868f398e34c1b9ab0584b10330c4900831553fa7a1a7d8c37b82e656b`  
		Last Modified: Wed, 23 Jun 2021 01:31:54 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b7d320fbcf8c5d3ada1230ad24b76895e82f9c64aab24c7b1277089b407495`  
		Last Modified: Wed, 23 Jun 2021 01:31:54 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3671d38ac3973369e633dad1b6c65dbf5c6647b751fdfc473136e8b58a51d6ce`  
		Last Modified: Wed, 23 Jun 2021 01:31:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:ee7de64ec82beb5599ea42440c207022371cea7dd70154c531d0dd204f0fe1ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64970066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:497dfb6049e215ad094fedd8fb7353d3853fd9f6b6c048c7394b5343eb2b2a74`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 22 Jun 2021 23:51:10 GMT
ADD file:0124cb1e13f08e2df3878b9faa69d962ba2b9c7d5afdf72fff8b1e22201ce065 in / 
# Tue, 22 Jun 2021 23:51:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:15:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 00:16:27 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Wed, 23 Jun 2021 00:16:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 00:16:35 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 23 Jun 2021 00:16:35 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 23 Jun 2021 00:16:35 GMT
EXPOSE 8888
# Wed, 23 Jun 2021 00:16:35 GMT
VOLUME [/var/lib/chronograf]
# Wed, 23 Jun 2021 00:16:36 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 23 Jun 2021 00:16:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 00:16:36 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:3ac59e1f301a0b03211a0a7f10a84730165b09211c4a8ef9636673101bf1220f`  
		Last Modified: Tue, 22 Jun 2021 23:58:21 GMT  
		Size: 20.4 MB (20389316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d993398ba1c7b159c102a03973e704ab0adc4f058b6750f1a526c6b95a7d5719`  
		Last Modified: Wed, 23 Jun 2021 00:17:01 GMT  
		Size: 6.0 MB (6047480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a5953512166f332b9f8db7b08c0d0a01687b815852ea6195c1c92dd1dfa85`  
		Last Modified: Wed, 23 Jun 2021 00:17:40 GMT  
		Size: 38.5 MB (38508873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48773f0f24739d12b881bd49de70c3cfb42fd31fa646a1cffc1430340f933359`  
		Last Modified: Wed, 23 Jun 2021 00:17:34 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac60121b4e9702f1640a18c8df67572ba9a84608747d1e71d5cc4c8ccbdbc6b`  
		Last Modified: Wed, 23 Jun 2021 00:17:34 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e8305b24a21d8df9c1039af388229008c6dccd68e91011c08ce1544299484d`  
		Last Modified: Wed, 23 Jun 2021 00:17:34 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
