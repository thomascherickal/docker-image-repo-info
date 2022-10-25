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
$ docker pull chronograf@sha256:9934c4ad3603cc81961a93d256471b923513266b3a843833796f032609cd23f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.10` - linux; amd64

```console
$ docker pull chronograf@sha256:a97033bb97681c58bbf5b0c4b73a3f49ac3cdd5dadac6a0581298fa7a766693a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81261149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f66aad845a91f9085260f66c75a8fa648b0adc39b72a04ea5cccfcdd2d6c754c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:15:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 09:15:59 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Tue, 25 Oct 2022 09:16:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 09:16:08 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 09:16:08 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 09:16:08 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 09:16:09 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 09:16:09 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 09:16:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 09:16:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac31433f39d12daf226b0453431c2893ea68d4ca9e95016933cd0edcac586e8`  
		Last Modified: Tue, 25 Oct 2022 09:16:47 GMT  
		Size: 5.2 MB (5228634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebec2214fc5d441aae29437543b4180a09ef3f10f541850e04242bfe9809e70`  
		Last Modified: Tue, 25 Oct 2022 09:17:22 GMT  
		Size: 44.6 MB (44588085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255af7b2596c78a8a348397afef7ca5eae1fad1219b42db8eb54b50dc28439fd`  
		Last Modified: Tue, 25 Oct 2022 09:17:15 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6793fd1b24d959954f2d2acd575efdf8a9a1b9f975dbe93c398e8ce24592066`  
		Last Modified: Tue, 25 Oct 2022 09:17:15 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00e618cc14b44536304063224621d2804a0603dd5d75b7f2efe2e6d759c2638`  
		Last Modified: Tue, 25 Oct 2022 09:17:15 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:7ac31c5a43030c20f35a79c2da4bf346947c5d1e05b3e9d9445dbedfe99f229b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73563597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf8854c34693f89ab353b81801cc7a1fefaf7bf996970e7c714b3c9a56f2c12`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 12:53:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 12:54:00 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Tue, 25 Oct 2022 12:54:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 12:54:09 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 12:54:09 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 12:54:09 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 12:54:09 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 12:54:10 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 12:54:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 12:54:10 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f1749ac90bfa69003129e242051632c3420cf35e2a888329d8709010afae29`  
		Last Modified: Tue, 25 Oct 2022 12:55:02 GMT  
		Size: 4.5 MB (4494994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fc4ff7d1f4516f3810e6354425d49541ff9ad663d48c35410d514b836a5da1`  
		Last Modified: Tue, 25 Oct 2022 12:55:45 GMT  
		Size: 42.5 MB (42464917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df95d9ae6a19b1e1e9cb18c93597ce98317251569f5cd855d4af3606f9a2dc4e`  
		Last Modified: Tue, 25 Oct 2022 12:55:37 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494ef46291b2362156ed0fe658a1f43b2950377c3f62d0623cf215d2175e6be6`  
		Last Modified: Tue, 25 Oct 2022 12:55:37 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94a2368587118a72f6f1ca4a4ccb2a0179f7e77af6da9e20954e4dc88fa5989`  
		Last Modified: Tue, 25 Oct 2022 12:55:37 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:c9ad1548053c5343bef238546bc24b2f5b9d164772c869d7883dab79764397f2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.9 MB (77917795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:621b8643698227f3e041ea9e759c2604049932d25e024fadef21fdd064f8b36c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:38:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 08:38:31 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Tue, 25 Oct 2022 08:38:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 08:38:38 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 08:38:38 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 08:38:38 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 08:38:38 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 08:38:39 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 08:38:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 08:38:39 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7b3c23d0957a403636903049e3f2ee067f7db24d1189f980fc21302028781d`  
		Last Modified: Tue, 25 Oct 2022 08:39:06 GMT  
		Size: 5.2 MB (5211554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa58d779a4fb96cfe4fc04d985e65f4fdaa11560a21388a1b4fbca05931841db`  
		Last Modified: Tue, 25 Oct 2022 08:39:38 GMT  
		Size: 42.6 MB (42617940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452d6327993901bdf4ebf07f7a49a37a88e2d07f288d80cf37c0206f47ec24c1`  
		Last Modified: Tue, 25 Oct 2022 08:39:33 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5d48b03794eeb85fbb87600d45cb4c9ff690ef4782885d5487aa069e408bdd`  
		Last Modified: Tue, 25 Oct 2022 08:39:33 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77c39d0ee6b7fa8173fc740ad5e236d2fe3e9c533931d20aaeabcdf360286ee`  
		Last Modified: Tue, 25 Oct 2022 08:39:33 GMT  
		Size: 238.0 B  
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
$ docker pull chronograf@sha256:9934c4ad3603cc81961a93d256471b923513266b3a843833796f032609cd23f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.10.0` - linux; amd64

```console
$ docker pull chronograf@sha256:a97033bb97681c58bbf5b0c4b73a3f49ac3cdd5dadac6a0581298fa7a766693a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81261149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f66aad845a91f9085260f66c75a8fa648b0adc39b72a04ea5cccfcdd2d6c754c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:15:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 09:15:59 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Tue, 25 Oct 2022 09:16:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 09:16:08 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 09:16:08 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 09:16:08 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 09:16:09 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 09:16:09 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 09:16:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 09:16:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac31433f39d12daf226b0453431c2893ea68d4ca9e95016933cd0edcac586e8`  
		Last Modified: Tue, 25 Oct 2022 09:16:47 GMT  
		Size: 5.2 MB (5228634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebec2214fc5d441aae29437543b4180a09ef3f10f541850e04242bfe9809e70`  
		Last Modified: Tue, 25 Oct 2022 09:17:22 GMT  
		Size: 44.6 MB (44588085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255af7b2596c78a8a348397afef7ca5eae1fad1219b42db8eb54b50dc28439fd`  
		Last Modified: Tue, 25 Oct 2022 09:17:15 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6793fd1b24d959954f2d2acd575efdf8a9a1b9f975dbe93c398e8ce24592066`  
		Last Modified: Tue, 25 Oct 2022 09:17:15 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00e618cc14b44536304063224621d2804a0603dd5d75b7f2efe2e6d759c2638`  
		Last Modified: Tue, 25 Oct 2022 09:17:15 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10.0` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:7ac31c5a43030c20f35a79c2da4bf346947c5d1e05b3e9d9445dbedfe99f229b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73563597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf8854c34693f89ab353b81801cc7a1fefaf7bf996970e7c714b3c9a56f2c12`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 12:53:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 12:54:00 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Tue, 25 Oct 2022 12:54:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 12:54:09 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 12:54:09 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 12:54:09 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 12:54:09 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 12:54:10 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 12:54:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 12:54:10 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f1749ac90bfa69003129e242051632c3420cf35e2a888329d8709010afae29`  
		Last Modified: Tue, 25 Oct 2022 12:55:02 GMT  
		Size: 4.5 MB (4494994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fc4ff7d1f4516f3810e6354425d49541ff9ad663d48c35410d514b836a5da1`  
		Last Modified: Tue, 25 Oct 2022 12:55:45 GMT  
		Size: 42.5 MB (42464917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df95d9ae6a19b1e1e9cb18c93597ce98317251569f5cd855d4af3606f9a2dc4e`  
		Last Modified: Tue, 25 Oct 2022 12:55:37 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494ef46291b2362156ed0fe658a1f43b2950377c3f62d0623cf215d2175e6be6`  
		Last Modified: Tue, 25 Oct 2022 12:55:37 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94a2368587118a72f6f1ca4a4ccb2a0179f7e77af6da9e20954e4dc88fa5989`  
		Last Modified: Tue, 25 Oct 2022 12:55:37 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10.0` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:c9ad1548053c5343bef238546bc24b2f5b9d164772c869d7883dab79764397f2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.9 MB (77917795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:621b8643698227f3e041ea9e759c2604049932d25e024fadef21fdd064f8b36c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:38:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 08:38:31 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Tue, 25 Oct 2022 08:38:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 08:38:38 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 08:38:38 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 08:38:38 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 08:38:38 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 08:38:39 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 08:38:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 08:38:39 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7b3c23d0957a403636903049e3f2ee067f7db24d1189f980fc21302028781d`  
		Last Modified: Tue, 25 Oct 2022 08:39:06 GMT  
		Size: 5.2 MB (5211554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa58d779a4fb96cfe4fc04d985e65f4fdaa11560a21388a1b4fbca05931841db`  
		Last Modified: Tue, 25 Oct 2022 08:39:38 GMT  
		Size: 42.6 MB (42617940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452d6327993901bdf4ebf07f7a49a37a88e2d07f288d80cf37c0206f47ec24c1`  
		Last Modified: Tue, 25 Oct 2022 08:39:33 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5d48b03794eeb85fbb87600d45cb4c9ff690ef4782885d5487aa069e408bdd`  
		Last Modified: Tue, 25 Oct 2022 08:39:33 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77c39d0ee6b7fa8173fc740ad5e236d2fe3e9c533931d20aaeabcdf360286ee`  
		Last Modified: Tue, 25 Oct 2022 08:39:33 GMT  
		Size: 238.0 B  
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
$ docker pull chronograf@sha256:46c1c92bcc0a478724a19d2b00537a350bce3e74d1225bb78343508f6b80708d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7` - linux; amd64

```console
$ docker pull chronograf@sha256:54ffd36b1951741a597dbbf8500a5a0d5d2f036b60bb78234f13fbca388df4a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70602203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de03bd4520657954f99553c861a4dc5494f92c1cbb46f0b63c6e340be0c64ba2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:15:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 09:15:05 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 25 Oct 2022 09:15:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 09:15:14 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 09:15:15 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 09:15:15 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 09:15:15 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 09:15:15 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 09:15:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 09:15:15 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afad2525e675db66e7c61f397bac1b87e20bbd893d43609199a9eb59b520c87e`  
		Last Modified: Tue, 25 Oct 2022 09:16:32 GMT  
		Size: 4.4 MB (4418920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bbaa7c3ccbcb3be930298137d5914f5d65d68621108a6ecda2ea8abba6bf94`  
		Last Modified: Tue, 25 Oct 2022 09:16:36 GMT  
		Size: 34.7 MB (34738859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7dbb3839d8ce12ba8092a84bf06cc7fc54351a38cd7ae154b9e65c59b6df9d`  
		Last Modified: Tue, 25 Oct 2022 09:16:32 GMT  
		Size: 12.2 KB (12242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d45df95673533033cd39b1a635a7b81955c20f354569a8110234bed3298dec`  
		Last Modified: Tue, 25 Oct 2022 09:16:32 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebed7c1d3e377c458f905b3dd1f40e12d07a5224fd601e2a14e754fe495370d1`  
		Last Modified: Tue, 25 Oct 2022 09:16:32 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:6fc935dc6c039ddc5b11b0bb1b83b1bf8d150bd699af63afe379d3700285613c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63422436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2fbe33f96134563eaa044e6135f1d1a625626c4baed325925a464c870a21fc5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 12:53:03 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 12:53:03 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 25 Oct 2022 12:53:13 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 12:53:13 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 12:53:13 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 12:53:14 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 12:53:14 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 12:53:14 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 12:53:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 12:53:14 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31c3e9e24e975c089ecf2d1d0746bd3baf2cee02e0b41bbfad7ba91b7759832`  
		Last Modified: Tue, 25 Oct 2022 12:54:45 GMT  
		Size: 3.7 MB (3720261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ad4e9d1579e38cb3ac71972eebc39be364100425374b36ec2566e7422d253d`  
		Last Modified: Tue, 25 Oct 2022 12:54:50 GMT  
		Size: 33.1 MB (33098489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1e6693bcfd9b863df9163cc7af78a0d0c47b8ac1745533138d77d5339b534f`  
		Last Modified: Tue, 25 Oct 2022 12:54:44 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f72bf714c3fffb723eba8fdfab7873683a74cd1dc233874cf4e9f9a4efeee7`  
		Last Modified: Tue, 25 Oct 2022 12:54:44 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d9edb04a8523842fb7a8ffed6b327e82d324c7bf4957cade5105f4b7f614cb`  
		Last Modified: Tue, 25 Oct 2022 12:54:44 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:dcbe42c987322f3a3d9e34b887f6a9082318931ba7ed8219b4cabe4ecf23903b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67747096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0870f105097b62b99a3e23534afe81c7ffcaadde97ef527f113503ae8d3fcdc2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:37:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 08:37:56 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 25 Oct 2022 08:38:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 08:38:04 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 08:38:04 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 08:38:04 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 08:38:04 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 08:38:04 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 08:38:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 08:38:04 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2d78ae245fa8ca64a3a155985a04e9614c285f914078857c92e54925706e0c`  
		Last Modified: Tue, 25 Oct 2022 08:38:53 GMT  
		Size: 4.4 MB (4420047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f961677d25ffd4e9c3badd96e9dc83a5155b6cfcb77f3e203192c61425ec95`  
		Last Modified: Tue, 25 Oct 2022 08:38:56 GMT  
		Size: 33.2 MB (33238751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66f1243a9bcc00b6bb39e77653e02027c0590d31e536bf374d592b7310c08fc`  
		Last Modified: Tue, 25 Oct 2022 08:38:53 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a934632c2ff34abb5f4bd988c743cf1e392845dc3ac1fe0ea3f356eed42e578d`  
		Last Modified: Tue, 25 Oct 2022 08:38:53 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674c476d8c3b56a1f2b2e47b9fb9e8d84cd088c3438a17a98cf1678356026ad0`  
		Last Modified: Tue, 25 Oct 2022 08:38:53 GMT  
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
$ docker pull chronograf@sha256:46c1c92bcc0a478724a19d2b00537a350bce3e74d1225bb78343508f6b80708d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7.17` - linux; amd64

```console
$ docker pull chronograf@sha256:54ffd36b1951741a597dbbf8500a5a0d5d2f036b60bb78234f13fbca388df4a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70602203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de03bd4520657954f99553c861a4dc5494f92c1cbb46f0b63c6e340be0c64ba2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:15:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 09:15:05 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 25 Oct 2022 09:15:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 09:15:14 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 09:15:15 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 09:15:15 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 09:15:15 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 09:15:15 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 09:15:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 09:15:15 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afad2525e675db66e7c61f397bac1b87e20bbd893d43609199a9eb59b520c87e`  
		Last Modified: Tue, 25 Oct 2022 09:16:32 GMT  
		Size: 4.4 MB (4418920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bbaa7c3ccbcb3be930298137d5914f5d65d68621108a6ecda2ea8abba6bf94`  
		Last Modified: Tue, 25 Oct 2022 09:16:36 GMT  
		Size: 34.7 MB (34738859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7dbb3839d8ce12ba8092a84bf06cc7fc54351a38cd7ae154b9e65c59b6df9d`  
		Last Modified: Tue, 25 Oct 2022 09:16:32 GMT  
		Size: 12.2 KB (12242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d45df95673533033cd39b1a635a7b81955c20f354569a8110234bed3298dec`  
		Last Modified: Tue, 25 Oct 2022 09:16:32 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebed7c1d3e377c458f905b3dd1f40e12d07a5224fd601e2a14e754fe495370d1`  
		Last Modified: Tue, 25 Oct 2022 09:16:32 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:6fc935dc6c039ddc5b11b0bb1b83b1bf8d150bd699af63afe379d3700285613c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63422436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2fbe33f96134563eaa044e6135f1d1a625626c4baed325925a464c870a21fc5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 12:53:03 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 12:53:03 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 25 Oct 2022 12:53:13 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 12:53:13 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 12:53:13 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 12:53:14 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 12:53:14 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 12:53:14 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 12:53:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 12:53:14 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31c3e9e24e975c089ecf2d1d0746bd3baf2cee02e0b41bbfad7ba91b7759832`  
		Last Modified: Tue, 25 Oct 2022 12:54:45 GMT  
		Size: 3.7 MB (3720261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ad4e9d1579e38cb3ac71972eebc39be364100425374b36ec2566e7422d253d`  
		Last Modified: Tue, 25 Oct 2022 12:54:50 GMT  
		Size: 33.1 MB (33098489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1e6693bcfd9b863df9163cc7af78a0d0c47b8ac1745533138d77d5339b534f`  
		Last Modified: Tue, 25 Oct 2022 12:54:44 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f72bf714c3fffb723eba8fdfab7873683a74cd1dc233874cf4e9f9a4efeee7`  
		Last Modified: Tue, 25 Oct 2022 12:54:44 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d9edb04a8523842fb7a8ffed6b327e82d324c7bf4957cade5105f4b7f614cb`  
		Last Modified: Tue, 25 Oct 2022 12:54:44 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:dcbe42c987322f3a3d9e34b887f6a9082318931ba7ed8219b4cabe4ecf23903b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67747096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0870f105097b62b99a3e23534afe81c7ffcaadde97ef527f113503ae8d3fcdc2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:37:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 08:37:56 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 25 Oct 2022 08:38:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 08:38:04 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 08:38:04 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 08:38:04 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 08:38:04 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 08:38:04 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 08:38:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 08:38:04 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2d78ae245fa8ca64a3a155985a04e9614c285f914078857c92e54925706e0c`  
		Last Modified: Tue, 25 Oct 2022 08:38:53 GMT  
		Size: 4.4 MB (4420047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f961677d25ffd4e9c3badd96e9dc83a5155b6cfcb77f3e203192c61425ec95`  
		Last Modified: Tue, 25 Oct 2022 08:38:56 GMT  
		Size: 33.2 MB (33238751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66f1243a9bcc00b6bb39e77653e02027c0590d31e536bf374d592b7310c08fc`  
		Last Modified: Tue, 25 Oct 2022 08:38:53 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a934632c2ff34abb5f4bd988c743cf1e392845dc3ac1fe0ea3f356eed42e578d`  
		Last Modified: Tue, 25 Oct 2022 08:38:53 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674c476d8c3b56a1f2b2e47b9fb9e8d84cd088c3438a17a98cf1678356026ad0`  
		Last Modified: Tue, 25 Oct 2022 08:38:53 GMT  
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
$ docker pull chronograf@sha256:6be0f223b2a3452a1aac7b1c6badf11a64f46312b82958276e4d563317d037ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8` - linux; amd64

```console
$ docker pull chronograf@sha256:86f423c746db208a52eb02967ca1444c5368bb112234e035115435913383a02b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71252777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e28275bc1b97fb5ca38df9864324d45a532ab8c91277b2368d79c77dc326ab20`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:15:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 09:15:28 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 25 Oct 2022 09:15:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 09:15:41 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 09:15:41 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 09:15:41 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 09:15:41 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 09:15:41 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 09:15:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 09:15:41 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac31433f39d12daf226b0453431c2893ea68d4ca9e95016933cd0edcac586e8`  
		Last Modified: Tue, 25 Oct 2022 09:16:47 GMT  
		Size: 5.2 MB (5228634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e60ed484a3666014196dc7376afee772704c698ff61c39b11fa4c1c93aba36`  
		Last Modified: Tue, 25 Oct 2022 09:16:51 GMT  
		Size: 34.6 MB (34579716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112dd76406c21c5bb6819f5b7e041b34a229d03fea520eb2cbd89dcfd739a4bc`  
		Last Modified: Tue, 25 Oct 2022 09:16:46 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97587a220125b766bad784383ec7d7d80dd4ce7b6dc1e90d7e0034883361f8fb`  
		Last Modified: Tue, 25 Oct 2022 09:16:46 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c3fb2032cb954b685aafa9c147e56725e1e3dbd3c655f1140ba28e88eb4e1e`  
		Last Modified: Tue, 25 Oct 2022 09:16:46 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:befea31ea86df17af10517dd4437e5efffbf4ef29305caaa576e9fbd301fec2a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63849916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7dff58c2393ff8c2722f58082df04be4c66f21609dab86e63b34d7a8602c1b5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 12:53:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 12:53:28 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 25 Oct 2022 12:53:36 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 12:53:36 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 12:53:37 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 12:53:37 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 12:53:37 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 12:53:37 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 12:53:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 12:53:37 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f1749ac90bfa69003129e242051632c3420cf35e2a888329d8709010afae29`  
		Last Modified: Tue, 25 Oct 2022 12:55:02 GMT  
		Size: 4.5 MB (4494994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4638362b727ada9e3a2c8ed11b884a4e1f04a2d5313b170892a434d1ef5c710d`  
		Last Modified: Tue, 25 Oct 2022 12:55:08 GMT  
		Size: 32.8 MB (32751236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f2273aee395b843b9893287408ecf12f76d2e79e5535d8aaac8805a31812ba`  
		Last Modified: Tue, 25 Oct 2022 12:55:01 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ba2422d64e37570091cfcfce5055db81e95cdd33daa11ea45eaaeba29aebd0`  
		Last Modified: Tue, 25 Oct 2022 12:55:01 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72311b79f90a42cfcf3044dd676ace14df3ca6a2fe7b433d6f0de939ae0422d4`  
		Last Modified: Tue, 25 Oct 2022 12:55:02 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:173e66d0bad66417145906a3208eaf9e618655905411f3e89187761f8ba33cfd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67944351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32714ebde89ac643caaf84b2d5a55826b82821a255c3cbcd18186035f502606e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:38:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 08:38:13 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 25 Oct 2022 08:38:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 08:38:19 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 08:38:19 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 08:38:19 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 08:38:19 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 08:38:19 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 08:38:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 08:38:20 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7b3c23d0957a403636903049e3f2ee067f7db24d1189f980fc21302028781d`  
		Last Modified: Tue, 25 Oct 2022 08:39:06 GMT  
		Size: 5.2 MB (5211554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ccebdc5913d0e5a9ab10d2dc7c3a962ee292655b10c85ce575668dcf68fd87`  
		Last Modified: Tue, 25 Oct 2022 08:39:11 GMT  
		Size: 32.6 MB (32644496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e491b00122d042a4837369ff0e61faad6f8fdc7db1d58a02a8a9e16f1aa33838`  
		Last Modified: Tue, 25 Oct 2022 08:39:05 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce8dd85dee83c8028be85cc95696a9f96a3d57e923f62b88f084dc95d8d82ad`  
		Last Modified: Tue, 25 Oct 2022 08:39:05 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c35993471c387cd63d219f25a0fab94c732e209098702fe2dd3aee16932c97`  
		Last Modified: Tue, 25 Oct 2022 08:39:05 GMT  
		Size: 240.0 B  
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
$ docker pull chronograf@sha256:6be0f223b2a3452a1aac7b1c6badf11a64f46312b82958276e4d563317d037ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8.10` - linux; amd64

```console
$ docker pull chronograf@sha256:86f423c746db208a52eb02967ca1444c5368bb112234e035115435913383a02b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71252777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e28275bc1b97fb5ca38df9864324d45a532ab8c91277b2368d79c77dc326ab20`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:15:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 09:15:28 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 25 Oct 2022 09:15:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 09:15:41 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 09:15:41 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 09:15:41 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 09:15:41 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 09:15:41 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 09:15:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 09:15:41 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac31433f39d12daf226b0453431c2893ea68d4ca9e95016933cd0edcac586e8`  
		Last Modified: Tue, 25 Oct 2022 09:16:47 GMT  
		Size: 5.2 MB (5228634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e60ed484a3666014196dc7376afee772704c698ff61c39b11fa4c1c93aba36`  
		Last Modified: Tue, 25 Oct 2022 09:16:51 GMT  
		Size: 34.6 MB (34579716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112dd76406c21c5bb6819f5b7e041b34a229d03fea520eb2cbd89dcfd739a4bc`  
		Last Modified: Tue, 25 Oct 2022 09:16:46 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97587a220125b766bad784383ec7d7d80dd4ce7b6dc1e90d7e0034883361f8fb`  
		Last Modified: Tue, 25 Oct 2022 09:16:46 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c3fb2032cb954b685aafa9c147e56725e1e3dbd3c655f1140ba28e88eb4e1e`  
		Last Modified: Tue, 25 Oct 2022 09:16:46 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.10` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:befea31ea86df17af10517dd4437e5efffbf4ef29305caaa576e9fbd301fec2a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63849916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7dff58c2393ff8c2722f58082df04be4c66f21609dab86e63b34d7a8602c1b5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 12:53:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 12:53:28 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 25 Oct 2022 12:53:36 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 12:53:36 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 12:53:37 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 12:53:37 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 12:53:37 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 12:53:37 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 12:53:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 12:53:37 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f1749ac90bfa69003129e242051632c3420cf35e2a888329d8709010afae29`  
		Last Modified: Tue, 25 Oct 2022 12:55:02 GMT  
		Size: 4.5 MB (4494994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4638362b727ada9e3a2c8ed11b884a4e1f04a2d5313b170892a434d1ef5c710d`  
		Last Modified: Tue, 25 Oct 2022 12:55:08 GMT  
		Size: 32.8 MB (32751236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f2273aee395b843b9893287408ecf12f76d2e79e5535d8aaac8805a31812ba`  
		Last Modified: Tue, 25 Oct 2022 12:55:01 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ba2422d64e37570091cfcfce5055db81e95cdd33daa11ea45eaaeba29aebd0`  
		Last Modified: Tue, 25 Oct 2022 12:55:01 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72311b79f90a42cfcf3044dd676ace14df3ca6a2fe7b433d6f0de939ae0422d4`  
		Last Modified: Tue, 25 Oct 2022 12:55:02 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.10` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:173e66d0bad66417145906a3208eaf9e618655905411f3e89187761f8ba33cfd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67944351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32714ebde89ac643caaf84b2d5a55826b82821a255c3cbcd18186035f502606e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:38:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 08:38:13 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 25 Oct 2022 08:38:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 08:38:19 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 08:38:19 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 08:38:19 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 08:38:19 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 08:38:19 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 08:38:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 08:38:20 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7b3c23d0957a403636903049e3f2ee067f7db24d1189f980fc21302028781d`  
		Last Modified: Tue, 25 Oct 2022 08:39:06 GMT  
		Size: 5.2 MB (5211554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ccebdc5913d0e5a9ab10d2dc7c3a962ee292655b10c85ce575668dcf68fd87`  
		Last Modified: Tue, 25 Oct 2022 08:39:11 GMT  
		Size: 32.6 MB (32644496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e491b00122d042a4837369ff0e61faad6f8fdc7db1d58a02a8a9e16f1aa33838`  
		Last Modified: Tue, 25 Oct 2022 08:39:05 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce8dd85dee83c8028be85cc95696a9f96a3d57e923f62b88f084dc95d8d82ad`  
		Last Modified: Tue, 25 Oct 2022 08:39:05 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c35993471c387cd63d219f25a0fab94c732e209098702fe2dd3aee16932c97`  
		Last Modified: Tue, 25 Oct 2022 08:39:05 GMT  
		Size: 240.0 B  
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
$ docker pull chronograf@sha256:f297dbe245e6fcb2a7cc1fd62e99262f250e95d2a5b648fd4af828c60a15b101
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.9` - linux; amd64

```console
$ docker pull chronograf@sha256:2b7a871bc4164c5d4fd9b898b68211211a08820cee34305aefc04acba26a5ffa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71900293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc2bb4952af2650ec11c36009cc4165b61aa7e49b047a987c9d81af8a6569c66`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:15:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 09:15:46 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 25 Oct 2022 09:15:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 09:15:54 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 09:15:54 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 09:15:54 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 09:15:54 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 09:15:55 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 09:15:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 09:15:55 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac31433f39d12daf226b0453431c2893ea68d4ca9e95016933cd0edcac586e8`  
		Last Modified: Tue, 25 Oct 2022 09:16:47 GMT  
		Size: 5.2 MB (5228634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4213fd0a2c107f89224c6ffd0cc72d7789b9854429945105d270dc62b12971f4`  
		Last Modified: Tue, 25 Oct 2022 09:17:05 GMT  
		Size: 35.2 MB (35227242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b119be2fb660edb1ffdd9f9660eddbd3ea4769f2056fbe4e126892709810f06`  
		Last Modified: Tue, 25 Oct 2022 09:17:01 GMT  
		Size: 12.2 KB (12239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6856d73f65d30e6a5b1045ad0a8a917ba46614fc5ed6b621442cc52da1ef177`  
		Last Modified: Tue, 25 Oct 2022 09:17:01 GMT  
		Size: 11.9 KB (11901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8beaca774f9e28447307a5b3617dcb7dd0a6cbd22b2412fc8dd40f578140886`  
		Last Modified: Tue, 25 Oct 2022 09:17:01 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:d39db9c5bee245adab9e2d279ae85081f5e8cdc9bc4a08e8a5c1a4fa3e882b9d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64625976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45220ed124c058e72b8ca2abf28cc304b74717a1b9cec565c0a6a848f813e8c3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 12:53:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 12:53:44 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 25 Oct 2022 12:53:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 12:53:53 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 12:53:53 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 12:53:53 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 12:53:53 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 12:53:53 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 12:53:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 12:53:53 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f1749ac90bfa69003129e242051632c3420cf35e2a888329d8709010afae29`  
		Last Modified: Tue, 25 Oct 2022 12:55:02 GMT  
		Size: 4.5 MB (4494994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e8db9c3d57be2294d02966f878b5757729d88fef4b55fae953e9ccc65f19ea`  
		Last Modified: Tue, 25 Oct 2022 12:55:25 GMT  
		Size: 33.5 MB (33527297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4585677714f44662fc1cf39c8142de63850610b0b0da8f64669c90b7c7f13a4a`  
		Last Modified: Tue, 25 Oct 2022 12:55:20 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45098fb25922115244c237d7449f3919d0aecf8f3027d12ee9e210687f9b6467`  
		Last Modified: Tue, 25 Oct 2022 12:55:20 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e399d15b9ffd9d2ae5af3b9e490a75a71c00ad3e9f28d377e3e605a1e83857`  
		Last Modified: Tue, 25 Oct 2022 12:55:20 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:5ba768bf227ccc47b78cc3beadb0386a24083ad0daf7aa352f2abe269a81bd2c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68696018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ecbe05ef389f89d2c990338329668c1d3399e360227c8a1bd077ac44988b476`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:38:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 08:38:23 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 25 Oct 2022 08:38:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 08:38:29 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 08:38:29 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 08:38:29 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 08:38:29 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 08:38:29 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 08:38:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 08:38:29 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7b3c23d0957a403636903049e3f2ee067f7db24d1189f980fc21302028781d`  
		Last Modified: Tue, 25 Oct 2022 08:39:06 GMT  
		Size: 5.2 MB (5211554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a982e14ccb4cc18d1e0c3b8f186b973be90cd4b9ef6ebe6d3afba5a81c21be68`  
		Last Modified: Tue, 25 Oct 2022 08:39:24 GMT  
		Size: 33.4 MB (33396167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eae55a830e348cd136e530df6507112153a911067fb005ffd3d1027e00af1ed`  
		Last Modified: Tue, 25 Oct 2022 08:39:21 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8b55afffb752cacfa4ee18c739e1af7166ae13a95b250fd99b9263eb165ebe`  
		Last Modified: Tue, 25 Oct 2022 08:39:20 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148a8a02094f868590e9cff0852379f15fa1731fdcca464755479278690a7bb3`  
		Last Modified: Tue, 25 Oct 2022 08:39:20 GMT  
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
$ docker pull chronograf@sha256:f297dbe245e6fcb2a7cc1fd62e99262f250e95d2a5b648fd4af828c60a15b101
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.9.4` - linux; amd64

```console
$ docker pull chronograf@sha256:2b7a871bc4164c5d4fd9b898b68211211a08820cee34305aefc04acba26a5ffa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71900293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc2bb4952af2650ec11c36009cc4165b61aa7e49b047a987c9d81af8a6569c66`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:15:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 09:15:46 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 25 Oct 2022 09:15:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 09:15:54 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 09:15:54 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 09:15:54 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 09:15:54 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 09:15:55 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 09:15:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 09:15:55 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac31433f39d12daf226b0453431c2893ea68d4ca9e95016933cd0edcac586e8`  
		Last Modified: Tue, 25 Oct 2022 09:16:47 GMT  
		Size: 5.2 MB (5228634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4213fd0a2c107f89224c6ffd0cc72d7789b9854429945105d270dc62b12971f4`  
		Last Modified: Tue, 25 Oct 2022 09:17:05 GMT  
		Size: 35.2 MB (35227242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b119be2fb660edb1ffdd9f9660eddbd3ea4769f2056fbe4e126892709810f06`  
		Last Modified: Tue, 25 Oct 2022 09:17:01 GMT  
		Size: 12.2 KB (12239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6856d73f65d30e6a5b1045ad0a8a917ba46614fc5ed6b621442cc52da1ef177`  
		Last Modified: Tue, 25 Oct 2022 09:17:01 GMT  
		Size: 11.9 KB (11901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8beaca774f9e28447307a5b3617dcb7dd0a6cbd22b2412fc8dd40f578140886`  
		Last Modified: Tue, 25 Oct 2022 09:17:01 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9.4` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:d39db9c5bee245adab9e2d279ae85081f5e8cdc9bc4a08e8a5c1a4fa3e882b9d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64625976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45220ed124c058e72b8ca2abf28cc304b74717a1b9cec565c0a6a848f813e8c3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 12:53:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 12:53:44 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 25 Oct 2022 12:53:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 12:53:53 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 12:53:53 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 12:53:53 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 12:53:53 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 12:53:53 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 12:53:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 12:53:53 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f1749ac90bfa69003129e242051632c3420cf35e2a888329d8709010afae29`  
		Last Modified: Tue, 25 Oct 2022 12:55:02 GMT  
		Size: 4.5 MB (4494994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e8db9c3d57be2294d02966f878b5757729d88fef4b55fae953e9ccc65f19ea`  
		Last Modified: Tue, 25 Oct 2022 12:55:25 GMT  
		Size: 33.5 MB (33527297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4585677714f44662fc1cf39c8142de63850610b0b0da8f64669c90b7c7f13a4a`  
		Last Modified: Tue, 25 Oct 2022 12:55:20 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45098fb25922115244c237d7449f3919d0aecf8f3027d12ee9e210687f9b6467`  
		Last Modified: Tue, 25 Oct 2022 12:55:20 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e399d15b9ffd9d2ae5af3b9e490a75a71c00ad3e9f28d377e3e605a1e83857`  
		Last Modified: Tue, 25 Oct 2022 12:55:20 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9.4` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:5ba768bf227ccc47b78cc3beadb0386a24083ad0daf7aa352f2abe269a81bd2c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68696018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ecbe05ef389f89d2c990338329668c1d3399e360227c8a1bd077ac44988b476`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:38:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 08:38:23 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 25 Oct 2022 08:38:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 08:38:29 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 08:38:29 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 08:38:29 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 08:38:29 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 08:38:29 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 08:38:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 08:38:29 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7b3c23d0957a403636903049e3f2ee067f7db24d1189f980fc21302028781d`  
		Last Modified: Tue, 25 Oct 2022 08:39:06 GMT  
		Size: 5.2 MB (5211554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a982e14ccb4cc18d1e0c3b8f186b973be90cd4b9ef6ebe6d3afba5a81c21be68`  
		Last Modified: Tue, 25 Oct 2022 08:39:24 GMT  
		Size: 33.4 MB (33396167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eae55a830e348cd136e530df6507112153a911067fb005ffd3d1027e00af1ed`  
		Last Modified: Tue, 25 Oct 2022 08:39:21 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8b55afffb752cacfa4ee18c739e1af7166ae13a95b250fd99b9263eb165ebe`  
		Last Modified: Tue, 25 Oct 2022 08:39:20 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148a8a02094f868590e9cff0852379f15fa1731fdcca464755479278690a7bb3`  
		Last Modified: Tue, 25 Oct 2022 08:39:20 GMT  
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
$ docker pull chronograf@sha256:9934c4ad3603cc81961a93d256471b923513266b3a843833796f032609cd23f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:a97033bb97681c58bbf5b0c4b73a3f49ac3cdd5dadac6a0581298fa7a766693a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81261149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f66aad845a91f9085260f66c75a8fa648b0adc39b72a04ea5cccfcdd2d6c754c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:15:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 09:15:59 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Tue, 25 Oct 2022 09:16:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 09:16:08 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 09:16:08 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 09:16:08 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 09:16:09 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 09:16:09 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 09:16:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 09:16:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac31433f39d12daf226b0453431c2893ea68d4ca9e95016933cd0edcac586e8`  
		Last Modified: Tue, 25 Oct 2022 09:16:47 GMT  
		Size: 5.2 MB (5228634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebec2214fc5d441aae29437543b4180a09ef3f10f541850e04242bfe9809e70`  
		Last Modified: Tue, 25 Oct 2022 09:17:22 GMT  
		Size: 44.6 MB (44588085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255af7b2596c78a8a348397afef7ca5eae1fad1219b42db8eb54b50dc28439fd`  
		Last Modified: Tue, 25 Oct 2022 09:17:15 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6793fd1b24d959954f2d2acd575efdf8a9a1b9f975dbe93c398e8ce24592066`  
		Last Modified: Tue, 25 Oct 2022 09:17:15 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00e618cc14b44536304063224621d2804a0603dd5d75b7f2efe2e6d759c2638`  
		Last Modified: Tue, 25 Oct 2022 09:17:15 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:7ac31c5a43030c20f35a79c2da4bf346947c5d1e05b3e9d9445dbedfe99f229b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73563597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf8854c34693f89ab353b81801cc7a1fefaf7bf996970e7c714b3c9a56f2c12`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 12:53:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 12:54:00 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Tue, 25 Oct 2022 12:54:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 12:54:09 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 12:54:09 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 12:54:09 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 12:54:09 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 12:54:10 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 12:54:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 12:54:10 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f1749ac90bfa69003129e242051632c3420cf35e2a888329d8709010afae29`  
		Last Modified: Tue, 25 Oct 2022 12:55:02 GMT  
		Size: 4.5 MB (4494994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fc4ff7d1f4516f3810e6354425d49541ff9ad663d48c35410d514b836a5da1`  
		Last Modified: Tue, 25 Oct 2022 12:55:45 GMT  
		Size: 42.5 MB (42464917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df95d9ae6a19b1e1e9cb18c93597ce98317251569f5cd855d4af3606f9a2dc4e`  
		Last Modified: Tue, 25 Oct 2022 12:55:37 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494ef46291b2362156ed0fe658a1f43b2950377c3f62d0623cf215d2175e6be6`  
		Last Modified: Tue, 25 Oct 2022 12:55:37 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94a2368587118a72f6f1ca4a4ccb2a0179f7e77af6da9e20954e4dc88fa5989`  
		Last Modified: Tue, 25 Oct 2022 12:55:37 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:c9ad1548053c5343bef238546bc24b2f5b9d164772c869d7883dab79764397f2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.9 MB (77917795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:621b8643698227f3e041ea9e759c2604049932d25e024fadef21fdd064f8b36c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:38:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 25 Oct 2022 08:38:31 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Tue, 25 Oct 2022 08:38:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 08:38:38 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 25 Oct 2022 08:38:38 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 25 Oct 2022 08:38:38 GMT
EXPOSE 8888
# Tue, 25 Oct 2022 08:38:38 GMT
VOLUME [/var/lib/chronograf]
# Tue, 25 Oct 2022 08:38:39 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 25 Oct 2022 08:38:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 08:38:39 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7b3c23d0957a403636903049e3f2ee067f7db24d1189f980fc21302028781d`  
		Last Modified: Tue, 25 Oct 2022 08:39:06 GMT  
		Size: 5.2 MB (5211554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa58d779a4fb96cfe4fc04d985e65f4fdaa11560a21388a1b4fbca05931841db`  
		Last Modified: Tue, 25 Oct 2022 08:39:38 GMT  
		Size: 42.6 MB (42617940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452d6327993901bdf4ebf07f7a49a37a88e2d07f288d80cf37c0206f47ec24c1`  
		Last Modified: Tue, 25 Oct 2022 08:39:33 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5d48b03794eeb85fbb87600d45cb4c9ff690ef4782885d5487aa069e408bdd`  
		Last Modified: Tue, 25 Oct 2022 08:39:33 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77c39d0ee6b7fa8173fc740ad5e236d2fe3e9c533931d20aaeabcdf360286ee`  
		Last Modified: Tue, 25 Oct 2022 08:39:33 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
