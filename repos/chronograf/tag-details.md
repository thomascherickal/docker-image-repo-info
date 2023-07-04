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
$ docker pull chronograf@sha256:a55b1724a890b78bbfa5aff4152632c4039e47b27166b957f06da9c44d0490f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.10` - linux; amd64

```console
$ docker pull chronograf@sha256:4c8a72a31cf1c6751c665bdb090cf7dcfdf2c4d29cc6a826c0341c1ac4e287e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.8 MB (82809646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e30929b3c76af4d2c56658f9ad656760fa3a66bd6034fdeef441fad99114c79c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:18:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 04:19:17 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Tue, 04 Jul 2023 04:19:24 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 04:19:24 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 04 Jul 2023 04:19:24 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 04 Jul 2023 04:19:24 GMT
EXPOSE 8888
# Tue, 04 Jul 2023 04:19:24 GMT
VOLUME [/var/lib/chronograf]
# Tue, 04 Jul 2023 04:19:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 04 Jul 2023 04:19:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 04:19:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2442302dfe8f99302044b2f10fa8cb2af7595d343d96ac7aa33263bd2e73be1b`  
		Last Modified: Tue, 04 Jul 2023 04:20:00 GMT  
		Size: 5.2 MB (5226360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009868036e3e962809f4734cf4a0d4c68017aaf3d8bc1bdc7a4f2388de7e8388`  
		Last Modified: Tue, 04 Jul 2023 04:20:34 GMT  
		Size: 46.1 MB (46141511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18dcb6401f859ffb576f7f730b11d86414e2091c979468533f9e84c3c70c940c`  
		Last Modified: Tue, 04 Jul 2023 04:20:27 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7c6e4727dfa5750009dc64b69a2a5b1603636489dd98a085839f1c0840fee6`  
		Last Modified: Tue, 04 Jul 2023 04:20:27 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e8a3c9c5d09608504a1d10e1fcdbb69d6a907d419e03a07cb380209ee9042c`  
		Last Modified: Tue, 04 Jul 2023 04:20:27 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:263afb762b7a64411805f8857c33ded7f85e4f7413b1325cbfba47ddb44021cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74945189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d20eb2acb74bc852b09805e44be7ad3878f729f19494eb31d4e6eded5b45c19c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:47 GMT
ADD file:319a24b7e30fc548f9dcf48ad6cee469e8bf7e89c67901cf3851e41e75693489 in / 
# Mon, 12 Jun 2023 23:58:47 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 14:29:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 14:29:44 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Tue, 13 Jun 2023 14:30:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 14:30:08 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Jun 2023 14:30:08 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Jun 2023 14:30:09 GMT
EXPOSE 8888
# Tue, 13 Jun 2023 14:30:09 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Jun 2023 14:30:09 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Jun 2023 14:30:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 14:30:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b7c295cb849275e211d18b720d2349cc84c0038be1a362aca4765ceb3342043c`  
		Last Modified: Tue, 13 Jun 2023 00:04:24 GMT  
		Size: 26.6 MB (26578690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9828e77333b987f92a40b4d360e7caddfe3d4e15ab3704412d441c76c6f2f6e5`  
		Last Modified: Tue, 13 Jun 2023 14:30:36 GMT  
		Size: 4.5 MB (4491786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b32968d44f52b6cd3d1a65cb11cb4004bcc25c8b863203712f1bb8e5055f6c4`  
		Last Modified: Tue, 13 Jun 2023 14:31:10 GMT  
		Size: 43.9 MB (43850332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6de1a7010815c4e6669c17f8c9fc45d44542c9176c207b5a114d9d30a57344`  
		Last Modified: Tue, 13 Jun 2023 14:31:03 GMT  
		Size: 12.2 KB (12242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86be71e5593ed6f80300bbf7584cb55c79c3fdba2651086f4c664a7acfcee3b`  
		Last Modified: Tue, 13 Jun 2023 14:31:03 GMT  
		Size: 11.9 KB (11900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b4a29eb988930d4c676ee015ec2ba2e59882bf57198d75fadb4cbe47d9649b`  
		Last Modified: Tue, 13 Jun 2023 14:31:03 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:148be15bcf895d8b0c8c34ba9b5720811a41ca1f59c1d857c97d6155c6fd3193
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79151450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4129cf123b5472fd6f3874fc6b1174ff1677956fab058a43dbffb7c963569c33`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:49:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 04:49:20 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Tue, 13 Jun 2023 04:49:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:49:28 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Jun 2023 04:49:28 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Jun 2023 04:49:28 GMT
EXPOSE 8888
# Tue, 13 Jun 2023 04:49:28 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Jun 2023 04:49:29 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Jun 2023 04:49:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 04:49:29 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35881321b38cbd2cd0adca84b7f3eebd013709fb394b85cae0e1582b75d85b8e`  
		Last Modified: Tue, 13 Jun 2023 04:49:52 GMT  
		Size: 5.2 MB (5209405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8289f2a411b0fce95afd518dddcfa36f6c20a39d1edaaf2e7a33eedcf48d0cbf`  
		Last Modified: Tue, 13 Jun 2023 04:50:18 GMT  
		Size: 43.9 MB (43854831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2885bdd478f1729f1eef9e06f9b1327cef8e7d4f9abe94aa4da65fbfb597af7`  
		Last Modified: Tue, 13 Jun 2023 04:50:13 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a703d39b907ff7e8a7d24961e05de092327594eae96b440bd8a3221e0493ec3c`  
		Last Modified: Tue, 13 Jun 2023 04:50:13 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c8d401aa0a406ade4e84cfe8f4b1215200aabd2cbac7d67c883bf1d0767f14`  
		Last Modified: Tue, 13 Jun 2023 04:50:13 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.10-alpine`

```console
$ docker pull chronograf@sha256:9d62c72cebc36f428c0060313c3ef3e3377e0309711addf0170493a0620920a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.10-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:612bc34865193e974de365f3e61f464ac77ea1ad3c828c125ce158034cd22205
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31471523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d92372eb76aa713e1f80da30fab50499e9f6a9a5124e579f57eab9642694097`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:35:00 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 15 Jun 2023 04:35:33 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Thu, 15 Jun 2023 04:35:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 15 Jun 2023 04:35:39 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 15 Jun 2023 04:35:39 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 15 Jun 2023 04:35:39 GMT
EXPOSE 8888
# Thu, 15 Jun 2023 04:35:39 GMT
VOLUME [/var/lib/chronograf]
# Thu, 15 Jun 2023 04:35:39 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 15 Jun 2023 04:35:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 04:35:39 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd2f215a0656c3952ad3cfce3a088aa7765b3195f9e051a0a7995b2b4260c48`  
		Last Modified: Thu, 15 Jun 2023 04:35:57 GMT  
		Size: 284.9 KB (284929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de727897c91e79266c88af5c343cde0e3e5167b458a9e128d56da665c573a039`  
		Last Modified: Thu, 15 Jun 2023 04:36:38 GMT  
		Size: 27.8 MB (27787202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4d3f77996a15dce0f8e8ac9c5a89eb2d6db2ff2ef00bd3fb6c2f4efa1ec675`  
		Last Modified: Thu, 15 Jun 2023 04:36:33 GMT  
		Size: 12.3 KB (12266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0347e88c27ad598445a0a65573552937a41150af7f36b834b4d4a85d4bad794b`  
		Last Modified: Thu, 15 Jun 2023 04:36:33 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0656947d8c90443cbc4edb28052852f49a1a523a4b6e8e23bf7d0967ef2dc3bd`  
		Last Modified: Thu, 15 Jun 2023 04:36:33 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.10.1`

```console
$ docker pull chronograf@sha256:a55b1724a890b78bbfa5aff4152632c4039e47b27166b957f06da9c44d0490f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.10.1` - linux; amd64

```console
$ docker pull chronograf@sha256:4c8a72a31cf1c6751c665bdb090cf7dcfdf2c4d29cc6a826c0341c1ac4e287e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.8 MB (82809646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e30929b3c76af4d2c56658f9ad656760fa3a66bd6034fdeef441fad99114c79c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:18:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 04:19:17 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Tue, 04 Jul 2023 04:19:24 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 04:19:24 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 04 Jul 2023 04:19:24 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 04 Jul 2023 04:19:24 GMT
EXPOSE 8888
# Tue, 04 Jul 2023 04:19:24 GMT
VOLUME [/var/lib/chronograf]
# Tue, 04 Jul 2023 04:19:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 04 Jul 2023 04:19:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 04:19:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2442302dfe8f99302044b2f10fa8cb2af7595d343d96ac7aa33263bd2e73be1b`  
		Last Modified: Tue, 04 Jul 2023 04:20:00 GMT  
		Size: 5.2 MB (5226360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009868036e3e962809f4734cf4a0d4c68017aaf3d8bc1bdc7a4f2388de7e8388`  
		Last Modified: Tue, 04 Jul 2023 04:20:34 GMT  
		Size: 46.1 MB (46141511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18dcb6401f859ffb576f7f730b11d86414e2091c979468533f9e84c3c70c940c`  
		Last Modified: Tue, 04 Jul 2023 04:20:27 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7c6e4727dfa5750009dc64b69a2a5b1603636489dd98a085839f1c0840fee6`  
		Last Modified: Tue, 04 Jul 2023 04:20:27 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e8a3c9c5d09608504a1d10e1fcdbb69d6a907d419e03a07cb380209ee9042c`  
		Last Modified: Tue, 04 Jul 2023 04:20:27 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10.1` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:263afb762b7a64411805f8857c33ded7f85e4f7413b1325cbfba47ddb44021cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74945189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d20eb2acb74bc852b09805e44be7ad3878f729f19494eb31d4e6eded5b45c19c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:47 GMT
ADD file:319a24b7e30fc548f9dcf48ad6cee469e8bf7e89c67901cf3851e41e75693489 in / 
# Mon, 12 Jun 2023 23:58:47 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 14:29:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 14:29:44 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Tue, 13 Jun 2023 14:30:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 14:30:08 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Jun 2023 14:30:08 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Jun 2023 14:30:09 GMT
EXPOSE 8888
# Tue, 13 Jun 2023 14:30:09 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Jun 2023 14:30:09 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Jun 2023 14:30:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 14:30:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b7c295cb849275e211d18b720d2349cc84c0038be1a362aca4765ceb3342043c`  
		Last Modified: Tue, 13 Jun 2023 00:04:24 GMT  
		Size: 26.6 MB (26578690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9828e77333b987f92a40b4d360e7caddfe3d4e15ab3704412d441c76c6f2f6e5`  
		Last Modified: Tue, 13 Jun 2023 14:30:36 GMT  
		Size: 4.5 MB (4491786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b32968d44f52b6cd3d1a65cb11cb4004bcc25c8b863203712f1bb8e5055f6c4`  
		Last Modified: Tue, 13 Jun 2023 14:31:10 GMT  
		Size: 43.9 MB (43850332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6de1a7010815c4e6669c17f8c9fc45d44542c9176c207b5a114d9d30a57344`  
		Last Modified: Tue, 13 Jun 2023 14:31:03 GMT  
		Size: 12.2 KB (12242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86be71e5593ed6f80300bbf7584cb55c79c3fdba2651086f4c664a7acfcee3b`  
		Last Modified: Tue, 13 Jun 2023 14:31:03 GMT  
		Size: 11.9 KB (11900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b4a29eb988930d4c676ee015ec2ba2e59882bf57198d75fadb4cbe47d9649b`  
		Last Modified: Tue, 13 Jun 2023 14:31:03 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10.1` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:148be15bcf895d8b0c8c34ba9b5720811a41ca1f59c1d857c97d6155c6fd3193
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79151450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4129cf123b5472fd6f3874fc6b1174ff1677956fab058a43dbffb7c963569c33`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:49:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 04:49:20 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Tue, 13 Jun 2023 04:49:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:49:28 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Jun 2023 04:49:28 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Jun 2023 04:49:28 GMT
EXPOSE 8888
# Tue, 13 Jun 2023 04:49:28 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Jun 2023 04:49:29 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Jun 2023 04:49:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 04:49:29 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35881321b38cbd2cd0adca84b7f3eebd013709fb394b85cae0e1582b75d85b8e`  
		Last Modified: Tue, 13 Jun 2023 04:49:52 GMT  
		Size: 5.2 MB (5209405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8289f2a411b0fce95afd518dddcfa36f6c20a39d1edaaf2e7a33eedcf48d0cbf`  
		Last Modified: Tue, 13 Jun 2023 04:50:18 GMT  
		Size: 43.9 MB (43854831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2885bdd478f1729f1eef9e06f9b1327cef8e7d4f9abe94aa4da65fbfb597af7`  
		Last Modified: Tue, 13 Jun 2023 04:50:13 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a703d39b907ff7e8a7d24961e05de092327594eae96b440bd8a3221e0493ec3c`  
		Last Modified: Tue, 13 Jun 2023 04:50:13 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c8d401aa0a406ade4e84cfe8f4b1215200aabd2cbac7d67c883bf1d0767f14`  
		Last Modified: Tue, 13 Jun 2023 04:50:13 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.10.1-alpine`

```console
$ docker pull chronograf@sha256:9d62c72cebc36f428c0060313c3ef3e3377e0309711addf0170493a0620920a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.10.1-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:612bc34865193e974de365f3e61f464ac77ea1ad3c828c125ce158034cd22205
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31471523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d92372eb76aa713e1f80da30fab50499e9f6a9a5124e579f57eab9642694097`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:35:00 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 15 Jun 2023 04:35:33 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Thu, 15 Jun 2023 04:35:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 15 Jun 2023 04:35:39 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 15 Jun 2023 04:35:39 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 15 Jun 2023 04:35:39 GMT
EXPOSE 8888
# Thu, 15 Jun 2023 04:35:39 GMT
VOLUME [/var/lib/chronograf]
# Thu, 15 Jun 2023 04:35:39 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 15 Jun 2023 04:35:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 04:35:39 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd2f215a0656c3952ad3cfce3a088aa7765b3195f9e051a0a7995b2b4260c48`  
		Last Modified: Thu, 15 Jun 2023 04:35:57 GMT  
		Size: 284.9 KB (284929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de727897c91e79266c88af5c343cde0e3e5167b458a9e128d56da665c573a039`  
		Last Modified: Thu, 15 Jun 2023 04:36:38 GMT  
		Size: 27.8 MB (27787202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4d3f77996a15dce0f8e8ac9c5a89eb2d6db2ff2ef00bd3fb6c2f4efa1ec675`  
		Last Modified: Thu, 15 Jun 2023 04:36:33 GMT  
		Size: 12.3 KB (12266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0347e88c27ad598445a0a65573552937a41150af7f36b834b4d4a85d4bad794b`  
		Last Modified: Thu, 15 Jun 2023 04:36:33 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0656947d8c90443cbc4edb28052852f49a1a523a4b6e8e23bf7d0967ef2dc3bd`  
		Last Modified: Thu, 15 Jun 2023 04:36:33 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7`

```console
$ docker pull chronograf@sha256:ce37a61eb63ca7400f8ee0d7bcfc1904496a677de0f2328624cda46517e09321
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7` - linux; amd64

```console
$ docker pull chronograf@sha256:c3102c9461b097ab32f3cc9de5c2040aa694adae55ad0ad37cfba5c5a61565e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70596127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bce694b906d0d7e517e4ded2c67f08a25ed031870d1f066a9d47550b4f17b5bb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:18:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 04:18:30 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 04 Jul 2023 04:18:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 04:18:39 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 04 Jul 2023 04:18:39 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 04 Jul 2023 04:18:39 GMT
EXPOSE 8888
# Tue, 04 Jul 2023 04:18:39 GMT
VOLUME [/var/lib/chronograf]
# Tue, 04 Jul 2023 04:18:39 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 04 Jul 2023 04:18:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 04:18:39 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc2603c0c701dea36776169c235816328b2f92bae43270ab42e5310926f4efa`  
		Last Modified: Tue, 04 Jul 2023 04:19:45 GMT  
		Size: 4.4 MB (4416615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f4d7e03a922d610329c2a37bda571f1280064460004093c4ef5eaa3c7352c0`  
		Last Modified: Tue, 04 Jul 2023 04:19:49 GMT  
		Size: 34.7 MB (34737741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a96f2be06d0a50c183c1497555144f0ba56f80950541147a86212c1f8ca18c`  
		Last Modified: Tue, 04 Jul 2023 04:19:45 GMT  
		Size: 12.2 KB (12242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908eaf4d7d6063e965af904cb722d15d84399c042ac0d3683c3c12de679c1cc0`  
		Last Modified: Tue, 04 Jul 2023 04:19:44 GMT  
		Size: 11.9 KB (11902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8064acecdd5a3dcbcbb64156672a6d4adefe7716e0f603a98f4d18ee2632ddcd`  
		Last Modified: Tue, 04 Jul 2023 04:19:44 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:4baa776fe0cfb469d4fa69170dc6e5f3ef8ef2b4d7268514675d8856379fe557
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63419491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b90eac8a4a8cbe8c2c96460843cf7ce6e1f163ca71312c612e4cba3224e8e770`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:47 GMT
ADD file:319a24b7e30fc548f9dcf48ad6cee469e8bf7e89c67901cf3851e41e75693489 in / 
# Mon, 12 Jun 2023 23:58:47 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 14:28:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 14:28:44 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 13 Jun 2023 14:28:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 14:28:59 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Jun 2023 14:29:00 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Jun 2023 14:29:00 GMT
EXPOSE 8888
# Tue, 13 Jun 2023 14:29:00 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Jun 2023 14:29:00 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Jun 2023 14:29:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 14:29:01 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b7c295cb849275e211d18b720d2349cc84c0038be1a362aca4765ceb3342043c`  
		Last Modified: Tue, 13 Jun 2023 00:04:24 GMT  
		Size: 26.6 MB (26578690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a9f7da5201973875a1e791bbb0216b08661818501a3c3caeab251c2e691090`  
		Last Modified: Tue, 13 Jun 2023 14:30:22 GMT  
		Size: 3.7 MB (3719124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc8335e28b2ceb3ec97474fde72bee09819d757d0db93e4781e39b770b99cb2`  
		Last Modified: Tue, 13 Jun 2023 14:30:27 GMT  
		Size: 33.1 MB (33097279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce81203a10d5f76cb696e7b612b469248953983cc700eb9a380b9c1235a6fd0f`  
		Last Modified: Tue, 13 Jun 2023 14:30:21 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa53ab46b2f0798eee6b9b3bcdda375cabde670601e4ed2a34695329b62b7e97`  
		Last Modified: Tue, 13 Jun 2023 14:30:21 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccba37c4609ef5fbe194aba590ea1f7aa72894ba187eeb2d404f7ad0077fca9`  
		Last Modified: Tue, 13 Jun 2023 14:30:22 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:26e6709185743f72dc709fbfc19be30e84b4bb5fc69ea0d38be28a4a4ed3a03c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67742922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c488130c1543dac95e143a9b415731ebb0c7a4a665168bfce653b1be3e32016a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:48:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 04:48:43 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 13 Jun 2023 04:48:51 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:48:51 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Jun 2023 04:48:51 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Jun 2023 04:48:51 GMT
EXPOSE 8888
# Tue, 13 Jun 2023 04:48:51 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Jun 2023 04:48:51 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Jun 2023 04:48:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 04:48:51 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c8daf4ce67b49aaf6aeba437f5eaa0cfe39d43f8f50b5014a08c849a02968a`  
		Last Modified: Tue, 13 Jun 2023 04:49:40 GMT  
		Size: 4.4 MB (4418132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8edc560c25d21563a2063fefa1cfa91f759b71de3dd9b58ae7929b743861cf97`  
		Last Modified: Tue, 13 Jun 2023 04:49:42 GMT  
		Size: 33.2 MB (33237563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea40a7670d9b2099ad31a18f6e902f82131921fe6608d626f6c39262bf4edb8`  
		Last Modified: Tue, 13 Jun 2023 04:49:39 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8786eb72117fa6629016baa43ccee5dad9fb7bb545ef499e151bc4117b3ec54`  
		Last Modified: Tue, 13 Jun 2023 04:49:39 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77eb0bb7610e8af2c9c6bb270c5b17a540d6ac94f59bff5daef149735f0c7d41`  
		Last Modified: Tue, 13 Jun 2023 04:49:39 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7-alpine`

```console
$ docker pull chronograf@sha256:c45bc7d84366cea6b1b902851fe180efb2d3dad959a7384a275057d32f4a24e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.7-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:3eaa1c6b4d57274c2a181e92e4d32f5e3b2ce74083938b0f57c32898f90296e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.2 MB (23241488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2655192cf47553a9da71225d9570b0a6ed514c8963e7e8f81fceb7f0d9fd6d2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:35:00 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 15 Jun 2023 04:35:00 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 15 Jun 2023 04:35:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 15 Jun 2023 04:35:05 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 15 Jun 2023 04:35:06 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 15 Jun 2023 04:35:06 GMT
EXPOSE 8888
# Thu, 15 Jun 2023 04:35:06 GMT
VOLUME [/var/lib/chronograf]
# Thu, 15 Jun 2023 04:35:06 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 15 Jun 2023 04:35:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 04:35:06 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd2f215a0656c3952ad3cfce3a088aa7765b3195f9e051a0a7995b2b4260c48`  
		Last Modified: Thu, 15 Jun 2023 04:35:57 GMT  
		Size: 284.9 KB (284929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d939a17986882c795cafbd0e8fed626f72a6055e186f1966c9dcfc722fd9d87`  
		Last Modified: Thu, 15 Jun 2023 04:36:00 GMT  
		Size: 19.6 MB (19557178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6037df3946668958b094a0d7cb915b643b97438ba4e6d75213139f55df998970`  
		Last Modified: Thu, 15 Jun 2023 04:35:57 GMT  
		Size: 12.3 KB (12259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4628dcb858423f19f1e7df9bee5e95e129c6ad4fde51b5759f2398c9fac50be`  
		Last Modified: Thu, 15 Jun 2023 04:35:57 GMT  
		Size: 11.9 KB (11893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f1676910e4ded7481e4fe3b71d8a329c053e23ce9c689e45a53d2b9a7cf2ea`  
		Last Modified: Thu, 15 Jun 2023 04:35:57 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17`

```console
$ docker pull chronograf@sha256:ce37a61eb63ca7400f8ee0d7bcfc1904496a677de0f2328624cda46517e09321
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7.17` - linux; amd64

```console
$ docker pull chronograf@sha256:c3102c9461b097ab32f3cc9de5c2040aa694adae55ad0ad37cfba5c5a61565e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70596127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bce694b906d0d7e517e4ded2c67f08a25ed031870d1f066a9d47550b4f17b5bb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:18:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 04:18:30 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 04 Jul 2023 04:18:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 04:18:39 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 04 Jul 2023 04:18:39 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 04 Jul 2023 04:18:39 GMT
EXPOSE 8888
# Tue, 04 Jul 2023 04:18:39 GMT
VOLUME [/var/lib/chronograf]
# Tue, 04 Jul 2023 04:18:39 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 04 Jul 2023 04:18:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 04:18:39 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc2603c0c701dea36776169c235816328b2f92bae43270ab42e5310926f4efa`  
		Last Modified: Tue, 04 Jul 2023 04:19:45 GMT  
		Size: 4.4 MB (4416615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f4d7e03a922d610329c2a37bda571f1280064460004093c4ef5eaa3c7352c0`  
		Last Modified: Tue, 04 Jul 2023 04:19:49 GMT  
		Size: 34.7 MB (34737741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a96f2be06d0a50c183c1497555144f0ba56f80950541147a86212c1f8ca18c`  
		Last Modified: Tue, 04 Jul 2023 04:19:45 GMT  
		Size: 12.2 KB (12242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908eaf4d7d6063e965af904cb722d15d84399c042ac0d3683c3c12de679c1cc0`  
		Last Modified: Tue, 04 Jul 2023 04:19:44 GMT  
		Size: 11.9 KB (11902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8064acecdd5a3dcbcbb64156672a6d4adefe7716e0f603a98f4d18ee2632ddcd`  
		Last Modified: Tue, 04 Jul 2023 04:19:44 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:4baa776fe0cfb469d4fa69170dc6e5f3ef8ef2b4d7268514675d8856379fe557
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63419491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b90eac8a4a8cbe8c2c96460843cf7ce6e1f163ca71312c612e4cba3224e8e770`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:47 GMT
ADD file:319a24b7e30fc548f9dcf48ad6cee469e8bf7e89c67901cf3851e41e75693489 in / 
# Mon, 12 Jun 2023 23:58:47 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 14:28:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 14:28:44 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 13 Jun 2023 14:28:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 14:28:59 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Jun 2023 14:29:00 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Jun 2023 14:29:00 GMT
EXPOSE 8888
# Tue, 13 Jun 2023 14:29:00 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Jun 2023 14:29:00 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Jun 2023 14:29:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 14:29:01 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b7c295cb849275e211d18b720d2349cc84c0038be1a362aca4765ceb3342043c`  
		Last Modified: Tue, 13 Jun 2023 00:04:24 GMT  
		Size: 26.6 MB (26578690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a9f7da5201973875a1e791bbb0216b08661818501a3c3caeab251c2e691090`  
		Last Modified: Tue, 13 Jun 2023 14:30:22 GMT  
		Size: 3.7 MB (3719124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc8335e28b2ceb3ec97474fde72bee09819d757d0db93e4781e39b770b99cb2`  
		Last Modified: Tue, 13 Jun 2023 14:30:27 GMT  
		Size: 33.1 MB (33097279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce81203a10d5f76cb696e7b612b469248953983cc700eb9a380b9c1235a6fd0f`  
		Last Modified: Tue, 13 Jun 2023 14:30:21 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa53ab46b2f0798eee6b9b3bcdda375cabde670601e4ed2a34695329b62b7e97`  
		Last Modified: Tue, 13 Jun 2023 14:30:21 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccba37c4609ef5fbe194aba590ea1f7aa72894ba187eeb2d404f7ad0077fca9`  
		Last Modified: Tue, 13 Jun 2023 14:30:22 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:26e6709185743f72dc709fbfc19be30e84b4bb5fc69ea0d38be28a4a4ed3a03c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67742922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c488130c1543dac95e143a9b415731ebb0c7a4a665168bfce653b1be3e32016a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:48:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 04:48:43 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 13 Jun 2023 04:48:51 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:48:51 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Jun 2023 04:48:51 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Jun 2023 04:48:51 GMT
EXPOSE 8888
# Tue, 13 Jun 2023 04:48:51 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Jun 2023 04:48:51 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Jun 2023 04:48:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 04:48:51 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c8daf4ce67b49aaf6aeba437f5eaa0cfe39d43f8f50b5014a08c849a02968a`  
		Last Modified: Tue, 13 Jun 2023 04:49:40 GMT  
		Size: 4.4 MB (4418132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8edc560c25d21563a2063fefa1cfa91f759b71de3dd9b58ae7929b743861cf97`  
		Last Modified: Tue, 13 Jun 2023 04:49:42 GMT  
		Size: 33.2 MB (33237563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea40a7670d9b2099ad31a18f6e902f82131921fe6608d626f6c39262bf4edb8`  
		Last Modified: Tue, 13 Jun 2023 04:49:39 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8786eb72117fa6629016baa43ccee5dad9fb7bb545ef499e151bc4117b3ec54`  
		Last Modified: Tue, 13 Jun 2023 04:49:39 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77eb0bb7610e8af2c9c6bb270c5b17a540d6ac94f59bff5daef149735f0c7d41`  
		Last Modified: Tue, 13 Jun 2023 04:49:39 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17-alpine`

```console
$ docker pull chronograf@sha256:c45bc7d84366cea6b1b902851fe180efb2d3dad959a7384a275057d32f4a24e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.7.17-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:3eaa1c6b4d57274c2a181e92e4d32f5e3b2ce74083938b0f57c32898f90296e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.2 MB (23241488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2655192cf47553a9da71225d9570b0a6ed514c8963e7e8f81fceb7f0d9fd6d2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:35:00 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 15 Jun 2023 04:35:00 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 15 Jun 2023 04:35:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 15 Jun 2023 04:35:05 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 15 Jun 2023 04:35:06 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 15 Jun 2023 04:35:06 GMT
EXPOSE 8888
# Thu, 15 Jun 2023 04:35:06 GMT
VOLUME [/var/lib/chronograf]
# Thu, 15 Jun 2023 04:35:06 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 15 Jun 2023 04:35:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 04:35:06 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd2f215a0656c3952ad3cfce3a088aa7765b3195f9e051a0a7995b2b4260c48`  
		Last Modified: Thu, 15 Jun 2023 04:35:57 GMT  
		Size: 284.9 KB (284929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d939a17986882c795cafbd0e8fed626f72a6055e186f1966c9dcfc722fd9d87`  
		Last Modified: Thu, 15 Jun 2023 04:36:00 GMT  
		Size: 19.6 MB (19557178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6037df3946668958b094a0d7cb915b643b97438ba4e6d75213139f55df998970`  
		Last Modified: Thu, 15 Jun 2023 04:35:57 GMT  
		Size: 12.3 KB (12259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4628dcb858423f19f1e7df9bee5e95e129c6ad4fde51b5759f2398c9fac50be`  
		Last Modified: Thu, 15 Jun 2023 04:35:57 GMT  
		Size: 11.9 KB (11893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f1676910e4ded7481e4fe3b71d8a329c053e23ce9c689e45a53d2b9a7cf2ea`  
		Last Modified: Thu, 15 Jun 2023 04:35:57 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8`

```console
$ docker pull chronograf@sha256:c4202a920b4b9e002f562a6e1737b07ad98265ecc3cc25f22fc6a423f109e7a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8` - linux; amd64

```console
$ docker pull chronograf@sha256:47fb875ec0e8ce1a13e5b1f4ea597228b51c6c3c27c5c2ccd3440c264491be74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.2 MB (71247223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d71cad4f6770a970ee61513b308a24d28245afd9fc1cef89d9b812ac5e71804`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:18:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 04:18:53 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 04 Jul 2023 04:19:00 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 04:19:00 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 04 Jul 2023 04:19:00 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 04 Jul 2023 04:19:00 GMT
EXPOSE 8888
# Tue, 04 Jul 2023 04:19:00 GMT
VOLUME [/var/lib/chronograf]
# Tue, 04 Jul 2023 04:19:00 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 04 Jul 2023 04:19:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 04:19:00 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2442302dfe8f99302044b2f10fa8cb2af7595d343d96ac7aa33263bd2e73be1b`  
		Last Modified: Tue, 04 Jul 2023 04:20:00 GMT  
		Size: 5.2 MB (5226360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9269842128bc0b52ce9020a379de8f6c7ca488f52e56f82d6beb5e9f014b620d`  
		Last Modified: Tue, 04 Jul 2023 04:20:03 GMT  
		Size: 34.6 MB (34579086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5240e62f6dea38b6e1f99292839cc2ad0e9ae45221a429e88576ef3c651245`  
		Last Modified: Tue, 04 Jul 2023 04:19:58 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18cc5a3b74a0739ee53e7fc7f92e0e7f8d01d93559d6f6ec8b0a25a9da6277c`  
		Last Modified: Tue, 04 Jul 2023 04:19:59 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d35d924643ba624e5664eec24a3ce2c85672d75daae2dc8b30cbcb641258b83`  
		Last Modified: Tue, 04 Jul 2023 04:19:58 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:3053d3c88cc9407936db2311ffee028aec4189e97c47f28bb2b371d1edc47b29
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63845252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0468f16096fe953f4b4e0fb5150898cf546309691df4d38b93f651f5e294c2f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:47 GMT
ADD file:319a24b7e30fc548f9dcf48ad6cee469e8bf7e89c67901cf3851e41e75693489 in / 
# Mon, 12 Jun 2023 23:58:47 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 14:29:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 14:29:15 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 13 Jun 2023 14:29:25 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 14:29:26 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Jun 2023 14:29:26 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Jun 2023 14:29:26 GMT
EXPOSE 8888
# Tue, 13 Jun 2023 14:29:26 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Jun 2023 14:29:26 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Jun 2023 14:29:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 14:29:26 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b7c295cb849275e211d18b720d2349cc84c0038be1a362aca4765ceb3342043c`  
		Last Modified: Tue, 13 Jun 2023 00:04:24 GMT  
		Size: 26.6 MB (26578690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9828e77333b987f92a40b4d360e7caddfe3d4e15ab3704412d441c76c6f2f6e5`  
		Last Modified: Tue, 13 Jun 2023 14:30:36 GMT  
		Size: 4.5 MB (4491786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37257470c47e9dd76af589ded12781e5aa03340766c037862c3cb4029b40b3fc`  
		Last Modified: Tue, 13 Jun 2023 14:30:41 GMT  
		Size: 32.8 MB (32750379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5441fb90e4ccefb2f0a96a245bcb75f250e5c97398db47040ea3f3e7a965f9`  
		Last Modified: Tue, 13 Jun 2023 14:30:36 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cedae55d3bee55cddef3668dafd6fa437c8812d88d6959788c8a6f6ea73862`  
		Last Modified: Tue, 13 Jun 2023 14:30:36 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1b0b8a8ff425b5b19164c61f63598c913ac7c3624feb83ba20fe6d9833a701`  
		Last Modified: Tue, 13 Jun 2023 14:30:36 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:4ef1d9b93663385ab4103851d80433aa05bf7cb4a048f8dd2f341e0507af3305
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67940567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fae85f0e577f4da2e84dafe6f9d77bb1201f5d251565b988af15026df55a9a94`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:49:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 04:49:01 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 13 Jun 2023 04:49:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:49:08 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Jun 2023 04:49:08 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Jun 2023 04:49:08 GMT
EXPOSE 8888
# Tue, 13 Jun 2023 04:49:08 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Jun 2023 04:49:08 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Jun 2023 04:49:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 04:49:08 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35881321b38cbd2cd0adca84b7f3eebd013709fb394b85cae0e1582b75d85b8e`  
		Last Modified: Tue, 13 Jun 2023 04:49:52 GMT  
		Size: 5.2 MB (5209405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa6e83f18b6ccd5cd7df430782949e604471ed05954f79f9c4fe13955d1e2fb`  
		Last Modified: Tue, 13 Jun 2023 04:49:54 GMT  
		Size: 32.6 MB (32643934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3cb2828ebfbb0d3457daaf745c96b9146ad7bcb771d3e82d535664e12162c2`  
		Last Modified: Tue, 13 Jun 2023 04:49:51 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b0407ebbbffd2197b006dbf8220a8efaa01fd9c8bf2161248a2a07a29716dd`  
		Last Modified: Tue, 13 Jun 2023 04:49:51 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d483c1a6745ce72710646e98a5017832a5ee2dd7ea01bfcffea9c90839f1219a`  
		Last Modified: Tue, 13 Jun 2023 04:49:51 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8-alpine`

```console
$ docker pull chronograf@sha256:69e8bc014ccc7b13212883a21876c0c86602fd0880dfbb246ec5e977022287ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:e71099b850f644dcda89e33b77eb5041228a1deaa61179c1c32b2d08207c9bd6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22888506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c14c2b253d74665ff5424b287945be9913bdf9c7e3a2887f8fc7fda48f741cb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:35:00 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 15 Jun 2023 04:35:11 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Thu, 15 Jun 2023 04:35:17 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 15 Jun 2023 04:35:17 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 15 Jun 2023 04:35:17 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 15 Jun 2023 04:35:17 GMT
EXPOSE 8888
# Thu, 15 Jun 2023 04:35:17 GMT
VOLUME [/var/lib/chronograf]
# Thu, 15 Jun 2023 04:35:17 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 15 Jun 2023 04:35:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 04:35:17 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd2f215a0656c3952ad3cfce3a088aa7765b3195f9e051a0a7995b2b4260c48`  
		Last Modified: Thu, 15 Jun 2023 04:35:57 GMT  
		Size: 284.9 KB (284929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5039647d7dd02cb310b5dba71112e2ee3f5a9937a775a318ee674af152f7c3`  
		Last Modified: Thu, 15 Jun 2023 04:36:12 GMT  
		Size: 19.2 MB (19204182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff8ab86cdd06603524b29868cb5c948fbdbe2a2661ad331911719ae767f06a0`  
		Last Modified: Thu, 15 Jun 2023 04:36:08 GMT  
		Size: 12.3 KB (12267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e979ff46c3cf2ce097cb605de70b9907411b76d12cc403c7ab5a1143f5215820`  
		Last Modified: Thu, 15 Jun 2023 04:36:08 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ee4514cdf253fe353946dcae9a81a37f706e09d216ded1cf1c54b9336dc7e7`  
		Last Modified: Thu, 15 Jun 2023 04:36:08 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.10`

```console
$ docker pull chronograf@sha256:c4202a920b4b9e002f562a6e1737b07ad98265ecc3cc25f22fc6a423f109e7a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8.10` - linux; amd64

```console
$ docker pull chronograf@sha256:47fb875ec0e8ce1a13e5b1f4ea597228b51c6c3c27c5c2ccd3440c264491be74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.2 MB (71247223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d71cad4f6770a970ee61513b308a24d28245afd9fc1cef89d9b812ac5e71804`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:18:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 04:18:53 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 04 Jul 2023 04:19:00 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 04:19:00 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 04 Jul 2023 04:19:00 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 04 Jul 2023 04:19:00 GMT
EXPOSE 8888
# Tue, 04 Jul 2023 04:19:00 GMT
VOLUME [/var/lib/chronograf]
# Tue, 04 Jul 2023 04:19:00 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 04 Jul 2023 04:19:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 04:19:00 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2442302dfe8f99302044b2f10fa8cb2af7595d343d96ac7aa33263bd2e73be1b`  
		Last Modified: Tue, 04 Jul 2023 04:20:00 GMT  
		Size: 5.2 MB (5226360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9269842128bc0b52ce9020a379de8f6c7ca488f52e56f82d6beb5e9f014b620d`  
		Last Modified: Tue, 04 Jul 2023 04:20:03 GMT  
		Size: 34.6 MB (34579086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5240e62f6dea38b6e1f99292839cc2ad0e9ae45221a429e88576ef3c651245`  
		Last Modified: Tue, 04 Jul 2023 04:19:58 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18cc5a3b74a0739ee53e7fc7f92e0e7f8d01d93559d6f6ec8b0a25a9da6277c`  
		Last Modified: Tue, 04 Jul 2023 04:19:59 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d35d924643ba624e5664eec24a3ce2c85672d75daae2dc8b30cbcb641258b83`  
		Last Modified: Tue, 04 Jul 2023 04:19:58 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.10` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:3053d3c88cc9407936db2311ffee028aec4189e97c47f28bb2b371d1edc47b29
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63845252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0468f16096fe953f4b4e0fb5150898cf546309691df4d38b93f651f5e294c2f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:47 GMT
ADD file:319a24b7e30fc548f9dcf48ad6cee469e8bf7e89c67901cf3851e41e75693489 in / 
# Mon, 12 Jun 2023 23:58:47 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 14:29:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 14:29:15 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 13 Jun 2023 14:29:25 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 14:29:26 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Jun 2023 14:29:26 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Jun 2023 14:29:26 GMT
EXPOSE 8888
# Tue, 13 Jun 2023 14:29:26 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Jun 2023 14:29:26 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Jun 2023 14:29:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 14:29:26 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b7c295cb849275e211d18b720d2349cc84c0038be1a362aca4765ceb3342043c`  
		Last Modified: Tue, 13 Jun 2023 00:04:24 GMT  
		Size: 26.6 MB (26578690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9828e77333b987f92a40b4d360e7caddfe3d4e15ab3704412d441c76c6f2f6e5`  
		Last Modified: Tue, 13 Jun 2023 14:30:36 GMT  
		Size: 4.5 MB (4491786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37257470c47e9dd76af589ded12781e5aa03340766c037862c3cb4029b40b3fc`  
		Last Modified: Tue, 13 Jun 2023 14:30:41 GMT  
		Size: 32.8 MB (32750379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5441fb90e4ccefb2f0a96a245bcb75f250e5c97398db47040ea3f3e7a965f9`  
		Last Modified: Tue, 13 Jun 2023 14:30:36 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cedae55d3bee55cddef3668dafd6fa437c8812d88d6959788c8a6f6ea73862`  
		Last Modified: Tue, 13 Jun 2023 14:30:36 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1b0b8a8ff425b5b19164c61f63598c913ac7c3624feb83ba20fe6d9833a701`  
		Last Modified: Tue, 13 Jun 2023 14:30:36 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.10` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:4ef1d9b93663385ab4103851d80433aa05bf7cb4a048f8dd2f341e0507af3305
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67940567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fae85f0e577f4da2e84dafe6f9d77bb1201f5d251565b988af15026df55a9a94`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:49:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 04:49:01 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 13 Jun 2023 04:49:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:49:08 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Jun 2023 04:49:08 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Jun 2023 04:49:08 GMT
EXPOSE 8888
# Tue, 13 Jun 2023 04:49:08 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Jun 2023 04:49:08 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Jun 2023 04:49:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 04:49:08 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35881321b38cbd2cd0adca84b7f3eebd013709fb394b85cae0e1582b75d85b8e`  
		Last Modified: Tue, 13 Jun 2023 04:49:52 GMT  
		Size: 5.2 MB (5209405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa6e83f18b6ccd5cd7df430782949e604471ed05954f79f9c4fe13955d1e2fb`  
		Last Modified: Tue, 13 Jun 2023 04:49:54 GMT  
		Size: 32.6 MB (32643934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3cb2828ebfbb0d3457daaf745c96b9146ad7bcb771d3e82d535664e12162c2`  
		Last Modified: Tue, 13 Jun 2023 04:49:51 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b0407ebbbffd2197b006dbf8220a8efaa01fd9c8bf2161248a2a07a29716dd`  
		Last Modified: Tue, 13 Jun 2023 04:49:51 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d483c1a6745ce72710646e98a5017832a5ee2dd7ea01bfcffea9c90839f1219a`  
		Last Modified: Tue, 13 Jun 2023 04:49:51 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.10-alpine`

```console
$ docker pull chronograf@sha256:69e8bc014ccc7b13212883a21876c0c86602fd0880dfbb246ec5e977022287ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.8.10-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:e71099b850f644dcda89e33b77eb5041228a1deaa61179c1c32b2d08207c9bd6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22888506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c14c2b253d74665ff5424b287945be9913bdf9c7e3a2887f8fc7fda48f741cb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:35:00 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 15 Jun 2023 04:35:11 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Thu, 15 Jun 2023 04:35:17 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 15 Jun 2023 04:35:17 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 15 Jun 2023 04:35:17 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 15 Jun 2023 04:35:17 GMT
EXPOSE 8888
# Thu, 15 Jun 2023 04:35:17 GMT
VOLUME [/var/lib/chronograf]
# Thu, 15 Jun 2023 04:35:17 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 15 Jun 2023 04:35:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 04:35:17 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd2f215a0656c3952ad3cfce3a088aa7765b3195f9e051a0a7995b2b4260c48`  
		Last Modified: Thu, 15 Jun 2023 04:35:57 GMT  
		Size: 284.9 KB (284929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5039647d7dd02cb310b5dba71112e2ee3f5a9937a775a318ee674af152f7c3`  
		Last Modified: Thu, 15 Jun 2023 04:36:12 GMT  
		Size: 19.2 MB (19204182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff8ab86cdd06603524b29868cb5c948fbdbe2a2661ad331911719ae767f06a0`  
		Last Modified: Thu, 15 Jun 2023 04:36:08 GMT  
		Size: 12.3 KB (12267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e979ff46c3cf2ce097cb605de70b9907411b76d12cc403c7ab5a1143f5215820`  
		Last Modified: Thu, 15 Jun 2023 04:36:08 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ee4514cdf253fe353946dcae9a81a37f706e09d216ded1cf1c54b9336dc7e7`  
		Last Modified: Thu, 15 Jun 2023 04:36:08 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9`

```console
$ docker pull chronograf@sha256:9a9d644f3f19b1bebf6ef8e69ea8014d5d8c1c2eae9754aee1383550c6168ce7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.9` - linux; amd64

```console
$ docker pull chronograf@sha256:d3aa9903808e40ec23e7946af9271bd97c1495fff4377edb773ac5a58bd4fa38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71894735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:052ffda5d479a5372700c1fb6c786de559a7c28c53c335d6049a4ae87ddb684f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:18:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 04:19:05 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 04 Jul 2023 04:19:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 04:19:12 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 04 Jul 2023 04:19:12 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 04 Jul 2023 04:19:12 GMT
EXPOSE 8888
# Tue, 04 Jul 2023 04:19:12 GMT
VOLUME [/var/lib/chronograf]
# Tue, 04 Jul 2023 04:19:12 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 04 Jul 2023 04:19:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 04:19:13 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2442302dfe8f99302044b2f10fa8cb2af7595d343d96ac7aa33263bd2e73be1b`  
		Last Modified: Tue, 04 Jul 2023 04:20:00 GMT  
		Size: 5.2 MB (5226360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf3cc6deabbb718c6c64047b43b90a641652aac960683f34af898b095380e95`  
		Last Modified: Tue, 04 Jul 2023 04:20:18 GMT  
		Size: 35.2 MB (35226607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3196af2fce16cc2aae910610219e5999c96fd96477e95812a51f622c87f64a2e`  
		Last Modified: Tue, 04 Jul 2023 04:20:13 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4eee56e0ac2ff68e735b9980a7e0d5399e94274fde1768b9edfdabc76979f4`  
		Last Modified: Tue, 04 Jul 2023 04:20:13 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7c590d9c3f2994bad810ed621ad407731601891a307aff8a7193b2d72c3f0a`  
		Last Modified: Tue, 04 Jul 2023 04:20:13 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:dd048d971c6ebd837dbd36e6cdd394f0da7be221fae91d51b3c0f8cc026f2d79
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64621451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4992998c6c63a0a12d12e15a86e46dec7fb63e99c9e37c2acd1769199750b317`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:47 GMT
ADD file:319a24b7e30fc548f9dcf48ad6cee469e8bf7e89c67901cf3851e41e75693489 in / 
# Mon, 12 Jun 2023 23:58:47 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 14:29:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 14:29:31 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 13 Jun 2023 14:29:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 14:29:40 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Jun 2023 14:29:40 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Jun 2023 14:29:41 GMT
EXPOSE 8888
# Tue, 13 Jun 2023 14:29:41 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Jun 2023 14:29:41 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Jun 2023 14:29:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 14:29:41 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b7c295cb849275e211d18b720d2349cc84c0038be1a362aca4765ceb3342043c`  
		Last Modified: Tue, 13 Jun 2023 00:04:24 GMT  
		Size: 26.6 MB (26578690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9828e77333b987f92a40b4d360e7caddfe3d4e15ab3704412d441c76c6f2f6e5`  
		Last Modified: Tue, 13 Jun 2023 14:30:36 GMT  
		Size: 4.5 MB (4491786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fad395e5e47ee176d76e247a95fcee30d8ff732e71957e5a7a5047da8234c0`  
		Last Modified: Tue, 13 Jun 2023 14:30:55 GMT  
		Size: 33.5 MB (33526579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70752b749c4eb72989dd76043467d5cb01eb5c1f7a60655513d553344e6d2e90`  
		Last Modified: Tue, 13 Jun 2023 14:30:49 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554c1f7eb23f3a97e890fcada4e8e0a38cec1ce1cc44e4ece3be7e379c4e1750`  
		Last Modified: Tue, 13 Jun 2023 14:30:49 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3975785b108365f8f68339ff8d9cd0e9deedd9a275c470249635f45e91fec140`  
		Last Modified: Tue, 13 Jun 2023 14:30:49 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:5baedc879b83a683a511141528617d551e2bc09f4816ebf6359141abc171563e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68692224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:442e8eb18270c21a0ce338d08b7a962d9043c53635bc0ba804f8ece1df6fda57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:49:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 04:49:11 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 13 Jun 2023 04:49:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:49:18 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Jun 2023 04:49:18 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Jun 2023 04:49:18 GMT
EXPOSE 8888
# Tue, 13 Jun 2023 04:49:18 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Jun 2023 04:49:18 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Jun 2023 04:49:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 04:49:18 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35881321b38cbd2cd0adca84b7f3eebd013709fb394b85cae0e1582b75d85b8e`  
		Last Modified: Tue, 13 Jun 2023 04:49:52 GMT  
		Size: 5.2 MB (5209405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3797983ce6d77e0c54c75a72a08d6944ee34c561a684c047e31e7f43c2b32b34`  
		Last Modified: Tue, 13 Jun 2023 04:50:05 GMT  
		Size: 33.4 MB (33395592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59c0528f1307fc95a7c14e371a610881ee3eba9dd708f52b1e6c7f45df0d1a3`  
		Last Modified: Tue, 13 Jun 2023 04:50:02 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02a31f28d0d016d8851f5019834dcff87ef53511b7ce21c79dbd2e6e6222ef5`  
		Last Modified: Tue, 13 Jun 2023 04:50:02 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd792139a10e376b26c2c1170f3887a58c38b5475b4a83395d7d3fdce1fd57ca`  
		Last Modified: Tue, 13 Jun 2023 04:50:02 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9-alpine`

```console
$ docker pull chronograf@sha256:adb1ec8ffa83a784f6f8f0766c5189ef428ec67ea964f6d9eea9067dd77d0e12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.9-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:89fceeaa051048e2099e7c38fe8224f18dd2462774f8bf44df6439c8fff43f48
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23356515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11eda8116721d2210f91fdff75be7847611674c8ef6a74a5d9fa0e8bb282db66`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:35:00 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 15 Jun 2023 04:35:22 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Thu, 15 Jun 2023 04:35:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 15 Jun 2023 04:35:27 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 15 Jun 2023 04:35:27 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 15 Jun 2023 04:35:27 GMT
EXPOSE 8888
# Thu, 15 Jun 2023 04:35:27 GMT
VOLUME [/var/lib/chronograf]
# Thu, 15 Jun 2023 04:35:28 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 15 Jun 2023 04:35:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 04:35:28 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd2f215a0656c3952ad3cfce3a088aa7765b3195f9e051a0a7995b2b4260c48`  
		Last Modified: Thu, 15 Jun 2023 04:35:57 GMT  
		Size: 284.9 KB (284929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc089fbd9f70a18f48551ca37ed446f30b06acd413388c7c5b3a619d5c81dd5`  
		Last Modified: Thu, 15 Jun 2023 04:36:24 GMT  
		Size: 19.7 MB (19672199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84aa2385f6a0c11646291b7a2eba18f763125735aff856a106935ce44ab5519e`  
		Last Modified: Thu, 15 Jun 2023 04:36:20 GMT  
		Size: 12.3 KB (12265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3b4e4ca4491b416a322e12a3b27dbd6067965faefd0a9a90ac93a9145f8548`  
		Last Modified: Thu, 15 Jun 2023 04:36:20 GMT  
		Size: 11.9 KB (11894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c2340f1a40772b9c155a1bec1dadb5e661b5d510f65e38e1d6bda5b770a43f`  
		Last Modified: Thu, 15 Jun 2023 04:36:20 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9.4`

```console
$ docker pull chronograf@sha256:9a9d644f3f19b1bebf6ef8e69ea8014d5d8c1c2eae9754aee1383550c6168ce7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.9.4` - linux; amd64

```console
$ docker pull chronograf@sha256:d3aa9903808e40ec23e7946af9271bd97c1495fff4377edb773ac5a58bd4fa38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71894735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:052ffda5d479a5372700c1fb6c786de559a7c28c53c335d6049a4ae87ddb684f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:18:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 04:19:05 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 04 Jul 2023 04:19:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 04:19:12 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 04 Jul 2023 04:19:12 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 04 Jul 2023 04:19:12 GMT
EXPOSE 8888
# Tue, 04 Jul 2023 04:19:12 GMT
VOLUME [/var/lib/chronograf]
# Tue, 04 Jul 2023 04:19:12 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 04 Jul 2023 04:19:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 04:19:13 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2442302dfe8f99302044b2f10fa8cb2af7595d343d96ac7aa33263bd2e73be1b`  
		Last Modified: Tue, 04 Jul 2023 04:20:00 GMT  
		Size: 5.2 MB (5226360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf3cc6deabbb718c6c64047b43b90a641652aac960683f34af898b095380e95`  
		Last Modified: Tue, 04 Jul 2023 04:20:18 GMT  
		Size: 35.2 MB (35226607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3196af2fce16cc2aae910610219e5999c96fd96477e95812a51f622c87f64a2e`  
		Last Modified: Tue, 04 Jul 2023 04:20:13 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4eee56e0ac2ff68e735b9980a7e0d5399e94274fde1768b9edfdabc76979f4`  
		Last Modified: Tue, 04 Jul 2023 04:20:13 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7c590d9c3f2994bad810ed621ad407731601891a307aff8a7193b2d72c3f0a`  
		Last Modified: Tue, 04 Jul 2023 04:20:13 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9.4` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:dd048d971c6ebd837dbd36e6cdd394f0da7be221fae91d51b3c0f8cc026f2d79
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64621451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4992998c6c63a0a12d12e15a86e46dec7fb63e99c9e37c2acd1769199750b317`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:47 GMT
ADD file:319a24b7e30fc548f9dcf48ad6cee469e8bf7e89c67901cf3851e41e75693489 in / 
# Mon, 12 Jun 2023 23:58:47 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 14:29:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 14:29:31 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 13 Jun 2023 14:29:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 14:29:40 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Jun 2023 14:29:40 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Jun 2023 14:29:41 GMT
EXPOSE 8888
# Tue, 13 Jun 2023 14:29:41 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Jun 2023 14:29:41 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Jun 2023 14:29:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 14:29:41 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b7c295cb849275e211d18b720d2349cc84c0038be1a362aca4765ceb3342043c`  
		Last Modified: Tue, 13 Jun 2023 00:04:24 GMT  
		Size: 26.6 MB (26578690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9828e77333b987f92a40b4d360e7caddfe3d4e15ab3704412d441c76c6f2f6e5`  
		Last Modified: Tue, 13 Jun 2023 14:30:36 GMT  
		Size: 4.5 MB (4491786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fad395e5e47ee176d76e247a95fcee30d8ff732e71957e5a7a5047da8234c0`  
		Last Modified: Tue, 13 Jun 2023 14:30:55 GMT  
		Size: 33.5 MB (33526579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70752b749c4eb72989dd76043467d5cb01eb5c1f7a60655513d553344e6d2e90`  
		Last Modified: Tue, 13 Jun 2023 14:30:49 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554c1f7eb23f3a97e890fcada4e8e0a38cec1ce1cc44e4ece3be7e379c4e1750`  
		Last Modified: Tue, 13 Jun 2023 14:30:49 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3975785b108365f8f68339ff8d9cd0e9deedd9a275c470249635f45e91fec140`  
		Last Modified: Tue, 13 Jun 2023 14:30:49 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9.4` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:5baedc879b83a683a511141528617d551e2bc09f4816ebf6359141abc171563e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68692224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:442e8eb18270c21a0ce338d08b7a962d9043c53635bc0ba804f8ece1df6fda57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:49:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 04:49:11 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 13 Jun 2023 04:49:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:49:18 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Jun 2023 04:49:18 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Jun 2023 04:49:18 GMT
EXPOSE 8888
# Tue, 13 Jun 2023 04:49:18 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Jun 2023 04:49:18 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Jun 2023 04:49:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 04:49:18 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35881321b38cbd2cd0adca84b7f3eebd013709fb394b85cae0e1582b75d85b8e`  
		Last Modified: Tue, 13 Jun 2023 04:49:52 GMT  
		Size: 5.2 MB (5209405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3797983ce6d77e0c54c75a72a08d6944ee34c561a684c047e31e7f43c2b32b34`  
		Last Modified: Tue, 13 Jun 2023 04:50:05 GMT  
		Size: 33.4 MB (33395592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59c0528f1307fc95a7c14e371a610881ee3eba9dd708f52b1e6c7f45df0d1a3`  
		Last Modified: Tue, 13 Jun 2023 04:50:02 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02a31f28d0d016d8851f5019834dcff87ef53511b7ce21c79dbd2e6e6222ef5`  
		Last Modified: Tue, 13 Jun 2023 04:50:02 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd792139a10e376b26c2c1170f3887a58c38b5475b4a83395d7d3fdce1fd57ca`  
		Last Modified: Tue, 13 Jun 2023 04:50:02 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9.4-alpine`

```console
$ docker pull chronograf@sha256:adb1ec8ffa83a784f6f8f0766c5189ef428ec67ea964f6d9eea9067dd77d0e12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.9.4-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:89fceeaa051048e2099e7c38fe8224f18dd2462774f8bf44df6439c8fff43f48
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23356515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11eda8116721d2210f91fdff75be7847611674c8ef6a74a5d9fa0e8bb282db66`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:35:00 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 15 Jun 2023 04:35:22 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Thu, 15 Jun 2023 04:35:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 15 Jun 2023 04:35:27 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 15 Jun 2023 04:35:27 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 15 Jun 2023 04:35:27 GMT
EXPOSE 8888
# Thu, 15 Jun 2023 04:35:27 GMT
VOLUME [/var/lib/chronograf]
# Thu, 15 Jun 2023 04:35:28 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 15 Jun 2023 04:35:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 04:35:28 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd2f215a0656c3952ad3cfce3a088aa7765b3195f9e051a0a7995b2b4260c48`  
		Last Modified: Thu, 15 Jun 2023 04:35:57 GMT  
		Size: 284.9 KB (284929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc089fbd9f70a18f48551ca37ed446f30b06acd413388c7c5b3a619d5c81dd5`  
		Last Modified: Thu, 15 Jun 2023 04:36:24 GMT  
		Size: 19.7 MB (19672199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84aa2385f6a0c11646291b7a2eba18f763125735aff856a106935ce44ab5519e`  
		Last Modified: Thu, 15 Jun 2023 04:36:20 GMT  
		Size: 12.3 KB (12265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3b4e4ca4491b416a322e12a3b27dbd6067965faefd0a9a90ac93a9145f8548`  
		Last Modified: Thu, 15 Jun 2023 04:36:20 GMT  
		Size: 11.9 KB (11894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c2340f1a40772b9c155a1bec1dadb5e661b5d510f65e38e1d6bda5b770a43f`  
		Last Modified: Thu, 15 Jun 2023 04:36:20 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:alpine`

```console
$ docker pull chronograf@sha256:9d62c72cebc36f428c0060313c3ef3e3377e0309711addf0170493a0620920a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:612bc34865193e974de365f3e61f464ac77ea1ad3c828c125ce158034cd22205
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31471523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d92372eb76aa713e1f80da30fab50499e9f6a9a5124e579f57eab9642694097`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:35:00 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 15 Jun 2023 04:35:33 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Thu, 15 Jun 2023 04:35:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 15 Jun 2023 04:35:39 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 15 Jun 2023 04:35:39 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 15 Jun 2023 04:35:39 GMT
EXPOSE 8888
# Thu, 15 Jun 2023 04:35:39 GMT
VOLUME [/var/lib/chronograf]
# Thu, 15 Jun 2023 04:35:39 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 15 Jun 2023 04:35:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 04:35:39 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd2f215a0656c3952ad3cfce3a088aa7765b3195f9e051a0a7995b2b4260c48`  
		Last Modified: Thu, 15 Jun 2023 04:35:57 GMT  
		Size: 284.9 KB (284929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de727897c91e79266c88af5c343cde0e3e5167b458a9e128d56da665c573a039`  
		Last Modified: Thu, 15 Jun 2023 04:36:38 GMT  
		Size: 27.8 MB (27787202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4d3f77996a15dce0f8e8ac9c5a89eb2d6db2ff2ef00bd3fb6c2f4efa1ec675`  
		Last Modified: Thu, 15 Jun 2023 04:36:33 GMT  
		Size: 12.3 KB (12266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0347e88c27ad598445a0a65573552937a41150af7f36b834b4d4a85d4bad794b`  
		Last Modified: Thu, 15 Jun 2023 04:36:33 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0656947d8c90443cbc4edb28052852f49a1a523a4b6e8e23bf7d0967ef2dc3bd`  
		Last Modified: Thu, 15 Jun 2023 04:36:33 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:latest`

```console
$ docker pull chronograf@sha256:a55b1724a890b78bbfa5aff4152632c4039e47b27166b957f06da9c44d0490f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:4c8a72a31cf1c6751c665bdb090cf7dcfdf2c4d29cc6a826c0341c1ac4e287e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.8 MB (82809646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e30929b3c76af4d2c56658f9ad656760fa3a66bd6034fdeef441fad99114c79c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:18:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 04:19:17 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Tue, 04 Jul 2023 04:19:24 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 04:19:24 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 04 Jul 2023 04:19:24 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 04 Jul 2023 04:19:24 GMT
EXPOSE 8888
# Tue, 04 Jul 2023 04:19:24 GMT
VOLUME [/var/lib/chronograf]
# Tue, 04 Jul 2023 04:19:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 04 Jul 2023 04:19:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 04:19:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2442302dfe8f99302044b2f10fa8cb2af7595d343d96ac7aa33263bd2e73be1b`  
		Last Modified: Tue, 04 Jul 2023 04:20:00 GMT  
		Size: 5.2 MB (5226360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009868036e3e962809f4734cf4a0d4c68017aaf3d8bc1bdc7a4f2388de7e8388`  
		Last Modified: Tue, 04 Jul 2023 04:20:34 GMT  
		Size: 46.1 MB (46141511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18dcb6401f859ffb576f7f730b11d86414e2091c979468533f9e84c3c70c940c`  
		Last Modified: Tue, 04 Jul 2023 04:20:27 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7c6e4727dfa5750009dc64b69a2a5b1603636489dd98a085839f1c0840fee6`  
		Last Modified: Tue, 04 Jul 2023 04:20:27 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e8a3c9c5d09608504a1d10e1fcdbb69d6a907d419e03a07cb380209ee9042c`  
		Last Modified: Tue, 04 Jul 2023 04:20:27 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:263afb762b7a64411805f8857c33ded7f85e4f7413b1325cbfba47ddb44021cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74945189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d20eb2acb74bc852b09805e44be7ad3878f729f19494eb31d4e6eded5b45c19c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:47 GMT
ADD file:319a24b7e30fc548f9dcf48ad6cee469e8bf7e89c67901cf3851e41e75693489 in / 
# Mon, 12 Jun 2023 23:58:47 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 14:29:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 14:29:44 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Tue, 13 Jun 2023 14:30:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 14:30:08 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Jun 2023 14:30:08 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Jun 2023 14:30:09 GMT
EXPOSE 8888
# Tue, 13 Jun 2023 14:30:09 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Jun 2023 14:30:09 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Jun 2023 14:30:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 14:30:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b7c295cb849275e211d18b720d2349cc84c0038be1a362aca4765ceb3342043c`  
		Last Modified: Tue, 13 Jun 2023 00:04:24 GMT  
		Size: 26.6 MB (26578690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9828e77333b987f92a40b4d360e7caddfe3d4e15ab3704412d441c76c6f2f6e5`  
		Last Modified: Tue, 13 Jun 2023 14:30:36 GMT  
		Size: 4.5 MB (4491786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b32968d44f52b6cd3d1a65cb11cb4004bcc25c8b863203712f1bb8e5055f6c4`  
		Last Modified: Tue, 13 Jun 2023 14:31:10 GMT  
		Size: 43.9 MB (43850332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6de1a7010815c4e6669c17f8c9fc45d44542c9176c207b5a114d9d30a57344`  
		Last Modified: Tue, 13 Jun 2023 14:31:03 GMT  
		Size: 12.2 KB (12242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86be71e5593ed6f80300bbf7584cb55c79c3fdba2651086f4c664a7acfcee3b`  
		Last Modified: Tue, 13 Jun 2023 14:31:03 GMT  
		Size: 11.9 KB (11900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b4a29eb988930d4c676ee015ec2ba2e59882bf57198d75fadb4cbe47d9649b`  
		Last Modified: Tue, 13 Jun 2023 14:31:03 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:148be15bcf895d8b0c8c34ba9b5720811a41ca1f59c1d857c97d6155c6fd3193
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79151450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4129cf123b5472fd6f3874fc6b1174ff1677956fab058a43dbffb7c963569c33`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:49:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 04:49:20 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Tue, 13 Jun 2023 04:49:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:49:28 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 13 Jun 2023 04:49:28 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 13 Jun 2023 04:49:28 GMT
EXPOSE 8888
# Tue, 13 Jun 2023 04:49:28 GMT
VOLUME [/var/lib/chronograf]
# Tue, 13 Jun 2023 04:49:29 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 13 Jun 2023 04:49:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 04:49:29 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35881321b38cbd2cd0adca84b7f3eebd013709fb394b85cae0e1582b75d85b8e`  
		Last Modified: Tue, 13 Jun 2023 04:49:52 GMT  
		Size: 5.2 MB (5209405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8289f2a411b0fce95afd518dddcfa36f6c20a39d1edaaf2e7a33eedcf48d0cbf`  
		Last Modified: Tue, 13 Jun 2023 04:50:18 GMT  
		Size: 43.9 MB (43854831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2885bdd478f1729f1eef9e06f9b1327cef8e7d4f9abe94aa4da65fbfb597af7`  
		Last Modified: Tue, 13 Jun 2023 04:50:13 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a703d39b907ff7e8a7d24961e05de092327594eae96b440bd8a3221e0493ec3c`  
		Last Modified: Tue, 13 Jun 2023 04:50:13 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c8d401aa0a406ade4e84cfe8f4b1215200aabd2cbac7d67c883bf1d0767f14`  
		Last Modified: Tue, 13 Jun 2023 04:50:13 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
