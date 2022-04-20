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
$ docker pull chronograf@sha256:f4bf6ff1804b4af9d1b3f37db2bac9caccf47fb15a8d353397b79119bc98c0b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6` - linux; amd64

```console
$ docker pull chronograf@sha256:0b1bd14e25f2f963b977702b2ee65bfe9cc6dc062ed64c2aae8fae853c50e227
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49397747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2f1d13828d02a2c177361462a428bf617736fb0c9a9ff9ab0e943b5ad4d9100`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 04:45:25 GMT
ADD file:0fafb7f95dc18699227154856361058bc9aba65de2ff88bf55cc66363142a05e in / 
# Wed, 20 Apr 2022 04:45:25 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:53:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 06:53:25 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 20 Apr 2022 06:53:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 06:53:33 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 06:53:33 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 06:53:33 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 06:53:33 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 06:53:33 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 06:53:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 06:53:33 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:8bd3f5a20b90c0e84cc65ea4a9172a51b7b5c0b9a097fa88d7102cac91cddf2c`  
		Last Modified: Wed, 20 Apr 2022 04:52:27 GMT  
		Size: 22.6 MB (22567235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d1c45c938fb4526994828d87717ecc6b59f277d8ebfc4e01a11e9523f3867a`  
		Last Modified: Wed, 20 Apr 2022 06:54:52 GMT  
		Size: 6.8 MB (6760462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d70b2c9386cc1e53eca36a7ac0e7cb71e58f94bb637562c89fcb8522b758b5e`  
		Last Modified: Wed, 20 Apr 2022 06:54:54 GMT  
		Size: 20.0 MB (20045657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a28dbe2987a34ceecefcbb3faceecc5336afd8db5ecb566e17dbec16ae0abab`  
		Last Modified: Wed, 20 Apr 2022 06:54:51 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b32f242dd51424300feb9aab9d19d5c8193853c590098d39aff7e1ea2a287b`  
		Last Modified: Wed, 20 Apr 2022 06:54:50 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e624d31c053076cc0774335740470d6b5d923b31f73cc867e265a3f919edc9ac`  
		Last Modified: Wed, 20 Apr 2022 06:54:51 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:971888d95702a5de9185e6839e1e60f006eec18baa96e54d342936eb36f2c54e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43986024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b52c780aacf75c582a3c62ddf1a0a1ed01e684b3ad80e460cf8d63aa2185e09`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 13:33:51 GMT
ADD file:096692331564a30a9a9c6b24e681d99d68b54eeeabb7c5ac7d4073de06e050b2 in / 
# Wed, 20 Apr 2022 13:33:51 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:44:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 20:44:12 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 20 Apr 2022 20:44:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 20:44:31 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 20:44:31 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 20:44:31 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 20:44:32 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 20:44:32 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 20:44:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 20:44:33 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:08da560f0b65b004ba95f9a431d3ac51b8807b16ec6ef170e2e00dc55330246d`  
		Last Modified: Wed, 20 Apr 2022 13:51:07 GMT  
		Size: 19.4 MB (19359807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b404038787532b9a02cd78f02daf4f9413398993cee60ba553069a25266fc2`  
		Last Modified: Wed, 20 Apr 2022 20:47:53 GMT  
		Size: 5.8 MB (5780828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416c8f7a646f2b86823f942eda691b04bf08081aded6323c3004d17f571c6c1e`  
		Last Modified: Wed, 20 Apr 2022 20:48:03 GMT  
		Size: 18.8 MB (18820997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9161aa5fba7e55069bc6f18c09fc1590c962d07f9df8acada3eaaa85c8a4a9`  
		Last Modified: Wed, 20 Apr 2022 20:47:50 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d2fbb32bb0db70fb38285e8cd72ef8715f4259c435b6701786e4d9169a75e1`  
		Last Modified: Wed, 20 Apr 2022 20:47:50 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8a123003d9adf87a4e08f8af00b1c49aba0fab0b3db21b45d996295d070a48`  
		Last Modified: Wed, 20 Apr 2022 20:47:50 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:83a56793fd10b8c564f40c805de7ca089a8a6b39def0fb1e189247929b280dfc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45457051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:987d0edc1b202fcd6d670530dd459477873b80f251702c330d3b3186e4f9b0eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 04:31:34 GMT
ADD file:02ad9214474cf0e6d278d7015dee30e6a8e24cdc699812f5fb3915491177e92b in / 
# Wed, 20 Apr 2022 04:31:34 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:59:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 06:59:32 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 20 Apr 2022 06:59:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 06:59:41 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 06:59:42 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 06:59:42 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 06:59:43 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 06:59:45 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 06:59:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 06:59:46 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0fca491399855be4c9b780dca621b48440831235d7916e5695b876698df84db7`  
		Last Modified: Wed, 20 Apr 2022 04:40:05 GMT  
		Size: 20.4 MB (20424115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e40f4666ba5562961008676822baf755b62dc19df0f3c8f7afb99d53358f0b`  
		Last Modified: Wed, 20 Apr 2022 07:01:24 GMT  
		Size: 6.0 MB (6047044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816d166b6c0ca1feca6fdda4cf5d0533f4dacb479862c9e0f8d97636b367ec85`  
		Last Modified: Wed, 20 Apr 2022 07:01:26 GMT  
		Size: 19.0 MB (18961506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2b0ff128586f79a8c97b75db01c5544b88a96ea74c495e46b53b567930a868`  
		Last Modified: Wed, 20 Apr 2022 07:01:23 GMT  
		Size: 12.2 KB (12242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14458e0e6ba5fa4fa0ea86860c36402079764415f00b0fd4d8247bc4df70911`  
		Last Modified: Wed, 20 Apr 2022 07:01:23 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b86b80570f2dc4fa9d5d3616a0183c97f9f593bcc78f6cd3d1dfa709e902b10`  
		Last Modified: Wed, 20 Apr 2022 07:01:23 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6-alpine`

```console
$ docker pull chronograf@sha256:23417672f50b4d8e10c2afe16fb30256ea18d11c8b18476774bb7d582d31d80c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.6-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:6f8f433011148165c541c6c2b5a4e5b6a0e17ed7a30e489da79572ffb65511b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14852447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7955bca787a43198659959f56224c8b4bcdcec4f04756f3179ed0041b6b3c97a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:26:16 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 04:26:16 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 05 Apr 2022 04:26:20 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 05 Apr 2022 04:26:20 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Tue, 05 Apr 2022 04:26:20 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 05 Apr 2022 04:26:20 GMT
EXPOSE 8888
# Tue, 05 Apr 2022 04:26:20 GMT
VOLUME [/var/lib/chronograf]
# Tue, 05 Apr 2022 04:26:21 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Tue, 05 Apr 2022 04:26:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 04:26:21 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58beb826c7b7288de69f85c4476fd6f04b58ceed760dd1b9e51a7d80aeb0e471`  
		Last Modified: Tue, 05 Apr 2022 04:27:20 GMT  
		Size: 271.7 KB (271678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec6a02657fcad83f14ccaebfe65596c725dc1a85062cc10c59315a08a6b4139`  
		Last Modified: Tue, 05 Apr 2022 04:27:21 GMT  
		Size: 11.7 MB (11737836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f48b6b7852557acd0c24a3412aff3571ae06abe1235cec3ae3c10d78c63a7f`  
		Last Modified: Tue, 05 Apr 2022 04:27:20 GMT  
		Size: 12.3 KB (12274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216f28bcf9418aa7355c3934973e69b52e1bba48dd0e758a66049eaef57cbd96`  
		Last Modified: Tue, 05 Apr 2022 04:27:20 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d36456c8c8f7725ba610682fd161c3b25b5bc41b4a3e2a9d384a197f9d65cc0`  
		Last Modified: Tue, 05 Apr 2022 04:27:19 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2`

```console
$ docker pull chronograf@sha256:f4bf6ff1804b4af9d1b3f37db2bac9caccf47fb15a8d353397b79119bc98c0b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6.2` - linux; amd64

```console
$ docker pull chronograf@sha256:0b1bd14e25f2f963b977702b2ee65bfe9cc6dc062ed64c2aae8fae853c50e227
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49397747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2f1d13828d02a2c177361462a428bf617736fb0c9a9ff9ab0e943b5ad4d9100`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 04:45:25 GMT
ADD file:0fafb7f95dc18699227154856361058bc9aba65de2ff88bf55cc66363142a05e in / 
# Wed, 20 Apr 2022 04:45:25 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:53:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 06:53:25 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 20 Apr 2022 06:53:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 06:53:33 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 06:53:33 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 06:53:33 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 06:53:33 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 06:53:33 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 06:53:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 06:53:33 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:8bd3f5a20b90c0e84cc65ea4a9172a51b7b5c0b9a097fa88d7102cac91cddf2c`  
		Last Modified: Wed, 20 Apr 2022 04:52:27 GMT  
		Size: 22.6 MB (22567235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d1c45c938fb4526994828d87717ecc6b59f277d8ebfc4e01a11e9523f3867a`  
		Last Modified: Wed, 20 Apr 2022 06:54:52 GMT  
		Size: 6.8 MB (6760462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d70b2c9386cc1e53eca36a7ac0e7cb71e58f94bb637562c89fcb8522b758b5e`  
		Last Modified: Wed, 20 Apr 2022 06:54:54 GMT  
		Size: 20.0 MB (20045657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a28dbe2987a34ceecefcbb3faceecc5336afd8db5ecb566e17dbec16ae0abab`  
		Last Modified: Wed, 20 Apr 2022 06:54:51 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b32f242dd51424300feb9aab9d19d5c8193853c590098d39aff7e1ea2a287b`  
		Last Modified: Wed, 20 Apr 2022 06:54:50 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e624d31c053076cc0774335740470d6b5d923b31f73cc867e265a3f919edc9ac`  
		Last Modified: Wed, 20 Apr 2022 06:54:51 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:971888d95702a5de9185e6839e1e60f006eec18baa96e54d342936eb36f2c54e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43986024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b52c780aacf75c582a3c62ddf1a0a1ed01e684b3ad80e460cf8d63aa2185e09`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 13:33:51 GMT
ADD file:096692331564a30a9a9c6b24e681d99d68b54eeeabb7c5ac7d4073de06e050b2 in / 
# Wed, 20 Apr 2022 13:33:51 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:44:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 20:44:12 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 20 Apr 2022 20:44:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 20:44:31 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 20:44:31 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 20:44:31 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 20:44:32 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 20:44:32 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 20:44:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 20:44:33 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:08da560f0b65b004ba95f9a431d3ac51b8807b16ec6ef170e2e00dc55330246d`  
		Last Modified: Wed, 20 Apr 2022 13:51:07 GMT  
		Size: 19.4 MB (19359807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b404038787532b9a02cd78f02daf4f9413398993cee60ba553069a25266fc2`  
		Last Modified: Wed, 20 Apr 2022 20:47:53 GMT  
		Size: 5.8 MB (5780828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416c8f7a646f2b86823f942eda691b04bf08081aded6323c3004d17f571c6c1e`  
		Last Modified: Wed, 20 Apr 2022 20:48:03 GMT  
		Size: 18.8 MB (18820997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9161aa5fba7e55069bc6f18c09fc1590c962d07f9df8acada3eaaa85c8a4a9`  
		Last Modified: Wed, 20 Apr 2022 20:47:50 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d2fbb32bb0db70fb38285e8cd72ef8715f4259c435b6701786e4d9169a75e1`  
		Last Modified: Wed, 20 Apr 2022 20:47:50 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8a123003d9adf87a4e08f8af00b1c49aba0fab0b3db21b45d996295d070a48`  
		Last Modified: Wed, 20 Apr 2022 20:47:50 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:83a56793fd10b8c564f40c805de7ca089a8a6b39def0fb1e189247929b280dfc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45457051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:987d0edc1b202fcd6d670530dd459477873b80f251702c330d3b3186e4f9b0eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 04:31:34 GMT
ADD file:02ad9214474cf0e6d278d7015dee30e6a8e24cdc699812f5fb3915491177e92b in / 
# Wed, 20 Apr 2022 04:31:34 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:59:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 06:59:32 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 20 Apr 2022 06:59:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 06:59:41 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 06:59:42 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 06:59:42 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 06:59:43 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 06:59:45 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 06:59:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 06:59:46 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0fca491399855be4c9b780dca621b48440831235d7916e5695b876698df84db7`  
		Last Modified: Wed, 20 Apr 2022 04:40:05 GMT  
		Size: 20.4 MB (20424115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e40f4666ba5562961008676822baf755b62dc19df0f3c8f7afb99d53358f0b`  
		Last Modified: Wed, 20 Apr 2022 07:01:24 GMT  
		Size: 6.0 MB (6047044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816d166b6c0ca1feca6fdda4cf5d0533f4dacb479862c9e0f8d97636b367ec85`  
		Last Modified: Wed, 20 Apr 2022 07:01:26 GMT  
		Size: 19.0 MB (18961506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2b0ff128586f79a8c97b75db01c5544b88a96ea74c495e46b53b567930a868`  
		Last Modified: Wed, 20 Apr 2022 07:01:23 GMT  
		Size: 12.2 KB (12242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14458e0e6ba5fa4fa0ea86860c36402079764415f00b0fd4d8247bc4df70911`  
		Last Modified: Wed, 20 Apr 2022 07:01:23 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b86b80570f2dc4fa9d5d3616a0183c97f9f593bcc78f6cd3d1dfa709e902b10`  
		Last Modified: Wed, 20 Apr 2022 07:01:23 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2-alpine`

```console
$ docker pull chronograf@sha256:23417672f50b4d8e10c2afe16fb30256ea18d11c8b18476774bb7d582d31d80c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.6.2-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:6f8f433011148165c541c6c2b5a4e5b6a0e17ed7a30e489da79572ffb65511b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14852447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7955bca787a43198659959f56224c8b4bcdcec4f04756f3179ed0041b6b3c97a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:26:16 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 04:26:16 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 05 Apr 2022 04:26:20 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 05 Apr 2022 04:26:20 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Tue, 05 Apr 2022 04:26:20 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 05 Apr 2022 04:26:20 GMT
EXPOSE 8888
# Tue, 05 Apr 2022 04:26:20 GMT
VOLUME [/var/lib/chronograf]
# Tue, 05 Apr 2022 04:26:21 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Tue, 05 Apr 2022 04:26:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 04:26:21 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58beb826c7b7288de69f85c4476fd6f04b58ceed760dd1b9e51a7d80aeb0e471`  
		Last Modified: Tue, 05 Apr 2022 04:27:20 GMT  
		Size: 271.7 KB (271678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec6a02657fcad83f14ccaebfe65596c725dc1a85062cc10c59315a08a6b4139`  
		Last Modified: Tue, 05 Apr 2022 04:27:21 GMT  
		Size: 11.7 MB (11737836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f48b6b7852557acd0c24a3412aff3571ae06abe1235cec3ae3c10d78c63a7f`  
		Last Modified: Tue, 05 Apr 2022 04:27:20 GMT  
		Size: 12.3 KB (12274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216f28bcf9418aa7355c3934973e69b52e1bba48dd0e758a66049eaef57cbd96`  
		Last Modified: Tue, 05 Apr 2022 04:27:20 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d36456c8c8f7725ba610682fd161c3b25b5bc41b4a3e2a9d384a197f9d65cc0`  
		Last Modified: Tue, 05 Apr 2022 04:27:19 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7`

```console
$ docker pull chronograf@sha256:d93782e82d32eb2c87e652421ebc0efe9f54b3a74e10d0299668479fa39dbc12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7` - linux; amd64

```console
$ docker pull chronograf@sha256:be1dd1911b4e60cb1eef578ac4fe4c625a42b81f746cd3630265d617105b4900
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65426989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9baa124cdcc2f02cb7c6329c0efd3ef99c63b0973a02a76cdbba0b5fa6bde72`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 04:45:25 GMT
ADD file:0fafb7f95dc18699227154856361058bc9aba65de2ff88bf55cc66363142a05e in / 
# Wed, 20 Apr 2022 04:45:25 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:53:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 06:53:47 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 20 Apr 2022 06:53:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 06:53:58 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 06:53:58 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 06:53:58 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 06:53:58 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 06:53:58 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 06:53:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 06:53:58 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:8bd3f5a20b90c0e84cc65ea4a9172a51b7b5c0b9a097fa88d7102cac91cddf2c`  
		Last Modified: Wed, 20 Apr 2022 04:52:27 GMT  
		Size: 22.6 MB (22567235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da204c9653f9c0837667da82f54ff584cd171627934b98d3151b843bf61cdb4`  
		Last Modified: Wed, 20 Apr 2022 06:55:05 GMT  
		Size: 4.5 MB (4506795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8dbdc881d509fc523e142df82d6d87afea9581b2da5cd8a33f1d0dbc22e2a0`  
		Last Modified: Wed, 20 Apr 2022 06:55:10 GMT  
		Size: 38.3 MB (38328563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c81bcf05f6c1162c425df5b8193b0b2338cb8d60bbeec1fbd9308cfab86bbd`  
		Last Modified: Wed, 20 Apr 2022 06:55:04 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7574fedf2ec643d07956ae2edcea6d16aef45724670f8c9b654b87d0a77f1f96`  
		Last Modified: Wed, 20 Apr 2022 06:55:04 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01f25936148706f4eda88ad4cc274dbaf55fe95fe075309f54a84d6654d57c9`  
		Last Modified: Wed, 20 Apr 2022 06:55:04 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:e7ec365a6954e07788a7ddb7aca194beda2460b7195c9a11f8915d75624445af
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (59048122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f9794af3bebd8469e95647ebfbf2b95f48415ddeb5d6380fa63736dd17f94f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 13:33:51 GMT
ADD file:096692331564a30a9a9c6b24e681d99d68b54eeeabb7c5ac7d4073de06e050b2 in / 
# Wed, 20 Apr 2022 13:33:51 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:45:06 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 20:45:07 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 20 Apr 2022 20:45:39 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 20:45:40 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 20:45:40 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 20:45:40 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 20:45:41 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 20:45:41 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 20:45:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 20:45:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:08da560f0b65b004ba95f9a431d3ac51b8807b16ec6ef170e2e00dc55330246d`  
		Last Modified: Wed, 20 Apr 2022 13:51:07 GMT  
		Size: 19.4 MB (19359807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8a6dca9e034bf11c1a9450661bac9b09ea57fb12ac3ed0e1561c2bdf9dfc67`  
		Last Modified: Wed, 20 Apr 2022 20:48:17 GMT  
		Size: 3.9 MB (3880171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23598a4e800556dcfe6d3f3a99a986a0f48f309d308139ec6c5694cffbb6f5e9`  
		Last Modified: Wed, 20 Apr 2022 20:48:35 GMT  
		Size: 35.8 MB (35783750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3aa82a8c3a7c91a41f390dc9f0a16a42d06c26e71f73dd20f5243ed77b2df62`  
		Last Modified: Wed, 20 Apr 2022 20:48:15 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54911414074d28d24f532f112b4584ba6fe2bdb7d219ab11a0b9ea04b14d26`  
		Last Modified: Wed, 20 Apr 2022 20:48:15 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87357fe9bb4e66d2375f1f1b0687f3207ff31396b5eb8a7ea5748ebeedf8424`  
		Last Modified: Wed, 20 Apr 2022 20:48:15 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:525bc2b4bbaa71d4b72c984d0b1f25c7b7db44e22d99a75a8a6ba4c8ac8d0450
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60329536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:705d3dc43eb4547bb50ff3f62b0b8cb765f5a383b12c8e7d00875595e017f09b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 04:31:34 GMT
ADD file:02ad9214474cf0e6d278d7015dee30e6a8e24cdc699812f5fb3915491177e92b in / 
# Wed, 20 Apr 2022 04:31:34 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:59:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 06:59:59 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 20 Apr 2022 07:00:10 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 07:00:12 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 07:00:13 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 07:00:13 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 07:00:14 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 07:00:16 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 07:00:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 07:00:17 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0fca491399855be4c9b780dca621b48440831235d7916e5695b876698df84db7`  
		Last Modified: Wed, 20 Apr 2022 04:40:05 GMT  
		Size: 20.4 MB (20424115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfcd7b161a5360bb61794a7b56341cefff4c84503e2637519d9aa33301c0788`  
		Last Modified: Wed, 20 Apr 2022 07:01:38 GMT  
		Size: 3.9 MB (3893924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a532c04775c96fd665e684692e71018273901bb0add4640f14474d3d064b6339`  
		Last Modified: Wed, 20 Apr 2022 07:01:42 GMT  
		Size: 36.0 MB (35987103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51d17add7b54b2c55bf117b4fb083ba356565e50b505649f3ed039450ea6aec`  
		Last Modified: Wed, 20 Apr 2022 07:01:37 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c3e787f99292c161ff3afb8e36bb9b083b1312f374b40912d0fb2491ccfeb83`  
		Last Modified: Wed, 20 Apr 2022 07:01:37 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845c8bedacd9a5421bddd470498c3048fc02c28039b31743ffdb029a9beca29c`  
		Last Modified: Wed, 20 Apr 2022 07:01:37 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7-alpine`

```console
$ docker pull chronograf@sha256:990421b8bc9b5dd6d472bd68efb5b165bf5f909c1b4a841756198933b14513d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.7-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:386f11aba61ccd79dd3d8105edce283d4eac402a7c92b802beb7ad89cf3136a1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22670798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf7c75f57862ead544bf92efebf86f59028a171990d14514c9cc621d7807042a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:26:16 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 04:26:26 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 05 Apr 2022 04:26:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 05 Apr 2022 04:26:31 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 05 Apr 2022 04:26:31 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 05 Apr 2022 04:26:31 GMT
EXPOSE 8888
# Tue, 05 Apr 2022 04:26:32 GMT
VOLUME [/var/lib/chronograf]
# Tue, 05 Apr 2022 04:26:32 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Tue, 05 Apr 2022 04:26:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 04:26:32 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58beb826c7b7288de69f85c4476fd6f04b58ceed760dd1b9e51a7d80aeb0e471`  
		Last Modified: Tue, 05 Apr 2022 04:27:20 GMT  
		Size: 271.7 KB (271678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8ba42ef9e34fc8eb0a6b88a3cd9242247e7029eaaed6b3d13f3f77eba9bb4f`  
		Last Modified: Tue, 05 Apr 2022 04:27:35 GMT  
		Size: 19.6 MB (19556196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e98e5f05434dd7e69e4acfb1c9682f93ab2c0d204b09dac76ccbc8fac82952`  
		Last Modified: Tue, 05 Apr 2022 04:27:32 GMT  
		Size: 12.3 KB (12264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12636f40cb960e763e7c41f0b801007ade339c74aac79418124da7df48f27a7f`  
		Last Modified: Tue, 05 Apr 2022 04:27:32 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7c964b7b93ca840cc02a49bcee2e824dccd67e40f48c0d16b239cc3b3e2be1`  
		Last Modified: Tue, 05 Apr 2022 04:27:32 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17`

```console
$ docker pull chronograf@sha256:d93782e82d32eb2c87e652421ebc0efe9f54b3a74e10d0299668479fa39dbc12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7.17` - linux; amd64

```console
$ docker pull chronograf@sha256:be1dd1911b4e60cb1eef578ac4fe4c625a42b81f746cd3630265d617105b4900
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65426989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9baa124cdcc2f02cb7c6329c0efd3ef99c63b0973a02a76cdbba0b5fa6bde72`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 04:45:25 GMT
ADD file:0fafb7f95dc18699227154856361058bc9aba65de2ff88bf55cc66363142a05e in / 
# Wed, 20 Apr 2022 04:45:25 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:53:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 06:53:47 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 20 Apr 2022 06:53:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 06:53:58 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 06:53:58 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 06:53:58 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 06:53:58 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 06:53:58 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 06:53:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 06:53:58 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:8bd3f5a20b90c0e84cc65ea4a9172a51b7b5c0b9a097fa88d7102cac91cddf2c`  
		Last Modified: Wed, 20 Apr 2022 04:52:27 GMT  
		Size: 22.6 MB (22567235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da204c9653f9c0837667da82f54ff584cd171627934b98d3151b843bf61cdb4`  
		Last Modified: Wed, 20 Apr 2022 06:55:05 GMT  
		Size: 4.5 MB (4506795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8dbdc881d509fc523e142df82d6d87afea9581b2da5cd8a33f1d0dbc22e2a0`  
		Last Modified: Wed, 20 Apr 2022 06:55:10 GMT  
		Size: 38.3 MB (38328563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c81bcf05f6c1162c425df5b8193b0b2338cb8d60bbeec1fbd9308cfab86bbd`  
		Last Modified: Wed, 20 Apr 2022 06:55:04 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7574fedf2ec643d07956ae2edcea6d16aef45724670f8c9b654b87d0a77f1f96`  
		Last Modified: Wed, 20 Apr 2022 06:55:04 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01f25936148706f4eda88ad4cc274dbaf55fe95fe075309f54a84d6654d57c9`  
		Last Modified: Wed, 20 Apr 2022 06:55:04 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:e7ec365a6954e07788a7ddb7aca194beda2460b7195c9a11f8915d75624445af
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (59048122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f9794af3bebd8469e95647ebfbf2b95f48415ddeb5d6380fa63736dd17f94f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 13:33:51 GMT
ADD file:096692331564a30a9a9c6b24e681d99d68b54eeeabb7c5ac7d4073de06e050b2 in / 
# Wed, 20 Apr 2022 13:33:51 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:45:06 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 20:45:07 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 20 Apr 2022 20:45:39 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 20:45:40 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 20:45:40 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 20:45:40 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 20:45:41 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 20:45:41 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 20:45:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 20:45:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:08da560f0b65b004ba95f9a431d3ac51b8807b16ec6ef170e2e00dc55330246d`  
		Last Modified: Wed, 20 Apr 2022 13:51:07 GMT  
		Size: 19.4 MB (19359807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8a6dca9e034bf11c1a9450661bac9b09ea57fb12ac3ed0e1561c2bdf9dfc67`  
		Last Modified: Wed, 20 Apr 2022 20:48:17 GMT  
		Size: 3.9 MB (3880171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23598a4e800556dcfe6d3f3a99a986a0f48f309d308139ec6c5694cffbb6f5e9`  
		Last Modified: Wed, 20 Apr 2022 20:48:35 GMT  
		Size: 35.8 MB (35783750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3aa82a8c3a7c91a41f390dc9f0a16a42d06c26e71f73dd20f5243ed77b2df62`  
		Last Modified: Wed, 20 Apr 2022 20:48:15 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54911414074d28d24f532f112b4584ba6fe2bdb7d219ab11a0b9ea04b14d26`  
		Last Modified: Wed, 20 Apr 2022 20:48:15 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87357fe9bb4e66d2375f1f1b0687f3207ff31396b5eb8a7ea5748ebeedf8424`  
		Last Modified: Wed, 20 Apr 2022 20:48:15 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:525bc2b4bbaa71d4b72c984d0b1f25c7b7db44e22d99a75a8a6ba4c8ac8d0450
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60329536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:705d3dc43eb4547bb50ff3f62b0b8cb765f5a383b12c8e7d00875595e017f09b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 04:31:34 GMT
ADD file:02ad9214474cf0e6d278d7015dee30e6a8e24cdc699812f5fb3915491177e92b in / 
# Wed, 20 Apr 2022 04:31:34 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:59:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 06:59:59 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 20 Apr 2022 07:00:10 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 07:00:12 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 07:00:13 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 07:00:13 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 07:00:14 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 07:00:16 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 07:00:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 07:00:17 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0fca491399855be4c9b780dca621b48440831235d7916e5695b876698df84db7`  
		Last Modified: Wed, 20 Apr 2022 04:40:05 GMT  
		Size: 20.4 MB (20424115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfcd7b161a5360bb61794a7b56341cefff4c84503e2637519d9aa33301c0788`  
		Last Modified: Wed, 20 Apr 2022 07:01:38 GMT  
		Size: 3.9 MB (3893924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a532c04775c96fd665e684692e71018273901bb0add4640f14474d3d064b6339`  
		Last Modified: Wed, 20 Apr 2022 07:01:42 GMT  
		Size: 36.0 MB (35987103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51d17add7b54b2c55bf117b4fb083ba356565e50b505649f3ed039450ea6aec`  
		Last Modified: Wed, 20 Apr 2022 07:01:37 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c3e787f99292c161ff3afb8e36bb9b083b1312f374b40912d0fb2491ccfeb83`  
		Last Modified: Wed, 20 Apr 2022 07:01:37 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845c8bedacd9a5421bddd470498c3048fc02c28039b31743ffdb029a9beca29c`  
		Last Modified: Wed, 20 Apr 2022 07:01:37 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17-alpine`

```console
$ docker pull chronograf@sha256:990421b8bc9b5dd6d472bd68efb5b165bf5f909c1b4a841756198933b14513d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.7.17-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:386f11aba61ccd79dd3d8105edce283d4eac402a7c92b802beb7ad89cf3136a1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22670798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf7c75f57862ead544bf92efebf86f59028a171990d14514c9cc621d7807042a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:26:16 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 04:26:26 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 05 Apr 2022 04:26:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 05 Apr 2022 04:26:31 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 05 Apr 2022 04:26:31 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 05 Apr 2022 04:26:31 GMT
EXPOSE 8888
# Tue, 05 Apr 2022 04:26:32 GMT
VOLUME [/var/lib/chronograf]
# Tue, 05 Apr 2022 04:26:32 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Tue, 05 Apr 2022 04:26:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 04:26:32 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58beb826c7b7288de69f85c4476fd6f04b58ceed760dd1b9e51a7d80aeb0e471`  
		Last Modified: Tue, 05 Apr 2022 04:27:20 GMT  
		Size: 271.7 KB (271678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8ba42ef9e34fc8eb0a6b88a3cd9242247e7029eaaed6b3d13f3f77eba9bb4f`  
		Last Modified: Tue, 05 Apr 2022 04:27:35 GMT  
		Size: 19.6 MB (19556196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e98e5f05434dd7e69e4acfb1c9682f93ab2c0d204b09dac76ccbc8fac82952`  
		Last Modified: Tue, 05 Apr 2022 04:27:32 GMT  
		Size: 12.3 KB (12264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12636f40cb960e763e7c41f0b801007ade339c74aac79418124da7df48f27a7f`  
		Last Modified: Tue, 05 Apr 2022 04:27:32 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7c964b7b93ca840cc02a49bcee2e824dccd67e40f48c0d16b239cc3b3e2be1`  
		Last Modified: Tue, 05 Apr 2022 04:27:32 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8`

```console
$ docker pull chronograf@sha256:ab33399a75a776e3c9c36cf4344b0e99b0cf60492db8815643f80ec1430fdac8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8` - linux; amd64

```console
$ docker pull chronograf@sha256:afbea9841d7712cec331374cf09f97a34def0ff462bce5df52dd0d9d20158cb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66278725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b866f88d6f7decc03f2b3979dc69ee7f75c6f887ff0fe25f07d404d6c9018e0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 04:45:25 GMT
ADD file:0fafb7f95dc18699227154856361058bc9aba65de2ff88bf55cc66363142a05e in / 
# Wed, 20 Apr 2022 04:45:25 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:53:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 06:54:05 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 20 Apr 2022 06:54:13 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 06:54:13 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 06:54:13 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 06:54:13 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 06:54:13 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 06:54:13 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 06:54:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 06:54:14 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:8bd3f5a20b90c0e84cc65ea4a9172a51b7b5c0b9a097fa88d7102cac91cddf2c`  
		Last Modified: Wed, 20 Apr 2022 04:52:27 GMT  
		Size: 22.6 MB (22567235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d1c45c938fb4526994828d87717ecc6b59f277d8ebfc4e01a11e9523f3867a`  
		Last Modified: Wed, 20 Apr 2022 06:54:52 GMT  
		Size: 6.8 MB (6760462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86041e6482a1f673aaafcf79aaf900aa48cfeab3dc770d17b7edb4c672cded04`  
		Last Modified: Wed, 20 Apr 2022 06:55:25 GMT  
		Size: 36.9 MB (36926635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b852d514975a0f26666598767ff55f58365b783fbc7e51bf1e71012fe10c69cd`  
		Last Modified: Wed, 20 Apr 2022 06:55:20 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d18aa921959f0bf043738349d836c7e12498a25ac89b83ff0cb9a8221c9fe5`  
		Last Modified: Wed, 20 Apr 2022 06:55:20 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4485fc2cb8d2f94ff964c537aa37ddabf82d735c744a6281380bfb95e4b0a102`  
		Last Modified: Wed, 20 Apr 2022 06:55:20 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:bd1e861decc262dbab541dfdafc11690ec8b58a4acf8770fe3034bb7b70907eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.7 MB (59677011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4d33cd12c12fb24a32514095d07063cc0e82acc3f13e3dc5c46ad86888a5046`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 13:33:51 GMT
ADD file:096692331564a30a9a9c6b24e681d99d68b54eeeabb7c5ac7d4073de06e050b2 in / 
# Wed, 20 Apr 2022 13:33:51 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:44:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 20:46:00 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 20 Apr 2022 20:46:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 20:46:20 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 20:46:21 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 20:46:21 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 20:46:22 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 20:46:22 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 20:46:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 20:46:23 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:08da560f0b65b004ba95f9a431d3ac51b8807b16ec6ef170e2e00dc55330246d`  
		Last Modified: Wed, 20 Apr 2022 13:51:07 GMT  
		Size: 19.4 MB (19359807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b404038787532b9a02cd78f02daf4f9413398993cee60ba553069a25266fc2`  
		Last Modified: Wed, 20 Apr 2022 20:47:53 GMT  
		Size: 5.8 MB (5780828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0386e28777a2df834a2289c8406b4f76d8783eed0ce948f024b53e84bdd203d8`  
		Last Modified: Wed, 20 Apr 2022 20:49:05 GMT  
		Size: 34.5 MB (34511981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e67fd1ed1b544d73cf39eb0f133a2b37222c478e6ba4ca6c86e56c6f2de900`  
		Last Modified: Wed, 20 Apr 2022 20:48:46 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76c94e5cdacd977353c02e1f153f00e3ee51cc0d8e529601f0825470435c13e`  
		Last Modified: Wed, 20 Apr 2022 20:48:46 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f177f6d3579e4acd920d4e9be6476f47d836e6aeffa5d1e91adb45950f35b33e`  
		Last Modified: Wed, 20 Apr 2022 20:48:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:88b242852106221964ba3c0e748e1992ebf15e8ec1bdcf770272c37a0deb1fc2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.9 MB (60927120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2e5208faa62a3c970aeb479d9c89621ebcf9881007bfaa74bb6e7827550597`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 04:31:34 GMT
ADD file:02ad9214474cf0e6d278d7015dee30e6a8e24cdc699812f5fb3915491177e92b in / 
# Wed, 20 Apr 2022 04:31:34 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:59:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 07:00:23 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 20 Apr 2022 07:00:31 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 07:00:32 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 07:00:33 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 07:00:33 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 07:00:34 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 07:00:36 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 07:00:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 07:00:37 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0fca491399855be4c9b780dca621b48440831235d7916e5695b876698df84db7`  
		Last Modified: Wed, 20 Apr 2022 04:40:05 GMT  
		Size: 20.4 MB (20424115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e40f4666ba5562961008676822baf755b62dc19df0f3c8f7afb99d53358f0b`  
		Last Modified: Wed, 20 Apr 2022 07:01:24 GMT  
		Size: 6.0 MB (6047044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd062c0f3097c1f89277d00a63026b533b5db5a95fbaab64e16872cf3ccbcbe4`  
		Last Modified: Wed, 20 Apr 2022 07:02:02 GMT  
		Size: 34.4 MB (34431569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26a961293f906c6f2635c4fb187fee69974d01e1449a720cb78f56f0eff83b0`  
		Last Modified: Wed, 20 Apr 2022 07:01:58 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6979e471c50c9c094080708c78d45bcea2ae39ed2cd5e3ad5d622216683c47`  
		Last Modified: Wed, 20 Apr 2022 07:01:58 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ca22c1d0daf7b02d4a33b9a70cc25f076abb53e3fc405c14810cfadcb8afb7`  
		Last Modified: Wed, 20 Apr 2022 07:01:58 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8-alpine`

```console
$ docker pull chronograf@sha256:d3e3bbce6ab55cead013b905eba19cdd95cc418e5f2acfb421159ccc1bf8cbd3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:b28beb85949241c005e5be21181999ce565e4b29dd96295f7e2f7d8ff833a80a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22318581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cb7b4f19d3448b5e558e8d6e7857db12751a4b8a0928e3f0fa36efaa296650b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:26:16 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 04:26:37 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 05 Apr 2022 04:26:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 05 Apr 2022 04:26:43 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 05 Apr 2022 04:26:43 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 05 Apr 2022 04:26:43 GMT
EXPOSE 8888
# Tue, 05 Apr 2022 04:26:43 GMT
VOLUME [/var/lib/chronograf]
# Tue, 05 Apr 2022 04:26:43 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Tue, 05 Apr 2022 04:26:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 04:26:43 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58beb826c7b7288de69f85c4476fd6f04b58ceed760dd1b9e51a7d80aeb0e471`  
		Last Modified: Tue, 05 Apr 2022 04:27:20 GMT  
		Size: 271.7 KB (271678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e780df476439b3a8749d6d1ec5009124d7cb47b7328d520390e5c1df5e5260f7`  
		Last Modified: Tue, 05 Apr 2022 04:27:49 GMT  
		Size: 19.2 MB (19203976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770779eb24c794631aa560ebb5145f2fd7a4bf2972a43459d9321581fc47084e`  
		Last Modified: Tue, 05 Apr 2022 04:27:45 GMT  
		Size: 12.3 KB (12267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e1701788eafedc43dca0570322f1ab0c00388a8d9a882173a472e4cc23774b`  
		Last Modified: Tue, 05 Apr 2022 04:27:45 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51eec10863e13223024d57ee99337a425873b97b7b2829d8f207c267a414b201`  
		Last Modified: Tue, 05 Apr 2022 04:27:45 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.10`

```console
$ docker pull chronograf@sha256:ab33399a75a776e3c9c36cf4344b0e99b0cf60492db8815643f80ec1430fdac8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8.10` - linux; amd64

```console
$ docker pull chronograf@sha256:afbea9841d7712cec331374cf09f97a34def0ff462bce5df52dd0d9d20158cb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66278725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b866f88d6f7decc03f2b3979dc69ee7f75c6f887ff0fe25f07d404d6c9018e0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 04:45:25 GMT
ADD file:0fafb7f95dc18699227154856361058bc9aba65de2ff88bf55cc66363142a05e in / 
# Wed, 20 Apr 2022 04:45:25 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:53:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 06:54:05 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 20 Apr 2022 06:54:13 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 06:54:13 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 06:54:13 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 06:54:13 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 06:54:13 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 06:54:13 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 06:54:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 06:54:14 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:8bd3f5a20b90c0e84cc65ea4a9172a51b7b5c0b9a097fa88d7102cac91cddf2c`  
		Last Modified: Wed, 20 Apr 2022 04:52:27 GMT  
		Size: 22.6 MB (22567235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d1c45c938fb4526994828d87717ecc6b59f277d8ebfc4e01a11e9523f3867a`  
		Last Modified: Wed, 20 Apr 2022 06:54:52 GMT  
		Size: 6.8 MB (6760462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86041e6482a1f673aaafcf79aaf900aa48cfeab3dc770d17b7edb4c672cded04`  
		Last Modified: Wed, 20 Apr 2022 06:55:25 GMT  
		Size: 36.9 MB (36926635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b852d514975a0f26666598767ff55f58365b783fbc7e51bf1e71012fe10c69cd`  
		Last Modified: Wed, 20 Apr 2022 06:55:20 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d18aa921959f0bf043738349d836c7e12498a25ac89b83ff0cb9a8221c9fe5`  
		Last Modified: Wed, 20 Apr 2022 06:55:20 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4485fc2cb8d2f94ff964c537aa37ddabf82d735c744a6281380bfb95e4b0a102`  
		Last Modified: Wed, 20 Apr 2022 06:55:20 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.10` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:bd1e861decc262dbab541dfdafc11690ec8b58a4acf8770fe3034bb7b70907eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.7 MB (59677011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4d33cd12c12fb24a32514095d07063cc0e82acc3f13e3dc5c46ad86888a5046`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 13:33:51 GMT
ADD file:096692331564a30a9a9c6b24e681d99d68b54eeeabb7c5ac7d4073de06e050b2 in / 
# Wed, 20 Apr 2022 13:33:51 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:44:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 20:46:00 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 20 Apr 2022 20:46:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 20:46:20 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 20:46:21 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 20:46:21 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 20:46:22 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 20:46:22 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 20:46:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 20:46:23 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:08da560f0b65b004ba95f9a431d3ac51b8807b16ec6ef170e2e00dc55330246d`  
		Last Modified: Wed, 20 Apr 2022 13:51:07 GMT  
		Size: 19.4 MB (19359807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b404038787532b9a02cd78f02daf4f9413398993cee60ba553069a25266fc2`  
		Last Modified: Wed, 20 Apr 2022 20:47:53 GMT  
		Size: 5.8 MB (5780828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0386e28777a2df834a2289c8406b4f76d8783eed0ce948f024b53e84bdd203d8`  
		Last Modified: Wed, 20 Apr 2022 20:49:05 GMT  
		Size: 34.5 MB (34511981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e67fd1ed1b544d73cf39eb0f133a2b37222c478e6ba4ca6c86e56c6f2de900`  
		Last Modified: Wed, 20 Apr 2022 20:48:46 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76c94e5cdacd977353c02e1f153f00e3ee51cc0d8e529601f0825470435c13e`  
		Last Modified: Wed, 20 Apr 2022 20:48:46 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f177f6d3579e4acd920d4e9be6476f47d836e6aeffa5d1e91adb45950f35b33e`  
		Last Modified: Wed, 20 Apr 2022 20:48:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.10` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:88b242852106221964ba3c0e748e1992ebf15e8ec1bdcf770272c37a0deb1fc2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.9 MB (60927120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2e5208faa62a3c970aeb479d9c89621ebcf9881007bfaa74bb6e7827550597`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 04:31:34 GMT
ADD file:02ad9214474cf0e6d278d7015dee30e6a8e24cdc699812f5fb3915491177e92b in / 
# Wed, 20 Apr 2022 04:31:34 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:59:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 07:00:23 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 20 Apr 2022 07:00:31 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 07:00:32 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 07:00:33 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 07:00:33 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 07:00:34 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 07:00:36 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 07:00:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 07:00:37 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0fca491399855be4c9b780dca621b48440831235d7916e5695b876698df84db7`  
		Last Modified: Wed, 20 Apr 2022 04:40:05 GMT  
		Size: 20.4 MB (20424115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e40f4666ba5562961008676822baf755b62dc19df0f3c8f7afb99d53358f0b`  
		Last Modified: Wed, 20 Apr 2022 07:01:24 GMT  
		Size: 6.0 MB (6047044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd062c0f3097c1f89277d00a63026b533b5db5a95fbaab64e16872cf3ccbcbe4`  
		Last Modified: Wed, 20 Apr 2022 07:02:02 GMT  
		Size: 34.4 MB (34431569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26a961293f906c6f2635c4fb187fee69974d01e1449a720cb78f56f0eff83b0`  
		Last Modified: Wed, 20 Apr 2022 07:01:58 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6979e471c50c9c094080708c78d45bcea2ae39ed2cd5e3ad5d622216683c47`  
		Last Modified: Wed, 20 Apr 2022 07:01:58 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ca22c1d0daf7b02d4a33b9a70cc25f076abb53e3fc405c14810cfadcb8afb7`  
		Last Modified: Wed, 20 Apr 2022 07:01:58 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.10-alpine`

```console
$ docker pull chronograf@sha256:d3e3bbce6ab55cead013b905eba19cdd95cc418e5f2acfb421159ccc1bf8cbd3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.8.10-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:b28beb85949241c005e5be21181999ce565e4b29dd96295f7e2f7d8ff833a80a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22318581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cb7b4f19d3448b5e558e8d6e7857db12751a4b8a0928e3f0fa36efaa296650b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:26:16 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 04:26:37 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 05 Apr 2022 04:26:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 05 Apr 2022 04:26:43 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 05 Apr 2022 04:26:43 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 05 Apr 2022 04:26:43 GMT
EXPOSE 8888
# Tue, 05 Apr 2022 04:26:43 GMT
VOLUME [/var/lib/chronograf]
# Tue, 05 Apr 2022 04:26:43 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Tue, 05 Apr 2022 04:26:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 04:26:43 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58beb826c7b7288de69f85c4476fd6f04b58ceed760dd1b9e51a7d80aeb0e471`  
		Last Modified: Tue, 05 Apr 2022 04:27:20 GMT  
		Size: 271.7 KB (271678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e780df476439b3a8749d6d1ec5009124d7cb47b7328d520390e5c1df5e5260f7`  
		Last Modified: Tue, 05 Apr 2022 04:27:49 GMT  
		Size: 19.2 MB (19203976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770779eb24c794631aa560ebb5145f2fd7a4bf2972a43459d9321581fc47084e`  
		Last Modified: Tue, 05 Apr 2022 04:27:45 GMT  
		Size: 12.3 KB (12267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e1701788eafedc43dca0570322f1ab0c00388a8d9a882173a472e4cc23774b`  
		Last Modified: Tue, 05 Apr 2022 04:27:45 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51eec10863e13223024d57ee99337a425873b97b7b2829d8f207c267a414b201`  
		Last Modified: Tue, 05 Apr 2022 04:27:45 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9`

```console
$ docker pull chronograf@sha256:b6ca8877aab7407b8a3ee9478bd8ac4a618e63bbaf9dc6bdba257550acc9f941
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.9` - linux; amd64

```console
$ docker pull chronograf@sha256:6033dc59b677c6aa6532339e3e793ad2b4cf6e3453ab6f3db9b72cd53983bbf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66922520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90c8c2f940e4acbaf6f20031d9769ab445024072f70ad7b2b7ffd446d4ff1bfb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 04:45:25 GMT
ADD file:0fafb7f95dc18699227154856361058bc9aba65de2ff88bf55cc66363142a05e in / 
# Wed, 20 Apr 2022 04:45:25 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:53:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 06:54:18 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 20 Apr 2022 06:54:26 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 06:54:26 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 06:54:26 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 06:54:26 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 06:54:26 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 06:54:26 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 06:54:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 06:54:27 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:8bd3f5a20b90c0e84cc65ea4a9172a51b7b5c0b9a097fa88d7102cac91cddf2c`  
		Last Modified: Wed, 20 Apr 2022 04:52:27 GMT  
		Size: 22.6 MB (22567235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d1c45c938fb4526994828d87717ecc6b59f277d8ebfc4e01a11e9523f3867a`  
		Last Modified: Wed, 20 Apr 2022 06:54:52 GMT  
		Size: 6.8 MB (6760462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c3707b0034bfaa5138ec2fe28e3b3bd5ee29a93eda25f36ec6cd99e909dbf0`  
		Last Modified: Wed, 20 Apr 2022 06:55:41 GMT  
		Size: 37.6 MB (37570443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1d14c56566c0f90fbaa893624b83fff4fe016c2ea573422f619debde21839a`  
		Last Modified: Wed, 20 Apr 2022 06:55:35 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40fecaa82ff715c3dcd9bf685a10e2b67f868770e9ce7450656a3c92cb429fe`  
		Last Modified: Wed, 20 Apr 2022 06:55:35 GMT  
		Size: 11.9 KB (11900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9177a78636ef84328dd8835647471f1c71832ff0eb77899a26c8d505e555f7`  
		Last Modified: Wed, 20 Apr 2022 06:55:36 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:7080ff4d4d25bd56dfc1698da8f915da5f2c6534355513bfcc7ba6979585c960
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60456520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68565f67efdeca82687fc4b9ebcc3ba19b8f864d41f19ebd0193b50bc2f009f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 13:33:51 GMT
ADD file:096692331564a30a9a9c6b24e681d99d68b54eeeabb7c5ac7d4073de06e050b2 in / 
# Wed, 20 Apr 2022 13:33:51 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:44:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 20:46:34 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 20 Apr 2022 20:46:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 20:46:54 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 20:46:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 20:46:55 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 20:46:55 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 20:46:56 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 20:46:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 20:46:57 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:08da560f0b65b004ba95f9a431d3ac51b8807b16ec6ef170e2e00dc55330246d`  
		Last Modified: Wed, 20 Apr 2022 13:51:07 GMT  
		Size: 19.4 MB (19359807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b404038787532b9a02cd78f02daf4f9413398993cee60ba553069a25266fc2`  
		Last Modified: Wed, 20 Apr 2022 20:47:53 GMT  
		Size: 5.8 MB (5780828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66a9b8033704d6beb570f434228299c84b17b1f28cb25050f1743137f68eff6`  
		Last Modified: Wed, 20 Apr 2022 20:49:36 GMT  
		Size: 35.3 MB (35291486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b924a31d1128a75ffcef7563f994638fe5a3987442eb2d8048ccf95c80f6d2d0`  
		Last Modified: Wed, 20 Apr 2022 20:49:17 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ecd9481c0c7c1fe43dfed2b9da2061660f320d6ecf441dafbeb6e960823c48`  
		Last Modified: Wed, 20 Apr 2022 20:49:17 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79bb56d646b1dd02e892c071e548c1293362e689eb091fcb389664ef7fefb39`  
		Last Modified: Wed, 20 Apr 2022 20:49:17 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:3d839961782f41d16a86070971a5cb94a6cb74076636b110403f01f2fc5c68ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61669514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a180e3ffea5b5cd9f69f5ec8758f3f30508cf7365f658bba79f77ec75a71268`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 04:31:34 GMT
ADD file:02ad9214474cf0e6d278d7015dee30e6a8e24cdc699812f5fb3915491177e92b in / 
# Wed, 20 Apr 2022 04:31:34 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:59:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 07:00:42 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 20 Apr 2022 07:00:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 07:00:51 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 07:00:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 07:00:52 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 07:00:53 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 07:00:55 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 07:00:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 07:00:56 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0fca491399855be4c9b780dca621b48440831235d7916e5695b876698df84db7`  
		Last Modified: Wed, 20 Apr 2022 04:40:05 GMT  
		Size: 20.4 MB (20424115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e40f4666ba5562961008676822baf755b62dc19df0f3c8f7afb99d53358f0b`  
		Last Modified: Wed, 20 Apr 2022 07:01:24 GMT  
		Size: 6.0 MB (6047044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f43894fdd799ef25fb1070140ee200ffb2dac0d2dae411de8caa42573313d53`  
		Last Modified: Wed, 20 Apr 2022 07:02:19 GMT  
		Size: 35.2 MB (35173963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be77256b514f3080aa7e607dc833ea08c7c3662fb3fd6b61076d0b6d49422e81`  
		Last Modified: Wed, 20 Apr 2022 07:02:14 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8bef315f0e60c5edfe896f37d62de6d28888cc2b586944c1328c83bca92b40`  
		Last Modified: Wed, 20 Apr 2022 07:02:14 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bd4f512d3cb9a481310f3577bdc41894d71cc842debb7caeb2b31eecd0f6db`  
		Last Modified: Wed, 20 Apr 2022 07:02:14 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9-alpine`

```console
$ docker pull chronograf@sha256:64529a79e1f42f21063f77e88d3b17a66dd5fe12b361ba459a496564f60deae5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.9-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:617112048d88886c7c56a0298d5022925bf60cea583bf42950f85da0b1543c30
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.8 MB (22786740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f641fefba39a03a8fb9f9a028aeeecec9f62c81b6a89da22334192b42afee733`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:26:16 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 04:26:47 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 05 Apr 2022 04:26:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 05 Apr 2022 04:26:55 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 05 Apr 2022 04:26:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 05 Apr 2022 04:26:55 GMT
EXPOSE 8888
# Tue, 05 Apr 2022 04:26:55 GMT
VOLUME [/var/lib/chronograf]
# Tue, 05 Apr 2022 04:26:55 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Tue, 05 Apr 2022 04:26:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 04:26:56 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58beb826c7b7288de69f85c4476fd6f04b58ceed760dd1b9e51a7d80aeb0e471`  
		Last Modified: Tue, 05 Apr 2022 04:27:20 GMT  
		Size: 271.7 KB (271678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03048cd652ea5c71fdf0fb436e4b84f533bce10501e6f8f75b34a3f5499ec3bc`  
		Last Modified: Tue, 05 Apr 2022 04:28:03 GMT  
		Size: 19.7 MB (19672143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcafdf6394d7dc10583226357da386688d2d1aa89d90e9d6c3e02d059d1ff7a0`  
		Last Modified: Tue, 05 Apr 2022 04:27:59 GMT  
		Size: 12.3 KB (12263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9df35e5b1a70215f7fa195a06d17ece074a61ec14d91da8c065c6f5426b8bc`  
		Last Modified: Tue, 05 Apr 2022 04:27:59 GMT  
		Size: 11.9 KB (11895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35eab2c8d98b5fdc4d6ed0e531c9766afacad54ccd952085aa98da4d57c5519a`  
		Last Modified: Tue, 05 Apr 2022 04:28:00 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9.4`

```console
$ docker pull chronograf@sha256:b6ca8877aab7407b8a3ee9478bd8ac4a618e63bbaf9dc6bdba257550acc9f941
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.9.4` - linux; amd64

```console
$ docker pull chronograf@sha256:6033dc59b677c6aa6532339e3e793ad2b4cf6e3453ab6f3db9b72cd53983bbf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66922520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90c8c2f940e4acbaf6f20031d9769ab445024072f70ad7b2b7ffd446d4ff1bfb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 04:45:25 GMT
ADD file:0fafb7f95dc18699227154856361058bc9aba65de2ff88bf55cc66363142a05e in / 
# Wed, 20 Apr 2022 04:45:25 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:53:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 06:54:18 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 20 Apr 2022 06:54:26 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 06:54:26 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 06:54:26 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 06:54:26 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 06:54:26 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 06:54:26 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 06:54:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 06:54:27 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:8bd3f5a20b90c0e84cc65ea4a9172a51b7b5c0b9a097fa88d7102cac91cddf2c`  
		Last Modified: Wed, 20 Apr 2022 04:52:27 GMT  
		Size: 22.6 MB (22567235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d1c45c938fb4526994828d87717ecc6b59f277d8ebfc4e01a11e9523f3867a`  
		Last Modified: Wed, 20 Apr 2022 06:54:52 GMT  
		Size: 6.8 MB (6760462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c3707b0034bfaa5138ec2fe28e3b3bd5ee29a93eda25f36ec6cd99e909dbf0`  
		Last Modified: Wed, 20 Apr 2022 06:55:41 GMT  
		Size: 37.6 MB (37570443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1d14c56566c0f90fbaa893624b83fff4fe016c2ea573422f619debde21839a`  
		Last Modified: Wed, 20 Apr 2022 06:55:35 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40fecaa82ff715c3dcd9bf685a10e2b67f868770e9ce7450656a3c92cb429fe`  
		Last Modified: Wed, 20 Apr 2022 06:55:35 GMT  
		Size: 11.9 KB (11900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9177a78636ef84328dd8835647471f1c71832ff0eb77899a26c8d505e555f7`  
		Last Modified: Wed, 20 Apr 2022 06:55:36 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9.4` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:7080ff4d4d25bd56dfc1698da8f915da5f2c6534355513bfcc7ba6979585c960
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60456520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68565f67efdeca82687fc4b9ebcc3ba19b8f864d41f19ebd0193b50bc2f009f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 13:33:51 GMT
ADD file:096692331564a30a9a9c6b24e681d99d68b54eeeabb7c5ac7d4073de06e050b2 in / 
# Wed, 20 Apr 2022 13:33:51 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:44:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 20:46:34 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 20 Apr 2022 20:46:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 20:46:54 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 20:46:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 20:46:55 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 20:46:55 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 20:46:56 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 20:46:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 20:46:57 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:08da560f0b65b004ba95f9a431d3ac51b8807b16ec6ef170e2e00dc55330246d`  
		Last Modified: Wed, 20 Apr 2022 13:51:07 GMT  
		Size: 19.4 MB (19359807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b404038787532b9a02cd78f02daf4f9413398993cee60ba553069a25266fc2`  
		Last Modified: Wed, 20 Apr 2022 20:47:53 GMT  
		Size: 5.8 MB (5780828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66a9b8033704d6beb570f434228299c84b17b1f28cb25050f1743137f68eff6`  
		Last Modified: Wed, 20 Apr 2022 20:49:36 GMT  
		Size: 35.3 MB (35291486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b924a31d1128a75ffcef7563f994638fe5a3987442eb2d8048ccf95c80f6d2d0`  
		Last Modified: Wed, 20 Apr 2022 20:49:17 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ecd9481c0c7c1fe43dfed2b9da2061660f320d6ecf441dafbeb6e960823c48`  
		Last Modified: Wed, 20 Apr 2022 20:49:17 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79bb56d646b1dd02e892c071e548c1293362e689eb091fcb389664ef7fefb39`  
		Last Modified: Wed, 20 Apr 2022 20:49:17 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9.4` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:3d839961782f41d16a86070971a5cb94a6cb74076636b110403f01f2fc5c68ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61669514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a180e3ffea5b5cd9f69f5ec8758f3f30508cf7365f658bba79f77ec75a71268`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 04:31:34 GMT
ADD file:02ad9214474cf0e6d278d7015dee30e6a8e24cdc699812f5fb3915491177e92b in / 
# Wed, 20 Apr 2022 04:31:34 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:59:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 07:00:42 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 20 Apr 2022 07:00:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 07:00:51 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 07:00:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 07:00:52 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 07:00:53 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 07:00:55 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 07:00:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 07:00:56 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0fca491399855be4c9b780dca621b48440831235d7916e5695b876698df84db7`  
		Last Modified: Wed, 20 Apr 2022 04:40:05 GMT  
		Size: 20.4 MB (20424115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e40f4666ba5562961008676822baf755b62dc19df0f3c8f7afb99d53358f0b`  
		Last Modified: Wed, 20 Apr 2022 07:01:24 GMT  
		Size: 6.0 MB (6047044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f43894fdd799ef25fb1070140ee200ffb2dac0d2dae411de8caa42573313d53`  
		Last Modified: Wed, 20 Apr 2022 07:02:19 GMT  
		Size: 35.2 MB (35173963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be77256b514f3080aa7e607dc833ea08c7c3662fb3fd6b61076d0b6d49422e81`  
		Last Modified: Wed, 20 Apr 2022 07:02:14 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8bef315f0e60c5edfe896f37d62de6d28888cc2b586944c1328c83bca92b40`  
		Last Modified: Wed, 20 Apr 2022 07:02:14 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bd4f512d3cb9a481310f3577bdc41894d71cc842debb7caeb2b31eecd0f6db`  
		Last Modified: Wed, 20 Apr 2022 07:02:14 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9.4-alpine`

```console
$ docker pull chronograf@sha256:64529a79e1f42f21063f77e88d3b17a66dd5fe12b361ba459a496564f60deae5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.9.4-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:617112048d88886c7c56a0298d5022925bf60cea583bf42950f85da0b1543c30
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.8 MB (22786740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f641fefba39a03a8fb9f9a028aeeecec9f62c81b6a89da22334192b42afee733`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:26:16 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 04:26:47 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 05 Apr 2022 04:26:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 05 Apr 2022 04:26:55 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 05 Apr 2022 04:26:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 05 Apr 2022 04:26:55 GMT
EXPOSE 8888
# Tue, 05 Apr 2022 04:26:55 GMT
VOLUME [/var/lib/chronograf]
# Tue, 05 Apr 2022 04:26:55 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Tue, 05 Apr 2022 04:26:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 04:26:56 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58beb826c7b7288de69f85c4476fd6f04b58ceed760dd1b9e51a7d80aeb0e471`  
		Last Modified: Tue, 05 Apr 2022 04:27:20 GMT  
		Size: 271.7 KB (271678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03048cd652ea5c71fdf0fb436e4b84f533bce10501e6f8f75b34a3f5499ec3bc`  
		Last Modified: Tue, 05 Apr 2022 04:28:03 GMT  
		Size: 19.7 MB (19672143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcafdf6394d7dc10583226357da386688d2d1aa89d90e9d6c3e02d059d1ff7a0`  
		Last Modified: Tue, 05 Apr 2022 04:27:59 GMT  
		Size: 12.3 KB (12263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9df35e5b1a70215f7fa195a06d17ece074a61ec14d91da8c065c6f5426b8bc`  
		Last Modified: Tue, 05 Apr 2022 04:27:59 GMT  
		Size: 11.9 KB (11895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35eab2c8d98b5fdc4d6ed0e531c9766afacad54ccd952085aa98da4d57c5519a`  
		Last Modified: Tue, 05 Apr 2022 04:28:00 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:alpine`

```console
$ docker pull chronograf@sha256:64529a79e1f42f21063f77e88d3b17a66dd5fe12b361ba459a496564f60deae5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:617112048d88886c7c56a0298d5022925bf60cea583bf42950f85da0b1543c30
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.8 MB (22786740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f641fefba39a03a8fb9f9a028aeeecec9f62c81b6a89da22334192b42afee733`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:26:16 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 04:26:47 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 05 Apr 2022 04:26:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 05 Apr 2022 04:26:55 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 05 Apr 2022 04:26:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 05 Apr 2022 04:26:55 GMT
EXPOSE 8888
# Tue, 05 Apr 2022 04:26:55 GMT
VOLUME [/var/lib/chronograf]
# Tue, 05 Apr 2022 04:26:55 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Tue, 05 Apr 2022 04:26:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 04:26:56 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58beb826c7b7288de69f85c4476fd6f04b58ceed760dd1b9e51a7d80aeb0e471`  
		Last Modified: Tue, 05 Apr 2022 04:27:20 GMT  
		Size: 271.7 KB (271678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03048cd652ea5c71fdf0fb436e4b84f533bce10501e6f8f75b34a3f5499ec3bc`  
		Last Modified: Tue, 05 Apr 2022 04:28:03 GMT  
		Size: 19.7 MB (19672143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcafdf6394d7dc10583226357da386688d2d1aa89d90e9d6c3e02d059d1ff7a0`  
		Last Modified: Tue, 05 Apr 2022 04:27:59 GMT  
		Size: 12.3 KB (12263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9df35e5b1a70215f7fa195a06d17ece074a61ec14d91da8c065c6f5426b8bc`  
		Last Modified: Tue, 05 Apr 2022 04:27:59 GMT  
		Size: 11.9 KB (11895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35eab2c8d98b5fdc4d6ed0e531c9766afacad54ccd952085aa98da4d57c5519a`  
		Last Modified: Tue, 05 Apr 2022 04:28:00 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:latest`

```console
$ docker pull chronograf@sha256:b6ca8877aab7407b8a3ee9478bd8ac4a618e63bbaf9dc6bdba257550acc9f941
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:6033dc59b677c6aa6532339e3e793ad2b4cf6e3453ab6f3db9b72cd53983bbf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66922520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90c8c2f940e4acbaf6f20031d9769ab445024072f70ad7b2b7ffd446d4ff1bfb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 04:45:25 GMT
ADD file:0fafb7f95dc18699227154856361058bc9aba65de2ff88bf55cc66363142a05e in / 
# Wed, 20 Apr 2022 04:45:25 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:53:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 06:54:18 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 20 Apr 2022 06:54:26 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 06:54:26 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 06:54:26 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 06:54:26 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 06:54:26 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 06:54:26 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 06:54:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 06:54:27 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:8bd3f5a20b90c0e84cc65ea4a9172a51b7b5c0b9a097fa88d7102cac91cddf2c`  
		Last Modified: Wed, 20 Apr 2022 04:52:27 GMT  
		Size: 22.6 MB (22567235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d1c45c938fb4526994828d87717ecc6b59f277d8ebfc4e01a11e9523f3867a`  
		Last Modified: Wed, 20 Apr 2022 06:54:52 GMT  
		Size: 6.8 MB (6760462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c3707b0034bfaa5138ec2fe28e3b3bd5ee29a93eda25f36ec6cd99e909dbf0`  
		Last Modified: Wed, 20 Apr 2022 06:55:41 GMT  
		Size: 37.6 MB (37570443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1d14c56566c0f90fbaa893624b83fff4fe016c2ea573422f619debde21839a`  
		Last Modified: Wed, 20 Apr 2022 06:55:35 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40fecaa82ff715c3dcd9bf685a10e2b67f868770e9ce7450656a3c92cb429fe`  
		Last Modified: Wed, 20 Apr 2022 06:55:35 GMT  
		Size: 11.9 KB (11900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9177a78636ef84328dd8835647471f1c71832ff0eb77899a26c8d505e555f7`  
		Last Modified: Wed, 20 Apr 2022 06:55:36 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:7080ff4d4d25bd56dfc1698da8f915da5f2c6534355513bfcc7ba6979585c960
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60456520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68565f67efdeca82687fc4b9ebcc3ba19b8f864d41f19ebd0193b50bc2f009f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 13:33:51 GMT
ADD file:096692331564a30a9a9c6b24e681d99d68b54eeeabb7c5ac7d4073de06e050b2 in / 
# Wed, 20 Apr 2022 13:33:51 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:44:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 20:46:34 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 20 Apr 2022 20:46:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 20:46:54 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 20:46:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 20:46:55 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 20:46:55 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 20:46:56 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 20:46:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 20:46:57 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:08da560f0b65b004ba95f9a431d3ac51b8807b16ec6ef170e2e00dc55330246d`  
		Last Modified: Wed, 20 Apr 2022 13:51:07 GMT  
		Size: 19.4 MB (19359807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b404038787532b9a02cd78f02daf4f9413398993cee60ba553069a25266fc2`  
		Last Modified: Wed, 20 Apr 2022 20:47:53 GMT  
		Size: 5.8 MB (5780828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66a9b8033704d6beb570f434228299c84b17b1f28cb25050f1743137f68eff6`  
		Last Modified: Wed, 20 Apr 2022 20:49:36 GMT  
		Size: 35.3 MB (35291486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b924a31d1128a75ffcef7563f994638fe5a3987442eb2d8048ccf95c80f6d2d0`  
		Last Modified: Wed, 20 Apr 2022 20:49:17 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ecd9481c0c7c1fe43dfed2b9da2061660f320d6ecf441dafbeb6e960823c48`  
		Last Modified: Wed, 20 Apr 2022 20:49:17 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79bb56d646b1dd02e892c071e548c1293362e689eb091fcb389664ef7fefb39`  
		Last Modified: Wed, 20 Apr 2022 20:49:17 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:3d839961782f41d16a86070971a5cb94a6cb74076636b110403f01f2fc5c68ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61669514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a180e3ffea5b5cd9f69f5ec8758f3f30508cf7365f658bba79f77ec75a71268`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 20 Apr 2022 04:31:34 GMT
ADD file:02ad9214474cf0e6d278d7015dee30e6a8e24cdc699812f5fb3915491177e92b in / 
# Wed, 20 Apr 2022 04:31:34 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:59:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 20 Apr 2022 07:00:42 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 20 Apr 2022 07:00:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 07:00:51 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 20 Apr 2022 07:00:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 20 Apr 2022 07:00:52 GMT
EXPOSE 8888
# Wed, 20 Apr 2022 07:00:53 GMT
VOLUME [/var/lib/chronograf]
# Wed, 20 Apr 2022 07:00:55 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 20 Apr 2022 07:00:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 07:00:56 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0fca491399855be4c9b780dca621b48440831235d7916e5695b876698df84db7`  
		Last Modified: Wed, 20 Apr 2022 04:40:05 GMT  
		Size: 20.4 MB (20424115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e40f4666ba5562961008676822baf755b62dc19df0f3c8f7afb99d53358f0b`  
		Last Modified: Wed, 20 Apr 2022 07:01:24 GMT  
		Size: 6.0 MB (6047044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f43894fdd799ef25fb1070140ee200ffb2dac0d2dae411de8caa42573313d53`  
		Last Modified: Wed, 20 Apr 2022 07:02:19 GMT  
		Size: 35.2 MB (35173963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be77256b514f3080aa7e607dc833ea08c7c3662fb3fd6b61076d0b6d49422e81`  
		Last Modified: Wed, 20 Apr 2022 07:02:14 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8bef315f0e60c5edfe896f37d62de6d28888cc2b586944c1328c83bca92b40`  
		Last Modified: Wed, 20 Apr 2022 07:02:14 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bd4f512d3cb9a481310f3577bdc41894d71cc842debb7caeb2b31eecd0f6db`  
		Last Modified: Wed, 20 Apr 2022 07:02:14 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
