<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `chronograf`

-	[`chronograf:1.10`](#chronograf110)
-	[`chronograf:1.10-alpine`](#chronograf110-alpine)
-	[`chronograf:1.10.1`](#chronograf1101)
-	[`chronograf:1.10.1-alpine`](#chronograf1101-alpine)
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
$ docker pull chronograf@sha256:3d77e6c9aea81e0d0f00fd65e5d2feed23dec5bef6ac91f8e277b5b2c5e14fa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.10` - linux; amd64

```console
$ docker pull chronograf@sha256:1575b03b10ca5ccf30556eea9dbd26982e1a99d692d5de81f0377d84c8a91438
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.8 MB (82803422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:054a06db258d36e98f5dc5ae85d5a8d56fde1d3ea6097bb7a5ac4c7f3251bb58`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:11:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Mar 2023 06:11:59 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Thu, 23 Mar 2023 06:12:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 06:12:06 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Mar 2023 06:12:06 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Mar 2023 06:12:06 GMT
EXPOSE 8888
# Thu, 23 Mar 2023 06:12:06 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Mar 2023 06:12:06 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Mar 2023 06:12:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 06:12:06 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b38a80a9c9f14745c5d3c39eca2ab0731ac3ad6e829bda6ab0ba1876fa33b2`  
		Last Modified: Thu, 23 Mar 2023 06:12:36 GMT  
		Size: 5.2 MB (5226171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6b1b6422de45b88751631cd54d00aa6d1c9874585581faddd81344f0acf2f5`  
		Last Modified: Thu, 23 Mar 2023 06:13:08 GMT  
		Size: 46.1 MB (46141452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685b83b562e36e2face4136733838671e6425ac7f52a0d3016937da2327e260b`  
		Last Modified: Thu, 23 Mar 2023 06:13:02 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af80511b750f16f6e44c34b5cf5820739dd58ba881371c8486917b9e1f2f47d7`  
		Last Modified: Thu, 23 Mar 2023 06:13:02 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144629686b91940362645ae1fa7bf7ebbf5121109839bebd74562587534c1931`  
		Last Modified: Thu, 23 Mar 2023 06:13:02 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:0236ae34e7f3fd8dcb6b3dd18f40c795f316e11c08e6ba8522f475112c7a0050
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74943587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ec091f267a7b261d28f060556268eb5067b2c6cd38cc917fbde1db51f2f28ea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:23:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Mar 2023 13:23:54 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Thu, 23 Mar 2023 13:24:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 13:24:03 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Mar 2023 13:24:03 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Mar 2023 13:24:03 GMT
EXPOSE 8888
# Thu, 23 Mar 2023 13:24:03 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Mar 2023 13:24:04 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Mar 2023 13:24:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 13:24:04 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48bdccd5f6d7a7f2a2045df36ec26beea220a468695975eb1146d58b1737dc5`  
		Last Modified: Thu, 23 Mar 2023 13:24:26 GMT  
		Size: 4.5 MB (4491664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c196ce85113ecf0ec03684d0e68394dd58b4d0c618746eeec78d1aed39443f8`  
		Last Modified: Thu, 23 Mar 2023 13:24:56 GMT  
		Size: 43.9 MB (43850197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23338b9c5719d08a89afae62665541bd907344d136f89aade4cb8421a2a24ee9`  
		Last Modified: Thu, 23 Mar 2023 13:24:49 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf694109367e4ab8897da76728f00e57301d62fa2867226ef97e4d6ccf5750`  
		Last Modified: Thu, 23 Mar 2023 13:24:49 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f9d7aaebdf9fb9009f624c051e2bb8b36a356fa649b8b0d0ea6585c3d58a0e`  
		Last Modified: Thu, 23 Mar 2023 13:24:49 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:61723a713e5e956511babbb5720cac4539df70a4fa0e363fe6d3d18bfdef4c6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79152403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f65ba602b25252bc53e80ff5e1143cf5c59529a9379c1b11b8bf4b1386dee4f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:16:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 01:16:49 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Wed, 12 Apr 2023 01:16:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:16:55 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 12 Apr 2023 01:16:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 12 Apr 2023 01:16:55 GMT
EXPOSE 8888
# Wed, 12 Apr 2023 01:16:55 GMT
VOLUME [/var/lib/chronograf]
# Wed, 12 Apr 2023 01:16:55 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 12 Apr 2023 01:16:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 01:16:56 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8d0543e677dafef62b6b0cbed79f1e23b76b074feeec13c79ac54cdd154a33`  
		Last Modified: Wed, 12 Apr 2023 01:17:20 GMT  
		Size: 5.2 MB (5209387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f76b035a31a949a5946475fe6e1dc30b9939da944e0e9a6eae9cf255a31eea`  
		Last Modified: Wed, 12 Apr 2023 01:17:45 GMT  
		Size: 43.9 MB (43854802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37431348a86ec9a9ef0da51d65733c7c2ac2bc724c6f8c37b17551038bb70a45`  
		Last Modified: Wed, 12 Apr 2023 01:17:40 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0313fc537cd1c011b154938f1d65d0d66e7a589f4a2a9bf00b5748732d691fba`  
		Last Modified: Wed, 12 Apr 2023 01:17:41 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c78d43e9fb235b2d40a2a345f8a244952572332d461048af98ec37895a1d973`  
		Last Modified: Wed, 12 Apr 2023 01:17:41 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.10-alpine`

```console
$ docker pull chronograf@sha256:98831602a8aa62cc195baea1c779fe5ca4bd888b12b4bc749c5973b57c5e3297
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.10-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:6062289ea692c0047e6608134571368e6f528b7f374c6644d374691a33720997
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31471176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6444543c380851da2dd2360a89fc011204ccaa4e28c7aea94ad6ba2a96efd413`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 19:46:51 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 29 Mar 2023 19:47:24 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Wed, 29 Mar 2023 19:47:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 29 Mar 2023 19:47:30 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 29 Mar 2023 19:47:30 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 29 Mar 2023 19:47:30 GMT
EXPOSE 8888
# Wed, 29 Mar 2023 19:47:30 GMT
VOLUME [/var/lib/chronograf]
# Wed, 29 Mar 2023 19:47:30 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 29 Mar 2023 19:47:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 19:47:31 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc6fa7c28a8decb0b5d8e618de112a92abffb23d50587ab655da8c0377b5600`  
		Last Modified: Wed, 29 Mar 2023 19:47:47 GMT  
		Size: 284.8 KB (284812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867fc62a9977fb48ebff54478afb2ae589ea2a08853a70b3f93a131ce67ee55f`  
		Last Modified: Wed, 29 Mar 2023 19:48:26 GMT  
		Size: 27.8 MB (27787123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03de77a31cf58915f9a2085eadee11338ee3e454f6d0a2c4d064e4ca5fc369e3`  
		Last Modified: Wed, 29 Mar 2023 19:48:21 GMT  
		Size: 12.3 KB (12266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9bccc09d6b731509690ff6112f9dd2b9cc3408ce4f6942d2285ce32f54667a`  
		Last Modified: Wed, 29 Mar 2023 19:48:21 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4dbd842e2dd7377ae86030ceece05fa917381af338a44999315838b590e941`  
		Last Modified: Wed, 29 Mar 2023 19:48:21 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.10.1`

```console
$ docker pull chronograf@sha256:3d77e6c9aea81e0d0f00fd65e5d2feed23dec5bef6ac91f8e277b5b2c5e14fa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.10.1` - linux; amd64

```console
$ docker pull chronograf@sha256:1575b03b10ca5ccf30556eea9dbd26982e1a99d692d5de81f0377d84c8a91438
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.8 MB (82803422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:054a06db258d36e98f5dc5ae85d5a8d56fde1d3ea6097bb7a5ac4c7f3251bb58`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:11:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Mar 2023 06:11:59 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Thu, 23 Mar 2023 06:12:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 06:12:06 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Mar 2023 06:12:06 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Mar 2023 06:12:06 GMT
EXPOSE 8888
# Thu, 23 Mar 2023 06:12:06 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Mar 2023 06:12:06 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Mar 2023 06:12:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 06:12:06 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b38a80a9c9f14745c5d3c39eca2ab0731ac3ad6e829bda6ab0ba1876fa33b2`  
		Last Modified: Thu, 23 Mar 2023 06:12:36 GMT  
		Size: 5.2 MB (5226171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6b1b6422de45b88751631cd54d00aa6d1c9874585581faddd81344f0acf2f5`  
		Last Modified: Thu, 23 Mar 2023 06:13:08 GMT  
		Size: 46.1 MB (46141452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685b83b562e36e2face4136733838671e6425ac7f52a0d3016937da2327e260b`  
		Last Modified: Thu, 23 Mar 2023 06:13:02 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af80511b750f16f6e44c34b5cf5820739dd58ba881371c8486917b9e1f2f47d7`  
		Last Modified: Thu, 23 Mar 2023 06:13:02 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144629686b91940362645ae1fa7bf7ebbf5121109839bebd74562587534c1931`  
		Last Modified: Thu, 23 Mar 2023 06:13:02 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10.1` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:0236ae34e7f3fd8dcb6b3dd18f40c795f316e11c08e6ba8522f475112c7a0050
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74943587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ec091f267a7b261d28f060556268eb5067b2c6cd38cc917fbde1db51f2f28ea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:23:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Mar 2023 13:23:54 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Thu, 23 Mar 2023 13:24:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 13:24:03 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Mar 2023 13:24:03 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Mar 2023 13:24:03 GMT
EXPOSE 8888
# Thu, 23 Mar 2023 13:24:03 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Mar 2023 13:24:04 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Mar 2023 13:24:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 13:24:04 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48bdccd5f6d7a7f2a2045df36ec26beea220a468695975eb1146d58b1737dc5`  
		Last Modified: Thu, 23 Mar 2023 13:24:26 GMT  
		Size: 4.5 MB (4491664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c196ce85113ecf0ec03684d0e68394dd58b4d0c618746eeec78d1aed39443f8`  
		Last Modified: Thu, 23 Mar 2023 13:24:56 GMT  
		Size: 43.9 MB (43850197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23338b9c5719d08a89afae62665541bd907344d136f89aade4cb8421a2a24ee9`  
		Last Modified: Thu, 23 Mar 2023 13:24:49 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf694109367e4ab8897da76728f00e57301d62fa2867226ef97e4d6ccf5750`  
		Last Modified: Thu, 23 Mar 2023 13:24:49 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f9d7aaebdf9fb9009f624c051e2bb8b36a356fa649b8b0d0ea6585c3d58a0e`  
		Last Modified: Thu, 23 Mar 2023 13:24:49 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10.1` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:61723a713e5e956511babbb5720cac4539df70a4fa0e363fe6d3d18bfdef4c6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79152403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f65ba602b25252bc53e80ff5e1143cf5c59529a9379c1b11b8bf4b1386dee4f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:16:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 01:16:49 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Wed, 12 Apr 2023 01:16:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:16:55 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 12 Apr 2023 01:16:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 12 Apr 2023 01:16:55 GMT
EXPOSE 8888
# Wed, 12 Apr 2023 01:16:55 GMT
VOLUME [/var/lib/chronograf]
# Wed, 12 Apr 2023 01:16:55 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 12 Apr 2023 01:16:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 01:16:56 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8d0543e677dafef62b6b0cbed79f1e23b76b074feeec13c79ac54cdd154a33`  
		Last Modified: Wed, 12 Apr 2023 01:17:20 GMT  
		Size: 5.2 MB (5209387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f76b035a31a949a5946475fe6e1dc30b9939da944e0e9a6eae9cf255a31eea`  
		Last Modified: Wed, 12 Apr 2023 01:17:45 GMT  
		Size: 43.9 MB (43854802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37431348a86ec9a9ef0da51d65733c7c2ac2bc724c6f8c37b17551038bb70a45`  
		Last Modified: Wed, 12 Apr 2023 01:17:40 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0313fc537cd1c011b154938f1d65d0d66e7a589f4a2a9bf00b5748732d691fba`  
		Last Modified: Wed, 12 Apr 2023 01:17:41 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c78d43e9fb235b2d40a2a345f8a244952572332d461048af98ec37895a1d973`  
		Last Modified: Wed, 12 Apr 2023 01:17:41 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.10.1-alpine`

```console
$ docker pull chronograf@sha256:98831602a8aa62cc195baea1c779fe5ca4bd888b12b4bc749c5973b57c5e3297
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.10.1-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:6062289ea692c0047e6608134571368e6f528b7f374c6644d374691a33720997
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31471176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6444543c380851da2dd2360a89fc011204ccaa4e28c7aea94ad6ba2a96efd413`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 19:46:51 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 29 Mar 2023 19:47:24 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Wed, 29 Mar 2023 19:47:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 29 Mar 2023 19:47:30 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 29 Mar 2023 19:47:30 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 29 Mar 2023 19:47:30 GMT
EXPOSE 8888
# Wed, 29 Mar 2023 19:47:30 GMT
VOLUME [/var/lib/chronograf]
# Wed, 29 Mar 2023 19:47:30 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 29 Mar 2023 19:47:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 19:47:31 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc6fa7c28a8decb0b5d8e618de112a92abffb23d50587ab655da8c0377b5600`  
		Last Modified: Wed, 29 Mar 2023 19:47:47 GMT  
		Size: 284.8 KB (284812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867fc62a9977fb48ebff54478afb2ae589ea2a08853a70b3f93a131ce67ee55f`  
		Last Modified: Wed, 29 Mar 2023 19:48:26 GMT  
		Size: 27.8 MB (27787123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03de77a31cf58915f9a2085eadee11338ee3e454f6d0a2c4d064e4ca5fc369e3`  
		Last Modified: Wed, 29 Mar 2023 19:48:21 GMT  
		Size: 12.3 KB (12266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9bccc09d6b731509690ff6112f9dd2b9cc3408ce4f6942d2285ce32f54667a`  
		Last Modified: Wed, 29 Mar 2023 19:48:21 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4dbd842e2dd7377ae86030ceece05fa917381af338a44999315838b590e941`  
		Last Modified: Wed, 29 Mar 2023 19:48:21 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7`

```console
$ docker pull chronograf@sha256:8c4533a97a7d66b4783623b299494aaba403048441f8d15d22a4835c2d1e775e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7` - linux; amd64

```console
$ docker pull chronograf@sha256:5d54d6796c7647401174632ba4e8261ff5882d576315ba17486450436cb2967d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70589663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc3e032472df72439e6f75d60e6b1d99df1306c92455b287296cc3001ec45d29`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:11:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Mar 2023 06:11:16 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 23 Mar 2023 06:11:25 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 06:11:25 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Mar 2023 06:11:25 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Mar 2023 06:11:25 GMT
EXPOSE 8888
# Thu, 23 Mar 2023 06:11:25 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Mar 2023 06:11:25 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Mar 2023 06:11:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 06:11:26 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5ee2f97013796ca61338dafa41afc07f64d22f87e9f6e30f476e7f1adc1465`  
		Last Modified: Thu, 23 Mar 2023 06:12:22 GMT  
		Size: 4.4 MB (4416479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe144243e4e37f784469f1d7abe2f5ed84b457884a4414a08a50d065e667171`  
		Last Modified: Thu, 23 Mar 2023 06:12:26 GMT  
		Size: 34.7 MB (34737380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1501659ddede463460d9df1fea8676c1c68e1f2eea571da93540c603dacc53e7`  
		Last Modified: Thu, 23 Mar 2023 06:12:22 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338cab9a5d9028c6adec3cc2184d2d9e1d612e385073721fe8966fb264e5214d`  
		Last Modified: Thu, 23 Mar 2023 06:12:22 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3216407121620f08b32c7977c224cae6f8a257923963cb557a6abdafb40a81f`  
		Last Modified: Thu, 23 Mar 2023 06:12:22 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:a96c5495c6f4e684de015e81a3bc6f897de3b1031c4f6e17c7bb87e211861831
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63417680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc40def7bab5a6c8e3aea81916807728d755c054557c4d46f748e4cdc358a4c9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:23:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Mar 2023 13:23:13 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 23 Mar 2023 13:23:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 13:23:21 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Mar 2023 13:23:21 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Mar 2023 13:23:21 GMT
EXPOSE 8888
# Thu, 23 Mar 2023 13:23:22 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Mar 2023 13:23:22 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Mar 2023 13:23:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 13:23:22 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4c2f92b429d0dfca3deb246420647efac647e42d799fd22cb827d923d6c02f`  
		Last Modified: Thu, 23 Mar 2023 13:24:14 GMT  
		Size: 3.7 MB (3718979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909ec621762dc15026c4c9f31fa3c4694f13a6f38340655701a242e091f71198`  
		Last Modified: Thu, 23 Mar 2023 13:24:17 GMT  
		Size: 33.1 MB (33096974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765515885b6241b725b32ee66cc54417608f34df62e131e9fda754e5086da629`  
		Last Modified: Thu, 23 Mar 2023 13:24:13 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959c699050a7e80ca660ea61a5479f7efd9af25b3049c8cb96f8a883d20ccd8d`  
		Last Modified: Thu, 23 Mar 2023 13:24:13 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f637e09ccf13788560a8ba87c89871f7650fba7f6d954905cbd2b6de9e1a16`  
		Last Modified: Thu, 23 Mar 2023 13:24:13 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:b74a8f519b286967fe3bb86b27123a812450ccb8baa83484f8c9c1c7aaa4b9d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67743826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:274d3d8116afca97c2fcb15631237573b35a530e40dede3f70234b36b9c7fdf4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:16:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 01:16:13 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 12 Apr 2023 01:16:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:16:21 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 12 Apr 2023 01:16:21 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 12 Apr 2023 01:16:21 GMT
EXPOSE 8888
# Wed, 12 Apr 2023 01:16:21 GMT
VOLUME [/var/lib/chronograf]
# Wed, 12 Apr 2023 01:16:21 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 12 Apr 2023 01:16:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 01:16:21 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efd93819c64e2d9eb6306fe7cf74b654c02078b0baf2e98e8dcffa0428b1bdc`  
		Last Modified: Wed, 12 Apr 2023 01:17:07 GMT  
		Size: 4.4 MB (4418105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fbe9415ba9d49675bac720a5905f8113f96662a07b9dc6fc92dac78b4199740`  
		Last Modified: Wed, 12 Apr 2023 01:17:10 GMT  
		Size: 33.2 MB (33237508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a4d0165a68871c5d1f012ec0fdd4567d51b9add26a33881c6f11d402e689be`  
		Last Modified: Wed, 12 Apr 2023 01:17:07 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1304df58f82f6fbb2e6641dc25de52009bf311417b5e98091c9b95eecd97d317`  
		Last Modified: Wed, 12 Apr 2023 01:17:06 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822829d2c2cc5626545f61b687938380aea3c1140a994ce8a056ac7f07665f64`  
		Last Modified: Wed, 12 Apr 2023 01:17:06 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7-alpine`

```console
$ docker pull chronograf@sha256:7867f13ed5e05a05afdf06caf330f0b023af41976a11e2e00daa3a241d1c3d23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.7-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:33f7da386ea266f6451683b85b10ce23564ba4e3e9ba807618dcc6b05c5bb3ae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.2 MB (23241224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72c34872d98623ad6911d292117520af5997ff73c02ec51f1105bad2547a8ece`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 19:46:51 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 29 Mar 2023 19:46:51 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 29 Mar 2023 19:46:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 29 Mar 2023 19:46:56 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 29 Mar 2023 19:46:56 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 29 Mar 2023 19:46:56 GMT
EXPOSE 8888
# Wed, 29 Mar 2023 19:46:56 GMT
VOLUME [/var/lib/chronograf]
# Wed, 29 Mar 2023 19:46:56 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 29 Mar 2023 19:46:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 19:46:57 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc6fa7c28a8decb0b5d8e618de112a92abffb23d50587ab655da8c0377b5600`  
		Last Modified: Wed, 29 Mar 2023 19:47:47 GMT  
		Size: 284.8 KB (284812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741374cef378319c81f594eca08bc22a394b83a4ca0974d6c971f0d2da986a6a`  
		Last Modified: Wed, 29 Mar 2023 19:47:50 GMT  
		Size: 19.6 MB (19557169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9781bde67afa3375cd653cb2231ba0c884ac3308384f5e6b6f569bc37d4ff3`  
		Last Modified: Wed, 29 Mar 2023 19:47:47 GMT  
		Size: 12.3 KB (12268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b4fbb2ed4b661a30eab82318cc94a29f4c8d40aeed67f5964174ea33d11f72`  
		Last Modified: Wed, 29 Mar 2023 19:47:47 GMT  
		Size: 11.9 KB (11897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dc771f295338381421a45da3c638fb6d377da5bc81e5956de4eb553ca5af8e`  
		Last Modified: Wed, 29 Mar 2023 19:47:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17`

```console
$ docker pull chronograf@sha256:8c4533a97a7d66b4783623b299494aaba403048441f8d15d22a4835c2d1e775e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7.17` - linux; amd64

```console
$ docker pull chronograf@sha256:5d54d6796c7647401174632ba4e8261ff5882d576315ba17486450436cb2967d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70589663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc3e032472df72439e6f75d60e6b1d99df1306c92455b287296cc3001ec45d29`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:11:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Mar 2023 06:11:16 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 23 Mar 2023 06:11:25 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 06:11:25 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Mar 2023 06:11:25 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Mar 2023 06:11:25 GMT
EXPOSE 8888
# Thu, 23 Mar 2023 06:11:25 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Mar 2023 06:11:25 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Mar 2023 06:11:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 06:11:26 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5ee2f97013796ca61338dafa41afc07f64d22f87e9f6e30f476e7f1adc1465`  
		Last Modified: Thu, 23 Mar 2023 06:12:22 GMT  
		Size: 4.4 MB (4416479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe144243e4e37f784469f1d7abe2f5ed84b457884a4414a08a50d065e667171`  
		Last Modified: Thu, 23 Mar 2023 06:12:26 GMT  
		Size: 34.7 MB (34737380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1501659ddede463460d9df1fea8676c1c68e1f2eea571da93540c603dacc53e7`  
		Last Modified: Thu, 23 Mar 2023 06:12:22 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338cab9a5d9028c6adec3cc2184d2d9e1d612e385073721fe8966fb264e5214d`  
		Last Modified: Thu, 23 Mar 2023 06:12:22 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3216407121620f08b32c7977c224cae6f8a257923963cb557a6abdafb40a81f`  
		Last Modified: Thu, 23 Mar 2023 06:12:22 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:a96c5495c6f4e684de015e81a3bc6f897de3b1031c4f6e17c7bb87e211861831
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63417680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc40def7bab5a6c8e3aea81916807728d755c054557c4d46f748e4cdc358a4c9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:23:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Mar 2023 13:23:13 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 23 Mar 2023 13:23:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 13:23:21 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Mar 2023 13:23:21 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Mar 2023 13:23:21 GMT
EXPOSE 8888
# Thu, 23 Mar 2023 13:23:22 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Mar 2023 13:23:22 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Mar 2023 13:23:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 13:23:22 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4c2f92b429d0dfca3deb246420647efac647e42d799fd22cb827d923d6c02f`  
		Last Modified: Thu, 23 Mar 2023 13:24:14 GMT  
		Size: 3.7 MB (3718979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909ec621762dc15026c4c9f31fa3c4694f13a6f38340655701a242e091f71198`  
		Last Modified: Thu, 23 Mar 2023 13:24:17 GMT  
		Size: 33.1 MB (33096974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765515885b6241b725b32ee66cc54417608f34df62e131e9fda754e5086da629`  
		Last Modified: Thu, 23 Mar 2023 13:24:13 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959c699050a7e80ca660ea61a5479f7efd9af25b3049c8cb96f8a883d20ccd8d`  
		Last Modified: Thu, 23 Mar 2023 13:24:13 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f637e09ccf13788560a8ba87c89871f7650fba7f6d954905cbd2b6de9e1a16`  
		Last Modified: Thu, 23 Mar 2023 13:24:13 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:b74a8f519b286967fe3bb86b27123a812450ccb8baa83484f8c9c1c7aaa4b9d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67743826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:274d3d8116afca97c2fcb15631237573b35a530e40dede3f70234b36b9c7fdf4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:16:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 01:16:13 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 12 Apr 2023 01:16:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:16:21 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 12 Apr 2023 01:16:21 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 12 Apr 2023 01:16:21 GMT
EXPOSE 8888
# Wed, 12 Apr 2023 01:16:21 GMT
VOLUME [/var/lib/chronograf]
# Wed, 12 Apr 2023 01:16:21 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 12 Apr 2023 01:16:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 01:16:21 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efd93819c64e2d9eb6306fe7cf74b654c02078b0baf2e98e8dcffa0428b1bdc`  
		Last Modified: Wed, 12 Apr 2023 01:17:07 GMT  
		Size: 4.4 MB (4418105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fbe9415ba9d49675bac720a5905f8113f96662a07b9dc6fc92dac78b4199740`  
		Last Modified: Wed, 12 Apr 2023 01:17:10 GMT  
		Size: 33.2 MB (33237508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a4d0165a68871c5d1f012ec0fdd4567d51b9add26a33881c6f11d402e689be`  
		Last Modified: Wed, 12 Apr 2023 01:17:07 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1304df58f82f6fbb2e6641dc25de52009bf311417b5e98091c9b95eecd97d317`  
		Last Modified: Wed, 12 Apr 2023 01:17:06 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822829d2c2cc5626545f61b687938380aea3c1140a994ce8a056ac7f07665f64`  
		Last Modified: Wed, 12 Apr 2023 01:17:06 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17-alpine`

```console
$ docker pull chronograf@sha256:7867f13ed5e05a05afdf06caf330f0b023af41976a11e2e00daa3a241d1c3d23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.7.17-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:33f7da386ea266f6451683b85b10ce23564ba4e3e9ba807618dcc6b05c5bb3ae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.2 MB (23241224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72c34872d98623ad6911d292117520af5997ff73c02ec51f1105bad2547a8ece`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 19:46:51 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 29 Mar 2023 19:46:51 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 29 Mar 2023 19:46:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 29 Mar 2023 19:46:56 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 29 Mar 2023 19:46:56 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 29 Mar 2023 19:46:56 GMT
EXPOSE 8888
# Wed, 29 Mar 2023 19:46:56 GMT
VOLUME [/var/lib/chronograf]
# Wed, 29 Mar 2023 19:46:56 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 29 Mar 2023 19:46:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 19:46:57 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc6fa7c28a8decb0b5d8e618de112a92abffb23d50587ab655da8c0377b5600`  
		Last Modified: Wed, 29 Mar 2023 19:47:47 GMT  
		Size: 284.8 KB (284812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741374cef378319c81f594eca08bc22a394b83a4ca0974d6c971f0d2da986a6a`  
		Last Modified: Wed, 29 Mar 2023 19:47:50 GMT  
		Size: 19.6 MB (19557169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9781bde67afa3375cd653cb2231ba0c884ac3308384f5e6b6f569bc37d4ff3`  
		Last Modified: Wed, 29 Mar 2023 19:47:47 GMT  
		Size: 12.3 KB (12268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b4fbb2ed4b661a30eab82318cc94a29f4c8d40aeed67f5964174ea33d11f72`  
		Last Modified: Wed, 29 Mar 2023 19:47:47 GMT  
		Size: 11.9 KB (11897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dc771f295338381421a45da3c638fb6d377da5bc81e5956de4eb553ca5af8e`  
		Last Modified: Wed, 29 Mar 2023 19:47:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8`

```console
$ docker pull chronograf@sha256:2e5217574071d5da90d91a37826b89393cd81aba22160e16fe2c92749e87ebf9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8` - linux; amd64

```console
$ docker pull chronograf@sha256:d5c267ecd20ee2bd410d30c0dc42aa5e37f9b0841b62f5a4a58742b1436eb308
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.2 MB (71240949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5cd8cc544951fd0ff71fc99961a02c193858b222ac6135c08c38ce029e9b690`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:11:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Mar 2023 06:11:37 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Thu, 23 Mar 2023 06:11:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 06:11:43 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Mar 2023 06:11:43 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Mar 2023 06:11:43 GMT
EXPOSE 8888
# Thu, 23 Mar 2023 06:11:43 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Mar 2023 06:11:43 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Mar 2023 06:11:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 06:11:43 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b38a80a9c9f14745c5d3c39eca2ab0731ac3ad6e829bda6ab0ba1876fa33b2`  
		Last Modified: Thu, 23 Mar 2023 06:12:36 GMT  
		Size: 5.2 MB (5226171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa39c924992902744aa1e6d0ec24a57c5ceac251cd245c70b048ba493a88a717`  
		Last Modified: Thu, 23 Mar 2023 06:12:39 GMT  
		Size: 34.6 MB (34578976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634ccb6519123dedae91ececd01a0bbfda5c481ef3333f5337214655e3f49ece`  
		Last Modified: Thu, 23 Mar 2023 06:12:35 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec444031881454f7b613a330771dfc6821a4aef1bdc7029fdea9e7ee8aca7e35`  
		Last Modified: Thu, 23 Mar 2023 06:12:35 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be954e0035ff49b0ee01cf3ddc26a2b4adcbadbe35740f5bf0a41d3f367d9f56`  
		Last Modified: Thu, 23 Mar 2023 06:12:35 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:60786ec7c07058f39313af7887a07dae6dccf39b64bbb7d945c2c6025660d702
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63843589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfa33c78bbf9838bccd5247cc0638a86daf37378bd0c4ab7dd8d7a02ade75f88`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:23:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Mar 2023 13:23:33 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Thu, 23 Mar 2023 13:23:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 13:23:41 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Mar 2023 13:23:41 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Mar 2023 13:23:41 GMT
EXPOSE 8888
# Thu, 23 Mar 2023 13:23:41 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Mar 2023 13:23:41 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Mar 2023 13:23:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 13:23:41 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48bdccd5f6d7a7f2a2045df36ec26beea220a468695975eb1146d58b1737dc5`  
		Last Modified: Thu, 23 Mar 2023 13:24:26 GMT  
		Size: 4.5 MB (4491664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6175a1191ed4e7dde0a5af3daeca99f0e0050e390ff8c62a1def6002bcd03e84`  
		Last Modified: Thu, 23 Mar 2023 13:24:30 GMT  
		Size: 32.8 MB (32750199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b477330cf38d31553d29b0095e449f3088d967f8abd999106b2a41f08f8d78e2`  
		Last Modified: Thu, 23 Mar 2023 13:24:26 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b91a1d011d4bc43f43794e13a8546acb8c1910a807883752e97edbec454c47`  
		Last Modified: Thu, 23 Mar 2023 13:24:26 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9242837f6d7c8b34788881a68a813f398e0121de48191f3f17f27a89adb86e`  
		Last Modified: Thu, 23 Mar 2023 13:24:26 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:b86a8d6dbeef7bcb0b5fa0223bcafc66f9e21ccd5507a7f16ab71770e0a7c747
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67941430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:264df0ca3bead32e50c1dfa54cb244b68f9d7e28b7a252e860dd153618fcb7ab`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:16:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 01:16:30 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 12 Apr 2023 01:16:36 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:16:36 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 12 Apr 2023 01:16:36 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 12 Apr 2023 01:16:36 GMT
EXPOSE 8888
# Wed, 12 Apr 2023 01:16:36 GMT
VOLUME [/var/lib/chronograf]
# Wed, 12 Apr 2023 01:16:36 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 12 Apr 2023 01:16:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 01:16:37 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8d0543e677dafef62b6b0cbed79f1e23b76b074feeec13c79ac54cdd154a33`  
		Last Modified: Wed, 12 Apr 2023 01:17:20 GMT  
		Size: 5.2 MB (5209387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c60b1c7c5a384549291dc92649a139620b5b6ee91e6b20368347d4979d8016f`  
		Last Modified: Wed, 12 Apr 2023 01:17:21 GMT  
		Size: 32.6 MB (32643822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2919cf3fdd56b48266aa8a0d5d195c56353e2c499b6e48e3a8e431de687f52`  
		Last Modified: Wed, 12 Apr 2023 01:17:18 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ab1c1238d012fd8130766a747e70a56e6d953dda9fece1b4f7a655a2e75171`  
		Last Modified: Wed, 12 Apr 2023 01:17:18 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9deedd4ab510bf3dcd0011ff677493e3b5f7500b8789c7a59892010d368182da`  
		Last Modified: Wed, 12 Apr 2023 01:17:18 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8-alpine`

```console
$ docker pull chronograf@sha256:e60095ede17376b4c03f67a2f456888f5f2b923885bff7b68ddf3e3dd02f7f51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:5e27bfc9734a3b128ce7328af10d8b2c1159c1043e20966a61143c1bd269dd0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22888222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:686e49688a842468eebc393eafcdbb57dbf812dd59fcd3407c3d635e81f53d83`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 19:46:51 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 29 Mar 2023 19:47:01 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 29 Mar 2023 19:47:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 29 Mar 2023 19:47:09 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 29 Mar 2023 19:47:09 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 29 Mar 2023 19:47:09 GMT
EXPOSE 8888
# Wed, 29 Mar 2023 19:47:09 GMT
VOLUME [/var/lib/chronograf]
# Wed, 29 Mar 2023 19:47:10 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 29 Mar 2023 19:47:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 19:47:10 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc6fa7c28a8decb0b5d8e618de112a92abffb23d50587ab655da8c0377b5600`  
		Last Modified: Wed, 29 Mar 2023 19:47:47 GMT  
		Size: 284.8 KB (284812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21cf95c5a006a671912de5168918eddd1e9c05cd421dff12f887a8c181f70e0`  
		Last Modified: Wed, 29 Mar 2023 19:48:02 GMT  
		Size: 19.2 MB (19204176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2bcffaef79fdff21ef7d1aab7e29c3979f02fc09722d31579c2becec4a6cc4`  
		Last Modified: Wed, 29 Mar 2023 19:47:58 GMT  
		Size: 12.3 KB (12262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbf4b0bd987fdf74326dc60a63e79ff2b7ed724c7891b189f56ff7164ade697`  
		Last Modified: Wed, 29 Mar 2023 19:47:58 GMT  
		Size: 11.9 KB (11894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b531f569476374ba4b720bad481fdcc01e110c2c27877b7a79753751bf5d6f`  
		Last Modified: Wed, 29 Mar 2023 19:47:58 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.10`

```console
$ docker pull chronograf@sha256:2e5217574071d5da90d91a37826b89393cd81aba22160e16fe2c92749e87ebf9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8.10` - linux; amd64

```console
$ docker pull chronograf@sha256:d5c267ecd20ee2bd410d30c0dc42aa5e37f9b0841b62f5a4a58742b1436eb308
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.2 MB (71240949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5cd8cc544951fd0ff71fc99961a02c193858b222ac6135c08c38ce029e9b690`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:11:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Mar 2023 06:11:37 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Thu, 23 Mar 2023 06:11:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 06:11:43 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Mar 2023 06:11:43 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Mar 2023 06:11:43 GMT
EXPOSE 8888
# Thu, 23 Mar 2023 06:11:43 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Mar 2023 06:11:43 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Mar 2023 06:11:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 06:11:43 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b38a80a9c9f14745c5d3c39eca2ab0731ac3ad6e829bda6ab0ba1876fa33b2`  
		Last Modified: Thu, 23 Mar 2023 06:12:36 GMT  
		Size: 5.2 MB (5226171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa39c924992902744aa1e6d0ec24a57c5ceac251cd245c70b048ba493a88a717`  
		Last Modified: Thu, 23 Mar 2023 06:12:39 GMT  
		Size: 34.6 MB (34578976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634ccb6519123dedae91ececd01a0bbfda5c481ef3333f5337214655e3f49ece`  
		Last Modified: Thu, 23 Mar 2023 06:12:35 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec444031881454f7b613a330771dfc6821a4aef1bdc7029fdea9e7ee8aca7e35`  
		Last Modified: Thu, 23 Mar 2023 06:12:35 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be954e0035ff49b0ee01cf3ddc26a2b4adcbadbe35740f5bf0a41d3f367d9f56`  
		Last Modified: Thu, 23 Mar 2023 06:12:35 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.10` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:60786ec7c07058f39313af7887a07dae6dccf39b64bbb7d945c2c6025660d702
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63843589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfa33c78bbf9838bccd5247cc0638a86daf37378bd0c4ab7dd8d7a02ade75f88`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:23:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Mar 2023 13:23:33 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Thu, 23 Mar 2023 13:23:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 13:23:41 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Mar 2023 13:23:41 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Mar 2023 13:23:41 GMT
EXPOSE 8888
# Thu, 23 Mar 2023 13:23:41 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Mar 2023 13:23:41 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Mar 2023 13:23:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 13:23:41 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48bdccd5f6d7a7f2a2045df36ec26beea220a468695975eb1146d58b1737dc5`  
		Last Modified: Thu, 23 Mar 2023 13:24:26 GMT  
		Size: 4.5 MB (4491664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6175a1191ed4e7dde0a5af3daeca99f0e0050e390ff8c62a1def6002bcd03e84`  
		Last Modified: Thu, 23 Mar 2023 13:24:30 GMT  
		Size: 32.8 MB (32750199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b477330cf38d31553d29b0095e449f3088d967f8abd999106b2a41f08f8d78e2`  
		Last Modified: Thu, 23 Mar 2023 13:24:26 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b91a1d011d4bc43f43794e13a8546acb8c1910a807883752e97edbec454c47`  
		Last Modified: Thu, 23 Mar 2023 13:24:26 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9242837f6d7c8b34788881a68a813f398e0121de48191f3f17f27a89adb86e`  
		Last Modified: Thu, 23 Mar 2023 13:24:26 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.10` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:b86a8d6dbeef7bcb0b5fa0223bcafc66f9e21ccd5507a7f16ab71770e0a7c747
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67941430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:264df0ca3bead32e50c1dfa54cb244b68f9d7e28b7a252e860dd153618fcb7ab`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:16:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 01:16:30 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 12 Apr 2023 01:16:36 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:16:36 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 12 Apr 2023 01:16:36 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 12 Apr 2023 01:16:36 GMT
EXPOSE 8888
# Wed, 12 Apr 2023 01:16:36 GMT
VOLUME [/var/lib/chronograf]
# Wed, 12 Apr 2023 01:16:36 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 12 Apr 2023 01:16:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 01:16:37 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8d0543e677dafef62b6b0cbed79f1e23b76b074feeec13c79ac54cdd154a33`  
		Last Modified: Wed, 12 Apr 2023 01:17:20 GMT  
		Size: 5.2 MB (5209387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c60b1c7c5a384549291dc92649a139620b5b6ee91e6b20368347d4979d8016f`  
		Last Modified: Wed, 12 Apr 2023 01:17:21 GMT  
		Size: 32.6 MB (32643822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2919cf3fdd56b48266aa8a0d5d195c56353e2c499b6e48e3a8e431de687f52`  
		Last Modified: Wed, 12 Apr 2023 01:17:18 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ab1c1238d012fd8130766a747e70a56e6d953dda9fece1b4f7a655a2e75171`  
		Last Modified: Wed, 12 Apr 2023 01:17:18 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9deedd4ab510bf3dcd0011ff677493e3b5f7500b8789c7a59892010d368182da`  
		Last Modified: Wed, 12 Apr 2023 01:17:18 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.10-alpine`

```console
$ docker pull chronograf@sha256:e60095ede17376b4c03f67a2f456888f5f2b923885bff7b68ddf3e3dd02f7f51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.8.10-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:5e27bfc9734a3b128ce7328af10d8b2c1159c1043e20966a61143c1bd269dd0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22888222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:686e49688a842468eebc393eafcdbb57dbf812dd59fcd3407c3d635e81f53d83`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 19:46:51 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 29 Mar 2023 19:47:01 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 29 Mar 2023 19:47:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 29 Mar 2023 19:47:09 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 29 Mar 2023 19:47:09 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 29 Mar 2023 19:47:09 GMT
EXPOSE 8888
# Wed, 29 Mar 2023 19:47:09 GMT
VOLUME [/var/lib/chronograf]
# Wed, 29 Mar 2023 19:47:10 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 29 Mar 2023 19:47:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 19:47:10 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc6fa7c28a8decb0b5d8e618de112a92abffb23d50587ab655da8c0377b5600`  
		Last Modified: Wed, 29 Mar 2023 19:47:47 GMT  
		Size: 284.8 KB (284812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21cf95c5a006a671912de5168918eddd1e9c05cd421dff12f887a8c181f70e0`  
		Last Modified: Wed, 29 Mar 2023 19:48:02 GMT  
		Size: 19.2 MB (19204176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2bcffaef79fdff21ef7d1aab7e29c3979f02fc09722d31579c2becec4a6cc4`  
		Last Modified: Wed, 29 Mar 2023 19:47:58 GMT  
		Size: 12.3 KB (12262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbf4b0bd987fdf74326dc60a63e79ff2b7ed724c7891b189f56ff7164ade697`  
		Last Modified: Wed, 29 Mar 2023 19:47:58 GMT  
		Size: 11.9 KB (11894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b531f569476374ba4b720bad481fdcc01e110c2c27877b7a79753751bf5d6f`  
		Last Modified: Wed, 29 Mar 2023 19:47:58 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9`

```console
$ docker pull chronograf@sha256:cfafc296da5de8b322f15f1e711cb1428eebcf39a5886cb3535a3dfece2ec00f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.9` - linux; amd64

```console
$ docker pull chronograf@sha256:8275a47e8954dc9de3421eb12e3caefb95c0d8e05d8a41867b802a34ffe27b72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71888473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:267a9bd73fdd1e8c17e24d067bfbd4cde282b2be1fcb589d7d43a71964bcdbd1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:11:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Mar 2023 06:11:48 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Thu, 23 Mar 2023 06:11:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 06:11:55 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Mar 2023 06:11:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Mar 2023 06:11:55 GMT
EXPOSE 8888
# Thu, 23 Mar 2023 06:11:55 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Mar 2023 06:11:55 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Mar 2023 06:11:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 06:11:55 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b38a80a9c9f14745c5d3c39eca2ab0731ac3ad6e829bda6ab0ba1876fa33b2`  
		Last Modified: Thu, 23 Mar 2023 06:12:36 GMT  
		Size: 5.2 MB (5226171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b1074cfc6898328ebc115273d16edcf708f557d75b47102188683bea317a70`  
		Last Modified: Thu, 23 Mar 2023 06:12:52 GMT  
		Size: 35.2 MB (35226508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894913378309de72c4d5cae996455b7c1e379bdef4512ebd6752b61a3df279b6`  
		Last Modified: Thu, 23 Mar 2023 06:12:48 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a834c2d89c4157fe731213688a8cd8f862d9d835dde017a4252ab0d917a5ef`  
		Last Modified: Thu, 23 Mar 2023 06:12:48 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e612f740fb125f7fdd57accad65147f45c4630aa533ea4f1d6fb033b873bb3`  
		Last Modified: Thu, 23 Mar 2023 06:12:48 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:47abecad645b82fdb5fad48d32856293a9f1a7229702148da7d0c59b73ee5f8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64619779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d80f35957ab98e2156d4eea73c3fa0a0a61a8e9f6545fb852f719a26000750f9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:23:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Mar 2023 13:23:45 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Thu, 23 Mar 2023 13:23:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 13:23:52 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Mar 2023 13:23:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Mar 2023 13:23:52 GMT
EXPOSE 8888
# Thu, 23 Mar 2023 13:23:52 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Mar 2023 13:23:53 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Mar 2023 13:23:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 13:23:53 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48bdccd5f6d7a7f2a2045df36ec26beea220a468695975eb1146d58b1737dc5`  
		Last Modified: Thu, 23 Mar 2023 13:24:26 GMT  
		Size: 4.5 MB (4491664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16462e1b7a9c26af858f8363701d33b850b4650b9a6e3f9aff27674d736d99ce`  
		Last Modified: Thu, 23 Mar 2023 13:24:41 GMT  
		Size: 33.5 MB (33526401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66af931b4d20c51bdba984e4370c959aed0c6260bc82cd95f7b6e059d14b3e3a`  
		Last Modified: Thu, 23 Mar 2023 13:24:37 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fab08484bd3a76aec08a5548251311ade493a67318fdd56106387838e9461d`  
		Last Modified: Thu, 23 Mar 2023 13:24:37 GMT  
		Size: 11.9 KB (11901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29131c4b3e0749ac0651fda92779119721d77593d80b0dd12316837c6fdef49b`  
		Last Modified: Thu, 23 Mar 2023 13:24:37 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:de9b5c2cb1aa18a0e39c61445feb50f3154d1a17871e4512212ccd4315bfb95d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68693042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdd5b6aade16387cbea4659c07cb3ddde2fe40977a7ac89e98b3a21962aad1d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:16:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 01:16:39 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 12 Apr 2023 01:16:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:16:45 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 12 Apr 2023 01:16:45 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 12 Apr 2023 01:16:46 GMT
EXPOSE 8888
# Wed, 12 Apr 2023 01:16:46 GMT
VOLUME [/var/lib/chronograf]
# Wed, 12 Apr 2023 01:16:46 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 12 Apr 2023 01:16:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 01:16:46 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8d0543e677dafef62b6b0cbed79f1e23b76b074feeec13c79ac54cdd154a33`  
		Last Modified: Wed, 12 Apr 2023 01:17:20 GMT  
		Size: 5.2 MB (5209387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a34d1b01dc9a8cf22edc87551227483d5d6b0158907e5c07117fb33c33246e`  
		Last Modified: Wed, 12 Apr 2023 01:17:33 GMT  
		Size: 33.4 MB (33395434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4fb446ad1ed3e3dd444b7200a36adebf28a4ff868a4df959738be203f48f86`  
		Last Modified: Wed, 12 Apr 2023 01:17:30 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823435ebf2b77206743f2562341483635458807a5fd04d9ef0bf92e077678ca4`  
		Last Modified: Wed, 12 Apr 2023 01:17:29 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56edbe45c7552660781d25584eb72d1507e96a01f922bbdd92b6f462ba0930ea`  
		Last Modified: Wed, 12 Apr 2023 01:17:30 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9-alpine`

```console
$ docker pull chronograf@sha256:29364ddcf6f0e0c8ef7d5e350d15621839f4594de457e89da15409bf91a6b8cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.9-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:acbbaeba463a83f4b5c1b8b6fc3aa57e90b466303565ed43c1c232225dd32115
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23356204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:569571223e58815ba31b87372f85abbf3d4c671d28918608ef7495d468e54845`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 19:46:51 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 29 Mar 2023 19:47:14 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 29 Mar 2023 19:47:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 29 Mar 2023 19:47:20 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 29 Mar 2023 19:47:20 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 29 Mar 2023 19:47:20 GMT
EXPOSE 8888
# Wed, 29 Mar 2023 19:47:20 GMT
VOLUME [/var/lib/chronograf]
# Wed, 29 Mar 2023 19:47:20 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 29 Mar 2023 19:47:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 19:47:20 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc6fa7c28a8decb0b5d8e618de112a92abffb23d50587ab655da8c0377b5600`  
		Last Modified: Wed, 29 Mar 2023 19:47:47 GMT  
		Size: 284.8 KB (284812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6dc9599f47216f2e8a1f2d98af6c416343d4817a5f9f5190d5d89582ba0fa0`  
		Last Modified: Wed, 29 Mar 2023 19:48:13 GMT  
		Size: 19.7 MB (19672158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f872500289b35787a2c10279e2512b492ee25177524a619367ab91a84425060`  
		Last Modified: Wed, 29 Mar 2023 19:48:10 GMT  
		Size: 12.3 KB (12260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e70f250c30a788217d166003c358e678ffa41bda5e7dc0d90f888784d9a37f`  
		Last Modified: Wed, 29 Mar 2023 19:48:10 GMT  
		Size: 11.9 KB (11897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae049a6108ae0a63f98bc3c9093ac1368ef5baeb6226527cc525786b0ed7f082`  
		Last Modified: Wed, 29 Mar 2023 19:48:10 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9.4`

```console
$ docker pull chronograf@sha256:cfafc296da5de8b322f15f1e711cb1428eebcf39a5886cb3535a3dfece2ec00f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.9.4` - linux; amd64

```console
$ docker pull chronograf@sha256:8275a47e8954dc9de3421eb12e3caefb95c0d8e05d8a41867b802a34ffe27b72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71888473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:267a9bd73fdd1e8c17e24d067bfbd4cde282b2be1fcb589d7d43a71964bcdbd1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:11:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Mar 2023 06:11:48 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Thu, 23 Mar 2023 06:11:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 06:11:55 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Mar 2023 06:11:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Mar 2023 06:11:55 GMT
EXPOSE 8888
# Thu, 23 Mar 2023 06:11:55 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Mar 2023 06:11:55 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Mar 2023 06:11:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 06:11:55 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b38a80a9c9f14745c5d3c39eca2ab0731ac3ad6e829bda6ab0ba1876fa33b2`  
		Last Modified: Thu, 23 Mar 2023 06:12:36 GMT  
		Size: 5.2 MB (5226171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b1074cfc6898328ebc115273d16edcf708f557d75b47102188683bea317a70`  
		Last Modified: Thu, 23 Mar 2023 06:12:52 GMT  
		Size: 35.2 MB (35226508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894913378309de72c4d5cae996455b7c1e379bdef4512ebd6752b61a3df279b6`  
		Last Modified: Thu, 23 Mar 2023 06:12:48 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a834c2d89c4157fe731213688a8cd8f862d9d835dde017a4252ab0d917a5ef`  
		Last Modified: Thu, 23 Mar 2023 06:12:48 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e612f740fb125f7fdd57accad65147f45c4630aa533ea4f1d6fb033b873bb3`  
		Last Modified: Thu, 23 Mar 2023 06:12:48 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9.4` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:47abecad645b82fdb5fad48d32856293a9f1a7229702148da7d0c59b73ee5f8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64619779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d80f35957ab98e2156d4eea73c3fa0a0a61a8e9f6545fb852f719a26000750f9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:23:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Mar 2023 13:23:45 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Thu, 23 Mar 2023 13:23:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 13:23:52 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Mar 2023 13:23:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Mar 2023 13:23:52 GMT
EXPOSE 8888
# Thu, 23 Mar 2023 13:23:52 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Mar 2023 13:23:53 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Mar 2023 13:23:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 13:23:53 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48bdccd5f6d7a7f2a2045df36ec26beea220a468695975eb1146d58b1737dc5`  
		Last Modified: Thu, 23 Mar 2023 13:24:26 GMT  
		Size: 4.5 MB (4491664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16462e1b7a9c26af858f8363701d33b850b4650b9a6e3f9aff27674d736d99ce`  
		Last Modified: Thu, 23 Mar 2023 13:24:41 GMT  
		Size: 33.5 MB (33526401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66af931b4d20c51bdba984e4370c959aed0c6260bc82cd95f7b6e059d14b3e3a`  
		Last Modified: Thu, 23 Mar 2023 13:24:37 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fab08484bd3a76aec08a5548251311ade493a67318fdd56106387838e9461d`  
		Last Modified: Thu, 23 Mar 2023 13:24:37 GMT  
		Size: 11.9 KB (11901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29131c4b3e0749ac0651fda92779119721d77593d80b0dd12316837c6fdef49b`  
		Last Modified: Thu, 23 Mar 2023 13:24:37 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9.4` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:de9b5c2cb1aa18a0e39c61445feb50f3154d1a17871e4512212ccd4315bfb95d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68693042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdd5b6aade16387cbea4659c07cb3ddde2fe40977a7ac89e98b3a21962aad1d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:16:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 01:16:39 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 12 Apr 2023 01:16:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:16:45 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 12 Apr 2023 01:16:45 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 12 Apr 2023 01:16:46 GMT
EXPOSE 8888
# Wed, 12 Apr 2023 01:16:46 GMT
VOLUME [/var/lib/chronograf]
# Wed, 12 Apr 2023 01:16:46 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 12 Apr 2023 01:16:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 01:16:46 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8d0543e677dafef62b6b0cbed79f1e23b76b074feeec13c79ac54cdd154a33`  
		Last Modified: Wed, 12 Apr 2023 01:17:20 GMT  
		Size: 5.2 MB (5209387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a34d1b01dc9a8cf22edc87551227483d5d6b0158907e5c07117fb33c33246e`  
		Last Modified: Wed, 12 Apr 2023 01:17:33 GMT  
		Size: 33.4 MB (33395434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4fb446ad1ed3e3dd444b7200a36adebf28a4ff868a4df959738be203f48f86`  
		Last Modified: Wed, 12 Apr 2023 01:17:30 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823435ebf2b77206743f2562341483635458807a5fd04d9ef0bf92e077678ca4`  
		Last Modified: Wed, 12 Apr 2023 01:17:29 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56edbe45c7552660781d25584eb72d1507e96a01f922bbdd92b6f462ba0930ea`  
		Last Modified: Wed, 12 Apr 2023 01:17:30 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9.4-alpine`

```console
$ docker pull chronograf@sha256:29364ddcf6f0e0c8ef7d5e350d15621839f4594de457e89da15409bf91a6b8cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.9.4-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:acbbaeba463a83f4b5c1b8b6fc3aa57e90b466303565ed43c1c232225dd32115
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23356204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:569571223e58815ba31b87372f85abbf3d4c671d28918608ef7495d468e54845`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 19:46:51 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 29 Mar 2023 19:47:14 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Wed, 29 Mar 2023 19:47:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 29 Mar 2023 19:47:20 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 29 Mar 2023 19:47:20 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 29 Mar 2023 19:47:20 GMT
EXPOSE 8888
# Wed, 29 Mar 2023 19:47:20 GMT
VOLUME [/var/lib/chronograf]
# Wed, 29 Mar 2023 19:47:20 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 29 Mar 2023 19:47:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 19:47:20 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc6fa7c28a8decb0b5d8e618de112a92abffb23d50587ab655da8c0377b5600`  
		Last Modified: Wed, 29 Mar 2023 19:47:47 GMT  
		Size: 284.8 KB (284812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6dc9599f47216f2e8a1f2d98af6c416343d4817a5f9f5190d5d89582ba0fa0`  
		Last Modified: Wed, 29 Mar 2023 19:48:13 GMT  
		Size: 19.7 MB (19672158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f872500289b35787a2c10279e2512b492ee25177524a619367ab91a84425060`  
		Last Modified: Wed, 29 Mar 2023 19:48:10 GMT  
		Size: 12.3 KB (12260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e70f250c30a788217d166003c358e678ffa41bda5e7dc0d90f888784d9a37f`  
		Last Modified: Wed, 29 Mar 2023 19:48:10 GMT  
		Size: 11.9 KB (11897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae049a6108ae0a63f98bc3c9093ac1368ef5baeb6226527cc525786b0ed7f082`  
		Last Modified: Wed, 29 Mar 2023 19:48:10 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:alpine`

```console
$ docker pull chronograf@sha256:98831602a8aa62cc195baea1c779fe5ca4bd888b12b4bc749c5973b57c5e3297
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:6062289ea692c0047e6608134571368e6f528b7f374c6644d374691a33720997
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31471176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6444543c380851da2dd2360a89fc011204ccaa4e28c7aea94ad6ba2a96efd413`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 19:46:51 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 29 Mar 2023 19:47:24 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Wed, 29 Mar 2023 19:47:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 29 Mar 2023 19:47:30 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 29 Mar 2023 19:47:30 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 29 Mar 2023 19:47:30 GMT
EXPOSE 8888
# Wed, 29 Mar 2023 19:47:30 GMT
VOLUME [/var/lib/chronograf]
# Wed, 29 Mar 2023 19:47:30 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 29 Mar 2023 19:47:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 19:47:31 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc6fa7c28a8decb0b5d8e618de112a92abffb23d50587ab655da8c0377b5600`  
		Last Modified: Wed, 29 Mar 2023 19:47:47 GMT  
		Size: 284.8 KB (284812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867fc62a9977fb48ebff54478afb2ae589ea2a08853a70b3f93a131ce67ee55f`  
		Last Modified: Wed, 29 Mar 2023 19:48:26 GMT  
		Size: 27.8 MB (27787123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03de77a31cf58915f9a2085eadee11338ee3e454f6d0a2c4d064e4ca5fc369e3`  
		Last Modified: Wed, 29 Mar 2023 19:48:21 GMT  
		Size: 12.3 KB (12266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9bccc09d6b731509690ff6112f9dd2b9cc3408ce4f6942d2285ce32f54667a`  
		Last Modified: Wed, 29 Mar 2023 19:48:21 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4dbd842e2dd7377ae86030ceece05fa917381af338a44999315838b590e941`  
		Last Modified: Wed, 29 Mar 2023 19:48:21 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:latest`

```console
$ docker pull chronograf@sha256:3d77e6c9aea81e0d0f00fd65e5d2feed23dec5bef6ac91f8e277b5b2c5e14fa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:1575b03b10ca5ccf30556eea9dbd26982e1a99d692d5de81f0377d84c8a91438
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.8 MB (82803422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:054a06db258d36e98f5dc5ae85d5a8d56fde1d3ea6097bb7a5ac4c7f3251bb58`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:11:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Mar 2023 06:11:59 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Thu, 23 Mar 2023 06:12:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 06:12:06 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Mar 2023 06:12:06 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Mar 2023 06:12:06 GMT
EXPOSE 8888
# Thu, 23 Mar 2023 06:12:06 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Mar 2023 06:12:06 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Mar 2023 06:12:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 06:12:06 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b38a80a9c9f14745c5d3c39eca2ab0731ac3ad6e829bda6ab0ba1876fa33b2`  
		Last Modified: Thu, 23 Mar 2023 06:12:36 GMT  
		Size: 5.2 MB (5226171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6b1b6422de45b88751631cd54d00aa6d1c9874585581faddd81344f0acf2f5`  
		Last Modified: Thu, 23 Mar 2023 06:13:08 GMT  
		Size: 46.1 MB (46141452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685b83b562e36e2face4136733838671e6425ac7f52a0d3016937da2327e260b`  
		Last Modified: Thu, 23 Mar 2023 06:13:02 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af80511b750f16f6e44c34b5cf5820739dd58ba881371c8486917b9e1f2f47d7`  
		Last Modified: Thu, 23 Mar 2023 06:13:02 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144629686b91940362645ae1fa7bf7ebbf5121109839bebd74562587534c1931`  
		Last Modified: Thu, 23 Mar 2023 06:13:02 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:0236ae34e7f3fd8dcb6b3dd18f40c795f316e11c08e6ba8522f475112c7a0050
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74943587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ec091f267a7b261d28f060556268eb5067b2c6cd38cc917fbde1db51f2f28ea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:23:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Mar 2023 13:23:54 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Thu, 23 Mar 2023 13:24:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 13:24:03 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 23 Mar 2023 13:24:03 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 23 Mar 2023 13:24:03 GMT
EXPOSE 8888
# Thu, 23 Mar 2023 13:24:03 GMT
VOLUME [/var/lib/chronograf]
# Thu, 23 Mar 2023 13:24:04 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 23 Mar 2023 13:24:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 13:24:04 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48bdccd5f6d7a7f2a2045df36ec26beea220a468695975eb1146d58b1737dc5`  
		Last Modified: Thu, 23 Mar 2023 13:24:26 GMT  
		Size: 4.5 MB (4491664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c196ce85113ecf0ec03684d0e68394dd58b4d0c618746eeec78d1aed39443f8`  
		Last Modified: Thu, 23 Mar 2023 13:24:56 GMT  
		Size: 43.9 MB (43850197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23338b9c5719d08a89afae62665541bd907344d136f89aade4cb8421a2a24ee9`  
		Last Modified: Thu, 23 Mar 2023 13:24:49 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf694109367e4ab8897da76728f00e57301d62fa2867226ef97e4d6ccf5750`  
		Last Modified: Thu, 23 Mar 2023 13:24:49 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f9d7aaebdf9fb9009f624c051e2bb8b36a356fa649b8b0d0ea6585c3d58a0e`  
		Last Modified: Thu, 23 Mar 2023 13:24:49 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:61723a713e5e956511babbb5720cac4539df70a4fa0e363fe6d3d18bfdef4c6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79152403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f65ba602b25252bc53e80ff5e1143cf5c59529a9379c1b11b8bf4b1386dee4f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:16:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 01:16:49 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Wed, 12 Apr 2023 01:16:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:16:55 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 12 Apr 2023 01:16:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 12 Apr 2023 01:16:55 GMT
EXPOSE 8888
# Wed, 12 Apr 2023 01:16:55 GMT
VOLUME [/var/lib/chronograf]
# Wed, 12 Apr 2023 01:16:55 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 12 Apr 2023 01:16:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 01:16:56 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8d0543e677dafef62b6b0cbed79f1e23b76b074feeec13c79ac54cdd154a33`  
		Last Modified: Wed, 12 Apr 2023 01:17:20 GMT  
		Size: 5.2 MB (5209387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f76b035a31a949a5946475fe6e1dc30b9939da944e0e9a6eae9cf255a31eea`  
		Last Modified: Wed, 12 Apr 2023 01:17:45 GMT  
		Size: 43.9 MB (43854802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37431348a86ec9a9ef0da51d65733c7c2ac2bc724c6f8c37b17551038bb70a45`  
		Last Modified: Wed, 12 Apr 2023 01:17:40 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0313fc537cd1c011b154938f1d65d0d66e7a589f4a2a9bf00b5748732d691fba`  
		Last Modified: Wed, 12 Apr 2023 01:17:41 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c78d43e9fb235b2d40a2a345f8a244952572332d461048af98ec37895a1d973`  
		Last Modified: Wed, 12 Apr 2023 01:17:41 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
