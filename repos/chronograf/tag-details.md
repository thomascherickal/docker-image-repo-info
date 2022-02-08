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
-	[`chronograf:1.9.3`](#chronograf193)
-	[`chronograf:1.9.3-alpine`](#chronograf193-alpine)
-	[`chronograf:alpine`](#chronografalpine)
-	[`chronograf:latest`](#chronograflatest)

## `chronograf:1.6`

```console
$ docker pull chronograf@sha256:6262e1e3f9e6cbd8807885241656136e77c77e1e11c693ecef6cba7ba2ce9ac5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6` - linux; amd64

```console
$ docker pull chronograf@sha256:8455e0cad58dffe33bb0c467bc3ffc5b070c907ad370fab021edb097042783e2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49358953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16460f65d0261816364d5444d9a5161b0ddb21144d0abaf25cb99964030b63fe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:57 GMT
ADD file:bed2454356c48f77207726865f8aee34a5b3db6927a881655573cbde13ce5a89 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:28:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 02:28:49 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 26 Jan 2022 02:28:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 02:28:58 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Jan 2022 02:28:58 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Jan 2022 02:28:58 GMT
EXPOSE 8888
# Wed, 26 Jan 2022 02:28:59 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Jan 2022 02:28:59 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Jan 2022 02:28:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 02:28:59 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:1cb79db8a9e79b4f5415eaa91602251fb1eafe68d236efb80fe931bacfe5b3d6`  
		Last Modified: Wed, 26 Jan 2022 01:51:06 GMT  
		Size: 22.5 MB (22529131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1faa9122d932af0ee2f4243589d2aeb6e06442f2e8b566f7028df3b67b2a2485`  
		Last Modified: Wed, 26 Jan 2022 02:31:23 GMT  
		Size: 6.8 MB (6760139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1375c4432f9b94ceaedb7ffac62d30a9f3a57d7dbd79e23b513e5ffa18e0ec`  
		Last Modified: Wed, 26 Jan 2022 02:31:25 GMT  
		Size: 20.0 MB (20045297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8945c080b35d84fcffb6c6d31eac5550c4297459f43a98911a42e681ebf9138b`  
		Last Modified: Wed, 26 Jan 2022 02:31:21 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0b49ae162609580f470de06f96ee239aa914d6e9d39fb207796e63ab36e534`  
		Last Modified: Wed, 26 Jan 2022 02:31:21 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e638cdd93008057c0d18bee6a009ce9fac4fb24da0c8540fcaa7f3690cf5f2`  
		Last Modified: Wed, 26 Jan 2022 02:31:21 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:e3530c4ca883788c8cd711117d8c4fcccb7d48fc07e266828d0785adfe9954b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43944295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:810e2e2da3c35ab4b49f7b42540d5959ef8f90be6fe0898e079c8db1c87abaff`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:48:08 GMT
ADD file:26e6c9015d58ffb5e67d6ea64451fd0e27a9a60c65340659b35b075d51ed5c45 in / 
# Wed, 26 Jan 2022 01:48:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 17:17:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 17:17:45 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 26 Jan 2022 17:18:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 17:18:04 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Jan 2022 17:18:04 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Jan 2022 17:18:05 GMT
EXPOSE 8888
# Wed, 26 Jan 2022 17:18:05 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Jan 2022 17:18:06 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Jan 2022 17:18:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 17:18:07 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b651abcd2676c0bd22abf9acddc50231c15d43b1004fd0446bb57150c0d4c96b`  
		Last Modified: Wed, 26 Jan 2022 02:05:54 GMT  
		Size: 19.3 MB (19318809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0c89d838bd5ed63affedd67004af12d134c4995c36285fc64f348e14039db5`  
		Last Modified: Wed, 26 Jan 2022 17:21:43 GMT  
		Size: 5.8 MB (5780469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06640ae92ed9581c5fafe215a4c1f0795b23bd16bdab997d73a5d3f3a8bca10e`  
		Last Modified: Wed, 26 Jan 2022 17:21:52 GMT  
		Size: 18.8 MB (18820622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5cd724aa261119c311394a222f615a3e4ee5aeb0f4f7edaf8702647f5fda95`  
		Last Modified: Wed, 26 Jan 2022 17:21:40 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff74e0bd064f19677b673ed3df84922efc519a45b4da9e139c3ba7d9da1e4215`  
		Last Modified: Wed, 26 Jan 2022 17:21:40 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215581fdc3366895ac986c8ee3e8c2917d82073d9a84c4fba40492f54873a789`  
		Last Modified: Wed, 26 Jan 2022 17:21:40 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:42a831f935d5b0d960e5ee16b47fb17dc885f39f6becfca426f50e02316ce036
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45421884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b39223714cf1bb1a855d5584cc66c55f79d10e9a91258f8c2ee27a1a30c2a475`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:48 GMT
ADD file:952345b92a37bdbcaea817a1a9e1466c68e040b5dee856ff2606afbd1297b1f0 in / 
# Wed, 26 Jan 2022 01:44:48 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:30:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 02:30:06 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 26 Jan 2022 02:30:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 02:30:18 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Jan 2022 02:30:19 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Jan 2022 02:30:19 GMT
EXPOSE 8888
# Wed, 26 Jan 2022 02:30:20 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Jan 2022 02:30:22 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Jan 2022 02:30:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 02:30:23 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0baeb81232d08980c2f78646547d7792710a684e89313d2da7499bdff69437d0`  
		Last Modified: Wed, 26 Jan 2022 01:53:21 GMT  
		Size: 20.4 MB (20389407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fa5ffb58fb1affd19c9a960e3ea691bf31aebc8d3eb9cd3d49009cde7b183c`  
		Last Modified: Wed, 26 Jan 2022 02:32:42 GMT  
		Size: 6.0 MB (6046875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b63f621856024d496e04f317df06cce7edccf34b851b5577511ed0c2f7938a2`  
		Last Modified: Wed, 26 Jan 2022 02:32:44 GMT  
		Size: 19.0 MB (18961209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879e53f2cd9445d2e484fca977c91c2727b3ddb0b0cdc86f838eaf734a9faf91`  
		Last Modified: Wed, 26 Jan 2022 02:32:41 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cbb5d5d7df9b96c20353152dee8a130a3c261b1eba2b707573a2d0113fdf35`  
		Last Modified: Wed, 26 Jan 2022 02:32:41 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affd316f145059ff81b2ad7c47de4c4dbd10cc5b3d0f93c0b9edb017828df112`  
		Last Modified: Wed, 26 Jan 2022 02:32:41 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6-alpine`

```console
$ docker pull chronograf@sha256:d83014d2850383073830fe3cc8b1dd10280ccadb3dc727fc46c18f0133876e24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.6-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:42be608ccf5cf8a282705866e53559a2f683cee86f301d5335d2b0a8a722d1a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14867541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72592bc7b5181925382f61d3755716a15c0a3222db4caad2f764f58f7c77f70b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:55:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 12 Nov 2021 21:55:18 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 12 Nov 2021 21:55:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 12 Nov 2021 21:55:32 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Fri, 12 Nov 2021 21:55:32 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Nov 2021 21:55:32 GMT
EXPOSE 8888
# Fri, 12 Nov 2021 21:55:32 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Nov 2021 21:55:33 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 12 Nov 2021 21:55:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 21:55:33 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aac166cdd02de2f1baf9250ebe4e1a5bec54cc49a59dbb3716570ed37d5bf63`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 282.0 KB (281961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168157deaab4ba90e7cb5d2b6d5e649804bbf43d504044d8e9f3b7d8572f1935`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 11.7 MB (11738046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7b8146058f9a9b104394531bbfffada3698450341aa41fa890a7a4aae65320`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 12.3 KB (12267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36021c872f9879231ff8873fe042d102c69ef4a5a63c1b5a3fdf00ac44b9467`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 11.9 KB (11895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b09ac85e2c2a25870fabd125b2933114782d6d8dc3b752bc9c5ebfd77bb0764`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2`

```console
$ docker pull chronograf@sha256:6262e1e3f9e6cbd8807885241656136e77c77e1e11c693ecef6cba7ba2ce9ac5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6.2` - linux; amd64

```console
$ docker pull chronograf@sha256:8455e0cad58dffe33bb0c467bc3ffc5b070c907ad370fab021edb097042783e2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49358953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16460f65d0261816364d5444d9a5161b0ddb21144d0abaf25cb99964030b63fe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:57 GMT
ADD file:bed2454356c48f77207726865f8aee34a5b3db6927a881655573cbde13ce5a89 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:28:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 02:28:49 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 26 Jan 2022 02:28:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 02:28:58 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Jan 2022 02:28:58 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Jan 2022 02:28:58 GMT
EXPOSE 8888
# Wed, 26 Jan 2022 02:28:59 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Jan 2022 02:28:59 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Jan 2022 02:28:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 02:28:59 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:1cb79db8a9e79b4f5415eaa91602251fb1eafe68d236efb80fe931bacfe5b3d6`  
		Last Modified: Wed, 26 Jan 2022 01:51:06 GMT  
		Size: 22.5 MB (22529131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1faa9122d932af0ee2f4243589d2aeb6e06442f2e8b566f7028df3b67b2a2485`  
		Last Modified: Wed, 26 Jan 2022 02:31:23 GMT  
		Size: 6.8 MB (6760139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1375c4432f9b94ceaedb7ffac62d30a9f3a57d7dbd79e23b513e5ffa18e0ec`  
		Last Modified: Wed, 26 Jan 2022 02:31:25 GMT  
		Size: 20.0 MB (20045297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8945c080b35d84fcffb6c6d31eac5550c4297459f43a98911a42e681ebf9138b`  
		Last Modified: Wed, 26 Jan 2022 02:31:21 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0b49ae162609580f470de06f96ee239aa914d6e9d39fb207796e63ab36e534`  
		Last Modified: Wed, 26 Jan 2022 02:31:21 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e638cdd93008057c0d18bee6a009ce9fac4fb24da0c8540fcaa7f3690cf5f2`  
		Last Modified: Wed, 26 Jan 2022 02:31:21 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:e3530c4ca883788c8cd711117d8c4fcccb7d48fc07e266828d0785adfe9954b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43944295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:810e2e2da3c35ab4b49f7b42540d5959ef8f90be6fe0898e079c8db1c87abaff`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:48:08 GMT
ADD file:26e6c9015d58ffb5e67d6ea64451fd0e27a9a60c65340659b35b075d51ed5c45 in / 
# Wed, 26 Jan 2022 01:48:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 17:17:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 17:17:45 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 26 Jan 2022 17:18:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 17:18:04 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Jan 2022 17:18:04 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Jan 2022 17:18:05 GMT
EXPOSE 8888
# Wed, 26 Jan 2022 17:18:05 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Jan 2022 17:18:06 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Jan 2022 17:18:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 17:18:07 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b651abcd2676c0bd22abf9acddc50231c15d43b1004fd0446bb57150c0d4c96b`  
		Last Modified: Wed, 26 Jan 2022 02:05:54 GMT  
		Size: 19.3 MB (19318809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0c89d838bd5ed63affedd67004af12d134c4995c36285fc64f348e14039db5`  
		Last Modified: Wed, 26 Jan 2022 17:21:43 GMT  
		Size: 5.8 MB (5780469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06640ae92ed9581c5fafe215a4c1f0795b23bd16bdab997d73a5d3f3a8bca10e`  
		Last Modified: Wed, 26 Jan 2022 17:21:52 GMT  
		Size: 18.8 MB (18820622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5cd724aa261119c311394a222f615a3e4ee5aeb0f4f7edaf8702647f5fda95`  
		Last Modified: Wed, 26 Jan 2022 17:21:40 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff74e0bd064f19677b673ed3df84922efc519a45b4da9e139c3ba7d9da1e4215`  
		Last Modified: Wed, 26 Jan 2022 17:21:40 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215581fdc3366895ac986c8ee3e8c2917d82073d9a84c4fba40492f54873a789`  
		Last Modified: Wed, 26 Jan 2022 17:21:40 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:42a831f935d5b0d960e5ee16b47fb17dc885f39f6becfca426f50e02316ce036
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45421884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b39223714cf1bb1a855d5584cc66c55f79d10e9a91258f8c2ee27a1a30c2a475`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:48 GMT
ADD file:952345b92a37bdbcaea817a1a9e1466c68e040b5dee856ff2606afbd1297b1f0 in / 
# Wed, 26 Jan 2022 01:44:48 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:30:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 02:30:06 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 26 Jan 2022 02:30:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 02:30:18 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Jan 2022 02:30:19 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Jan 2022 02:30:19 GMT
EXPOSE 8888
# Wed, 26 Jan 2022 02:30:20 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Jan 2022 02:30:22 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Jan 2022 02:30:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 02:30:23 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0baeb81232d08980c2f78646547d7792710a684e89313d2da7499bdff69437d0`  
		Last Modified: Wed, 26 Jan 2022 01:53:21 GMT  
		Size: 20.4 MB (20389407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fa5ffb58fb1affd19c9a960e3ea691bf31aebc8d3eb9cd3d49009cde7b183c`  
		Last Modified: Wed, 26 Jan 2022 02:32:42 GMT  
		Size: 6.0 MB (6046875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b63f621856024d496e04f317df06cce7edccf34b851b5577511ed0c2f7938a2`  
		Last Modified: Wed, 26 Jan 2022 02:32:44 GMT  
		Size: 19.0 MB (18961209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879e53f2cd9445d2e484fca977c91c2727b3ddb0b0cdc86f838eaf734a9faf91`  
		Last Modified: Wed, 26 Jan 2022 02:32:41 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cbb5d5d7df9b96c20353152dee8a130a3c261b1eba2b707573a2d0113fdf35`  
		Last Modified: Wed, 26 Jan 2022 02:32:41 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affd316f145059ff81b2ad7c47de4c4dbd10cc5b3d0f93c0b9edb017828df112`  
		Last Modified: Wed, 26 Jan 2022 02:32:41 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2-alpine`

```console
$ docker pull chronograf@sha256:d83014d2850383073830fe3cc8b1dd10280ccadb3dc727fc46c18f0133876e24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.6.2-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:42be608ccf5cf8a282705866e53559a2f683cee86f301d5335d2b0a8a722d1a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14867541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72592bc7b5181925382f61d3755716a15c0a3222db4caad2f764f58f7c77f70b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:55:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 12 Nov 2021 21:55:18 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 12 Nov 2021 21:55:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 12 Nov 2021 21:55:32 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Fri, 12 Nov 2021 21:55:32 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Nov 2021 21:55:32 GMT
EXPOSE 8888
# Fri, 12 Nov 2021 21:55:32 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Nov 2021 21:55:33 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 12 Nov 2021 21:55:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 21:55:33 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aac166cdd02de2f1baf9250ebe4e1a5bec54cc49a59dbb3716570ed37d5bf63`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 282.0 KB (281961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168157deaab4ba90e7cb5d2b6d5e649804bbf43d504044d8e9f3b7d8572f1935`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 11.7 MB (11738046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7b8146058f9a9b104394531bbfffada3698450341aa41fa890a7a4aae65320`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 12.3 KB (12267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36021c872f9879231ff8873fe042d102c69ef4a5a63c1b5a3fdf00ac44b9467`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 11.9 KB (11895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b09ac85e2c2a25870fabd125b2933114782d6d8dc3b752bc9c5ebfd77bb0764`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7`

```console
$ docker pull chronograf@sha256:7b2e5d938437cc0c1d7bdad1453dfe76320da2a7d60bc5cc2136148b503ba2e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7` - linux; amd64

```console
$ docker pull chronograf@sha256:10d1aa1bd3f086f31ee1ccf1d8660c6b33c9e69e19ce89d3e7db8b590976904e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65388158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9b0dc745ae54b510c7a1ca992a13e91ea9034dac87f681bb4fa4857569b1870`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:57 GMT
ADD file:bed2454356c48f77207726865f8aee34a5b3db6927a881655573cbde13ce5a89 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:29:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 02:29:59 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 26 Jan 2022 02:30:10 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 02:30:11 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Jan 2022 02:30:11 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Jan 2022 02:30:11 GMT
EXPOSE 8888
# Wed, 26 Jan 2022 02:30:11 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Jan 2022 02:30:12 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Jan 2022 02:30:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 02:30:12 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:1cb79db8a9e79b4f5415eaa91602251fb1eafe68d236efb80fe931bacfe5b3d6`  
		Last Modified: Wed, 26 Jan 2022 01:51:06 GMT  
		Size: 22.5 MB (22529131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369aa9ea2c72778c88e46c7e87af810dd7cdfe69c7e80c6b0d6b567d8a282815`  
		Last Modified: Wed, 26 Jan 2022 02:31:36 GMT  
		Size: 4.5 MB (4506587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd67c940010b51ea64ed329182e500dd2606f33f90c205e1aa547d890bc460d2`  
		Last Modified: Wed, 26 Jan 2022 02:31:41 GMT  
		Size: 38.3 MB (38328045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37113ea0708429f142a52d117c9a57f9858246f285d5836198166653a4942114`  
		Last Modified: Wed, 26 Jan 2022 02:31:35 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ec17839d8bb7db45bb0b6dc2580f28d4e4e50831eedf33066244ce21ee4039`  
		Last Modified: Wed, 26 Jan 2022 02:31:35 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cae4ad8a81ab61fd52fd2541eab056b3de654b31b579573ac719ead3ef5af5`  
		Last Modified: Wed, 26 Jan 2022 02:31:36 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:b4fd75b3364921e2d59d03eac23dcbd83b1333eddc6eea7fa7919efc1576fc30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (59006683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4523b7b3db95e6272ffd2bea8a084dda27bdeb9acb71c6318c29d1926bd24dc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:48:08 GMT
ADD file:26e6c9015d58ffb5e67d6ea64451fd0e27a9a60c65340659b35b075d51ed5c45 in / 
# Wed, 26 Jan 2022 01:48:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 17:18:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 17:18:55 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 26 Jan 2022 17:19:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 17:19:28 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Jan 2022 17:19:28 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Jan 2022 17:19:29 GMT
EXPOSE 8888
# Wed, 26 Jan 2022 17:19:29 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Jan 2022 17:19:30 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Jan 2022 17:19:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 17:19:31 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b651abcd2676c0bd22abf9acddc50231c15d43b1004fd0446bb57150c0d4c96b`  
		Last Modified: Wed, 26 Jan 2022 02:05:54 GMT  
		Size: 19.3 MB (19318809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296d9e048715e8505e32f6f6cbc3c100575b13f24ceb071fac2fd47d0fb6c1d8`  
		Last Modified: Wed, 26 Jan 2022 17:22:06 GMT  
		Size: 3.9 MB (3879910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02cd09be7712a357f3154373128d43badada230690aa4c0b5c2a328a472e2c3`  
		Last Modified: Wed, 26 Jan 2022 17:22:24 GMT  
		Size: 35.8 MB (35783577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cec652371cbae39fdb9e21516b204c2ff681734c99816608b84d469261c1dc`  
		Last Modified: Wed, 26 Jan 2022 17:22:04 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383ca24751904eb4c9df9db8f43150370ca39a21ac9225530625b2a1385bd45a`  
		Last Modified: Wed, 26 Jan 2022 17:22:04 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d8b602580fb655f164dd2e8a34a2b922092bd9fb1d229d6db781fc72aa246`  
		Last Modified: Wed, 26 Jan 2022 17:22:04 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:5715a42ec23d5718c6ec19ec8a3e599951331a907d654f4f244f02608756e772
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60294307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a970e286711d21b1821004043f74d40a962dc8d5478307f6fe06332d078ef5d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:48 GMT
ADD file:952345b92a37bdbcaea817a1a9e1466c68e040b5dee856ff2606afbd1297b1f0 in / 
# Wed, 26 Jan 2022 01:44:48 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:31:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 02:31:12 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 26 Jan 2022 02:31:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 02:31:25 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Jan 2022 02:31:26 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Jan 2022 02:31:26 GMT
EXPOSE 8888
# Wed, 26 Jan 2022 02:31:27 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Jan 2022 02:31:29 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Jan 2022 02:31:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 02:31:30 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0baeb81232d08980c2f78646547d7792710a684e89313d2da7499bdff69437d0`  
		Last Modified: Wed, 26 Jan 2022 01:53:21 GMT  
		Size: 20.4 MB (20389407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb1d5caa5ba835154f2ad8d8272debfa0b90afdbcff8b58413579017b6a0012`  
		Last Modified: Wed, 26 Jan 2022 02:32:58 GMT  
		Size: 3.9 MB (3893779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f016c7e81db5623626f86c52a7f24dad50b3fbf5ca500dc5922d6ab607a13658`  
		Last Modified: Wed, 26 Jan 2022 02:33:01 GMT  
		Size: 36.0 MB (35986732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17500bb6d4d4466754d296a1573d71db3a9e4778441c804a667dd7fa99782ffc`  
		Last Modified: Wed, 26 Jan 2022 02:32:56 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6428665ed53a31a56f551a5d629af068368a86597d9a2907a0916bfbd2477d08`  
		Last Modified: Wed, 26 Jan 2022 02:32:56 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce8fc0fd36edcc998a3da34f91ffe1d5ff827c9ee0b4848b670990446284c15`  
		Last Modified: Wed, 26 Jan 2022 02:32:56 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7-alpine`

```console
$ docker pull chronograf@sha256:997ecebb69bae99483291c00663c3d1d2ec0628a1c0abb4aae057cc7b004570c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.7-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:77cf883ffa62d74117fd7c6e4a998199f6fbb063e654a42b8046a6cfe3ce69b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22686062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c027745c7d556a42156b262cea5fa7ff78b10d534ae6c2a4decd69caaeedaa26`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:55:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 12 Nov 2021 21:55:38 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 12 Nov 2021 21:55:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 12 Nov 2021 21:55:45 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Nov 2021 21:55:45 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Nov 2021 21:55:45 GMT
EXPOSE 8888
# Fri, 12 Nov 2021 21:55:46 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Nov 2021 21:55:46 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 12 Nov 2021 21:55:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 21:55:46 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aac166cdd02de2f1baf9250ebe4e1a5bec54cc49a59dbb3716570ed37d5bf63`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 282.0 KB (281961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8283a3b7cad208670302a759a3e65783b946b1fb9221a8ab882fef07277d38d3`  
		Last Modified: Fri, 12 Nov 2021 21:56:59 GMT  
		Size: 19.6 MB (19556570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b447bd4534f47d32c04a9937b72b986d155e25c02cb3add58d4a1c700940c3`  
		Last Modified: Fri, 12 Nov 2021 21:56:55 GMT  
		Size: 12.3 KB (12263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deac552aa1d37ccee70bddc7022a3ce80dad98b87b9fd130543f7fa787be0caa`  
		Last Modified: Fri, 12 Nov 2021 21:56:55 GMT  
		Size: 11.9 KB (11895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1656207cac83a586c1a7cf9aec72e8f8cc2ee68c672d3cf8403ff18631c28cf2`  
		Last Modified: Fri, 12 Nov 2021 21:56:55 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17`

```console
$ docker pull chronograf@sha256:7b2e5d938437cc0c1d7bdad1453dfe76320da2a7d60bc5cc2136148b503ba2e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7.17` - linux; amd64

```console
$ docker pull chronograf@sha256:10d1aa1bd3f086f31ee1ccf1d8660c6b33c9e69e19ce89d3e7db8b590976904e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65388158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9b0dc745ae54b510c7a1ca992a13e91ea9034dac87f681bb4fa4857569b1870`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:57 GMT
ADD file:bed2454356c48f77207726865f8aee34a5b3db6927a881655573cbde13ce5a89 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:29:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 02:29:59 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 26 Jan 2022 02:30:10 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 02:30:11 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Jan 2022 02:30:11 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Jan 2022 02:30:11 GMT
EXPOSE 8888
# Wed, 26 Jan 2022 02:30:11 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Jan 2022 02:30:12 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Jan 2022 02:30:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 02:30:12 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:1cb79db8a9e79b4f5415eaa91602251fb1eafe68d236efb80fe931bacfe5b3d6`  
		Last Modified: Wed, 26 Jan 2022 01:51:06 GMT  
		Size: 22.5 MB (22529131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369aa9ea2c72778c88e46c7e87af810dd7cdfe69c7e80c6b0d6b567d8a282815`  
		Last Modified: Wed, 26 Jan 2022 02:31:36 GMT  
		Size: 4.5 MB (4506587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd67c940010b51ea64ed329182e500dd2606f33f90c205e1aa547d890bc460d2`  
		Last Modified: Wed, 26 Jan 2022 02:31:41 GMT  
		Size: 38.3 MB (38328045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37113ea0708429f142a52d117c9a57f9858246f285d5836198166653a4942114`  
		Last Modified: Wed, 26 Jan 2022 02:31:35 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ec17839d8bb7db45bb0b6dc2580f28d4e4e50831eedf33066244ce21ee4039`  
		Last Modified: Wed, 26 Jan 2022 02:31:35 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cae4ad8a81ab61fd52fd2541eab056b3de654b31b579573ac719ead3ef5af5`  
		Last Modified: Wed, 26 Jan 2022 02:31:36 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:b4fd75b3364921e2d59d03eac23dcbd83b1333eddc6eea7fa7919efc1576fc30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (59006683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4523b7b3db95e6272ffd2bea8a084dda27bdeb9acb71c6318c29d1926bd24dc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:48:08 GMT
ADD file:26e6c9015d58ffb5e67d6ea64451fd0e27a9a60c65340659b35b075d51ed5c45 in / 
# Wed, 26 Jan 2022 01:48:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 17:18:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 17:18:55 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 26 Jan 2022 17:19:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 17:19:28 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Jan 2022 17:19:28 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Jan 2022 17:19:29 GMT
EXPOSE 8888
# Wed, 26 Jan 2022 17:19:29 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Jan 2022 17:19:30 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Jan 2022 17:19:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 17:19:31 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b651abcd2676c0bd22abf9acddc50231c15d43b1004fd0446bb57150c0d4c96b`  
		Last Modified: Wed, 26 Jan 2022 02:05:54 GMT  
		Size: 19.3 MB (19318809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296d9e048715e8505e32f6f6cbc3c100575b13f24ceb071fac2fd47d0fb6c1d8`  
		Last Modified: Wed, 26 Jan 2022 17:22:06 GMT  
		Size: 3.9 MB (3879910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02cd09be7712a357f3154373128d43badada230690aa4c0b5c2a328a472e2c3`  
		Last Modified: Wed, 26 Jan 2022 17:22:24 GMT  
		Size: 35.8 MB (35783577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cec652371cbae39fdb9e21516b204c2ff681734c99816608b84d469261c1dc`  
		Last Modified: Wed, 26 Jan 2022 17:22:04 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383ca24751904eb4c9df9db8f43150370ca39a21ac9225530625b2a1385bd45a`  
		Last Modified: Wed, 26 Jan 2022 17:22:04 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d8b602580fb655f164dd2e8a34a2b922092bd9fb1d229d6db781fc72aa246`  
		Last Modified: Wed, 26 Jan 2022 17:22:04 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:5715a42ec23d5718c6ec19ec8a3e599951331a907d654f4f244f02608756e772
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60294307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a970e286711d21b1821004043f74d40a962dc8d5478307f6fe06332d078ef5d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:48 GMT
ADD file:952345b92a37bdbcaea817a1a9e1466c68e040b5dee856ff2606afbd1297b1f0 in / 
# Wed, 26 Jan 2022 01:44:48 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:31:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 02:31:12 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 26 Jan 2022 02:31:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 02:31:25 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Jan 2022 02:31:26 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Jan 2022 02:31:26 GMT
EXPOSE 8888
# Wed, 26 Jan 2022 02:31:27 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Jan 2022 02:31:29 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Jan 2022 02:31:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 02:31:30 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0baeb81232d08980c2f78646547d7792710a684e89313d2da7499bdff69437d0`  
		Last Modified: Wed, 26 Jan 2022 01:53:21 GMT  
		Size: 20.4 MB (20389407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb1d5caa5ba835154f2ad8d8272debfa0b90afdbcff8b58413579017b6a0012`  
		Last Modified: Wed, 26 Jan 2022 02:32:58 GMT  
		Size: 3.9 MB (3893779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f016c7e81db5623626f86c52a7f24dad50b3fbf5ca500dc5922d6ab607a13658`  
		Last Modified: Wed, 26 Jan 2022 02:33:01 GMT  
		Size: 36.0 MB (35986732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17500bb6d4d4466754d296a1573d71db3a9e4778441c804a667dd7fa99782ffc`  
		Last Modified: Wed, 26 Jan 2022 02:32:56 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6428665ed53a31a56f551a5d629af068368a86597d9a2907a0916bfbd2477d08`  
		Last Modified: Wed, 26 Jan 2022 02:32:56 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce8fc0fd36edcc998a3da34f91ffe1d5ff827c9ee0b4848b670990446284c15`  
		Last Modified: Wed, 26 Jan 2022 02:32:56 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17-alpine`

```console
$ docker pull chronograf@sha256:997ecebb69bae99483291c00663c3d1d2ec0628a1c0abb4aae057cc7b004570c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.7.17-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:77cf883ffa62d74117fd7c6e4a998199f6fbb063e654a42b8046a6cfe3ce69b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22686062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c027745c7d556a42156b262cea5fa7ff78b10d534ae6c2a4decd69caaeedaa26`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:55:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 12 Nov 2021 21:55:38 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 12 Nov 2021 21:55:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 12 Nov 2021 21:55:45 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Nov 2021 21:55:45 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Nov 2021 21:55:45 GMT
EXPOSE 8888
# Fri, 12 Nov 2021 21:55:46 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Nov 2021 21:55:46 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 12 Nov 2021 21:55:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 21:55:46 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aac166cdd02de2f1baf9250ebe4e1a5bec54cc49a59dbb3716570ed37d5bf63`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 282.0 KB (281961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8283a3b7cad208670302a759a3e65783b946b1fb9221a8ab882fef07277d38d3`  
		Last Modified: Fri, 12 Nov 2021 21:56:59 GMT  
		Size: 19.6 MB (19556570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b447bd4534f47d32c04a9937b72b986d155e25c02cb3add58d4a1c700940c3`  
		Last Modified: Fri, 12 Nov 2021 21:56:55 GMT  
		Size: 12.3 KB (12263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deac552aa1d37ccee70bddc7022a3ce80dad98b87b9fd130543f7fa787be0caa`  
		Last Modified: Fri, 12 Nov 2021 21:56:55 GMT  
		Size: 11.9 KB (11895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1656207cac83a586c1a7cf9aec72e8f8cc2ee68c672d3cf8403ff18631c28cf2`  
		Last Modified: Fri, 12 Nov 2021 21:56:55 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8`

```console
$ docker pull chronograf@sha256:29082d75ef60be51485a84e88443626d62b5355d169a385adc4789c5055c890d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8` - linux; amd64

```console
$ docker pull chronograf@sha256:c6a5f44940a94d109f104c18a9b3877254ec898dd44735ec0e7fe83d64863836
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66239950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93c24f2aa6e6bc4d00b11a560e8b8ac02db3109231645c73d56b934bdb251ba0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:57 GMT
ADD file:bed2454356c48f77207726865f8aee34a5b3db6927a881655573cbde13ce5a89 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:28:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 02:30:25 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 26 Jan 2022 02:30:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 02:30:34 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Jan 2022 02:30:34 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Jan 2022 02:30:34 GMT
EXPOSE 8888
# Wed, 26 Jan 2022 02:30:34 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Jan 2022 02:30:35 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Jan 2022 02:30:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 02:30:35 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:1cb79db8a9e79b4f5415eaa91602251fb1eafe68d236efb80fe931bacfe5b3d6`  
		Last Modified: Wed, 26 Jan 2022 01:51:06 GMT  
		Size: 22.5 MB (22529131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1faa9122d932af0ee2f4243589d2aeb6e06442f2e8b566f7028df3b67b2a2485`  
		Last Modified: Wed, 26 Jan 2022 02:31:23 GMT  
		Size: 6.8 MB (6760139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c56fb053de399f5a050a94cadc82d48681ab473d97cfd016d06f1b812b7c6f`  
		Last Modified: Wed, 26 Jan 2022 02:31:57 GMT  
		Size: 36.9 MB (36926290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04689b7681a5d97b79b7e10bdccac5854d34d631908c7751d8b6a2048ad8fa3`  
		Last Modified: Wed, 26 Jan 2022 02:31:52 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b3ad8a98cd36da28b642d426301eb9b43717d6af72319878758f00c65ef2bc`  
		Last Modified: Wed, 26 Jan 2022 02:31:53 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51b1ef608a8a0087c2cc43256652668cd3fd304daf288932a8206fd98fe20bd`  
		Last Modified: Wed, 26 Jan 2022 02:31:52 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:d7c1c8f0c17216a152c34347f6dcd7d6e72277d40c6f6b64116cf919a7bca884
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59635362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93a14e97b7817820e8071cb316af64965076dd7ba4bf4af5be0ad38ed73d4f43`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:48:08 GMT
ADD file:26e6c9015d58ffb5e67d6ea64451fd0e27a9a60c65340659b35b075d51ed5c45 in / 
# Wed, 26 Jan 2022 01:48:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 17:17:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 17:19:45 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 26 Jan 2022 17:20:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 17:20:06 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Jan 2022 17:20:07 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Jan 2022 17:20:07 GMT
EXPOSE 8888
# Wed, 26 Jan 2022 17:20:07 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Jan 2022 17:20:08 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Jan 2022 17:20:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 17:20:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b651abcd2676c0bd22abf9acddc50231c15d43b1004fd0446bb57150c0d4c96b`  
		Last Modified: Wed, 26 Jan 2022 02:05:54 GMT  
		Size: 19.3 MB (19318809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0c89d838bd5ed63affedd67004af12d134c4995c36285fc64f348e14039db5`  
		Last Modified: Wed, 26 Jan 2022 17:21:43 GMT  
		Size: 5.8 MB (5780469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abcb4889ceb58f28ea516bb54997ee5d1209bd57154c4d7abd4b669d4a7fabf`  
		Last Modified: Wed, 26 Jan 2022 17:22:54 GMT  
		Size: 34.5 MB (34511688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93526c85aa1fb820ef679f987339cf40b632701b1932fd69d38c8999b9cd063c`  
		Last Modified: Wed, 26 Jan 2022 17:22:37 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a58472d60d287853d1535d796c12530a560b2bb77fc201bfa9bc1a203fa9b2`  
		Last Modified: Wed, 26 Jan 2022 17:22:37 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c58eaa73aa3cc3ecff2ce533556b07b53d18e22c6908ccd2146c0d995e57772`  
		Last Modified: Wed, 26 Jan 2022 17:22:37 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:39ce3af5ee637b33abe6f376584cd495c579be1f7b462d16dbfe70e5e9cc0f0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.9 MB (60892055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44fb1f55ba6e93c35ca46c77f02d3b824b64cce5f3c0790a423dd8453d3a64c5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:48 GMT
ADD file:952345b92a37bdbcaea817a1a9e1466c68e040b5dee856ff2606afbd1297b1f0 in / 
# Wed, 26 Jan 2022 01:44:48 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:30:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 02:31:41 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 26 Jan 2022 02:31:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 02:31:51 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Jan 2022 02:31:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Jan 2022 02:31:52 GMT
EXPOSE 8888
# Wed, 26 Jan 2022 02:31:53 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Jan 2022 02:31:55 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Jan 2022 02:31:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 02:31:56 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0baeb81232d08980c2f78646547d7792710a684e89313d2da7499bdff69437d0`  
		Last Modified: Wed, 26 Jan 2022 01:53:21 GMT  
		Size: 20.4 MB (20389407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fa5ffb58fb1affd19c9a960e3ea691bf31aebc8d3eb9cd3d49009cde7b183c`  
		Last Modified: Wed, 26 Jan 2022 02:32:42 GMT  
		Size: 6.0 MB (6046875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582bd54c3c4ec3f4f34aa635d36b9196dddf0aa3db26b18f459775cf88e60c56`  
		Last Modified: Wed, 26 Jan 2022 02:33:17 GMT  
		Size: 34.4 MB (34431380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a5b27cff924956d6ff369872ad1a257df48e13d4bb4e893a2fcffb88247d2d`  
		Last Modified: Wed, 26 Jan 2022 02:33:13 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd02366c5be0e6528281f1a00e5eeba8c9a299566e56afea687ace3b855510e`  
		Last Modified: Wed, 26 Jan 2022 02:33:13 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c60d53f93f031f41368e163d83d2f80bda78a157683faf7055e7fdd20caf7ed`  
		Last Modified: Wed, 26 Jan 2022 02:33:13 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8-alpine`

```console
$ docker pull chronograf@sha256:37af8f9a75619ff9a41d61b2395fad185b1daaf94aea63c81ca013ddcc112510
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:4f2fdffd0f89e9d26b360b63d1a7794d2511e88417b624fa63e82aceb3ecdea5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22333670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01ac33f8cebe8e52e9d28a37599d6205b0aa51c9ba34cd1e2bbf18b32324fe96`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:55:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 12 Nov 2021 21:55:51 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Fri, 12 Nov 2021 21:56:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 12 Nov 2021 21:56:00 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Nov 2021 21:56:00 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Nov 2021 21:56:01 GMT
EXPOSE 8888
# Fri, 12 Nov 2021 21:56:01 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Nov 2021 21:56:01 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 12 Nov 2021 21:56:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 21:56:01 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aac166cdd02de2f1baf9250ebe4e1a5bec54cc49a59dbb3716570ed37d5bf63`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 282.0 KB (281961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799e7fd8ed3ec32e09323ac48e268943b7d77fc4ed3a618a2a93ae2bef5d99d4`  
		Last Modified: Fri, 12 Nov 2021 21:57:13 GMT  
		Size: 19.2 MB (19204166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126bd6c969f1bb9e4ad0a7f6f576cf330325d804279329adc1cc66549dc44358`  
		Last Modified: Fri, 12 Nov 2021 21:57:10 GMT  
		Size: 12.3 KB (12268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a5f10b7fe32ea10409e5fabd241935dfd702349e179ae54173d56679568d9c`  
		Last Modified: Fri, 12 Nov 2021 21:57:09 GMT  
		Size: 11.9 KB (11901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860006ae37408c8d020a52a83bc91fdb91f8aea8a67a319597dfcccb0268666f`  
		Last Modified: Fri, 12 Nov 2021 21:57:09 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.10`

```console
$ docker pull chronograf@sha256:29082d75ef60be51485a84e88443626d62b5355d169a385adc4789c5055c890d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8.10` - linux; amd64

```console
$ docker pull chronograf@sha256:c6a5f44940a94d109f104c18a9b3877254ec898dd44735ec0e7fe83d64863836
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66239950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93c24f2aa6e6bc4d00b11a560e8b8ac02db3109231645c73d56b934bdb251ba0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:57 GMT
ADD file:bed2454356c48f77207726865f8aee34a5b3db6927a881655573cbde13ce5a89 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:28:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 02:30:25 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 26 Jan 2022 02:30:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 02:30:34 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Jan 2022 02:30:34 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Jan 2022 02:30:34 GMT
EXPOSE 8888
# Wed, 26 Jan 2022 02:30:34 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Jan 2022 02:30:35 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Jan 2022 02:30:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 02:30:35 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:1cb79db8a9e79b4f5415eaa91602251fb1eafe68d236efb80fe931bacfe5b3d6`  
		Last Modified: Wed, 26 Jan 2022 01:51:06 GMT  
		Size: 22.5 MB (22529131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1faa9122d932af0ee2f4243589d2aeb6e06442f2e8b566f7028df3b67b2a2485`  
		Last Modified: Wed, 26 Jan 2022 02:31:23 GMT  
		Size: 6.8 MB (6760139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c56fb053de399f5a050a94cadc82d48681ab473d97cfd016d06f1b812b7c6f`  
		Last Modified: Wed, 26 Jan 2022 02:31:57 GMT  
		Size: 36.9 MB (36926290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04689b7681a5d97b79b7e10bdccac5854d34d631908c7751d8b6a2048ad8fa3`  
		Last Modified: Wed, 26 Jan 2022 02:31:52 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b3ad8a98cd36da28b642d426301eb9b43717d6af72319878758f00c65ef2bc`  
		Last Modified: Wed, 26 Jan 2022 02:31:53 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51b1ef608a8a0087c2cc43256652668cd3fd304daf288932a8206fd98fe20bd`  
		Last Modified: Wed, 26 Jan 2022 02:31:52 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.10` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:d7c1c8f0c17216a152c34347f6dcd7d6e72277d40c6f6b64116cf919a7bca884
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59635362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93a14e97b7817820e8071cb316af64965076dd7ba4bf4af5be0ad38ed73d4f43`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:48:08 GMT
ADD file:26e6c9015d58ffb5e67d6ea64451fd0e27a9a60c65340659b35b075d51ed5c45 in / 
# Wed, 26 Jan 2022 01:48:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 17:17:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 17:19:45 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 26 Jan 2022 17:20:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 17:20:06 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Jan 2022 17:20:07 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Jan 2022 17:20:07 GMT
EXPOSE 8888
# Wed, 26 Jan 2022 17:20:07 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Jan 2022 17:20:08 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Jan 2022 17:20:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 17:20:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b651abcd2676c0bd22abf9acddc50231c15d43b1004fd0446bb57150c0d4c96b`  
		Last Modified: Wed, 26 Jan 2022 02:05:54 GMT  
		Size: 19.3 MB (19318809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0c89d838bd5ed63affedd67004af12d134c4995c36285fc64f348e14039db5`  
		Last Modified: Wed, 26 Jan 2022 17:21:43 GMT  
		Size: 5.8 MB (5780469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abcb4889ceb58f28ea516bb54997ee5d1209bd57154c4d7abd4b669d4a7fabf`  
		Last Modified: Wed, 26 Jan 2022 17:22:54 GMT  
		Size: 34.5 MB (34511688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93526c85aa1fb820ef679f987339cf40b632701b1932fd69d38c8999b9cd063c`  
		Last Modified: Wed, 26 Jan 2022 17:22:37 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a58472d60d287853d1535d796c12530a560b2bb77fc201bfa9bc1a203fa9b2`  
		Last Modified: Wed, 26 Jan 2022 17:22:37 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c58eaa73aa3cc3ecff2ce533556b07b53d18e22c6908ccd2146c0d995e57772`  
		Last Modified: Wed, 26 Jan 2022 17:22:37 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.10` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:39ce3af5ee637b33abe6f376584cd495c579be1f7b462d16dbfe70e5e9cc0f0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.9 MB (60892055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44fb1f55ba6e93c35ca46c77f02d3b824b64cce5f3c0790a423dd8453d3a64c5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:48 GMT
ADD file:952345b92a37bdbcaea817a1a9e1466c68e040b5dee856ff2606afbd1297b1f0 in / 
# Wed, 26 Jan 2022 01:44:48 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:30:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 02:31:41 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Wed, 26 Jan 2022 02:31:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 02:31:51 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Jan 2022 02:31:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Jan 2022 02:31:52 GMT
EXPOSE 8888
# Wed, 26 Jan 2022 02:31:53 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Jan 2022 02:31:55 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Jan 2022 02:31:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 02:31:56 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0baeb81232d08980c2f78646547d7792710a684e89313d2da7499bdff69437d0`  
		Last Modified: Wed, 26 Jan 2022 01:53:21 GMT  
		Size: 20.4 MB (20389407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fa5ffb58fb1affd19c9a960e3ea691bf31aebc8d3eb9cd3d49009cde7b183c`  
		Last Modified: Wed, 26 Jan 2022 02:32:42 GMT  
		Size: 6.0 MB (6046875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582bd54c3c4ec3f4f34aa635d36b9196dddf0aa3db26b18f459775cf88e60c56`  
		Last Modified: Wed, 26 Jan 2022 02:33:17 GMT  
		Size: 34.4 MB (34431380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a5b27cff924956d6ff369872ad1a257df48e13d4bb4e893a2fcffb88247d2d`  
		Last Modified: Wed, 26 Jan 2022 02:33:13 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd02366c5be0e6528281f1a00e5eeba8c9a299566e56afea687ace3b855510e`  
		Last Modified: Wed, 26 Jan 2022 02:33:13 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c60d53f93f031f41368e163d83d2f80bda78a157683faf7055e7fdd20caf7ed`  
		Last Modified: Wed, 26 Jan 2022 02:33:13 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.10-alpine`

```console
$ docker pull chronograf@sha256:37af8f9a75619ff9a41d61b2395fad185b1daaf94aea63c81ca013ddcc112510
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.8.10-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:4f2fdffd0f89e9d26b360b63d1a7794d2511e88417b624fa63e82aceb3ecdea5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22333670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01ac33f8cebe8e52e9d28a37599d6205b0aa51c9ba34cd1e2bbf18b32324fe96`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:55:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 12 Nov 2021 21:55:51 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Fri, 12 Nov 2021 21:56:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 12 Nov 2021 21:56:00 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Nov 2021 21:56:00 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Nov 2021 21:56:01 GMT
EXPOSE 8888
# Fri, 12 Nov 2021 21:56:01 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Nov 2021 21:56:01 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 12 Nov 2021 21:56:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 21:56:01 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aac166cdd02de2f1baf9250ebe4e1a5bec54cc49a59dbb3716570ed37d5bf63`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 282.0 KB (281961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799e7fd8ed3ec32e09323ac48e268943b7d77fc4ed3a618a2a93ae2bef5d99d4`  
		Last Modified: Fri, 12 Nov 2021 21:57:13 GMT  
		Size: 19.2 MB (19204166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126bd6c969f1bb9e4ad0a7f6f576cf330325d804279329adc1cc66549dc44358`  
		Last Modified: Fri, 12 Nov 2021 21:57:10 GMT  
		Size: 12.3 KB (12268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a5f10b7fe32ea10409e5fabd241935dfd702349e179ae54173d56679568d9c`  
		Last Modified: Fri, 12 Nov 2021 21:57:09 GMT  
		Size: 11.9 KB (11901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860006ae37408c8d020a52a83bc91fdb91f8aea8a67a319597dfcccb0268666f`  
		Last Modified: Fri, 12 Nov 2021 21:57:09 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9`

```console
$ docker pull chronograf@sha256:deee773434009af45e31a5a5c579b9bdbfc24ccc353d9e98a7618d30fe725ccb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.9` - linux; amd64

```console
$ docker pull chronograf@sha256:3abe866e2e4bba1a36c718f8cc956aa739c3a4ec7494cd7560dce6ba07f2878c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66863308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c75c2938b013aca871002a6a1a60cb823459ecc21a1e179c86fd3ce80acd767`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:57 GMT
ADD file:bed2454356c48f77207726865f8aee34a5b3db6927a881655573cbde13ce5a89 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:28:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 07 Feb 2022 20:19:37 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Mon, 07 Feb 2022 20:19:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Mon, 07 Feb 2022 20:19:47 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Feb 2022 20:19:47 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Feb 2022 20:19:48 GMT
EXPOSE 8888
# Mon, 07 Feb 2022 20:19:48 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Feb 2022 20:19:48 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Mon, 07 Feb 2022 20:19:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Feb 2022 20:19:48 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:1cb79db8a9e79b4f5415eaa91602251fb1eafe68d236efb80fe931bacfe5b3d6`  
		Last Modified: Wed, 26 Jan 2022 01:51:06 GMT  
		Size: 22.5 MB (22529131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1faa9122d932af0ee2f4243589d2aeb6e06442f2e8b566f7028df3b67b2a2485`  
		Last Modified: Wed, 26 Jan 2022 02:31:23 GMT  
		Size: 6.8 MB (6760139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3747deb462fb661a7c6b1db78b9498c134664b8f73cae8b67bd754adfdab257b`  
		Last Modified: Mon, 07 Feb 2022 20:21:19 GMT  
		Size: 37.5 MB (37549646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447019c2cc2e2870853d38916cbfc345c36cef930af5097e6d8474b73dbdbaf6`  
		Last Modified: Mon, 07 Feb 2022 20:21:14 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de650196bb629817cea965607fa87f436b05db846d42b312e81cf3de8acf7f91`  
		Last Modified: Mon, 07 Feb 2022 20:21:14 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb432c6b967100a3f940ceb70eb8a1ac8e3304f32bc13406007f2ff1187ab4f4`  
		Last Modified: Mon, 07 Feb 2022 20:21:14 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:f66199300f35b98fa1abc6ff7cf1390a5ad020e672914a3ed887e2a5128de0d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60397922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5427017891514bf41dd84247288112a22b0fe3cda4bc524580128da761b0d37`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:48:08 GMT
ADD file:26e6c9015d58ffb5e67d6ea64451fd0e27a9a60c65340659b35b075d51ed5c45 in / 
# Wed, 26 Jan 2022 01:48:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 17:17:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 07 Feb 2022 20:58:08 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Mon, 07 Feb 2022 20:58:29 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Mon, 07 Feb 2022 20:58:30 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Feb 2022 20:58:30 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Feb 2022 20:58:31 GMT
EXPOSE 8888
# Mon, 07 Feb 2022 20:58:31 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Feb 2022 20:58:32 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Mon, 07 Feb 2022 20:58:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Feb 2022 20:58:32 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b651abcd2676c0bd22abf9acddc50231c15d43b1004fd0446bb57150c0d4c96b`  
		Last Modified: Wed, 26 Jan 2022 02:05:54 GMT  
		Size: 19.3 MB (19318809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0c89d838bd5ed63affedd67004af12d134c4995c36285fc64f348e14039db5`  
		Last Modified: Wed, 26 Jan 2022 17:21:43 GMT  
		Size: 5.8 MB (5780469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af69db638deb41ad9d7b5cbc013c46a84e04cab53e31e6b87aab6df01fe9b668`  
		Last Modified: Mon, 07 Feb 2022 20:59:51 GMT  
		Size: 35.3 MB (35274251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c3c5f760682c50cc5f2fd7b17aa84e064f4b7aef484a26b76bd3888ad18c5a`  
		Last Modified: Mon, 07 Feb 2022 20:59:33 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740af52e8e330091ec341265faabec88cb621c22d0eddd670a96863d66a05ca6`  
		Last Modified: Mon, 07 Feb 2022 20:59:33 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1629a43bd934c28cc69090f5c2d1995630cfbd84cd29e4c00fb94d0685db25af`  
		Last Modified: Mon, 07 Feb 2022 20:59:33 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:a66c25589d1e45541de78a7080b6be68dfe6526a336e7643b3d110faf19076c7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.6 MB (61611989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a0b50bf68f77f54151156b5b02e162c84e42111af4f09704e191a3059d15747`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:48 GMT
ADD file:952345b92a37bdbcaea817a1a9e1466c68e040b5dee856ff2606afbd1297b1f0 in / 
# Wed, 26 Jan 2022 01:44:48 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:30:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 07 Feb 2022 20:39:40 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Mon, 07 Feb 2022 20:39:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Mon, 07 Feb 2022 20:39:51 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Feb 2022 20:39:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Feb 2022 20:39:52 GMT
EXPOSE 8888
# Mon, 07 Feb 2022 20:39:53 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Feb 2022 20:39:55 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Mon, 07 Feb 2022 20:39:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Feb 2022 20:39:56 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0baeb81232d08980c2f78646547d7792710a684e89313d2da7499bdff69437d0`  
		Last Modified: Wed, 26 Jan 2022 01:53:21 GMT  
		Size: 20.4 MB (20389407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fa5ffb58fb1affd19c9a960e3ea691bf31aebc8d3eb9cd3d49009cde7b183c`  
		Last Modified: Wed, 26 Jan 2022 02:32:42 GMT  
		Size: 6.0 MB (6046875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7f783e7e2892f7f446d6a6c0dd1824eabed1256a2e736cad83c4aae81ac853`  
		Last Modified: Mon, 07 Feb 2022 20:40:31 GMT  
		Size: 35.2 MB (35151313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e7853742620112bd8955410efd101ba7a6a73a3958a5ebdd25acb47249eb42`  
		Last Modified: Mon, 07 Feb 2022 20:40:26 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dea2156bfe70f6ddad97c7e1b7b308a8dfba907c01be188645c618adebb737f`  
		Last Modified: Mon, 07 Feb 2022 20:40:26 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59df867c6ba00b39182716a7295b86de6b95af1e534d5fa1bc1b6520f3109b9a`  
		Last Modified: Mon, 07 Feb 2022 20:40:26 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9-alpine`

```console
$ docker pull chronograf@sha256:9ebd87004683273a6d352c1dabf306f561ecf873cea006daae763331b2bf642a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.9-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:fe5dad09313a95aeb6f3faa0d20bf01c7daebd16527566df2c7faa3b71a65dba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.8 MB (22785910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8611b7c391730471adb50e7bae386b30eb0a3fe228bbe052e4f2308e661545be`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:55:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Mon, 07 Feb 2022 20:19:51 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Mon, 07 Feb 2022 20:20:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 07 Feb 2022 20:20:39 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Feb 2022 20:20:39 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Feb 2022 20:20:40 GMT
EXPOSE 8888
# Mon, 07 Feb 2022 20:20:40 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Feb 2022 20:20:40 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Mon, 07 Feb 2022 20:20:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Feb 2022 20:20:40 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aac166cdd02de2f1baf9250ebe4e1a5bec54cc49a59dbb3716570ed37d5bf63`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 282.0 KB (281961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08744947235ba971fc0c84b86eef6bfb7de402e304f5e5c910e391a4c333da8`  
		Last Modified: Mon, 07 Feb 2022 20:21:35 GMT  
		Size: 19.7 MB (19656415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27fe1f701b1e4797e8a999acf10aee9f0ddde3af283ad155b63b2edcea8c2e4`  
		Last Modified: Mon, 07 Feb 2022 20:21:31 GMT  
		Size: 12.3 KB (12265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fd5f2b080123d57bf09d1f2551a787d2fc1d0a55c7974a0e8426d79285f79f`  
		Last Modified: Mon, 07 Feb 2022 20:21:31 GMT  
		Size: 11.9 KB (11896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5202266ede2b05845fa57e63ef2fc87dae30c72f2228da7db5c598e19e5b712a`  
		Last Modified: Mon, 07 Feb 2022 20:21:31 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9.3`

```console
$ docker pull chronograf@sha256:deee773434009af45e31a5a5c579b9bdbfc24ccc353d9e98a7618d30fe725ccb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.9.3` - linux; amd64

```console
$ docker pull chronograf@sha256:3abe866e2e4bba1a36c718f8cc956aa739c3a4ec7494cd7560dce6ba07f2878c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66863308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c75c2938b013aca871002a6a1a60cb823459ecc21a1e179c86fd3ce80acd767`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:57 GMT
ADD file:bed2454356c48f77207726865f8aee34a5b3db6927a881655573cbde13ce5a89 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:28:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 07 Feb 2022 20:19:37 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Mon, 07 Feb 2022 20:19:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Mon, 07 Feb 2022 20:19:47 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Feb 2022 20:19:47 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Feb 2022 20:19:48 GMT
EXPOSE 8888
# Mon, 07 Feb 2022 20:19:48 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Feb 2022 20:19:48 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Mon, 07 Feb 2022 20:19:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Feb 2022 20:19:48 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:1cb79db8a9e79b4f5415eaa91602251fb1eafe68d236efb80fe931bacfe5b3d6`  
		Last Modified: Wed, 26 Jan 2022 01:51:06 GMT  
		Size: 22.5 MB (22529131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1faa9122d932af0ee2f4243589d2aeb6e06442f2e8b566f7028df3b67b2a2485`  
		Last Modified: Wed, 26 Jan 2022 02:31:23 GMT  
		Size: 6.8 MB (6760139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3747deb462fb661a7c6b1db78b9498c134664b8f73cae8b67bd754adfdab257b`  
		Last Modified: Mon, 07 Feb 2022 20:21:19 GMT  
		Size: 37.5 MB (37549646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447019c2cc2e2870853d38916cbfc345c36cef930af5097e6d8474b73dbdbaf6`  
		Last Modified: Mon, 07 Feb 2022 20:21:14 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de650196bb629817cea965607fa87f436b05db846d42b312e81cf3de8acf7f91`  
		Last Modified: Mon, 07 Feb 2022 20:21:14 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb432c6b967100a3f940ceb70eb8a1ac8e3304f32bc13406007f2ff1187ab4f4`  
		Last Modified: Mon, 07 Feb 2022 20:21:14 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9.3` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:f66199300f35b98fa1abc6ff7cf1390a5ad020e672914a3ed887e2a5128de0d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60397922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5427017891514bf41dd84247288112a22b0fe3cda4bc524580128da761b0d37`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:48:08 GMT
ADD file:26e6c9015d58ffb5e67d6ea64451fd0e27a9a60c65340659b35b075d51ed5c45 in / 
# Wed, 26 Jan 2022 01:48:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 17:17:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 07 Feb 2022 20:58:08 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Mon, 07 Feb 2022 20:58:29 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Mon, 07 Feb 2022 20:58:30 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Feb 2022 20:58:30 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Feb 2022 20:58:31 GMT
EXPOSE 8888
# Mon, 07 Feb 2022 20:58:31 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Feb 2022 20:58:32 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Mon, 07 Feb 2022 20:58:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Feb 2022 20:58:32 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b651abcd2676c0bd22abf9acddc50231c15d43b1004fd0446bb57150c0d4c96b`  
		Last Modified: Wed, 26 Jan 2022 02:05:54 GMT  
		Size: 19.3 MB (19318809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0c89d838bd5ed63affedd67004af12d134c4995c36285fc64f348e14039db5`  
		Last Modified: Wed, 26 Jan 2022 17:21:43 GMT  
		Size: 5.8 MB (5780469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af69db638deb41ad9d7b5cbc013c46a84e04cab53e31e6b87aab6df01fe9b668`  
		Last Modified: Mon, 07 Feb 2022 20:59:51 GMT  
		Size: 35.3 MB (35274251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c3c5f760682c50cc5f2fd7b17aa84e064f4b7aef484a26b76bd3888ad18c5a`  
		Last Modified: Mon, 07 Feb 2022 20:59:33 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740af52e8e330091ec341265faabec88cb621c22d0eddd670a96863d66a05ca6`  
		Last Modified: Mon, 07 Feb 2022 20:59:33 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1629a43bd934c28cc69090f5c2d1995630cfbd84cd29e4c00fb94d0685db25af`  
		Last Modified: Mon, 07 Feb 2022 20:59:33 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9.3` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:a66c25589d1e45541de78a7080b6be68dfe6526a336e7643b3d110faf19076c7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.6 MB (61611989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a0b50bf68f77f54151156b5b02e162c84e42111af4f09704e191a3059d15747`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:48 GMT
ADD file:952345b92a37bdbcaea817a1a9e1466c68e040b5dee856ff2606afbd1297b1f0 in / 
# Wed, 26 Jan 2022 01:44:48 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:30:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 07 Feb 2022 20:39:40 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Mon, 07 Feb 2022 20:39:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Mon, 07 Feb 2022 20:39:51 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Feb 2022 20:39:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Feb 2022 20:39:52 GMT
EXPOSE 8888
# Mon, 07 Feb 2022 20:39:53 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Feb 2022 20:39:55 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Mon, 07 Feb 2022 20:39:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Feb 2022 20:39:56 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0baeb81232d08980c2f78646547d7792710a684e89313d2da7499bdff69437d0`  
		Last Modified: Wed, 26 Jan 2022 01:53:21 GMT  
		Size: 20.4 MB (20389407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fa5ffb58fb1affd19c9a960e3ea691bf31aebc8d3eb9cd3d49009cde7b183c`  
		Last Modified: Wed, 26 Jan 2022 02:32:42 GMT  
		Size: 6.0 MB (6046875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7f783e7e2892f7f446d6a6c0dd1824eabed1256a2e736cad83c4aae81ac853`  
		Last Modified: Mon, 07 Feb 2022 20:40:31 GMT  
		Size: 35.2 MB (35151313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e7853742620112bd8955410efd101ba7a6a73a3958a5ebdd25acb47249eb42`  
		Last Modified: Mon, 07 Feb 2022 20:40:26 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dea2156bfe70f6ddad97c7e1b7b308a8dfba907c01be188645c618adebb737f`  
		Last Modified: Mon, 07 Feb 2022 20:40:26 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59df867c6ba00b39182716a7295b86de6b95af1e534d5fa1bc1b6520f3109b9a`  
		Last Modified: Mon, 07 Feb 2022 20:40:26 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9.3-alpine`

```console
$ docker pull chronograf@sha256:9ebd87004683273a6d352c1dabf306f561ecf873cea006daae763331b2bf642a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.9.3-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:fe5dad09313a95aeb6f3faa0d20bf01c7daebd16527566df2c7faa3b71a65dba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.8 MB (22785910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8611b7c391730471adb50e7bae386b30eb0a3fe228bbe052e4f2308e661545be`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:55:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Mon, 07 Feb 2022 20:19:51 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Mon, 07 Feb 2022 20:20:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 07 Feb 2022 20:20:39 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Feb 2022 20:20:39 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Feb 2022 20:20:40 GMT
EXPOSE 8888
# Mon, 07 Feb 2022 20:20:40 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Feb 2022 20:20:40 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Mon, 07 Feb 2022 20:20:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Feb 2022 20:20:40 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aac166cdd02de2f1baf9250ebe4e1a5bec54cc49a59dbb3716570ed37d5bf63`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 282.0 KB (281961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08744947235ba971fc0c84b86eef6bfb7de402e304f5e5c910e391a4c333da8`  
		Last Modified: Mon, 07 Feb 2022 20:21:35 GMT  
		Size: 19.7 MB (19656415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27fe1f701b1e4797e8a999acf10aee9f0ddde3af283ad155b63b2edcea8c2e4`  
		Last Modified: Mon, 07 Feb 2022 20:21:31 GMT  
		Size: 12.3 KB (12265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fd5f2b080123d57bf09d1f2551a787d2fc1d0a55c7974a0e8426d79285f79f`  
		Last Modified: Mon, 07 Feb 2022 20:21:31 GMT  
		Size: 11.9 KB (11896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5202266ede2b05845fa57e63ef2fc87dae30c72f2228da7db5c598e19e5b712a`  
		Last Modified: Mon, 07 Feb 2022 20:21:31 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:alpine`

```console
$ docker pull chronograf@sha256:9ebd87004683273a6d352c1dabf306f561ecf873cea006daae763331b2bf642a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:fe5dad09313a95aeb6f3faa0d20bf01c7daebd16527566df2c7faa3b71a65dba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.8 MB (22785910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8611b7c391730471adb50e7bae386b30eb0a3fe228bbe052e4f2308e661545be`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:55:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Mon, 07 Feb 2022 20:19:51 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Mon, 07 Feb 2022 20:20:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 07 Feb 2022 20:20:39 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Feb 2022 20:20:39 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Feb 2022 20:20:40 GMT
EXPOSE 8888
# Mon, 07 Feb 2022 20:20:40 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Feb 2022 20:20:40 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Mon, 07 Feb 2022 20:20:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Feb 2022 20:20:40 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aac166cdd02de2f1baf9250ebe4e1a5bec54cc49a59dbb3716570ed37d5bf63`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 282.0 KB (281961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08744947235ba971fc0c84b86eef6bfb7de402e304f5e5c910e391a4c333da8`  
		Last Modified: Mon, 07 Feb 2022 20:21:35 GMT  
		Size: 19.7 MB (19656415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27fe1f701b1e4797e8a999acf10aee9f0ddde3af283ad155b63b2edcea8c2e4`  
		Last Modified: Mon, 07 Feb 2022 20:21:31 GMT  
		Size: 12.3 KB (12265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fd5f2b080123d57bf09d1f2551a787d2fc1d0a55c7974a0e8426d79285f79f`  
		Last Modified: Mon, 07 Feb 2022 20:21:31 GMT  
		Size: 11.9 KB (11896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5202266ede2b05845fa57e63ef2fc87dae30c72f2228da7db5c598e19e5b712a`  
		Last Modified: Mon, 07 Feb 2022 20:21:31 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:latest`

```console
$ docker pull chronograf@sha256:deee773434009af45e31a5a5c579b9bdbfc24ccc353d9e98a7618d30fe725ccb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:3abe866e2e4bba1a36c718f8cc956aa739c3a4ec7494cd7560dce6ba07f2878c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66863308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c75c2938b013aca871002a6a1a60cb823459ecc21a1e179c86fd3ce80acd767`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:57 GMT
ADD file:bed2454356c48f77207726865f8aee34a5b3db6927a881655573cbde13ce5a89 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:28:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 07 Feb 2022 20:19:37 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Mon, 07 Feb 2022 20:19:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Mon, 07 Feb 2022 20:19:47 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Feb 2022 20:19:47 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Feb 2022 20:19:48 GMT
EXPOSE 8888
# Mon, 07 Feb 2022 20:19:48 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Feb 2022 20:19:48 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Mon, 07 Feb 2022 20:19:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Feb 2022 20:19:48 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:1cb79db8a9e79b4f5415eaa91602251fb1eafe68d236efb80fe931bacfe5b3d6`  
		Last Modified: Wed, 26 Jan 2022 01:51:06 GMT  
		Size: 22.5 MB (22529131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1faa9122d932af0ee2f4243589d2aeb6e06442f2e8b566f7028df3b67b2a2485`  
		Last Modified: Wed, 26 Jan 2022 02:31:23 GMT  
		Size: 6.8 MB (6760139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3747deb462fb661a7c6b1db78b9498c134664b8f73cae8b67bd754adfdab257b`  
		Last Modified: Mon, 07 Feb 2022 20:21:19 GMT  
		Size: 37.5 MB (37549646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447019c2cc2e2870853d38916cbfc345c36cef930af5097e6d8474b73dbdbaf6`  
		Last Modified: Mon, 07 Feb 2022 20:21:14 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de650196bb629817cea965607fa87f436b05db846d42b312e81cf3de8acf7f91`  
		Last Modified: Mon, 07 Feb 2022 20:21:14 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb432c6b967100a3f940ceb70eb8a1ac8e3304f32bc13406007f2ff1187ab4f4`  
		Last Modified: Mon, 07 Feb 2022 20:21:14 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:f66199300f35b98fa1abc6ff7cf1390a5ad020e672914a3ed887e2a5128de0d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60397922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5427017891514bf41dd84247288112a22b0fe3cda4bc524580128da761b0d37`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:48:08 GMT
ADD file:26e6c9015d58ffb5e67d6ea64451fd0e27a9a60c65340659b35b075d51ed5c45 in / 
# Wed, 26 Jan 2022 01:48:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 17:17:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 07 Feb 2022 20:58:08 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Mon, 07 Feb 2022 20:58:29 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Mon, 07 Feb 2022 20:58:30 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Feb 2022 20:58:30 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Feb 2022 20:58:31 GMT
EXPOSE 8888
# Mon, 07 Feb 2022 20:58:31 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Feb 2022 20:58:32 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Mon, 07 Feb 2022 20:58:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Feb 2022 20:58:32 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b651abcd2676c0bd22abf9acddc50231c15d43b1004fd0446bb57150c0d4c96b`  
		Last Modified: Wed, 26 Jan 2022 02:05:54 GMT  
		Size: 19.3 MB (19318809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0c89d838bd5ed63affedd67004af12d134c4995c36285fc64f348e14039db5`  
		Last Modified: Wed, 26 Jan 2022 17:21:43 GMT  
		Size: 5.8 MB (5780469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af69db638deb41ad9d7b5cbc013c46a84e04cab53e31e6b87aab6df01fe9b668`  
		Last Modified: Mon, 07 Feb 2022 20:59:51 GMT  
		Size: 35.3 MB (35274251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c3c5f760682c50cc5f2fd7b17aa84e064f4b7aef484a26b76bd3888ad18c5a`  
		Last Modified: Mon, 07 Feb 2022 20:59:33 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740af52e8e330091ec341265faabec88cb621c22d0eddd670a96863d66a05ca6`  
		Last Modified: Mon, 07 Feb 2022 20:59:33 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1629a43bd934c28cc69090f5c2d1995630cfbd84cd29e4c00fb94d0685db25af`  
		Last Modified: Mon, 07 Feb 2022 20:59:33 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:a66c25589d1e45541de78a7080b6be68dfe6526a336e7643b3d110faf19076c7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.6 MB (61611989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a0b50bf68f77f54151156b5b02e162c84e42111af4f09704e191a3059d15747`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:48 GMT
ADD file:952345b92a37bdbcaea817a1a9e1466c68e040b5dee856ff2606afbd1297b1f0 in / 
# Wed, 26 Jan 2022 01:44:48 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:30:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 07 Feb 2022 20:39:40 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Mon, 07 Feb 2022 20:39:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Mon, 07 Feb 2022 20:39:51 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Mon, 07 Feb 2022 20:39:52 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Mon, 07 Feb 2022 20:39:52 GMT
EXPOSE 8888
# Mon, 07 Feb 2022 20:39:53 GMT
VOLUME [/var/lib/chronograf]
# Mon, 07 Feb 2022 20:39:55 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Mon, 07 Feb 2022 20:39:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Feb 2022 20:39:56 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0baeb81232d08980c2f78646547d7792710a684e89313d2da7499bdff69437d0`  
		Last Modified: Wed, 26 Jan 2022 01:53:21 GMT  
		Size: 20.4 MB (20389407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fa5ffb58fb1affd19c9a960e3ea691bf31aebc8d3eb9cd3d49009cde7b183c`  
		Last Modified: Wed, 26 Jan 2022 02:32:42 GMT  
		Size: 6.0 MB (6046875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7f783e7e2892f7f446d6a6c0dd1824eabed1256a2e736cad83c4aae81ac853`  
		Last Modified: Mon, 07 Feb 2022 20:40:31 GMT  
		Size: 35.2 MB (35151313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e7853742620112bd8955410efd101ba7a6a73a3958a5ebdd25acb47249eb42`  
		Last Modified: Mon, 07 Feb 2022 20:40:26 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dea2156bfe70f6ddad97c7e1b7b308a8dfba907c01be188645c618adebb737f`  
		Last Modified: Mon, 07 Feb 2022 20:40:26 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59df867c6ba00b39182716a7295b86de6b95af1e534d5fa1bc1b6520f3109b9a`  
		Last Modified: Mon, 07 Feb 2022 20:40:26 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
