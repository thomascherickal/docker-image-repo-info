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
$ docker pull chronograf@sha256:2bebf820b10d130d2f9951a7ac0ff3b79eb55ea42d831bc6a828430893cef354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6` - linux; amd64

```console
$ docker pull chronograf@sha256:93f47a1cbb8c6d0280a105d82da3f08c16dbd594c0f83f755ab9a6de125ac5e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49398093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b50e92ef46146f03f27e63a296e018c488235b060c70322a76547b785ee22249`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:48 GMT
ADD file:9fc739b295073dd1d9293d2ea8106e21156de790c82a9d19be210c0c63bfb527 in / 
# Thu, 17 Mar 2022 04:06:48 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:38:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Mar 2022 08:38:22 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Thu, 17 Mar 2022 08:38:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Mar 2022 08:38:30 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Mar 2022 08:38:31 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Mar 2022 08:38:31 GMT
EXPOSE 8888
# Thu, 17 Mar 2022 08:38:31 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Mar 2022 08:38:31 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 17 Mar 2022 08:38:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 08:38:31 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:5d9da879a61c05a35520eabaa04d22b4867d0cf84a91f4c7b078128e1c820ce5`  
		Last Modified: Thu, 17 Mar 2022 04:14:03 GMT  
		Size: 22.6 MB (22567740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964f48dfa9fa2029216316deab45629f6c3afbc5021d72278ae08424dd0774b0`  
		Last Modified: Thu, 17 Mar 2022 08:40:28 GMT  
		Size: 6.8 MB (6760337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720123d698908d3e60989ef3cfe84d0c107ec7145b33009d067b420bd45f2ee2`  
		Last Modified: Thu, 17 Mar 2022 08:40:30 GMT  
		Size: 20.0 MB (20045618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa28a36515fe8774f75f7786b2b5c40633a4c6ba62dfa2da92eeb02c0e26eec3`  
		Last Modified: Thu, 17 Mar 2022 08:40:26 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d20de19d9d79907dedb1c3aa3c0494ff3db6e315756997f058b8824deb9735`  
		Last Modified: Thu, 17 Mar 2022 08:40:27 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed760e0aae03c7d7dfcb33f876744360ae56125660c9b220ba0b5d1c160b70a`  
		Last Modified: Thu, 17 Mar 2022 08:40:26 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:ca67d0da2960fafcc5387eecb839bebfffee733a59a43985d83be71a37f69232
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43944436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07a2a886019d887e27b55f5dfcadb2a94e3f8cbf5d82fec5b837385b0da55459`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 01 Mar 2022 02:09:29 GMT
ADD file:b573bfb75b0df3ee547a99ec724d80518fbba40b260dadfe30467b24057bb391 in / 
# Tue, 01 Mar 2022 02:09:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:04:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 01 Mar 2022 10:04:32 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 01 Mar 2022 10:04:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 01 Mar 2022 10:04:50 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 01 Mar 2022 10:04:50 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 01 Mar 2022 10:04:51 GMT
EXPOSE 8888
# Tue, 01 Mar 2022 10:04:51 GMT
VOLUME [/var/lib/chronograf]
# Tue, 01 Mar 2022 10:04:52 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 01 Mar 2022 10:04:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 01 Mar 2022 10:04:53 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:52aa216cc1f7f3b5d4ed3b10d96ffe1a02174398f1c9377415eb8bb643cb1782`  
		Last Modified: Tue, 01 Mar 2022 02:26:16 GMT  
		Size: 19.3 MB (19318791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804bc2cf457bc72a961a14f07cfde54ad58d9c46bb9b0fa52c8e07da4b6992cb`  
		Last Modified: Tue, 01 Mar 2022 10:08:06 GMT  
		Size: 5.8 MB (5780607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489b62ec6d99aa18b81f84e11c2af6760f5c06836586f3497983cb0209ee60e`  
		Last Modified: Tue, 01 Mar 2022 10:08:16 GMT  
		Size: 18.8 MB (18820650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b33b57f9d84a3499ab2921b9df284edf09df8424f034330b8adb5ebba743a5`  
		Last Modified: Tue, 01 Mar 2022 10:08:03 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce87c3544037c851ce587fdcffd2d69919b20f73632bee4b3dd4e303f6ff017`  
		Last Modified: Tue, 01 Mar 2022 10:08:03 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c6ef4db66d25bba4dcf41abe3234325eead6f3419138bbfd135d5b130416ff`  
		Last Modified: Tue, 01 Mar 2022 10:08:03 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:3efcd27fad0b1d1c691abf60c5db33e54a2851e556839c5ffdddad6454520d53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45456978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a792c808ec8ba2d16916eec975edf492ce240e66b18509a5c7a3333c2eba4dd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:16 GMT
ADD file:9d9c04bf28d7e6075270ca8a75c01a6d4015bc3eccc4812a82681a7fabf27027 in / 
# Thu, 17 Mar 2022 03:24:17 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:26:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Mar 2022 22:26:57 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Thu, 17 Mar 2022 22:27:04 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Mar 2022 22:27:06 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Mar 2022 22:27:07 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Mar 2022 22:27:07 GMT
EXPOSE 8888
# Thu, 17 Mar 2022 22:27:08 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Mar 2022 22:27:10 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 17 Mar 2022 22:27:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 22:27:11 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:ecb1e7e01fa06e43b3018b38895366ba643cbac6d46bce566be2aa1cf10abf48`  
		Last Modified: Thu, 17 Mar 2022 03:32:58 GMT  
		Size: 20.4 MB (20423817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdcc9ed8b864108c2f441d508e2349d88968c42f8446c04f18fb121e256bd9bb`  
		Last Modified: Thu, 17 Mar 2022 22:29:15 GMT  
		Size: 6.0 MB (6047145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49eb31bf8b92102afa0e9611d2127d24ba5d02a40d548d28d1fe63a56123c15`  
		Last Modified: Thu, 17 Mar 2022 22:29:17 GMT  
		Size: 19.0 MB (18961619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f0f56891e4dd9e5e2e04eefbfd4ab2db58b05a943764ea37b56c31b26d145e`  
		Last Modified: Thu, 17 Mar 2022 22:29:14 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e96f6a5814fd550c73b8f71ce07cff189d58c91084604bd5489b31cbcbd15a`  
		Last Modified: Thu, 17 Mar 2022 22:29:14 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e990ea0aab83a77e2dc2e2b7d9b9340424377aff0f41590a752dfab868ea17`  
		Last Modified: Thu, 17 Mar 2022 22:29:14 GMT  
		Size: 240.0 B  
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
$ docker pull chronograf@sha256:2bebf820b10d130d2f9951a7ac0ff3b79eb55ea42d831bc6a828430893cef354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6.2` - linux; amd64

```console
$ docker pull chronograf@sha256:93f47a1cbb8c6d0280a105d82da3f08c16dbd594c0f83f755ab9a6de125ac5e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49398093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b50e92ef46146f03f27e63a296e018c488235b060c70322a76547b785ee22249`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:48 GMT
ADD file:9fc739b295073dd1d9293d2ea8106e21156de790c82a9d19be210c0c63bfb527 in / 
# Thu, 17 Mar 2022 04:06:48 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:38:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Mar 2022 08:38:22 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Thu, 17 Mar 2022 08:38:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Mar 2022 08:38:30 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Mar 2022 08:38:31 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Mar 2022 08:38:31 GMT
EXPOSE 8888
# Thu, 17 Mar 2022 08:38:31 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Mar 2022 08:38:31 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 17 Mar 2022 08:38:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 08:38:31 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:5d9da879a61c05a35520eabaa04d22b4867d0cf84a91f4c7b078128e1c820ce5`  
		Last Modified: Thu, 17 Mar 2022 04:14:03 GMT  
		Size: 22.6 MB (22567740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964f48dfa9fa2029216316deab45629f6c3afbc5021d72278ae08424dd0774b0`  
		Last Modified: Thu, 17 Mar 2022 08:40:28 GMT  
		Size: 6.8 MB (6760337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720123d698908d3e60989ef3cfe84d0c107ec7145b33009d067b420bd45f2ee2`  
		Last Modified: Thu, 17 Mar 2022 08:40:30 GMT  
		Size: 20.0 MB (20045618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa28a36515fe8774f75f7786b2b5c40633a4c6ba62dfa2da92eeb02c0e26eec3`  
		Last Modified: Thu, 17 Mar 2022 08:40:26 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d20de19d9d79907dedb1c3aa3c0494ff3db6e315756997f058b8824deb9735`  
		Last Modified: Thu, 17 Mar 2022 08:40:27 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed760e0aae03c7d7dfcb33f876744360ae56125660c9b220ba0b5d1c160b70a`  
		Last Modified: Thu, 17 Mar 2022 08:40:26 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:ca67d0da2960fafcc5387eecb839bebfffee733a59a43985d83be71a37f69232
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43944436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07a2a886019d887e27b55f5dfcadb2a94e3f8cbf5d82fec5b837385b0da55459`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 01 Mar 2022 02:09:29 GMT
ADD file:b573bfb75b0df3ee547a99ec724d80518fbba40b260dadfe30467b24057bb391 in / 
# Tue, 01 Mar 2022 02:09:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:04:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 01 Mar 2022 10:04:32 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 01 Mar 2022 10:04:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 01 Mar 2022 10:04:50 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 01 Mar 2022 10:04:50 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 01 Mar 2022 10:04:51 GMT
EXPOSE 8888
# Tue, 01 Mar 2022 10:04:51 GMT
VOLUME [/var/lib/chronograf]
# Tue, 01 Mar 2022 10:04:52 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 01 Mar 2022 10:04:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 01 Mar 2022 10:04:53 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:52aa216cc1f7f3b5d4ed3b10d96ffe1a02174398f1c9377415eb8bb643cb1782`  
		Last Modified: Tue, 01 Mar 2022 02:26:16 GMT  
		Size: 19.3 MB (19318791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804bc2cf457bc72a961a14f07cfde54ad58d9c46bb9b0fa52c8e07da4b6992cb`  
		Last Modified: Tue, 01 Mar 2022 10:08:06 GMT  
		Size: 5.8 MB (5780607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489b62ec6d99aa18b81f84e11c2af6760f5c06836586f3497983cb0209ee60e`  
		Last Modified: Tue, 01 Mar 2022 10:08:16 GMT  
		Size: 18.8 MB (18820650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b33b57f9d84a3499ab2921b9df284edf09df8424f034330b8adb5ebba743a5`  
		Last Modified: Tue, 01 Mar 2022 10:08:03 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce87c3544037c851ce587fdcffd2d69919b20f73632bee4b3dd4e303f6ff017`  
		Last Modified: Tue, 01 Mar 2022 10:08:03 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c6ef4db66d25bba4dcf41abe3234325eead6f3419138bbfd135d5b130416ff`  
		Last Modified: Tue, 01 Mar 2022 10:08:03 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:3efcd27fad0b1d1c691abf60c5db33e54a2851e556839c5ffdddad6454520d53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45456978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a792c808ec8ba2d16916eec975edf492ce240e66b18509a5c7a3333c2eba4dd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:16 GMT
ADD file:9d9c04bf28d7e6075270ca8a75c01a6d4015bc3eccc4812a82681a7fabf27027 in / 
# Thu, 17 Mar 2022 03:24:17 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:26:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Mar 2022 22:26:57 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Thu, 17 Mar 2022 22:27:04 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Mar 2022 22:27:06 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Mar 2022 22:27:07 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Mar 2022 22:27:07 GMT
EXPOSE 8888
# Thu, 17 Mar 2022 22:27:08 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Mar 2022 22:27:10 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 17 Mar 2022 22:27:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 22:27:11 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:ecb1e7e01fa06e43b3018b38895366ba643cbac6d46bce566be2aa1cf10abf48`  
		Last Modified: Thu, 17 Mar 2022 03:32:58 GMT  
		Size: 20.4 MB (20423817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdcc9ed8b864108c2f441d508e2349d88968c42f8446c04f18fb121e256bd9bb`  
		Last Modified: Thu, 17 Mar 2022 22:29:15 GMT  
		Size: 6.0 MB (6047145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49eb31bf8b92102afa0e9611d2127d24ba5d02a40d548d28d1fe63a56123c15`  
		Last Modified: Thu, 17 Mar 2022 22:29:17 GMT  
		Size: 19.0 MB (18961619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f0f56891e4dd9e5e2e04eefbfd4ab2db58b05a943764ea37b56c31b26d145e`  
		Last Modified: Thu, 17 Mar 2022 22:29:14 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e96f6a5814fd550c73b8f71ce07cff189d58c91084604bd5489b31cbcbd15a`  
		Last Modified: Thu, 17 Mar 2022 22:29:14 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e990ea0aab83a77e2dc2e2b7d9b9340424377aff0f41590a752dfab868ea17`  
		Last Modified: Thu, 17 Mar 2022 22:29:14 GMT  
		Size: 240.0 B  
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
$ docker pull chronograf@sha256:d780f945edf21f568aeabc5bb12cfa9b2e574e8f4d3b32a95692e645ab8201e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7` - linux; amd64

```console
$ docker pull chronograf@sha256:ac2e6b46c9ee9427253ba61e75c7d4958aa3f2e1203674c83b62e09f5e5ab66e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65427515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e4e41c259365180de65f434878ea9288fc959b07737d4fc59184f084ef2f6be`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:48 GMT
ADD file:9fc739b295073dd1d9293d2ea8106e21156de790c82a9d19be210c0c63bfb527 in / 
# Thu, 17 Mar 2022 04:06:48 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:39:21 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Mar 2022 08:39:21 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 17 Mar 2022 08:39:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Mar 2022 08:39:32 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Mar 2022 08:39:32 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Mar 2022 08:39:32 GMT
EXPOSE 8888
# Thu, 17 Mar 2022 08:39:33 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Mar 2022 08:39:33 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 17 Mar 2022 08:39:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 08:39:33 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:5d9da879a61c05a35520eabaa04d22b4867d0cf84a91f4c7b078128e1c820ce5`  
		Last Modified: Thu, 17 Mar 2022 04:14:03 GMT  
		Size: 22.6 MB (22567740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0be2fb68be12739fe6fae16faf55148e9959d78683503adcca5929815df1a83`  
		Last Modified: Thu, 17 Mar 2022 08:40:42 GMT  
		Size: 4.5 MB (4506805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c3593347da1932911bccf1dc271e1cf2719319c5c1a0537b72564f0310cc7d`  
		Last Modified: Thu, 17 Mar 2022 08:40:47 GMT  
		Size: 38.3 MB (38328573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a2d8a1f30cc86cfd9dde2f4513fa66883f64f0f7c68a4ea6c21ecb4bd3b11e`  
		Last Modified: Thu, 17 Mar 2022 08:40:41 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecdfbe73fc67ee76cc610c7e1ab4812943cdd5c9b082942d2d2154b38f1db8f7`  
		Last Modified: Thu, 17 Mar 2022 08:40:41 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a55f867bbe20ef4e91e10dc00738edae0eeaebfff2490acbcc9b10f211596fc`  
		Last Modified: Thu, 17 Mar 2022 08:40:41 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:b2d4fa7fc7605e82d1c6679df49e8039b1c91a721647c65570fb0f035a027b80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (59006662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2fa00feceb0f782bd399e34f392c1d6e875c46701ded1ba96d3d2405ff02f14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 01 Mar 2022 02:09:29 GMT
ADD file:b573bfb75b0df3ee547a99ec724d80518fbba40b260dadfe30467b24057bb391 in / 
# Tue, 01 Mar 2022 02:09:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:05:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 01 Mar 2022 10:05:28 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 01 Mar 2022 10:05:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 01 Mar 2022 10:06:00 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 01 Mar 2022 10:06:00 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 01 Mar 2022 10:06:01 GMT
EXPOSE 8888
# Tue, 01 Mar 2022 10:06:01 GMT
VOLUME [/var/lib/chronograf]
# Tue, 01 Mar 2022 10:06:02 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 01 Mar 2022 10:06:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 01 Mar 2022 10:06:03 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:52aa216cc1f7f3b5d4ed3b10d96ffe1a02174398f1c9377415eb8bb643cb1782`  
		Last Modified: Tue, 01 Mar 2022 02:26:16 GMT  
		Size: 19.3 MB (19318791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3780784cb49aad0fe1dbc7f8d01c303a2bb833295040e0f9ede56a3f6f8e87`  
		Last Modified: Tue, 01 Mar 2022 10:08:29 GMT  
		Size: 3.9 MB (3879915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940c0e107d590e741e9cec31a40b88082d14cc24fa14cfa989f3cc6378265bbb`  
		Last Modified: Tue, 01 Mar 2022 10:08:47 GMT  
		Size: 35.8 MB (35783567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50eab8f59e545d679308edd574fa8a448bce8dc5b5e4594a9c917b7295ee075d`  
		Last Modified: Tue, 01 Mar 2022 10:08:27 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c431d2c0bcb6b54ba135dafbbd6ebeee7f95aea46598536f573aa5eb0f411b`  
		Last Modified: Tue, 01 Mar 2022 10:08:27 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88ffdc38b6de7876641a0bab1fdbfc11d07b3e9b472d45fb8c37fd8d50dc28b`  
		Last Modified: Tue, 01 Mar 2022 10:08:27 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:09e246219d0264d911a92ad0be54203fafc940702d62047c675f9f7dc290e9e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60329425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b05e26649361353c66ad71e26220aa0497937d3c2a8d29943cba4d8485c8dba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:16 GMT
ADD file:9d9c04bf28d7e6075270ca8a75c01a6d4015bc3eccc4812a82681a7fabf27027 in / 
# Thu, 17 Mar 2022 03:24:17 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:27:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Mar 2022 22:27:44 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 17 Mar 2022 22:27:56 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Mar 2022 22:27:57 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Mar 2022 22:27:58 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Mar 2022 22:27:58 GMT
EXPOSE 8888
# Thu, 17 Mar 2022 22:27:59 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Mar 2022 22:28:01 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 17 Mar 2022 22:28:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 22:28:02 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:ecb1e7e01fa06e43b3018b38895366ba643cbac6d46bce566be2aa1cf10abf48`  
		Last Modified: Thu, 17 Mar 2022 03:32:58 GMT  
		Size: 20.4 MB (20423817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c7e6a48dd13c5836b8b218a8372a493902f5c1fd57da5fd955912922b08908`  
		Last Modified: Thu, 17 Mar 2022 22:29:29 GMT  
		Size: 3.9 MB (3893978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee03b87db2ef7df6d347aa7fece6d1b742b3f04cc4326f790b492a35aba5ff3`  
		Last Modified: Thu, 17 Mar 2022 22:29:33 GMT  
		Size: 36.0 MB (35987238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26efabf26d8cda661366200eba61be6c70512fcb3a4b7075d8c246ae611cdb10`  
		Last Modified: Thu, 17 Mar 2022 22:29:28 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b4caa4fa7d35196b80ace1472f74b19ae694593e76f96317a47d711e50e227`  
		Last Modified: Thu, 17 Mar 2022 22:29:28 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24cb8978df300b2aaeecac468d0fc67f633057f78f17560b1cb51b90eab15205`  
		Last Modified: Thu, 17 Mar 2022 22:29:28 GMT  
		Size: 239.0 B  
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
$ docker pull chronograf@sha256:d780f945edf21f568aeabc5bb12cfa9b2e574e8f4d3b32a95692e645ab8201e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7.17` - linux; amd64

```console
$ docker pull chronograf@sha256:ac2e6b46c9ee9427253ba61e75c7d4958aa3f2e1203674c83b62e09f5e5ab66e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65427515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e4e41c259365180de65f434878ea9288fc959b07737d4fc59184f084ef2f6be`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:48 GMT
ADD file:9fc739b295073dd1d9293d2ea8106e21156de790c82a9d19be210c0c63bfb527 in / 
# Thu, 17 Mar 2022 04:06:48 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:39:21 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Mar 2022 08:39:21 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 17 Mar 2022 08:39:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Mar 2022 08:39:32 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Mar 2022 08:39:32 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Mar 2022 08:39:32 GMT
EXPOSE 8888
# Thu, 17 Mar 2022 08:39:33 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Mar 2022 08:39:33 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 17 Mar 2022 08:39:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 08:39:33 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:5d9da879a61c05a35520eabaa04d22b4867d0cf84a91f4c7b078128e1c820ce5`  
		Last Modified: Thu, 17 Mar 2022 04:14:03 GMT  
		Size: 22.6 MB (22567740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0be2fb68be12739fe6fae16faf55148e9959d78683503adcca5929815df1a83`  
		Last Modified: Thu, 17 Mar 2022 08:40:42 GMT  
		Size: 4.5 MB (4506805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c3593347da1932911bccf1dc271e1cf2719319c5c1a0537b72564f0310cc7d`  
		Last Modified: Thu, 17 Mar 2022 08:40:47 GMT  
		Size: 38.3 MB (38328573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a2d8a1f30cc86cfd9dde2f4513fa66883f64f0f7c68a4ea6c21ecb4bd3b11e`  
		Last Modified: Thu, 17 Mar 2022 08:40:41 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecdfbe73fc67ee76cc610c7e1ab4812943cdd5c9b082942d2d2154b38f1db8f7`  
		Last Modified: Thu, 17 Mar 2022 08:40:41 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a55f867bbe20ef4e91e10dc00738edae0eeaebfff2490acbcc9b10f211596fc`  
		Last Modified: Thu, 17 Mar 2022 08:40:41 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:b2d4fa7fc7605e82d1c6679df49e8039b1c91a721647c65570fb0f035a027b80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (59006662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2fa00feceb0f782bd399e34f392c1d6e875c46701ded1ba96d3d2405ff02f14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 01 Mar 2022 02:09:29 GMT
ADD file:b573bfb75b0df3ee547a99ec724d80518fbba40b260dadfe30467b24057bb391 in / 
# Tue, 01 Mar 2022 02:09:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:05:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 01 Mar 2022 10:05:28 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 01 Mar 2022 10:05:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 01 Mar 2022 10:06:00 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 01 Mar 2022 10:06:00 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 01 Mar 2022 10:06:01 GMT
EXPOSE 8888
# Tue, 01 Mar 2022 10:06:01 GMT
VOLUME [/var/lib/chronograf]
# Tue, 01 Mar 2022 10:06:02 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 01 Mar 2022 10:06:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 01 Mar 2022 10:06:03 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:52aa216cc1f7f3b5d4ed3b10d96ffe1a02174398f1c9377415eb8bb643cb1782`  
		Last Modified: Tue, 01 Mar 2022 02:26:16 GMT  
		Size: 19.3 MB (19318791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3780784cb49aad0fe1dbc7f8d01c303a2bb833295040e0f9ede56a3f6f8e87`  
		Last Modified: Tue, 01 Mar 2022 10:08:29 GMT  
		Size: 3.9 MB (3879915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940c0e107d590e741e9cec31a40b88082d14cc24fa14cfa989f3cc6378265bbb`  
		Last Modified: Tue, 01 Mar 2022 10:08:47 GMT  
		Size: 35.8 MB (35783567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50eab8f59e545d679308edd574fa8a448bce8dc5b5e4594a9c917b7295ee075d`  
		Last Modified: Tue, 01 Mar 2022 10:08:27 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c431d2c0bcb6b54ba135dafbbd6ebeee7f95aea46598536f573aa5eb0f411b`  
		Last Modified: Tue, 01 Mar 2022 10:08:27 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88ffdc38b6de7876641a0bab1fdbfc11d07b3e9b472d45fb8c37fd8d50dc28b`  
		Last Modified: Tue, 01 Mar 2022 10:08:27 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:09e246219d0264d911a92ad0be54203fafc940702d62047c675f9f7dc290e9e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60329425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b05e26649361353c66ad71e26220aa0497937d3c2a8d29943cba4d8485c8dba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:16 GMT
ADD file:9d9c04bf28d7e6075270ca8a75c01a6d4015bc3eccc4812a82681a7fabf27027 in / 
# Thu, 17 Mar 2022 03:24:17 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:27:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Mar 2022 22:27:44 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 17 Mar 2022 22:27:56 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Mar 2022 22:27:57 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Mar 2022 22:27:58 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Mar 2022 22:27:58 GMT
EXPOSE 8888
# Thu, 17 Mar 2022 22:27:59 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Mar 2022 22:28:01 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 17 Mar 2022 22:28:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 22:28:02 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:ecb1e7e01fa06e43b3018b38895366ba643cbac6d46bce566be2aa1cf10abf48`  
		Last Modified: Thu, 17 Mar 2022 03:32:58 GMT  
		Size: 20.4 MB (20423817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c7e6a48dd13c5836b8b218a8372a493902f5c1fd57da5fd955912922b08908`  
		Last Modified: Thu, 17 Mar 2022 22:29:29 GMT  
		Size: 3.9 MB (3893978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee03b87db2ef7df6d347aa7fece6d1b742b3f04cc4326f790b492a35aba5ff3`  
		Last Modified: Thu, 17 Mar 2022 22:29:33 GMT  
		Size: 36.0 MB (35987238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26efabf26d8cda661366200eba61be6c70512fcb3a4b7075d8c246ae611cdb10`  
		Last Modified: Thu, 17 Mar 2022 22:29:28 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b4caa4fa7d35196b80ace1472f74b19ae694593e76f96317a47d711e50e227`  
		Last Modified: Thu, 17 Mar 2022 22:29:28 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24cb8978df300b2aaeecac468d0fc67f633057f78f17560b1cb51b90eab15205`  
		Last Modified: Thu, 17 Mar 2022 22:29:28 GMT  
		Size: 239.0 B  
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
$ docker pull chronograf@sha256:1f5b1967776b2070604cd58bde61c1369f117c792cdc131abd97c6cb404f6427
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8` - linux; amd64

```console
$ docker pull chronograf@sha256:71720adff754f47be799c56494fd8e15eb2fda0f58fac358b2f5a8c84f035c6a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66279024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70ddb8df4a909d55e224c1f58d665520efb4de5f348d75aa9a8d80aa4610020a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:48 GMT
ADD file:9fc739b295073dd1d9293d2ea8106e21156de790c82a9d19be210c0c63bfb527 in / 
# Thu, 17 Mar 2022 04:06:48 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:38:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Mar 2022 08:39:38 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Thu, 17 Mar 2022 08:39:46 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Mar 2022 08:39:46 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Mar 2022 08:39:46 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Mar 2022 08:39:46 GMT
EXPOSE 8888
# Thu, 17 Mar 2022 08:39:46 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Mar 2022 08:39:46 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 17 Mar 2022 08:39:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 08:39:46 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:5d9da879a61c05a35520eabaa04d22b4867d0cf84a91f4c7b078128e1c820ce5`  
		Last Modified: Thu, 17 Mar 2022 04:14:03 GMT  
		Size: 22.6 MB (22567740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964f48dfa9fa2029216316deab45629f6c3afbc5021d72278ae08424dd0774b0`  
		Last Modified: Thu, 17 Mar 2022 08:40:28 GMT  
		Size: 6.8 MB (6760337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0628cff5565c1b1d727f5fb38edc6a84c913e1937bd7f4859e77e54b35d42d`  
		Last Modified: Thu, 17 Mar 2022 08:41:03 GMT  
		Size: 36.9 MB (36926565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2342aa887107fc7ca17bfbab46a2f800ceace0f64399cd9c4fa0c005ec7f3897`  
		Last Modified: Thu, 17 Mar 2022 08:40:58 GMT  
		Size: 12.2 KB (12242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e69d5532f76bba0cc882567ce4e49ae883248b1a3b236ce63464ee892d90d6`  
		Last Modified: Thu, 17 Mar 2022 08:40:58 GMT  
		Size: 11.9 KB (11901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b4060dfa2d51e4e395bd3c6ac9e6aa088edd5fa71ceabd978ce37d2067f8c8`  
		Last Modified: Thu, 17 Mar 2022 08:40:58 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:81bfeb0de95820d96ac126ca8e9add2acc9798e8fc54498759a2a662aa77f2ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59635548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50fdd4424c8f9b086989003723a8bd20371b0706fb3a94fdf657b647afeb0178`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 01 Mar 2022 02:09:29 GMT
ADD file:b573bfb75b0df3ee547a99ec724d80518fbba40b260dadfe30467b24057bb391 in / 
# Tue, 01 Mar 2022 02:09:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:04:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 01 Mar 2022 10:06:14 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 01 Mar 2022 10:06:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 01 Mar 2022 10:06:34 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 01 Mar 2022 10:06:34 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 01 Mar 2022 10:06:35 GMT
EXPOSE 8888
# Tue, 01 Mar 2022 10:06:35 GMT
VOLUME [/var/lib/chronograf]
# Tue, 01 Mar 2022 10:06:35 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 01 Mar 2022 10:06:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 01 Mar 2022 10:06:36 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:52aa216cc1f7f3b5d4ed3b10d96ffe1a02174398f1c9377415eb8bb643cb1782`  
		Last Modified: Tue, 01 Mar 2022 02:26:16 GMT  
		Size: 19.3 MB (19318791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804bc2cf457bc72a961a14f07cfde54ad58d9c46bb9b0fa52c8e07da4b6992cb`  
		Last Modified: Tue, 01 Mar 2022 10:08:06 GMT  
		Size: 5.8 MB (5780607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5faa490c5ab86facefc403661b2874d326cc17c30c13325fd769f168cfaa3f63`  
		Last Modified: Tue, 01 Mar 2022 10:09:16 GMT  
		Size: 34.5 MB (34511760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4e051a82252250932dee03e0a91939bc46d82607c01ce7893a37fc11cd7e4a`  
		Last Modified: Tue, 01 Mar 2022 10:08:59 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696140bbfdb5f96d16627cacd520a6c810c11a67d205ca033fa46722dbacb14b`  
		Last Modified: Tue, 01 Mar 2022 10:08:59 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1484460688916c633d88bcb2fe76d2cc9cfc8b6c83279cafbab8ad01fedcdd`  
		Last Modified: Tue, 01 Mar 2022 10:08:59 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:f4419f7c07ad710f862ede3620c211660b54f7a853b8ba1e49111ffffec60522
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.9 MB (60926992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e198a1d504a269c573cbb65153cf66b357f2bbb8819c47ac787875f47f4205c7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:16 GMT
ADD file:9d9c04bf28d7e6075270ca8a75c01a6d4015bc3eccc4812a82681a7fabf27027 in / 
# Thu, 17 Mar 2022 03:24:17 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:26:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Mar 2022 22:28:12 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Thu, 17 Mar 2022 22:28:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Mar 2022 22:28:22 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Mar 2022 22:28:23 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Mar 2022 22:28:23 GMT
EXPOSE 8888
# Thu, 17 Mar 2022 22:28:24 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Mar 2022 22:28:26 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 17 Mar 2022 22:28:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 22:28:27 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:ecb1e7e01fa06e43b3018b38895366ba643cbac6d46bce566be2aa1cf10abf48`  
		Last Modified: Thu, 17 Mar 2022 03:32:58 GMT  
		Size: 20.4 MB (20423817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdcc9ed8b864108c2f441d508e2349d88968c42f8446c04f18fb121e256bd9bb`  
		Last Modified: Thu, 17 Mar 2022 22:29:15 GMT  
		Size: 6.0 MB (6047145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feff8b25ef2859d6d5baa4cb27318419efe784820857970e2fcefc8ecceb4c92`  
		Last Modified: Thu, 17 Mar 2022 22:29:49 GMT  
		Size: 34.4 MB (34431638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d273285d82262d4299a0d4651c5e0afc50c7b84b6a692198d79215a6d7b5dbd8`  
		Last Modified: Thu, 17 Mar 2022 22:29:44 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9871739638ffdb446fc0ffec3c5269a1872cc3255467e1be724299bbef9813e1`  
		Last Modified: Thu, 17 Mar 2022 22:29:44 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2450f64c0a194bb55a966b877ba08cbbdbf5b1421237c417b0e87bd41c32acc9`  
		Last Modified: Thu, 17 Mar 2022 22:29:44 GMT  
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
$ docker pull chronograf@sha256:1f5b1967776b2070604cd58bde61c1369f117c792cdc131abd97c6cb404f6427
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8.10` - linux; amd64

```console
$ docker pull chronograf@sha256:71720adff754f47be799c56494fd8e15eb2fda0f58fac358b2f5a8c84f035c6a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66279024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70ddb8df4a909d55e224c1f58d665520efb4de5f348d75aa9a8d80aa4610020a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:48 GMT
ADD file:9fc739b295073dd1d9293d2ea8106e21156de790c82a9d19be210c0c63bfb527 in / 
# Thu, 17 Mar 2022 04:06:48 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:38:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Mar 2022 08:39:38 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Thu, 17 Mar 2022 08:39:46 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Mar 2022 08:39:46 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Mar 2022 08:39:46 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Mar 2022 08:39:46 GMT
EXPOSE 8888
# Thu, 17 Mar 2022 08:39:46 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Mar 2022 08:39:46 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 17 Mar 2022 08:39:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 08:39:46 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:5d9da879a61c05a35520eabaa04d22b4867d0cf84a91f4c7b078128e1c820ce5`  
		Last Modified: Thu, 17 Mar 2022 04:14:03 GMT  
		Size: 22.6 MB (22567740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964f48dfa9fa2029216316deab45629f6c3afbc5021d72278ae08424dd0774b0`  
		Last Modified: Thu, 17 Mar 2022 08:40:28 GMT  
		Size: 6.8 MB (6760337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0628cff5565c1b1d727f5fb38edc6a84c913e1937bd7f4859e77e54b35d42d`  
		Last Modified: Thu, 17 Mar 2022 08:41:03 GMT  
		Size: 36.9 MB (36926565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2342aa887107fc7ca17bfbab46a2f800ceace0f64399cd9c4fa0c005ec7f3897`  
		Last Modified: Thu, 17 Mar 2022 08:40:58 GMT  
		Size: 12.2 KB (12242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e69d5532f76bba0cc882567ce4e49ae883248b1a3b236ce63464ee892d90d6`  
		Last Modified: Thu, 17 Mar 2022 08:40:58 GMT  
		Size: 11.9 KB (11901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b4060dfa2d51e4e395bd3c6ac9e6aa088edd5fa71ceabd978ce37d2067f8c8`  
		Last Modified: Thu, 17 Mar 2022 08:40:58 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.10` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:81bfeb0de95820d96ac126ca8e9add2acc9798e8fc54498759a2a662aa77f2ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59635548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50fdd4424c8f9b086989003723a8bd20371b0706fb3a94fdf657b647afeb0178`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 01 Mar 2022 02:09:29 GMT
ADD file:b573bfb75b0df3ee547a99ec724d80518fbba40b260dadfe30467b24057bb391 in / 
# Tue, 01 Mar 2022 02:09:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:04:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 01 Mar 2022 10:06:14 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 01 Mar 2022 10:06:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 01 Mar 2022 10:06:34 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 01 Mar 2022 10:06:34 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 01 Mar 2022 10:06:35 GMT
EXPOSE 8888
# Tue, 01 Mar 2022 10:06:35 GMT
VOLUME [/var/lib/chronograf]
# Tue, 01 Mar 2022 10:06:35 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 01 Mar 2022 10:06:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 01 Mar 2022 10:06:36 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:52aa216cc1f7f3b5d4ed3b10d96ffe1a02174398f1c9377415eb8bb643cb1782`  
		Last Modified: Tue, 01 Mar 2022 02:26:16 GMT  
		Size: 19.3 MB (19318791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804bc2cf457bc72a961a14f07cfde54ad58d9c46bb9b0fa52c8e07da4b6992cb`  
		Last Modified: Tue, 01 Mar 2022 10:08:06 GMT  
		Size: 5.8 MB (5780607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5faa490c5ab86facefc403661b2874d326cc17c30c13325fd769f168cfaa3f63`  
		Last Modified: Tue, 01 Mar 2022 10:09:16 GMT  
		Size: 34.5 MB (34511760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4e051a82252250932dee03e0a91939bc46d82607c01ce7893a37fc11cd7e4a`  
		Last Modified: Tue, 01 Mar 2022 10:08:59 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696140bbfdb5f96d16627cacd520a6c810c11a67d205ca033fa46722dbacb14b`  
		Last Modified: Tue, 01 Mar 2022 10:08:59 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1484460688916c633d88bcb2fe76d2cc9cfc8b6c83279cafbab8ad01fedcdd`  
		Last Modified: Tue, 01 Mar 2022 10:08:59 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.10` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:f4419f7c07ad710f862ede3620c211660b54f7a853b8ba1e49111ffffec60522
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.9 MB (60926992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e198a1d504a269c573cbb65153cf66b357f2bbb8819c47ac787875f47f4205c7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:16 GMT
ADD file:9d9c04bf28d7e6075270ca8a75c01a6d4015bc3eccc4812a82681a7fabf27027 in / 
# Thu, 17 Mar 2022 03:24:17 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:26:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Mar 2022 22:28:12 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Thu, 17 Mar 2022 22:28:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Mar 2022 22:28:22 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Mar 2022 22:28:23 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Mar 2022 22:28:23 GMT
EXPOSE 8888
# Thu, 17 Mar 2022 22:28:24 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Mar 2022 22:28:26 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 17 Mar 2022 22:28:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 22:28:27 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:ecb1e7e01fa06e43b3018b38895366ba643cbac6d46bce566be2aa1cf10abf48`  
		Last Modified: Thu, 17 Mar 2022 03:32:58 GMT  
		Size: 20.4 MB (20423817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdcc9ed8b864108c2f441d508e2349d88968c42f8446c04f18fb121e256bd9bb`  
		Last Modified: Thu, 17 Mar 2022 22:29:15 GMT  
		Size: 6.0 MB (6047145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feff8b25ef2859d6d5baa4cb27318419efe784820857970e2fcefc8ecceb4c92`  
		Last Modified: Thu, 17 Mar 2022 22:29:49 GMT  
		Size: 34.4 MB (34431638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d273285d82262d4299a0d4651c5e0afc50c7b84b6a692198d79215a6d7b5dbd8`  
		Last Modified: Thu, 17 Mar 2022 22:29:44 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9871739638ffdb446fc0ffec3c5269a1872cc3255467e1be724299bbef9813e1`  
		Last Modified: Thu, 17 Mar 2022 22:29:44 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2450f64c0a194bb55a966b877ba08cbbdbf5b1421237c417b0e87bd41c32acc9`  
		Last Modified: Thu, 17 Mar 2022 22:29:44 GMT  
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
$ docker pull chronograf@sha256:ec67a34f27558e92b983eda587facff3f0bc97a8b34f283519b156090cd99e71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.9` - linux; amd64

```console
$ docker pull chronograf@sha256:203dd6718b0b014938013eb89474e890b7b1a9d22ce8f972bd29cca94c2d8e85
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66902345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ce596678bbf826cb544ef02c5deff44ba8028894ded7ba4a172ac61ca0a4da`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:48 GMT
ADD file:9fc739b295073dd1d9293d2ea8106e21156de790c82a9d19be210c0c63bfb527 in / 
# Thu, 17 Mar 2022 04:06:48 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:38:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Mar 2022 08:39:52 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Thu, 17 Mar 2022 08:39:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Mar 2022 08:40:00 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Mar 2022 08:40:00 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Mar 2022 08:40:00 GMT
EXPOSE 8888
# Thu, 17 Mar 2022 08:40:00 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Mar 2022 08:40:00 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 17 Mar 2022 08:40:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 08:40:00 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:5d9da879a61c05a35520eabaa04d22b4867d0cf84a91f4c7b078128e1c820ce5`  
		Last Modified: Thu, 17 Mar 2022 04:14:03 GMT  
		Size: 22.6 MB (22567740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964f48dfa9fa2029216316deab45629f6c3afbc5021d72278ae08424dd0774b0`  
		Last Modified: Thu, 17 Mar 2022 08:40:28 GMT  
		Size: 6.8 MB (6760337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c029f26fb2a489694f465bbac891f386b0e340a4e635f8827b3eab95ccab91`  
		Last Modified: Thu, 17 Mar 2022 08:41:20 GMT  
		Size: 37.5 MB (37549883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38654531a3feaa66eb33eac349aa2cdea510083c9feea5a4a23a6fa2bb56a42`  
		Last Modified: Thu, 17 Mar 2022 08:41:14 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90b5b800b4be88904d64f922fce3b13374b477ed48dbf656bcebc40438e1f72`  
		Last Modified: Thu, 17 Mar 2022 08:41:14 GMT  
		Size: 11.9 KB (11902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0660ca6c588b32688136748866e1b1be2c02f95b61ebec38d1622a8a61636048`  
		Last Modified: Thu, 17 Mar 2022 08:41:14 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:4c8dcb2c76b03c69951e6206895e87c3c8277dbf2044abb2801ef988262b604a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60397941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc61f8a67dbb70986d26b34a6a1071db195122333b3c60be0c6509cc704311c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 01 Mar 2022 02:09:29 GMT
ADD file:b573bfb75b0df3ee547a99ec724d80518fbba40b260dadfe30467b24057bb391 in / 
# Tue, 01 Mar 2022 02:09:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:04:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 01 Mar 2022 10:06:47 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Tue, 01 Mar 2022 10:07:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 01 Mar 2022 10:07:07 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 01 Mar 2022 10:07:07 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 01 Mar 2022 10:07:08 GMT
EXPOSE 8888
# Tue, 01 Mar 2022 10:07:08 GMT
VOLUME [/var/lib/chronograf]
# Tue, 01 Mar 2022 10:07:08 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 01 Mar 2022 10:07:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 01 Mar 2022 10:07:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:52aa216cc1f7f3b5d4ed3b10d96ffe1a02174398f1c9377415eb8bb643cb1782`  
		Last Modified: Tue, 01 Mar 2022 02:26:16 GMT  
		Size: 19.3 MB (19318791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804bc2cf457bc72a961a14f07cfde54ad58d9c46bb9b0fa52c8e07da4b6992cb`  
		Last Modified: Tue, 01 Mar 2022 10:08:06 GMT  
		Size: 5.8 MB (5780607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29965063ffeffa72f4b492187c19948aca6dd613d090bb0f0c6facc905cae0bf`  
		Last Modified: Tue, 01 Mar 2022 10:09:46 GMT  
		Size: 35.3 MB (35274150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613920705fd510f3dd6fdf774386aea78a30e5f6a8cff3961b8b5b38f38bb1ce`  
		Last Modified: Tue, 01 Mar 2022 10:09:27 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b782d37fb4448f5a4cc79f33d0139e6245e63419f00a47a676162b04bf641418`  
		Last Modified: Tue, 01 Mar 2022 10:09:27 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1854eb21aae3ef28744b14498f4494c2af63ad5e15e3be40e64ab115370d1e08`  
		Last Modified: Tue, 01 Mar 2022 10:09:27 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:f52fac89b61a5278ce979c1f7f60e5c179eb1a4c18d928bd4ddcfe8cb00c7a65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.6 MB (61646964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b427fe2410f408d91afd9856ca14acb5ecced77d1537ba5e4b68464916d1476d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:16 GMT
ADD file:9d9c04bf28d7e6075270ca8a75c01a6d4015bc3eccc4812a82681a7fabf27027 in / 
# Thu, 17 Mar 2022 03:24:17 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:26:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Mar 2022 22:28:34 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Thu, 17 Mar 2022 22:28:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Mar 2022 22:28:44 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Mar 2022 22:28:45 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Mar 2022 22:28:45 GMT
EXPOSE 8888
# Thu, 17 Mar 2022 22:28:46 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Mar 2022 22:28:48 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 17 Mar 2022 22:28:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 22:28:49 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:ecb1e7e01fa06e43b3018b38895366ba643cbac6d46bce566be2aa1cf10abf48`  
		Last Modified: Thu, 17 Mar 2022 03:32:58 GMT  
		Size: 20.4 MB (20423817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdcc9ed8b864108c2f441d508e2349d88968c42f8446c04f18fb121e256bd9bb`  
		Last Modified: Thu, 17 Mar 2022 22:29:15 GMT  
		Size: 6.0 MB (6047145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f040d7c1a75ca56bc6fbf940a552bf5588b145d5581ce22f2d1513663280a5f`  
		Last Modified: Thu, 17 Mar 2022 22:30:04 GMT  
		Size: 35.2 MB (35151607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b05e8d05a991c4ebbe50e4ca9764b751ae1f90a74f34e0af4f6ba4c665550e`  
		Last Modified: Thu, 17 Mar 2022 22:30:00 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8684be11bc343f7082742438054e0f34c167f975ddbf8588e103d3b78746a35`  
		Last Modified: Thu, 17 Mar 2022 22:29:59 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d2e3e0f9aa00fe6a50e430119c1ae1c4cb3eaabe5713be5e213114dd9c1c65`  
		Last Modified: Thu, 17 Mar 2022 22:29:59 GMT  
		Size: 239.0 B  
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
$ docker pull chronograf@sha256:ec67a34f27558e92b983eda587facff3f0bc97a8b34f283519b156090cd99e71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.9.3` - linux; amd64

```console
$ docker pull chronograf@sha256:203dd6718b0b014938013eb89474e890b7b1a9d22ce8f972bd29cca94c2d8e85
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66902345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ce596678bbf826cb544ef02c5deff44ba8028894ded7ba4a172ac61ca0a4da`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:48 GMT
ADD file:9fc739b295073dd1d9293d2ea8106e21156de790c82a9d19be210c0c63bfb527 in / 
# Thu, 17 Mar 2022 04:06:48 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:38:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Mar 2022 08:39:52 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Thu, 17 Mar 2022 08:39:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Mar 2022 08:40:00 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Mar 2022 08:40:00 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Mar 2022 08:40:00 GMT
EXPOSE 8888
# Thu, 17 Mar 2022 08:40:00 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Mar 2022 08:40:00 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 17 Mar 2022 08:40:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 08:40:00 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:5d9da879a61c05a35520eabaa04d22b4867d0cf84a91f4c7b078128e1c820ce5`  
		Last Modified: Thu, 17 Mar 2022 04:14:03 GMT  
		Size: 22.6 MB (22567740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964f48dfa9fa2029216316deab45629f6c3afbc5021d72278ae08424dd0774b0`  
		Last Modified: Thu, 17 Mar 2022 08:40:28 GMT  
		Size: 6.8 MB (6760337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c029f26fb2a489694f465bbac891f386b0e340a4e635f8827b3eab95ccab91`  
		Last Modified: Thu, 17 Mar 2022 08:41:20 GMT  
		Size: 37.5 MB (37549883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38654531a3feaa66eb33eac349aa2cdea510083c9feea5a4a23a6fa2bb56a42`  
		Last Modified: Thu, 17 Mar 2022 08:41:14 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90b5b800b4be88904d64f922fce3b13374b477ed48dbf656bcebc40438e1f72`  
		Last Modified: Thu, 17 Mar 2022 08:41:14 GMT  
		Size: 11.9 KB (11902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0660ca6c588b32688136748866e1b1be2c02f95b61ebec38d1622a8a61636048`  
		Last Modified: Thu, 17 Mar 2022 08:41:14 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9.3` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:4c8dcb2c76b03c69951e6206895e87c3c8277dbf2044abb2801ef988262b604a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60397941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc61f8a67dbb70986d26b34a6a1071db195122333b3c60be0c6509cc704311c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 01 Mar 2022 02:09:29 GMT
ADD file:b573bfb75b0df3ee547a99ec724d80518fbba40b260dadfe30467b24057bb391 in / 
# Tue, 01 Mar 2022 02:09:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:04:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 01 Mar 2022 10:06:47 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Tue, 01 Mar 2022 10:07:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 01 Mar 2022 10:07:07 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 01 Mar 2022 10:07:07 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 01 Mar 2022 10:07:08 GMT
EXPOSE 8888
# Tue, 01 Mar 2022 10:07:08 GMT
VOLUME [/var/lib/chronograf]
# Tue, 01 Mar 2022 10:07:08 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 01 Mar 2022 10:07:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 01 Mar 2022 10:07:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:52aa216cc1f7f3b5d4ed3b10d96ffe1a02174398f1c9377415eb8bb643cb1782`  
		Last Modified: Tue, 01 Mar 2022 02:26:16 GMT  
		Size: 19.3 MB (19318791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804bc2cf457bc72a961a14f07cfde54ad58d9c46bb9b0fa52c8e07da4b6992cb`  
		Last Modified: Tue, 01 Mar 2022 10:08:06 GMT  
		Size: 5.8 MB (5780607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29965063ffeffa72f4b492187c19948aca6dd613d090bb0f0c6facc905cae0bf`  
		Last Modified: Tue, 01 Mar 2022 10:09:46 GMT  
		Size: 35.3 MB (35274150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613920705fd510f3dd6fdf774386aea78a30e5f6a8cff3961b8b5b38f38bb1ce`  
		Last Modified: Tue, 01 Mar 2022 10:09:27 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b782d37fb4448f5a4cc79f33d0139e6245e63419f00a47a676162b04bf641418`  
		Last Modified: Tue, 01 Mar 2022 10:09:27 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1854eb21aae3ef28744b14498f4494c2af63ad5e15e3be40e64ab115370d1e08`  
		Last Modified: Tue, 01 Mar 2022 10:09:27 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9.3` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:f52fac89b61a5278ce979c1f7f60e5c179eb1a4c18d928bd4ddcfe8cb00c7a65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.6 MB (61646964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b427fe2410f408d91afd9856ca14acb5ecced77d1537ba5e4b68464916d1476d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:16 GMT
ADD file:9d9c04bf28d7e6075270ca8a75c01a6d4015bc3eccc4812a82681a7fabf27027 in / 
# Thu, 17 Mar 2022 03:24:17 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:26:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Mar 2022 22:28:34 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Thu, 17 Mar 2022 22:28:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Mar 2022 22:28:44 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Mar 2022 22:28:45 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Mar 2022 22:28:45 GMT
EXPOSE 8888
# Thu, 17 Mar 2022 22:28:46 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Mar 2022 22:28:48 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 17 Mar 2022 22:28:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 22:28:49 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:ecb1e7e01fa06e43b3018b38895366ba643cbac6d46bce566be2aa1cf10abf48`  
		Last Modified: Thu, 17 Mar 2022 03:32:58 GMT  
		Size: 20.4 MB (20423817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdcc9ed8b864108c2f441d508e2349d88968c42f8446c04f18fb121e256bd9bb`  
		Last Modified: Thu, 17 Mar 2022 22:29:15 GMT  
		Size: 6.0 MB (6047145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f040d7c1a75ca56bc6fbf940a552bf5588b145d5581ce22f2d1513663280a5f`  
		Last Modified: Thu, 17 Mar 2022 22:30:04 GMT  
		Size: 35.2 MB (35151607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b05e8d05a991c4ebbe50e4ca9764b751ae1f90a74f34e0af4f6ba4c665550e`  
		Last Modified: Thu, 17 Mar 2022 22:30:00 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8684be11bc343f7082742438054e0f34c167f975ddbf8588e103d3b78746a35`  
		Last Modified: Thu, 17 Mar 2022 22:29:59 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d2e3e0f9aa00fe6a50e430119c1ae1c4cb3eaabe5713be5e213114dd9c1c65`  
		Last Modified: Thu, 17 Mar 2022 22:29:59 GMT  
		Size: 239.0 B  
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
$ docker pull chronograf@sha256:ec67a34f27558e92b983eda587facff3f0bc97a8b34f283519b156090cd99e71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:203dd6718b0b014938013eb89474e890b7b1a9d22ce8f972bd29cca94c2d8e85
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66902345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ce596678bbf826cb544ef02c5deff44ba8028894ded7ba4a172ac61ca0a4da`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:48 GMT
ADD file:9fc739b295073dd1d9293d2ea8106e21156de790c82a9d19be210c0c63bfb527 in / 
# Thu, 17 Mar 2022 04:06:48 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:38:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Mar 2022 08:39:52 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Thu, 17 Mar 2022 08:39:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Mar 2022 08:40:00 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Mar 2022 08:40:00 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Mar 2022 08:40:00 GMT
EXPOSE 8888
# Thu, 17 Mar 2022 08:40:00 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Mar 2022 08:40:00 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 17 Mar 2022 08:40:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 08:40:00 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:5d9da879a61c05a35520eabaa04d22b4867d0cf84a91f4c7b078128e1c820ce5`  
		Last Modified: Thu, 17 Mar 2022 04:14:03 GMT  
		Size: 22.6 MB (22567740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964f48dfa9fa2029216316deab45629f6c3afbc5021d72278ae08424dd0774b0`  
		Last Modified: Thu, 17 Mar 2022 08:40:28 GMT  
		Size: 6.8 MB (6760337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c029f26fb2a489694f465bbac891f386b0e340a4e635f8827b3eab95ccab91`  
		Last Modified: Thu, 17 Mar 2022 08:41:20 GMT  
		Size: 37.5 MB (37549883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38654531a3feaa66eb33eac349aa2cdea510083c9feea5a4a23a6fa2bb56a42`  
		Last Modified: Thu, 17 Mar 2022 08:41:14 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90b5b800b4be88904d64f922fce3b13374b477ed48dbf656bcebc40438e1f72`  
		Last Modified: Thu, 17 Mar 2022 08:41:14 GMT  
		Size: 11.9 KB (11902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0660ca6c588b32688136748866e1b1be2c02f95b61ebec38d1622a8a61636048`  
		Last Modified: Thu, 17 Mar 2022 08:41:14 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:4c8dcb2c76b03c69951e6206895e87c3c8277dbf2044abb2801ef988262b604a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60397941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc61f8a67dbb70986d26b34a6a1071db195122333b3c60be0c6509cc704311c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 01 Mar 2022 02:09:29 GMT
ADD file:b573bfb75b0df3ee547a99ec724d80518fbba40b260dadfe30467b24057bb391 in / 
# Tue, 01 Mar 2022 02:09:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:04:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 01 Mar 2022 10:06:47 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Tue, 01 Mar 2022 10:07:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 01 Mar 2022 10:07:07 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 01 Mar 2022 10:07:07 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 01 Mar 2022 10:07:08 GMT
EXPOSE 8888
# Tue, 01 Mar 2022 10:07:08 GMT
VOLUME [/var/lib/chronograf]
# Tue, 01 Mar 2022 10:07:08 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 01 Mar 2022 10:07:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 01 Mar 2022 10:07:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:52aa216cc1f7f3b5d4ed3b10d96ffe1a02174398f1c9377415eb8bb643cb1782`  
		Last Modified: Tue, 01 Mar 2022 02:26:16 GMT  
		Size: 19.3 MB (19318791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804bc2cf457bc72a961a14f07cfde54ad58d9c46bb9b0fa52c8e07da4b6992cb`  
		Last Modified: Tue, 01 Mar 2022 10:08:06 GMT  
		Size: 5.8 MB (5780607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29965063ffeffa72f4b492187c19948aca6dd613d090bb0f0c6facc905cae0bf`  
		Last Modified: Tue, 01 Mar 2022 10:09:46 GMT  
		Size: 35.3 MB (35274150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613920705fd510f3dd6fdf774386aea78a30e5f6a8cff3961b8b5b38f38bb1ce`  
		Last Modified: Tue, 01 Mar 2022 10:09:27 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b782d37fb4448f5a4cc79f33d0139e6245e63419f00a47a676162b04bf641418`  
		Last Modified: Tue, 01 Mar 2022 10:09:27 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1854eb21aae3ef28744b14498f4494c2af63ad5e15e3be40e64ab115370d1e08`  
		Last Modified: Tue, 01 Mar 2022 10:09:27 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:f52fac89b61a5278ce979c1f7f60e5c179eb1a4c18d928bd4ddcfe8cb00c7a65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.6 MB (61646964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b427fe2410f408d91afd9856ca14acb5ecced77d1537ba5e4b68464916d1476d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:16 GMT
ADD file:9d9c04bf28d7e6075270ca8a75c01a6d4015bc3eccc4812a82681a7fabf27027 in / 
# Thu, 17 Mar 2022 03:24:17 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:26:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Mar 2022 22:28:34 GMT
ENV CHRONOGRAF_VERSION=1.9.3
# Thu, 17 Mar 2022 22:28:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Mar 2022 22:28:44 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Mar 2022 22:28:45 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Mar 2022 22:28:45 GMT
EXPOSE 8888
# Thu, 17 Mar 2022 22:28:46 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Mar 2022 22:28:48 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 17 Mar 2022 22:28:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 22:28:49 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:ecb1e7e01fa06e43b3018b38895366ba643cbac6d46bce566be2aa1cf10abf48`  
		Last Modified: Thu, 17 Mar 2022 03:32:58 GMT  
		Size: 20.4 MB (20423817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdcc9ed8b864108c2f441d508e2349d88968c42f8446c04f18fb121e256bd9bb`  
		Last Modified: Thu, 17 Mar 2022 22:29:15 GMT  
		Size: 6.0 MB (6047145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f040d7c1a75ca56bc6fbf940a552bf5588b145d5581ce22f2d1513663280a5f`  
		Last Modified: Thu, 17 Mar 2022 22:30:04 GMT  
		Size: 35.2 MB (35151607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b05e8d05a991c4ebbe50e4ca9764b751ae1f90a74f34e0af4f6ba4c665550e`  
		Last Modified: Thu, 17 Mar 2022 22:30:00 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8684be11bc343f7082742438054e0f34c167f975ddbf8588e103d3b78746a35`  
		Last Modified: Thu, 17 Mar 2022 22:29:59 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d2e3e0f9aa00fe6a50e430119c1ae1c4cb3eaabe5713be5e213114dd9c1c65`  
		Last Modified: Thu, 17 Mar 2022 22:29:59 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
