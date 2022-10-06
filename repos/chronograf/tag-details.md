<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `chronograf`

-	[`chronograf:1.10`](#chronograf110)
-	[`chronograf:1.10-alpine`](#chronograf110-alpine)
-	[`chronograf:1.10.0`](#chronograf1100)
-	[`chronograf:1.10.0-alpine`](#chronograf1100-alpine)
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

## `chronograf:1.10`

```console
$ docker pull chronograf@sha256:b6c6ea9e86b822cac1af490c33a5d9e415f76be8cf14c2f783bc72befe1ab494
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.10` - linux; amd64

```console
$ docker pull chronograf@sha256:1f767ad8f2b3a31f540d76c7ef867ed90dce17676678b0899843f7b66c3ee855
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81258440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d636e1959fa435a29e5434caa564b755f309185a46e6c82b0d11303a8a3efbe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:27:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 01:27:54 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Wed, 05 Oct 2022 01:28:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 01:28:02 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 01:28:02 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 01:28:02 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 01:28:02 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 01:28:02 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 01:28:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 01:28:02 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762cd6423542a86d6d1ec55ed5565d142da4efb99f27b261ed1efb69096c7b7c`  
		Last Modified: Wed, 05 Oct 2022 01:28:43 GMT  
		Size: 5.2 MB (5226783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6557ab7d007da9a7b6cc77c0e8e3c2691f0bcd8466caaae3250cd6fc76716a`  
		Last Modified: Wed, 05 Oct 2022 01:29:19 GMT  
		Size: 44.6 MB (44587169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b05df3b9ee91e8ccbae2347bded5c778ca8db5bff9c7c5aa823787f54196bf4`  
		Last Modified: Wed, 05 Oct 2022 01:29:13 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfa1ae42b93b5dc771bb62e284596d1591fff0327d258a1340c17dd786035ed`  
		Last Modified: Wed, 05 Oct 2022 01:29:13 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a521fe38dc78c302da861bae8abf36e9842ba54045ab95dcaf8ca6eb54d014`  
		Last Modified: Wed, 05 Oct 2022 01:29:13 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:74369d6a1722549033636ff6deae2ad8a6b22032830073fb7eceba29d595f1ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73562035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96c9aa985715d42e51fb74c1747427e927611ff0013d7f6e6d1e3cb6608334e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:04:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 01:04:39 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Wed, 05 Oct 2022 01:04:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 01:04:50 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 01:04:51 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 01:04:51 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 01:04:51 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 01:04:51 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 01:04:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 01:04:51 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc14fee07560a2936b1d20d8255a4bd556e62f7fbc6f6315b40f6414a1e4cc7a`  
		Last Modified: Wed, 05 Oct 2022 01:05:41 GMT  
		Size: 4.5 MB (4493786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5165c7780555fbc9f43e71ea6eb27a6bab287a68d2d802985d54f0da110fe045`  
		Last Modified: Wed, 05 Oct 2022 01:06:24 GMT  
		Size: 42.5 MB (42464659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4e18bc5a8fc51c5e1207e5a000659db2c321522baaa001df2da8a2921dd16e`  
		Last Modified: Wed, 05 Oct 2022 01:06:15 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd30d77fb4c42b51b944e736258a7bc25bce848283ba633ac7317f69d9e6457a`  
		Last Modified: Wed, 05 Oct 2022 01:06:15 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01214c89af7978821fdaa181b1c762c2e3336d1f89584134b888dbdd3892ec61`  
		Last Modified: Wed, 05 Oct 2022 01:06:16 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:ab8645fbd8402ce07d268e98499311ffbb24d00e5a5363ab624561379243ed72
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.5 MB (77493472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9d613a28bbc4f092549d7d95bc3eeb003b22ed879746050114afca2cfa421f3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:45:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 00:46:33 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Wed, 05 Oct 2022 00:46:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 00:46:43 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 00:46:44 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 00:46:44 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 00:46:45 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 00:46:47 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 00:46:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 00:46:48 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dbe41e7f952c059f146b958dd11b6c38b9d59877811c4e18d0a39f68d60a8d`  
		Last Modified: Wed, 05 Oct 2022 00:47:31 GMT  
		Size: 5.0 MB (5004266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3257b0dd82526de2a4ac4f4f98a2ac04007cf38c90ce431be31b6be1388116ea`  
		Last Modified: Wed, 05 Oct 2022 00:48:07 GMT  
		Size: 42.4 MB (42400420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227ef1fa822f9c77d8a5391f76b66e3e7ca1a891773cbb4aa4fde663a40ca8ac`  
		Last Modified: Wed, 05 Oct 2022 00:48:01 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da492be9085c913497b9f19970b5f7b6f87ac1a56205f95a292239a9adc84614`  
		Last Modified: Wed, 05 Oct 2022 00:48:01 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7ae266ac1469c396b608504f87dc74708ad757ebc00aa30023fbc52f5c4335`  
		Last Modified: Wed, 05 Oct 2022 00:48:01 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.10-alpine`

```console
$ docker pull chronograf@sha256:c92d2e5d3aaed3d5abd3e21e85b3dd60e8169f7bf6699f473aed28eabff1d043
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.10-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:de6c4148eeb1291ced92120697fad8332c74a726171672daf7c7b67e21d3850b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30311143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d58f859d1dc29bb2ee9f917635f6eb5621000d9d6619ec8ad4549203995550f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:15:37 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 20:16:09 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Thu, 06 Oct 2022 20:16:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 20:16:17 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 06 Oct 2022 20:16:17 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 06 Oct 2022 20:16:17 GMT
EXPOSE 8888
# Thu, 06 Oct 2022 20:16:17 GMT
VOLUME [/var/lib/chronograf]
# Thu, 06 Oct 2022 20:16:17 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 06 Oct 2022 20:16:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 20:16:17 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed07ae854e5b9e7d93d0c5eb8bbcfb2d6e5eddeb00720efe7b55766ce5bfbab`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 284.6 KB (284583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eea9d4a8a69cd5e2e5fca1b123ba2cd44364cf36b128c2fe59a5edf12221dfd`  
		Last Modified: Thu, 06 Oct 2022 20:17:26 GMT  
		Size: 27.2 MB (27174517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a685cca594b365e8c9e5d2a452959ac02b6fde12a79d898abf1a833a483707`  
		Last Modified: Thu, 06 Oct 2022 20:17:21 GMT  
		Size: 12.3 KB (12265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80dba48a5545ef21547b2590458104e7bf680e4a5afbd1707de156d2d9420751`  
		Last Modified: Thu, 06 Oct 2022 20:17:21 GMT  
		Size: 11.9 KB (11897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ece5a9a06b7739faf864ebca0e4561819e3e331b928666a09e2c5bb2b9b2181`  
		Last Modified: Thu, 06 Oct 2022 20:17:21 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.10.0`

```console
$ docker pull chronograf@sha256:b6c6ea9e86b822cac1af490c33a5d9e415f76be8cf14c2f783bc72befe1ab494
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.10.0` - linux; amd64

```console
$ docker pull chronograf@sha256:1f767ad8f2b3a31f540d76c7ef867ed90dce17676678b0899843f7b66c3ee855
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81258440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d636e1959fa435a29e5434caa564b755f309185a46e6c82b0d11303a8a3efbe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:27:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 01:27:54 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Wed, 05 Oct 2022 01:28:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 01:28:02 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 01:28:02 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 01:28:02 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 01:28:02 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 01:28:02 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 01:28:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 01:28:02 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762cd6423542a86d6d1ec55ed5565d142da4efb99f27b261ed1efb69096c7b7c`  
		Last Modified: Wed, 05 Oct 2022 01:28:43 GMT  
		Size: 5.2 MB (5226783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6557ab7d007da9a7b6cc77c0e8e3c2691f0bcd8466caaae3250cd6fc76716a`  
		Last Modified: Wed, 05 Oct 2022 01:29:19 GMT  
		Size: 44.6 MB (44587169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b05df3b9ee91e8ccbae2347bded5c778ca8db5bff9c7c5aa823787f54196bf4`  
		Last Modified: Wed, 05 Oct 2022 01:29:13 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfa1ae42b93b5dc771bb62e284596d1591fff0327d258a1340c17dd786035ed`  
		Last Modified: Wed, 05 Oct 2022 01:29:13 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a521fe38dc78c302da861bae8abf36e9842ba54045ab95dcaf8ca6eb54d014`  
		Last Modified: Wed, 05 Oct 2022 01:29:13 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10.0` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:74369d6a1722549033636ff6deae2ad8a6b22032830073fb7eceba29d595f1ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73562035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96c9aa985715d42e51fb74c1747427e927611ff0013d7f6e6d1e3cb6608334e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:04:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 01:04:39 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Wed, 05 Oct 2022 01:04:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 01:04:50 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 01:04:51 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 01:04:51 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 01:04:51 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 01:04:51 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 01:04:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 01:04:51 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc14fee07560a2936b1d20d8255a4bd556e62f7fbc6f6315b40f6414a1e4cc7a`  
		Last Modified: Wed, 05 Oct 2022 01:05:41 GMT  
		Size: 4.5 MB (4493786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5165c7780555fbc9f43e71ea6eb27a6bab287a68d2d802985d54f0da110fe045`  
		Last Modified: Wed, 05 Oct 2022 01:06:24 GMT  
		Size: 42.5 MB (42464659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4e18bc5a8fc51c5e1207e5a000659db2c321522baaa001df2da8a2921dd16e`  
		Last Modified: Wed, 05 Oct 2022 01:06:15 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd30d77fb4c42b51b944e736258a7bc25bce848283ba633ac7317f69d9e6457a`  
		Last Modified: Wed, 05 Oct 2022 01:06:15 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01214c89af7978821fdaa181b1c762c2e3336d1f89584134b888dbdd3892ec61`  
		Last Modified: Wed, 05 Oct 2022 01:06:16 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10.0` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:ab8645fbd8402ce07d268e98499311ffbb24d00e5a5363ab624561379243ed72
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.5 MB (77493472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9d613a28bbc4f092549d7d95bc3eeb003b22ed879746050114afca2cfa421f3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:45:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 00:46:33 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Wed, 05 Oct 2022 00:46:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 00:46:43 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 00:46:44 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 00:46:44 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 00:46:45 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 00:46:47 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 00:46:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 00:46:48 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dbe41e7f952c059f146b958dd11b6c38b9d59877811c4e18d0a39f68d60a8d`  
		Last Modified: Wed, 05 Oct 2022 00:47:31 GMT  
		Size: 5.0 MB (5004266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3257b0dd82526de2a4ac4f4f98a2ac04007cf38c90ce431be31b6be1388116ea`  
		Last Modified: Wed, 05 Oct 2022 00:48:07 GMT  
		Size: 42.4 MB (42400420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227ef1fa822f9c77d8a5391f76b66e3e7ca1a891773cbb4aa4fde663a40ca8ac`  
		Last Modified: Wed, 05 Oct 2022 00:48:01 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da492be9085c913497b9f19970b5f7b6f87ac1a56205f95a292239a9adc84614`  
		Last Modified: Wed, 05 Oct 2022 00:48:01 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7ae266ac1469c396b608504f87dc74708ad757ebc00aa30023fbc52f5c4335`  
		Last Modified: Wed, 05 Oct 2022 00:48:01 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.10.0-alpine`

```console
$ docker pull chronograf@sha256:c92d2e5d3aaed3d5abd3e21e85b3dd60e8169f7bf6699f473aed28eabff1d043
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.10.0-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:de6c4148eeb1291ced92120697fad8332c74a726171672daf7c7b67e21d3850b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30311143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d58f859d1dc29bb2ee9f917635f6eb5621000d9d6619ec8ad4549203995550f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:15:37 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 20:16:09 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Thu, 06 Oct 2022 20:16:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 20:16:17 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 06 Oct 2022 20:16:17 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 06 Oct 2022 20:16:17 GMT
EXPOSE 8888
# Thu, 06 Oct 2022 20:16:17 GMT
VOLUME [/var/lib/chronograf]
# Thu, 06 Oct 2022 20:16:17 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 06 Oct 2022 20:16:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 20:16:17 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed07ae854e5b9e7d93d0c5eb8bbcfb2d6e5eddeb00720efe7b55766ce5bfbab`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 284.6 KB (284583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eea9d4a8a69cd5e2e5fca1b123ba2cd44364cf36b128c2fe59a5edf12221dfd`  
		Last Modified: Thu, 06 Oct 2022 20:17:26 GMT  
		Size: 27.2 MB (27174517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a685cca594b365e8c9e5d2a452959ac02b6fde12a79d898abf1a833a483707`  
		Last Modified: Thu, 06 Oct 2022 20:17:21 GMT  
		Size: 12.3 KB (12265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80dba48a5545ef21547b2590458104e7bf680e4a5afbd1707de156d2d9420751`  
		Last Modified: Thu, 06 Oct 2022 20:17:21 GMT  
		Size: 11.9 KB (11897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ece5a9a06b7739faf864ebca0e4561819e3e331b928666a09e2c5bb2b9b2181`  
		Last Modified: Thu, 06 Oct 2022 20:17:21 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7`

```console
$ docker pull chronograf@sha256:e7e82a6abd6aa6c67c5226b68b42a0641d358a17ea7050761e78b9bc248c5a72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7` - linux; amd64

```console
$ docker pull chronograf@sha256:5c273d77c3c39d7db3483e2d9027ddf44fbae93b58f993820168d7f4a8ae7621
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70600182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b52007f7779292226206caf40da7c5678f94a0290b2cd6b422ff5185871a609b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:27:04 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 01:27:04 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 05 Oct 2022 01:27:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 01:27:14 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 01:27:14 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 01:27:14 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 01:27:15 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 01:27:15 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 01:27:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 01:27:15 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7e5371d9e3e0ff90a00cff790896b0e4fc23febe9aa45f5bd1a0b8e9cc413`  
		Last Modified: Wed, 05 Oct 2022 01:28:27 GMT  
		Size: 4.4 MB (4418220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70d229cd02f238f9231557de2a35ccb468eef76935acb116f7ea2b031b5263e`  
		Last Modified: Wed, 05 Oct 2022 01:28:31 GMT  
		Size: 34.7 MB (34737468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92d7656111b0714d352a87891d21fc2eb7b8f0cdfb6c92327e7888b61f61248`  
		Last Modified: Wed, 05 Oct 2022 01:28:26 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495ed12d63f43ecfb56c9e656841a4c1f20b79db62b39743d50b4c4bd35a160d`  
		Last Modified: Wed, 05 Oct 2022 01:28:26 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9a53d9fdcc32252e9838a7b5141b875faa2a369860dc661cc62e7c96c0d1cc`  
		Last Modified: Wed, 05 Oct 2022 01:28:26 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:4084c2b18a39914d1c000cea7bfecfdd2dc8c9b3c73abf49db5ac1860fc11b2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63420490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:134a2a9ec07e16fa4402f8c415e7ce22120ff13896d31b7244d4fd9760c04f4b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:03:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 01:03:40 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 05 Oct 2022 01:03:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 01:03:52 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 01:03:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 01:03:53 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 01:03:53 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 01:03:53 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 01:03:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 01:03:53 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e931f11d426389e45fd322323a3fe72a6011130c994318a8c88895eb403850b`  
		Last Modified: Wed, 05 Oct 2022 01:05:23 GMT  
		Size: 3.7 MB (3719646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e0d82c52c830b705e888c215329505bff540007ed58cc748ccf9212f5ad2e9`  
		Last Modified: Wed, 05 Oct 2022 01:05:28 GMT  
		Size: 33.1 MB (33097253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c53a3be0ec39c7d345cec125bfe633e90c666573f43186004fded74f35b2f1`  
		Last Modified: Wed, 05 Oct 2022 01:05:22 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ef0dcd6863600d8f216d50916bab30a4e763eaaee67aa124ae5f18c959c4d8`  
		Last Modified: Wed, 05 Oct 2022 01:05:22 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31090a231a7599fcfdf16ba32ab0acf19a1d44af130216b85bc871a8da844992`  
		Last Modified: Wed, 05 Oct 2022 01:05:22 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:5b01f415476a448413268a327e51815f3bf28c749e7904e431c7479e77bc8931
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67330678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91df70009ff272bd4f20603c1d3eb6417697d959cf682667337d0166c6d72e9b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:45:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 00:45:23 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 05 Oct 2022 00:45:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 00:45:34 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 00:45:35 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 00:45:35 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 00:45:36 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 00:45:38 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 00:45:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 00:45:39 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c247b250948b56a735fe4dab127b1af668dd096ad230a94ee0a521187e6c923`  
		Last Modified: Wed, 05 Oct 2022 00:47:16 GMT  
		Size: 4.2 MB (4211174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b41a6bf45f4414515340b8fb736e8c18d703680373ea1d0e5e40e6278a13d76`  
		Last Modified: Wed, 05 Oct 2022 00:47:19 GMT  
		Size: 33.0 MB (33030717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a7838b164987eeed60587e2b95200f505b563edd2d3623385248c991eaf2f`  
		Last Modified: Wed, 05 Oct 2022 00:47:15 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39297a9cd1cb6e1a169361dc32d0419b8a083d9b40efa6452709e2d8921394b`  
		Last Modified: Wed, 05 Oct 2022 00:47:15 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d1c2ac34db6e412347c93349601daf5ee0a21ac7fe755e8c526ce873f2f3e1`  
		Last Modified: Wed, 05 Oct 2022 00:47:15 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7-alpine`

```console
$ docker pull chronograf@sha256:9d26ac37c933bc166fe620ded24d156485d317e71f04c4eb2878c565b984849f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.7-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:4b6a35a54e58b60f161d3f2f58aed998b7a0ae7074ca382fda7ec2ada7c2e902
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22693433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6af57497b0aa0aca47fc1ff15bd6c753ed5fa7230450329b86857ba4351cc0a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:15:37 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 20:15:37 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 06 Oct 2022 20:15:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 20:15:42 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 06 Oct 2022 20:15:42 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 06 Oct 2022 20:15:42 GMT
EXPOSE 8888
# Thu, 06 Oct 2022 20:15:43 GMT
VOLUME [/var/lib/chronograf]
# Thu, 06 Oct 2022 20:15:43 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 06 Oct 2022 20:15:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 20:15:43 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed07ae854e5b9e7d93d0c5eb8bbcfb2d6e5eddeb00720efe7b55766ce5bfbab`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 284.6 KB (284583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fda7c0dc93cbe974534daa33cf7bf0b94c5803f47fb7f8116f83829cc52a701`  
		Last Modified: Thu, 06 Oct 2022 20:16:44 GMT  
		Size: 19.6 MB (19556809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bf26481c4767c4543af0f2684354471d9d92c1d3ff7e3a43f714669312ddb5`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 12.3 KB (12264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ba3ac2384cc84a067095232897c2f0e30822a778f2bc4d7136e30d336f9a7b`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 11.9 KB (11896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cdc8000c1828cc4d9f01bcd32824b8ef240f8130b247937bfb0159e925f412`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17`

```console
$ docker pull chronograf@sha256:e7e82a6abd6aa6c67c5226b68b42a0641d358a17ea7050761e78b9bc248c5a72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7.17` - linux; amd64

```console
$ docker pull chronograf@sha256:5c273d77c3c39d7db3483e2d9027ddf44fbae93b58f993820168d7f4a8ae7621
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70600182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b52007f7779292226206caf40da7c5678f94a0290b2cd6b422ff5185871a609b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:27:04 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 01:27:04 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 05 Oct 2022 01:27:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 01:27:14 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 01:27:14 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 01:27:14 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 01:27:15 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 01:27:15 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 01:27:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 01:27:15 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7e5371d9e3e0ff90a00cff790896b0e4fc23febe9aa45f5bd1a0b8e9cc413`  
		Last Modified: Wed, 05 Oct 2022 01:28:27 GMT  
		Size: 4.4 MB (4418220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70d229cd02f238f9231557de2a35ccb468eef76935acb116f7ea2b031b5263e`  
		Last Modified: Wed, 05 Oct 2022 01:28:31 GMT  
		Size: 34.7 MB (34737468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92d7656111b0714d352a87891d21fc2eb7b8f0cdfb6c92327e7888b61f61248`  
		Last Modified: Wed, 05 Oct 2022 01:28:26 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495ed12d63f43ecfb56c9e656841a4c1f20b79db62b39743d50b4c4bd35a160d`  
		Last Modified: Wed, 05 Oct 2022 01:28:26 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9a53d9fdcc32252e9838a7b5141b875faa2a369860dc661cc62e7c96c0d1cc`  
		Last Modified: Wed, 05 Oct 2022 01:28:26 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:4084c2b18a39914d1c000cea7bfecfdd2dc8c9b3c73abf49db5ac1860fc11b2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63420490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:134a2a9ec07e16fa4402f8c415e7ce22120ff13896d31b7244d4fd9760c04f4b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:03:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 01:03:40 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 05 Oct 2022 01:03:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 01:03:52 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 01:03:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 01:03:53 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 01:03:53 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 01:03:53 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 01:03:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 01:03:53 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e931f11d426389e45fd322323a3fe72a6011130c994318a8c88895eb403850b`  
		Last Modified: Wed, 05 Oct 2022 01:05:23 GMT  
		Size: 3.7 MB (3719646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e0d82c52c830b705e888c215329505bff540007ed58cc748ccf9212f5ad2e9`  
		Last Modified: Wed, 05 Oct 2022 01:05:28 GMT  
		Size: 33.1 MB (33097253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c53a3be0ec39c7d345cec125bfe633e90c666573f43186004fded74f35b2f1`  
		Last Modified: Wed, 05 Oct 2022 01:05:22 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ef0dcd6863600d8f216d50916bab30a4e763eaaee67aa124ae5f18c959c4d8`  
		Last Modified: Wed, 05 Oct 2022 01:05:22 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31090a231a7599fcfdf16ba32ab0acf19a1d44af130216b85bc871a8da844992`  
		Last Modified: Wed, 05 Oct 2022 01:05:22 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:5b01f415476a448413268a327e51815f3bf28c749e7904e431c7479e77bc8931
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67330678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91df70009ff272bd4f20603c1d3eb6417697d959cf682667337d0166c6d72e9b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:45:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 00:45:23 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 05 Oct 2022 00:45:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 00:45:34 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 00:45:35 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 00:45:35 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 00:45:36 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 00:45:38 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 00:45:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 00:45:39 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c247b250948b56a735fe4dab127b1af668dd096ad230a94ee0a521187e6c923`  
		Last Modified: Wed, 05 Oct 2022 00:47:16 GMT  
		Size: 4.2 MB (4211174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b41a6bf45f4414515340b8fb736e8c18d703680373ea1d0e5e40e6278a13d76`  
		Last Modified: Wed, 05 Oct 2022 00:47:19 GMT  
		Size: 33.0 MB (33030717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a7838b164987eeed60587e2b95200f505b563edd2d3623385248c991eaf2f`  
		Last Modified: Wed, 05 Oct 2022 00:47:15 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39297a9cd1cb6e1a169361dc32d0419b8a083d9b40efa6452709e2d8921394b`  
		Last Modified: Wed, 05 Oct 2022 00:47:15 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d1c2ac34db6e412347c93349601daf5ee0a21ac7fe755e8c526ce873f2f3e1`  
		Last Modified: Wed, 05 Oct 2022 00:47:15 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17-alpine`

```console
$ docker pull chronograf@sha256:9d26ac37c933bc166fe620ded24d156485d317e71f04c4eb2878c565b984849f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.7.17-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:4b6a35a54e58b60f161d3f2f58aed998b7a0ae7074ca382fda7ec2ada7c2e902
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22693433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6af57497b0aa0aca47fc1ff15bd6c753ed5fa7230450329b86857ba4351cc0a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:15:37 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 20:15:37 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 06 Oct 2022 20:15:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 20:15:42 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 06 Oct 2022 20:15:42 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 06 Oct 2022 20:15:42 GMT
EXPOSE 8888
# Thu, 06 Oct 2022 20:15:43 GMT
VOLUME [/var/lib/chronograf]
# Thu, 06 Oct 2022 20:15:43 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 06 Oct 2022 20:15:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 20:15:43 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed07ae854e5b9e7d93d0c5eb8bbcfb2d6e5eddeb00720efe7b55766ce5bfbab`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 284.6 KB (284583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fda7c0dc93cbe974534daa33cf7bf0b94c5803f47fb7f8116f83829cc52a701`  
		Last Modified: Thu, 06 Oct 2022 20:16:44 GMT  
		Size: 19.6 MB (19556809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bf26481c4767c4543af0f2684354471d9d92c1d3ff7e3a43f714669312ddb5`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 12.3 KB (12264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ba3ac2384cc84a067095232897c2f0e30822a778f2bc4d7136e30d336f9a7b`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 11.9 KB (11896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cdc8000c1828cc4d9f01bcd32824b8ef240f8130b247937bfb0159e925f412`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8`

```console
$ docker pull chronograf@sha256:a063ee9299f1e7ef901265c7318422f5392451f77a569cf0ee2c742218517871
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8` - linux; amd64

```console
$ docker pull chronograf@sha256:4a8be5a8fb644f94a99faa0e46e01ba30655f03d7024599784547730102b5880
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71250142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:551b9fdaedb29921bf4e66ed480cb6267a818a732ab80e79c6f5cf46382fb86e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:27:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 01:27:29 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 05 Oct 2022 01:27:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 01:27:35 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 01:27:36 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 01:27:36 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 01:27:36 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 01:27:36 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 01:27:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 01:27:36 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762cd6423542a86d6d1ec55ed5565d142da4efb99f27b261ed1efb69096c7b7c`  
		Last Modified: Wed, 05 Oct 2022 01:28:43 GMT  
		Size: 5.2 MB (5226783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18351f6041391f8432305284cdbc0ee44c9814bc95b1ca19782ef0f35e0c5799`  
		Last Modified: Wed, 05 Oct 2022 01:28:46 GMT  
		Size: 34.6 MB (34578861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae551c872abdfd179e4f76f6225f98997192a405b01a0671e5753f1945c61173`  
		Last Modified: Wed, 05 Oct 2022 01:28:42 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061d326730af10652a7bfed605e9566c79631790c7441e19a4d2223b0ed7f5de`  
		Last Modified: Wed, 05 Oct 2022 01:28:42 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638762b55e3eb30b87936f893bd78523f8eec18e6d0bdbe40dbe255049b85c57`  
		Last Modified: Wed, 05 Oct 2022 01:28:42 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:1eb3df82708a4cfd5be0ce5de63b0cb4700cc42502770560e36647c43000b8fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63847714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:421cda6a39820ab3b2b72a3c9440ddbb709fdbce85e0f398dc3506657249b0eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:04:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 01:04:08 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 05 Oct 2022 01:04:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 01:04:18 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 01:04:18 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 01:04:18 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 01:04:18 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 01:04:18 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 01:04:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 01:04:19 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc14fee07560a2936b1d20d8255a4bd556e62f7fbc6f6315b40f6414a1e4cc7a`  
		Last Modified: Wed, 05 Oct 2022 01:05:41 GMT  
		Size: 4.5 MB (4493786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c7d73bdff2efca9ccc47f7b35473b6788d6b44facbe7778b1955f1dac2ad61`  
		Last Modified: Wed, 05 Oct 2022 01:05:46 GMT  
		Size: 32.8 MB (32750327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd13a6d0ef7f2a508ad4df2b6d9732b431322a0846c7b365d21d112d6a3f70ca`  
		Last Modified: Wed, 05 Oct 2022 01:05:40 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0bea0b0f754b0e8d66654fbf099f74d76e8ca7170e50b2f8b702ded7f5cf4dc`  
		Last Modified: Wed, 05 Oct 2022 01:05:40 GMT  
		Size: 11.9 KB (11912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d262c7510b45c672d0de187e3ecdd70810801f22a407dc33f2e0bf4d4460245`  
		Last Modified: Wed, 05 Oct 2022 01:05:40 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:30f3713d9c4e563a003895b5d3f5d6c44379fbf9b42833ccdf4b140b6f6774e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67521146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ffce56c52f0c5f84e9455faed01012b6bfc37a42455e36e6b5b0b5416e363bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:45:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 00:45:55 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 05 Oct 2022 00:46:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 00:46:04 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 00:46:05 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 00:46:05 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 00:46:06 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 00:46:08 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 00:46:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 00:46:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dbe41e7f952c059f146b958dd11b6c38b9d59877811c4e18d0a39f68d60a8d`  
		Last Modified: Wed, 05 Oct 2022 00:47:31 GMT  
		Size: 5.0 MB (5004266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6290dc5a65327d6c4bce61c30a2bc726c45d57780b49933cfdf2f676521f2fde`  
		Last Modified: Wed, 05 Oct 2022 00:47:34 GMT  
		Size: 32.4 MB (32428092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6c37883d573ce741de94800940caee21f906412e04da29f3b30dd40594e252`  
		Last Modified: Wed, 05 Oct 2022 00:47:30 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d3aac2d484d90e6266db1a9e32852821dba849707e6d6ffd8ffa89255896465`  
		Last Modified: Wed, 05 Oct 2022 00:47:30 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8b27a47095599b776e2485c574d0a257feb20d4466383805b699467b058f39`  
		Last Modified: Wed, 05 Oct 2022 00:47:30 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8-alpine`

```console
$ docker pull chronograf@sha256:a430e7dd4d3f94b4b711a4000e847f59465fe1e3d7e9997d59800fc7a5da10cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:2d4ad97697ce5c225b6e38515e3ea3b543e28f102c45917f4239ecca0ebadda5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22340855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:610057aef173c70f1c0a6ce869e16af679c0a1e65c669ac3b8eaba8d112a527a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:15:37 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 20:15:47 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Thu, 06 Oct 2022 20:15:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 20:15:53 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 06 Oct 2022 20:15:53 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 06 Oct 2022 20:15:53 GMT
EXPOSE 8888
# Thu, 06 Oct 2022 20:15:53 GMT
VOLUME [/var/lib/chronograf]
# Thu, 06 Oct 2022 20:15:53 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 06 Oct 2022 20:15:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 20:15:53 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed07ae854e5b9e7d93d0c5eb8bbcfb2d6e5eddeb00720efe7b55766ce5bfbab`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 284.6 KB (284583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59d8c24f659459b77a60f9b6c97614166735dca2ae5a9254e7733b3382432fa`  
		Last Modified: Thu, 06 Oct 2022 20:16:58 GMT  
		Size: 19.2 MB (19204225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eaef5e9f5e1eba8a7b3a73db5c4d6efe6ba62e72d3c1a86384494b5fc0b6bc3`  
		Last Modified: Thu, 06 Oct 2022 20:16:55 GMT  
		Size: 12.3 KB (12267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd6d1543ef965519e2d993c8db13568b477c3c72bae7b6023a2cde9350376d1`  
		Last Modified: Thu, 06 Oct 2022 20:16:55 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f5df71d2bc59720fcde07d37a3c2f558595676b2519551f3efda4830e28abc`  
		Last Modified: Thu, 06 Oct 2022 20:16:55 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.10`

```console
$ docker pull chronograf@sha256:a063ee9299f1e7ef901265c7318422f5392451f77a569cf0ee2c742218517871
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8.10` - linux; amd64

```console
$ docker pull chronograf@sha256:4a8be5a8fb644f94a99faa0e46e01ba30655f03d7024599784547730102b5880
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71250142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:551b9fdaedb29921bf4e66ed480cb6267a818a732ab80e79c6f5cf46382fb86e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:27:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 01:27:29 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 05 Oct 2022 01:27:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 01:27:35 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 01:27:36 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 01:27:36 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 01:27:36 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 01:27:36 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 01:27:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 01:27:36 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762cd6423542a86d6d1ec55ed5565d142da4efb99f27b261ed1efb69096c7b7c`  
		Last Modified: Wed, 05 Oct 2022 01:28:43 GMT  
		Size: 5.2 MB (5226783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18351f6041391f8432305284cdbc0ee44c9814bc95b1ca19782ef0f35e0c5799`  
		Last Modified: Wed, 05 Oct 2022 01:28:46 GMT  
		Size: 34.6 MB (34578861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae551c872abdfd179e4f76f6225f98997192a405b01a0671e5753f1945c61173`  
		Last Modified: Wed, 05 Oct 2022 01:28:42 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061d326730af10652a7bfed605e9566c79631790c7441e19a4d2223b0ed7f5de`  
		Last Modified: Wed, 05 Oct 2022 01:28:42 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638762b55e3eb30b87936f893bd78523f8eec18e6d0bdbe40dbe255049b85c57`  
		Last Modified: Wed, 05 Oct 2022 01:28:42 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.10` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:1eb3df82708a4cfd5be0ce5de63b0cb4700cc42502770560e36647c43000b8fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63847714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:421cda6a39820ab3b2b72a3c9440ddbb709fdbce85e0f398dc3506657249b0eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:04:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 01:04:08 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 05 Oct 2022 01:04:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 01:04:18 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 01:04:18 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 01:04:18 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 01:04:18 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 01:04:18 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 01:04:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 01:04:19 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc14fee07560a2936b1d20d8255a4bd556e62f7fbc6f6315b40f6414a1e4cc7a`  
		Last Modified: Wed, 05 Oct 2022 01:05:41 GMT  
		Size: 4.5 MB (4493786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c7d73bdff2efca9ccc47f7b35473b6788d6b44facbe7778b1955f1dac2ad61`  
		Last Modified: Wed, 05 Oct 2022 01:05:46 GMT  
		Size: 32.8 MB (32750327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd13a6d0ef7f2a508ad4df2b6d9732b431322a0846c7b365d21d112d6a3f70ca`  
		Last Modified: Wed, 05 Oct 2022 01:05:40 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0bea0b0f754b0e8d66654fbf099f74d76e8ca7170e50b2f8b702ded7f5cf4dc`  
		Last Modified: Wed, 05 Oct 2022 01:05:40 GMT  
		Size: 11.9 KB (11912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d262c7510b45c672d0de187e3ecdd70810801f22a407dc33f2e0bf4d4460245`  
		Last Modified: Wed, 05 Oct 2022 01:05:40 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.10` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:30f3713d9c4e563a003895b5d3f5d6c44379fbf9b42833ccdf4b140b6f6774e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67521146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ffce56c52f0c5f84e9455faed01012b6bfc37a42455e36e6b5b0b5416e363bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:45:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 00:45:55 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 05 Oct 2022 00:46:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 00:46:04 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 00:46:05 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 00:46:05 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 00:46:06 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 00:46:08 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 00:46:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 00:46:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dbe41e7f952c059f146b958dd11b6c38b9d59877811c4e18d0a39f68d60a8d`  
		Last Modified: Wed, 05 Oct 2022 00:47:31 GMT  
		Size: 5.0 MB (5004266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6290dc5a65327d6c4bce61c30a2bc726c45d57780b49933cfdf2f676521f2fde`  
		Last Modified: Wed, 05 Oct 2022 00:47:34 GMT  
		Size: 32.4 MB (32428092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6c37883d573ce741de94800940caee21f906412e04da29f3b30dd40594e252`  
		Last Modified: Wed, 05 Oct 2022 00:47:30 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d3aac2d484d90e6266db1a9e32852821dba849707e6d6ffd8ffa89255896465`  
		Last Modified: Wed, 05 Oct 2022 00:47:30 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8b27a47095599b776e2485c574d0a257feb20d4466383805b699467b058f39`  
		Last Modified: Wed, 05 Oct 2022 00:47:30 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.10-alpine`

```console
$ docker pull chronograf@sha256:a430e7dd4d3f94b4b711a4000e847f59465fe1e3d7e9997d59800fc7a5da10cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.8.10-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:2d4ad97697ce5c225b6e38515e3ea3b543e28f102c45917f4239ecca0ebadda5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22340855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:610057aef173c70f1c0a6ce869e16af679c0a1e65c669ac3b8eaba8d112a527a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:15:37 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 20:15:47 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Thu, 06 Oct 2022 20:15:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 20:15:53 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 06 Oct 2022 20:15:53 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 06 Oct 2022 20:15:53 GMT
EXPOSE 8888
# Thu, 06 Oct 2022 20:15:53 GMT
VOLUME [/var/lib/chronograf]
# Thu, 06 Oct 2022 20:15:53 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 06 Oct 2022 20:15:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 20:15:53 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed07ae854e5b9e7d93d0c5eb8bbcfb2d6e5eddeb00720efe7b55766ce5bfbab`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 284.6 KB (284583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59d8c24f659459b77a60f9b6c97614166735dca2ae5a9254e7733b3382432fa`  
		Last Modified: Thu, 06 Oct 2022 20:16:58 GMT  
		Size: 19.2 MB (19204225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eaef5e9f5e1eba8a7b3a73db5c4d6efe6ba62e72d3c1a86384494b5fc0b6bc3`  
		Last Modified: Thu, 06 Oct 2022 20:16:55 GMT  
		Size: 12.3 KB (12267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd6d1543ef965519e2d993c8db13568b477c3c72bae7b6023a2cde9350376d1`  
		Last Modified: Thu, 06 Oct 2022 20:16:55 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f5df71d2bc59720fcde07d37a3c2f558595676b2519551f3efda4830e28abc`  
		Last Modified: Thu, 06 Oct 2022 20:16:55 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9`

```console
$ docker pull chronograf@sha256:494dd068bc3663c094cc86bc10819a0d31e1dc75aa050c2aa3e6432dbee81fd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.9` - linux; amd64

```console
$ docker pull chronograf@sha256:16c2da2a79ac1ed21bca89b8611eb417571dcf28463144d8414ae8b50ceabde6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71897687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c806adf73da0313c7b3ccb93d18442cae664c2208daea88ca95ac6f362d76d2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:27:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 01:27:43 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 05 Oct 2022 01:27:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 01:27:49 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 01:27:50 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 01:27:50 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 01:27:50 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 01:27:50 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 01:27:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 01:27:50 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762cd6423542a86d6d1ec55ed5565d142da4efb99f27b261ed1efb69096c7b7c`  
		Last Modified: Wed, 05 Oct 2022 01:28:43 GMT  
		Size: 5.2 MB (5226783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ecf369da3d3d0f79ceb05175bd9b33734c110b4f9185a247b64dde25b0c4c5b`  
		Last Modified: Wed, 05 Oct 2022 01:29:02 GMT  
		Size: 35.2 MB (35226408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70cee957ffcb85fb3d50a63a64ab8d0bd365956bbe291579f93768ca48fe723`  
		Last Modified: Wed, 05 Oct 2022 01:28:57 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66f0d39685106854e8ffbaf307236badc921a70095ada6b687adfe9276ca8aa`  
		Last Modified: Wed, 05 Oct 2022 01:28:58 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1df31476ed6bdd3a9ec9c5d284d21e0af1212c0bac1ef18fd92436d9f3cf54`  
		Last Modified: Wed, 05 Oct 2022 01:28:57 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:a3ea835845566de7e46098dac2788ccaea86e3ba60324ad33db22c50bdb7af43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64623938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4976d6dabea20fb462daf1a7484441d4a1e392e86f1cba5a2b1ad0d761328756`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:04:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 01:04:24 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 05 Oct 2022 01:04:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 01:04:33 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 01:04:33 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 01:04:33 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 01:04:34 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 01:04:34 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 01:04:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 01:04:34 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc14fee07560a2936b1d20d8255a4bd556e62f7fbc6f6315b40f6414a1e4cc7a`  
		Last Modified: Wed, 05 Oct 2022 01:05:41 GMT  
		Size: 4.5 MB (4493786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1a7989fd5466c4811e805213425dc0d14330f0743bb66edc3a23ac0caaa30c`  
		Last Modified: Wed, 05 Oct 2022 01:06:04 GMT  
		Size: 33.5 MB (33526559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdf18cf6ee1467d616e2e9c58cbebde414818beb542e4af0e3165f16b9e279a`  
		Last Modified: Wed, 05 Oct 2022 01:05:58 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905a01f7abbe00038cca3087de0603252f9ec9b72f419c0cb35e35d2fe748aab`  
		Last Modified: Wed, 05 Oct 2022 01:05:58 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e002105531f7862e0d8e2595e56d0d9ef416c19900bd7600a430e93d521dada4`  
		Last Modified: Wed, 05 Oct 2022 01:05:58 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:664925066dacbf84865cc305cbaa59458e13bafd552fe49e9e809ef19cb46656
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68272322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19d070c58efe6be41ad2dcad5dea7d880f0bd26bdedb6ec32c5b1633581ca6f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:45:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 00:46:14 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 05 Oct 2022 00:46:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 00:46:22 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 00:46:23 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 00:46:23 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 00:46:24 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 00:46:26 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 00:46:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 00:46:27 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dbe41e7f952c059f146b958dd11b6c38b9d59877811c4e18d0a39f68d60a8d`  
		Last Modified: Wed, 05 Oct 2022 00:47:31 GMT  
		Size: 5.0 MB (5004266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0337b1ec723076faec02f7099b2df121d8873f66a0c382bcc6e25ee47634a7a`  
		Last Modified: Wed, 05 Oct 2022 00:47:50 GMT  
		Size: 33.2 MB (33179267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29aceb288b7ad8513eb030c2af903f5a5a72f1fa367a94647af2dbce005e03a7`  
		Last Modified: Wed, 05 Oct 2022 00:47:45 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58189d45abd113f8e15a7d26ecf12e47915e2008ac7b3af2517beaaaad1edea0`  
		Last Modified: Wed, 05 Oct 2022 00:47:45 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8aaa63ceb4ecd783e409e13c38229f7bc762f245a246561f410aafcfe83983`  
		Last Modified: Wed, 05 Oct 2022 00:47:45 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9-alpine`

```console
$ docker pull chronograf@sha256:22f17928ed0e686715e2b906f6e647ccc55c1e216dff1a563b76264f87f5392d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.9-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:d0b7ec6f54d4499c9a81a50fd7148b478b660fc8ded25155fb3a13baa4bf6239
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.8 MB (22808795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a3777d2e14c286895c264ba3580085a048c076a33a63ce90569c4ea6d7b2f98`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:15:37 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 20:15:57 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Thu, 06 Oct 2022 20:16:03 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 20:16:03 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 06 Oct 2022 20:16:03 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 06 Oct 2022 20:16:04 GMT
EXPOSE 8888
# Thu, 06 Oct 2022 20:16:04 GMT
VOLUME [/var/lib/chronograf]
# Thu, 06 Oct 2022 20:16:04 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 06 Oct 2022 20:16:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 20:16:04 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed07ae854e5b9e7d93d0c5eb8bbcfb2d6e5eddeb00720efe7b55766ce5bfbab`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 284.6 KB (284583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dfd580c937a95d72fb2af50a28c6814b4886872b951143883b0ffde4712c5f`  
		Last Modified: Thu, 06 Oct 2022 20:17:11 GMT  
		Size: 19.7 MB (19672168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e61e6634ea5e9aa1e5e15257ac4db9252543ec14ac7bd8989d98dca8f7b54f`  
		Last Modified: Thu, 06 Oct 2022 20:17:08 GMT  
		Size: 12.3 KB (12265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f00f1a43c212b770a42e5c7bc1563a4df034c07a36e2d6f937d26b1d907303e`  
		Last Modified: Thu, 06 Oct 2022 20:17:08 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bb73bba03a148277f19627c4b0811fb06e034afa29b8939eb47b20577a3537`  
		Last Modified: Thu, 06 Oct 2022 20:17:08 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9.4`

```console
$ docker pull chronograf@sha256:494dd068bc3663c094cc86bc10819a0d31e1dc75aa050c2aa3e6432dbee81fd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.9.4` - linux; amd64

```console
$ docker pull chronograf@sha256:16c2da2a79ac1ed21bca89b8611eb417571dcf28463144d8414ae8b50ceabde6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71897687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c806adf73da0313c7b3ccb93d18442cae664c2208daea88ca95ac6f362d76d2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:27:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 01:27:43 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 05 Oct 2022 01:27:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 01:27:49 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 01:27:50 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 01:27:50 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 01:27:50 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 01:27:50 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 01:27:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 01:27:50 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762cd6423542a86d6d1ec55ed5565d142da4efb99f27b261ed1efb69096c7b7c`  
		Last Modified: Wed, 05 Oct 2022 01:28:43 GMT  
		Size: 5.2 MB (5226783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ecf369da3d3d0f79ceb05175bd9b33734c110b4f9185a247b64dde25b0c4c5b`  
		Last Modified: Wed, 05 Oct 2022 01:29:02 GMT  
		Size: 35.2 MB (35226408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70cee957ffcb85fb3d50a63a64ab8d0bd365956bbe291579f93768ca48fe723`  
		Last Modified: Wed, 05 Oct 2022 01:28:57 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66f0d39685106854e8ffbaf307236badc921a70095ada6b687adfe9276ca8aa`  
		Last Modified: Wed, 05 Oct 2022 01:28:58 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1df31476ed6bdd3a9ec9c5d284d21e0af1212c0bac1ef18fd92436d9f3cf54`  
		Last Modified: Wed, 05 Oct 2022 01:28:57 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9.4` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:a3ea835845566de7e46098dac2788ccaea86e3ba60324ad33db22c50bdb7af43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64623938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4976d6dabea20fb462daf1a7484441d4a1e392e86f1cba5a2b1ad0d761328756`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:04:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 01:04:24 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 05 Oct 2022 01:04:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 01:04:33 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 01:04:33 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 01:04:33 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 01:04:34 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 01:04:34 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 01:04:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 01:04:34 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc14fee07560a2936b1d20d8255a4bd556e62f7fbc6f6315b40f6414a1e4cc7a`  
		Last Modified: Wed, 05 Oct 2022 01:05:41 GMT  
		Size: 4.5 MB (4493786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1a7989fd5466c4811e805213425dc0d14330f0743bb66edc3a23ac0caaa30c`  
		Last Modified: Wed, 05 Oct 2022 01:06:04 GMT  
		Size: 33.5 MB (33526559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdf18cf6ee1467d616e2e9c58cbebde414818beb542e4af0e3165f16b9e279a`  
		Last Modified: Wed, 05 Oct 2022 01:05:58 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905a01f7abbe00038cca3087de0603252f9ec9b72f419c0cb35e35d2fe748aab`  
		Last Modified: Wed, 05 Oct 2022 01:05:58 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e002105531f7862e0d8e2595e56d0d9ef416c19900bd7600a430e93d521dada4`  
		Last Modified: Wed, 05 Oct 2022 01:05:58 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9.4` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:664925066dacbf84865cc305cbaa59458e13bafd552fe49e9e809ef19cb46656
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68272322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19d070c58efe6be41ad2dcad5dea7d880f0bd26bdedb6ec32c5b1633581ca6f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:45:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 00:46:14 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 05 Oct 2022 00:46:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 00:46:22 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 00:46:23 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 00:46:23 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 00:46:24 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 00:46:26 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 00:46:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 00:46:27 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dbe41e7f952c059f146b958dd11b6c38b9d59877811c4e18d0a39f68d60a8d`  
		Last Modified: Wed, 05 Oct 2022 00:47:31 GMT  
		Size: 5.0 MB (5004266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0337b1ec723076faec02f7099b2df121d8873f66a0c382bcc6e25ee47634a7a`  
		Last Modified: Wed, 05 Oct 2022 00:47:50 GMT  
		Size: 33.2 MB (33179267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29aceb288b7ad8513eb030c2af903f5a5a72f1fa367a94647af2dbce005e03a7`  
		Last Modified: Wed, 05 Oct 2022 00:47:45 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58189d45abd113f8e15a7d26ecf12e47915e2008ac7b3af2517beaaaad1edea0`  
		Last Modified: Wed, 05 Oct 2022 00:47:45 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8aaa63ceb4ecd783e409e13c38229f7bc762f245a246561f410aafcfe83983`  
		Last Modified: Wed, 05 Oct 2022 00:47:45 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9.4-alpine`

```console
$ docker pull chronograf@sha256:22f17928ed0e686715e2b906f6e647ccc55c1e216dff1a563b76264f87f5392d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.9.4-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:d0b7ec6f54d4499c9a81a50fd7148b478b660fc8ded25155fb3a13baa4bf6239
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.8 MB (22808795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a3777d2e14c286895c264ba3580085a048c076a33a63ce90569c4ea6d7b2f98`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:15:37 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 20:15:57 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Thu, 06 Oct 2022 20:16:03 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 20:16:03 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 06 Oct 2022 20:16:03 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 06 Oct 2022 20:16:04 GMT
EXPOSE 8888
# Thu, 06 Oct 2022 20:16:04 GMT
VOLUME [/var/lib/chronograf]
# Thu, 06 Oct 2022 20:16:04 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 06 Oct 2022 20:16:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 20:16:04 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed07ae854e5b9e7d93d0c5eb8bbcfb2d6e5eddeb00720efe7b55766ce5bfbab`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 284.6 KB (284583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dfd580c937a95d72fb2af50a28c6814b4886872b951143883b0ffde4712c5f`  
		Last Modified: Thu, 06 Oct 2022 20:17:11 GMT  
		Size: 19.7 MB (19672168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e61e6634ea5e9aa1e5e15257ac4db9252543ec14ac7bd8989d98dca8f7b54f`  
		Last Modified: Thu, 06 Oct 2022 20:17:08 GMT  
		Size: 12.3 KB (12265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f00f1a43c212b770a42e5c7bc1563a4df034c07a36e2d6f937d26b1d907303e`  
		Last Modified: Thu, 06 Oct 2022 20:17:08 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bb73bba03a148277f19627c4b0811fb06e034afa29b8939eb47b20577a3537`  
		Last Modified: Thu, 06 Oct 2022 20:17:08 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:alpine`

```console
$ docker pull chronograf@sha256:c92d2e5d3aaed3d5abd3e21e85b3dd60e8169f7bf6699f473aed28eabff1d043
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:de6c4148eeb1291ced92120697fad8332c74a726171672daf7c7b67e21d3850b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30311143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d58f859d1dc29bb2ee9f917635f6eb5621000d9d6619ec8ad4549203995550f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:15:37 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 20:16:09 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Thu, 06 Oct 2022 20:16:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 20:16:17 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 06 Oct 2022 20:16:17 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 06 Oct 2022 20:16:17 GMT
EXPOSE 8888
# Thu, 06 Oct 2022 20:16:17 GMT
VOLUME [/var/lib/chronograf]
# Thu, 06 Oct 2022 20:16:17 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 06 Oct 2022 20:16:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 20:16:17 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed07ae854e5b9e7d93d0c5eb8bbcfb2d6e5eddeb00720efe7b55766ce5bfbab`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 284.6 KB (284583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eea9d4a8a69cd5e2e5fca1b123ba2cd44364cf36b128c2fe59a5edf12221dfd`  
		Last Modified: Thu, 06 Oct 2022 20:17:26 GMT  
		Size: 27.2 MB (27174517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a685cca594b365e8c9e5d2a452959ac02b6fde12a79d898abf1a833a483707`  
		Last Modified: Thu, 06 Oct 2022 20:17:21 GMT  
		Size: 12.3 KB (12265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80dba48a5545ef21547b2590458104e7bf680e4a5afbd1707de156d2d9420751`  
		Last Modified: Thu, 06 Oct 2022 20:17:21 GMT  
		Size: 11.9 KB (11897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ece5a9a06b7739faf864ebca0e4561819e3e331b928666a09e2c5bb2b9b2181`  
		Last Modified: Thu, 06 Oct 2022 20:17:21 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:latest`

```console
$ docker pull chronograf@sha256:b6c6ea9e86b822cac1af490c33a5d9e415f76be8cf14c2f783bc72befe1ab494
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:1f767ad8f2b3a31f540d76c7ef867ed90dce17676678b0899843f7b66c3ee855
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81258440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d636e1959fa435a29e5434caa564b755f309185a46e6c82b0d11303a8a3efbe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:27:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 01:27:54 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Wed, 05 Oct 2022 01:28:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 01:28:02 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 01:28:02 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 01:28:02 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 01:28:02 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 01:28:02 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 01:28:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 01:28:02 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762cd6423542a86d6d1ec55ed5565d142da4efb99f27b261ed1efb69096c7b7c`  
		Last Modified: Wed, 05 Oct 2022 01:28:43 GMT  
		Size: 5.2 MB (5226783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6557ab7d007da9a7b6cc77c0e8e3c2691f0bcd8466caaae3250cd6fc76716a`  
		Last Modified: Wed, 05 Oct 2022 01:29:19 GMT  
		Size: 44.6 MB (44587169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b05df3b9ee91e8ccbae2347bded5c778ca8db5bff9c7c5aa823787f54196bf4`  
		Last Modified: Wed, 05 Oct 2022 01:29:13 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfa1ae42b93b5dc771bb62e284596d1591fff0327d258a1340c17dd786035ed`  
		Last Modified: Wed, 05 Oct 2022 01:29:13 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a521fe38dc78c302da861bae8abf36e9842ba54045ab95dcaf8ca6eb54d014`  
		Last Modified: Wed, 05 Oct 2022 01:29:13 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:74369d6a1722549033636ff6deae2ad8a6b22032830073fb7eceba29d595f1ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73562035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96c9aa985715d42e51fb74c1747427e927611ff0013d7f6e6d1e3cb6608334e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:04:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 01:04:39 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Wed, 05 Oct 2022 01:04:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 01:04:50 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 01:04:51 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 01:04:51 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 01:04:51 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 01:04:51 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 01:04:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 01:04:51 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc14fee07560a2936b1d20d8255a4bd556e62f7fbc6f6315b40f6414a1e4cc7a`  
		Last Modified: Wed, 05 Oct 2022 01:05:41 GMT  
		Size: 4.5 MB (4493786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5165c7780555fbc9f43e71ea6eb27a6bab287a68d2d802985d54f0da110fe045`  
		Last Modified: Wed, 05 Oct 2022 01:06:24 GMT  
		Size: 42.5 MB (42464659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4e18bc5a8fc51c5e1207e5a000659db2c321522baaa001df2da8a2921dd16e`  
		Last Modified: Wed, 05 Oct 2022 01:06:15 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd30d77fb4c42b51b944e736258a7bc25bce848283ba633ac7317f69d9e6457a`  
		Last Modified: Wed, 05 Oct 2022 01:06:15 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01214c89af7978821fdaa181b1c762c2e3336d1f89584134b888dbdd3892ec61`  
		Last Modified: Wed, 05 Oct 2022 01:06:16 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:ab8645fbd8402ce07d268e98499311ffbb24d00e5a5363ab624561379243ed72
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.5 MB (77493472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9d613a28bbc4f092549d7d95bc3eeb003b22ed879746050114afca2cfa421f3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:45:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 00:46:33 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Wed, 05 Oct 2022 00:46:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Oct 2022 00:46:43 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 05 Oct 2022 00:46:44 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 05 Oct 2022 00:46:44 GMT
EXPOSE 8888
# Wed, 05 Oct 2022 00:46:45 GMT
VOLUME [/var/lib/chronograf]
# Wed, 05 Oct 2022 00:46:47 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 05 Oct 2022 00:46:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 00:46:48 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dbe41e7f952c059f146b958dd11b6c38b9d59877811c4e18d0a39f68d60a8d`  
		Last Modified: Wed, 05 Oct 2022 00:47:31 GMT  
		Size: 5.0 MB (5004266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3257b0dd82526de2a4ac4f4f98a2ac04007cf38c90ce431be31b6be1388116ea`  
		Last Modified: Wed, 05 Oct 2022 00:48:07 GMT  
		Size: 42.4 MB (42400420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227ef1fa822f9c77d8a5391f76b66e3e7ca1a891773cbb4aa4fde663a40ca8ac`  
		Last Modified: Wed, 05 Oct 2022 00:48:01 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da492be9085c913497b9f19970b5f7b6f87ac1a56205f95a292239a9adc84614`  
		Last Modified: Wed, 05 Oct 2022 00:48:01 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7ae266ac1469c396b608504f87dc74708ad757ebc00aa30023fbc52f5c4335`  
		Last Modified: Wed, 05 Oct 2022 00:48:01 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
