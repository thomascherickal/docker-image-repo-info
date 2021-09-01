<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `docker`

-	[`docker:20`](#docker20)
-	[`docker:20-dind`](#docker20-dind)
-	[`docker:20-dind-rootless`](#docker20-dind-rootless)
-	[`docker:20-git`](#docker20-git)
-	[`docker:20-windowsservercore`](#docker20-windowsservercore)
-	[`docker:20-windowsservercore-1809`](#docker20-windowsservercore-1809)
-	[`docker:20.10`](#docker2010)
-	[`docker:20.10-dind`](#docker2010-dind)
-	[`docker:20.10-dind-rootless`](#docker2010-dind-rootless)
-	[`docker:20.10-git`](#docker2010-git)
-	[`docker:20.10-windowsservercore`](#docker2010-windowsservercore)
-	[`docker:20.10-windowsservercore-1809`](#docker2010-windowsservercore-1809)
-	[`docker:20.10.8`](#docker20108)
-	[`docker:20.10.8-alpine3.13`](#docker20108-alpine313)
-	[`docker:20.10.8-dind`](#docker20108-dind)
-	[`docker:20.10.8-dind-alpine3.13`](#docker20108-dind-alpine313)
-	[`docker:20.10.8-dind-rootless`](#docker20108-dind-rootless)
-	[`docker:20.10.8-git`](#docker20108-git)
-	[`docker:20.10.8-windowsservercore`](#docker20108-windowsservercore)
-	[`docker:20.10.8-windowsservercore-1809`](#docker20108-windowsservercore-1809)
-	[`docker:dind`](#dockerdind)
-	[`docker:dind-rootless`](#dockerdind-rootless)
-	[`docker:git`](#dockergit)
-	[`docker:latest`](#dockerlatest)
-	[`docker:windowsservercore`](#dockerwindowsservercore)
-	[`docker:windowsservercore-1809`](#dockerwindowsservercore-1809)

## `docker:20`

```console
$ docker pull docker@sha256:e496f1729171f76a9b1a9b2a99431003e8e89e67168ed411ad25b95a73445d13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20` - linux; amd64

```console
$ docker pull docker@sha256:35f612c47195c6e7c1e9ecc80c1b1a00402f3c039e768dd08b2ddb237fd5d0ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66151138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f67ee0b7de2f5cca0d60fe996f082ee6795d35fdd0c7823325b0f7855f57c342`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:26:39 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 00:26:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:26:40 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 00:26:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 00:26:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 00:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:48 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de31523ae09475f6d68e873b416f497c2bd9a92224d9dc9224e1ec4c0a6066e`  
		Last Modified: Wed, 01 Sep 2021 00:27:41 GMT  
		Size: 2.1 MB (2051151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856ddc4bf6a58ca53ceb6444141995979c00718b20dae8c849231fcf9bfae27`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2117e19917ef5839774785d348adb2ff996bccac5f12d461ca21ecfd58283314`  
		Last Modified: Wed, 01 Sep 2021 00:27:51 GMT  
		Size: 61.3 MB (61284048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53eeb058f8c3c25c5b9f9d12769ab386c353b9f48506daae8fdebd88a33a21`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9223565313e3813eda94fc3641a51cdd88a37775e7b9817ada2a57bd45050906`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa82c493f72cf1d33f4a0bd90320bdb1923957f3cb3b0d36596f52bad68ecb4`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:cbad49f1637b08b224d3bb36e840cc869624bbe08b359763bd6ada7026165403
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60193296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51720a73bc2639cb36d62b9239b6db9903861e48a613e6202cfc1224065d5c3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 12:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 12:09:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 12:09:34 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 12:09:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 12:09:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 12:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:39 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a21b349a3936e2b00dec57a9db1f448fc4a1a7a3f4ce187cab93819f045fb35`  
		Last Modified: Wed, 01 Sep 2021 12:11:04 GMT  
		Size: 2.1 MB (2058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd93908d94fd730b48322ef41072abf6ba75634aeca40153ef133aae9700fbf4`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2566d8104302856d2cfd150c099a6c900ecc92f214478aa574d755afc6ce191`  
		Last Modified: Wed, 01 Sep 2021 12:11:11 GMT  
		Size: 55.4 MB (55420371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0dc4a2cf61d4525db0351dcde1cc47f8005d1f7260470032b1b731c75757f6`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90454e11d6bb4b836cd9f026908873ed60d1f7e76b2cbcde812fcabe652fa8d`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a170ef51809d6a08fc091d84fc936b83c0aa5c141c7d0cf8ec41c885a79808`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind`

```console
$ docker pull docker@sha256:930d9041e55d0be64f84cc1a83c75be5d0ae456732b731ee3787fbb5e1f54303
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind` - linux; amd64

```console
$ docker pull docker@sha256:d1c7515d7ba19c572b6f60ec904cf0a875b3bf60c427205845b5ab7b432b05ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72680575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dc41137f712d794c3471c40b56f946667cfe729e112ebc6f1a824bcc775f679`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:26:39 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 00:26:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:26:40 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 00:26:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 00:26:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 00:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:48 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 00:26:54 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 00:26:55 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 00:26:55 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 00:26:57 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 00:26:57 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:57 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 00:26:57 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 00:26:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:58 GMT
CMD []
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de31523ae09475f6d68e873b416f497c2bd9a92224d9dc9224e1ec4c0a6066e`  
		Last Modified: Wed, 01 Sep 2021 00:27:41 GMT  
		Size: 2.1 MB (2051151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856ddc4bf6a58ca53ceb6444141995979c00718b20dae8c849231fcf9bfae27`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2117e19917ef5839774785d348adb2ff996bccac5f12d461ca21ecfd58283314`  
		Last Modified: Wed, 01 Sep 2021 00:27:51 GMT  
		Size: 61.3 MB (61284048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53eeb058f8c3c25c5b9f9d12769ab386c353b9f48506daae8fdebd88a33a21`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9223565313e3813eda94fc3641a51cdd88a37775e7b9817ada2a57bd45050906`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa82c493f72cf1d33f4a0bd90320bdb1923957f3cb3b0d36596f52bad68ecb4`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5973cffe69ed6ec4ab2e2a3a191794cfba7339588cdbc4f3c6355e040c05fb`  
		Last Modified: Wed, 01 Sep 2021 00:28:13 GMT  
		Size: 6.5 MB (6524532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a47d00d0a33090100f0be8b5d564e20357fa60a275aba922aea6db6fb47531`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ba8a29d06b5993e5468f57fa6a9d0adff807919d6c664b785a96b1fb6a96d8`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 978.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6762b64189d2495a0856c3f7d465d7ad0f91a4e2db42b4093e70c7b55e571211`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e2c074f5bc12ca897de843ea2a4be80c932562a92fa388759a9e3ca0510f1ebe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66613965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da28e79c019f7bf9d228ccbf4537acc4f791b8c17d88df076532d28c63c57725`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 12:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 12:09:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 12:09:34 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 12:09:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 12:09:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 12:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:39 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 12:09:48 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 12:09:49 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 12:09:49 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 12:09:50 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 12:09:51 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:51 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 12:09:51 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 12:09:51 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:51 GMT
CMD []
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a21b349a3936e2b00dec57a9db1f448fc4a1a7a3f4ce187cab93819f045fb35`  
		Last Modified: Wed, 01 Sep 2021 12:11:04 GMT  
		Size: 2.1 MB (2058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd93908d94fd730b48322ef41072abf6ba75634aeca40153ef133aae9700fbf4`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2566d8104302856d2cfd150c099a6c900ecc92f214478aa574d755afc6ce191`  
		Last Modified: Wed, 01 Sep 2021 12:11:11 GMT  
		Size: 55.4 MB (55420371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0dc4a2cf61d4525db0351dcde1cc47f8005d1f7260470032b1b731c75757f6`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90454e11d6bb4b836cd9f026908873ed60d1f7e76b2cbcde812fcabe652fa8d`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a170ef51809d6a08fc091d84fc936b83c0aa5c141c7d0cf8ec41c885a79808`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0e2259beeaa75ad2e5d9a651083197a65f1cc00f81974fe83c51617cc4c723`  
		Last Modified: Wed, 01 Sep 2021 12:11:33 GMT  
		Size: 6.4 MB (6415767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c21d52d8c2e860c682d8f1c65d2ffdde59adc3fa8885afe8f7ce95d69ca2a25`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c880d1f23bb87b195c065ca4feb4801fded56bc304979b1b896202db7974a3`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 977.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c833ed3f15c1989d0149c5389b60b295a9fb2ab1050d01c3ac94605805737daa`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:e20d60287be95c73a224d658b455181367f0d6be7e7810cb94e721ad4cb411e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:33a0761966c87569be2a9763c8c477dd3e8981982c8abc4324c090f9d2478231
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.9 MB (92930272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5357717b590217cbd992209ed6e2fb34e8ba65a74d3a5324c9b916395a15cb1b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:26:39 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 00:26:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:26:40 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 00:26:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 00:26:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 00:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:48 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 00:26:54 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 00:26:55 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 00:26:55 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 00:26:57 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 00:26:57 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:57 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 00:26:57 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 00:26:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:58 GMT
CMD []
# Wed, 01 Sep 2021 00:27:03 GMT
RUN apk add --no-cache iproute2
# Wed, 01 Sep 2021 00:27:03 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Sep 2021 00:27:04 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Sep 2021 00:27:06 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Sep 2021 00:27:07 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Sep 2021 00:27:08 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Sep 2021 00:27:08 GMT
USER rootless
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de31523ae09475f6d68e873b416f497c2bd9a92224d9dc9224e1ec4c0a6066e`  
		Last Modified: Wed, 01 Sep 2021 00:27:41 GMT  
		Size: 2.1 MB (2051151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856ddc4bf6a58ca53ceb6444141995979c00718b20dae8c849231fcf9bfae27`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2117e19917ef5839774785d348adb2ff996bccac5f12d461ca21ecfd58283314`  
		Last Modified: Wed, 01 Sep 2021 00:27:51 GMT  
		Size: 61.3 MB (61284048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53eeb058f8c3c25c5b9f9d12769ab386c353b9f48506daae8fdebd88a33a21`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9223565313e3813eda94fc3641a51cdd88a37775e7b9817ada2a57bd45050906`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa82c493f72cf1d33f4a0bd90320bdb1923957f3cb3b0d36596f52bad68ecb4`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5973cffe69ed6ec4ab2e2a3a191794cfba7339588cdbc4f3c6355e040c05fb`  
		Last Modified: Wed, 01 Sep 2021 00:28:13 GMT  
		Size: 6.5 MB (6524532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a47d00d0a33090100f0be8b5d564e20357fa60a275aba922aea6db6fb47531`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ba8a29d06b5993e5468f57fa6a9d0adff807919d6c664b785a96b1fb6a96d8`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 978.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6762b64189d2495a0856c3f7d465d7ad0f91a4e2db42b4093e70c7b55e571211`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62dbc14ca68582d0028413d0826f71ced2423d092126de153c91bbf05e4c98fa`  
		Last Modified: Wed, 01 Sep 2021 00:28:35 GMT  
		Size: 1.1 MB (1131899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2498ce93d923f17fb67004858df28e840d729cf6e6fbdfa82ed3c82679ebe4`  
		Last Modified: Wed, 01 Sep 2021 00:28:34 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64015873fa22ddcd58c65fa437669d9153f1a1fd72fd3a43dbd6873f129461b9`  
		Last Modified: Wed, 01 Sep 2021 00:28:35 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcf73021c4287b49de963988902f36818158f72e0ccd6e3b93af6bb3f4e7ef9`  
		Last Modified: Wed, 01 Sep 2021 00:28:39 GMT  
		Size: 19.1 MB (19116093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57ea275b05bd4bf7a61d8bc934c3d72b3d30ae866ed920fdd7d0a5d06933c0d`  
		Last Modified: Wed, 01 Sep 2021 00:28:34 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:b598f87e3cc82f736a2eeca9070c755d210c1e07e781dab8d10b4de0f667f70e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.9 MB (88863616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fd63c6c9164195ca3489088ce1c8c64b49592ed1226e03c7d92022039060851`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 12:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 12:09:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 12:09:34 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 12:09:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 12:09:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 12:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:39 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 12:09:48 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 12:09:49 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 12:09:49 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 12:09:50 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 12:09:51 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:51 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 12:09:51 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 12:09:51 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:51 GMT
CMD []
# Wed, 01 Sep 2021 12:09:59 GMT
RUN apk add --no-cache iproute2
# Wed, 01 Sep 2021 12:10:00 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Sep 2021 12:10:00 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Sep 2021 12:10:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Sep 2021 12:10:04 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Sep 2021 12:10:04 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Sep 2021 12:10:04 GMT
USER rootless
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a21b349a3936e2b00dec57a9db1f448fc4a1a7a3f4ce187cab93819f045fb35`  
		Last Modified: Wed, 01 Sep 2021 12:11:04 GMT  
		Size: 2.1 MB (2058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd93908d94fd730b48322ef41072abf6ba75634aeca40153ef133aae9700fbf4`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2566d8104302856d2cfd150c099a6c900ecc92f214478aa574d755afc6ce191`  
		Last Modified: Wed, 01 Sep 2021 12:11:11 GMT  
		Size: 55.4 MB (55420371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0dc4a2cf61d4525db0351dcde1cc47f8005d1f7260470032b1b731c75757f6`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90454e11d6bb4b836cd9f026908873ed60d1f7e76b2cbcde812fcabe652fa8d`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a170ef51809d6a08fc091d84fc936b83c0aa5c141c7d0cf8ec41c885a79808`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0e2259beeaa75ad2e5d9a651083197a65f1cc00f81974fe83c51617cc4c723`  
		Last Modified: Wed, 01 Sep 2021 12:11:33 GMT  
		Size: 6.4 MB (6415767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c21d52d8c2e860c682d8f1c65d2ffdde59adc3fa8885afe8f7ce95d69ca2a25`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c880d1f23bb87b195c065ca4feb4801fded56bc304979b1b896202db7974a3`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 977.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c833ed3f15c1989d0149c5389b60b295a9fb2ab1050d01c3ac94605805737daa`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a3816659f3ed80691c2440a71c52b701b209b0312b20ab035de66138b7ace4`  
		Last Modified: Wed, 01 Sep 2021 12:11:57 GMT  
		Size: 1.2 MB (1153143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b263473a450858ffea4d4f20398e671f3aed33088ea2f024d5ca85b05d483bc5`  
		Last Modified: Wed, 01 Sep 2021 12:11:56 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5dd74bf9b8a1eeb40d1eb049b50f17d218b6a8d3cda03762604975431b4e3f4`  
		Last Modified: Wed, 01 Sep 2021 12:11:56 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8c4d3ed13e9425941dcc5ec5474591f125fd656353e50ed00a1c285976395d`  
		Last Modified: Wed, 01 Sep 2021 12:12:00 GMT  
		Size: 21.1 MB (21094799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba347b526ac690189b994abf8234c930775ca075b958c325f24ac2c1c4bcf0e`  
		Last Modified: Wed, 01 Sep 2021 12:11:56 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-git`

```console
$ docker pull docker@sha256:5924323fafec1818770a7b001524ff526ab1865223b214a19055b87195912734
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-git` - linux; amd64

```console
$ docker pull docker@sha256:709ceab8cd1164fbf0c03b1991f8f412a1543023548fa7a30de2268d399723aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72553637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d03657b093bb281e2bf0c19460dbf0f73fbf181780da767109363461960b6de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:26:39 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 00:26:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:26:40 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 00:26:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 00:26:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 00:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:48 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 00:27:13 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de31523ae09475f6d68e873b416f497c2bd9a92224d9dc9224e1ec4c0a6066e`  
		Last Modified: Wed, 01 Sep 2021 00:27:41 GMT  
		Size: 2.1 MB (2051151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856ddc4bf6a58ca53ceb6444141995979c00718b20dae8c849231fcf9bfae27`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2117e19917ef5839774785d348adb2ff996bccac5f12d461ca21ecfd58283314`  
		Last Modified: Wed, 01 Sep 2021 00:27:51 GMT  
		Size: 61.3 MB (61284048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53eeb058f8c3c25c5b9f9d12769ab386c353b9f48506daae8fdebd88a33a21`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9223565313e3813eda94fc3641a51cdd88a37775e7b9817ada2a57bd45050906`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa82c493f72cf1d33f4a0bd90320bdb1923957f3cb3b0d36596f52bad68ecb4`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8c9f33643fb8321012f52f6a1ec572b42b9f29dcd29c0dcf2635ad0c9d1911`  
		Last Modified: Wed, 01 Sep 2021 00:29:00 GMT  
		Size: 6.4 MB (6402499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f250afada2977e1734ed8c977b720466c1fbc738a1e0ccb85ee0e9bf115dbb9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66680653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6314b14754b6270ce0116f6d93d356dab16dcd7a402b233399d25307483f405`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 12:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 12:09:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 12:09:34 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 12:09:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 12:09:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 12:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:39 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 12:10:12 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a21b349a3936e2b00dec57a9db1f448fc4a1a7a3f4ce187cab93819f045fb35`  
		Last Modified: Wed, 01 Sep 2021 12:11:04 GMT  
		Size: 2.1 MB (2058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd93908d94fd730b48322ef41072abf6ba75634aeca40153ef133aae9700fbf4`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2566d8104302856d2cfd150c099a6c900ecc92f214478aa574d755afc6ce191`  
		Last Modified: Wed, 01 Sep 2021 12:11:11 GMT  
		Size: 55.4 MB (55420371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0dc4a2cf61d4525db0351dcde1cc47f8005d1f7260470032b1b731c75757f6`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90454e11d6bb4b836cd9f026908873ed60d1f7e76b2cbcde812fcabe652fa8d`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a170ef51809d6a08fc091d84fc936b83c0aa5c141c7d0cf8ec41c885a79808`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d37843d9fbf619a9dab1b56a4e2582d767a5106ed2fa0c97f5c1cc3c23e18b`  
		Last Modified: Wed, 01 Sep 2021 12:12:21 GMT  
		Size: 6.5 MB (6487357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore`

```console
$ docker pull docker@sha256:81d849a5208118837827efb4f0433db49a305260c37f83ff813590c03521247f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `docker:20-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull docker@sha256:a86536c27f22717fed9d5bcb2ff43eb82f0c2e7eb602d6b9c5d714cd0b706e9a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737269694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e594329f431fd456d89c771444f5e662730713ccd58a9d03b52796bd7fa42e35`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 24 Aug 2021 23:23:49 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 24 Aug 2021 23:23:52 GMT
ENV DOCKER_VERSION=20.10.8
# Tue, 24 Aug 2021 23:23:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Tue, 24 Aug 2021 23:24:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c4896faf56da9e635d1215c12a54c8734e695682b57d6e038ca62fd90b532b`  
		Last Modified: Tue, 24 Aug 2021 23:25:13 GMT  
		Size: 378.4 KB (378370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe49ef5983ec79b546f9ba4e76c016df80499c33627052d1101b851ffb7b4fde`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8baf6cf9c02dbd2217455c62d5ee255fd65036a9a442d0d4794abb2fa68c59`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0b72a29873171e2e2cfc43d555ef003e482ffe643396157ba76e4b22ab3017`  
		Last Modified: Tue, 24 Aug 2021 23:26:06 GMT  
		Size: 50.9 MB (50889387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-1809`

```console
$ docker pull docker@sha256:81d849a5208118837827efb4f0433db49a305260c37f83ff813590c03521247f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `docker:20-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull docker@sha256:a86536c27f22717fed9d5bcb2ff43eb82f0c2e7eb602d6b9c5d714cd0b706e9a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737269694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e594329f431fd456d89c771444f5e662730713ccd58a9d03b52796bd7fa42e35`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 24 Aug 2021 23:23:49 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 24 Aug 2021 23:23:52 GMT
ENV DOCKER_VERSION=20.10.8
# Tue, 24 Aug 2021 23:23:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Tue, 24 Aug 2021 23:24:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c4896faf56da9e635d1215c12a54c8734e695682b57d6e038ca62fd90b532b`  
		Last Modified: Tue, 24 Aug 2021 23:25:13 GMT  
		Size: 378.4 KB (378370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe49ef5983ec79b546f9ba4e76c016df80499c33627052d1101b851ffb7b4fde`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8baf6cf9c02dbd2217455c62d5ee255fd65036a9a442d0d4794abb2fa68c59`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0b72a29873171e2e2cfc43d555ef003e482ffe643396157ba76e4b22ab3017`  
		Last Modified: Tue, 24 Aug 2021 23:26:06 GMT  
		Size: 50.9 MB (50889387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10`

```console
$ docker pull docker@sha256:e496f1729171f76a9b1a9b2a99431003e8e89e67168ed411ad25b95a73445d13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10` - linux; amd64

```console
$ docker pull docker@sha256:35f612c47195c6e7c1e9ecc80c1b1a00402f3c039e768dd08b2ddb237fd5d0ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66151138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f67ee0b7de2f5cca0d60fe996f082ee6795d35fdd0c7823325b0f7855f57c342`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:26:39 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 00:26:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:26:40 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 00:26:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 00:26:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 00:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:48 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de31523ae09475f6d68e873b416f497c2bd9a92224d9dc9224e1ec4c0a6066e`  
		Last Modified: Wed, 01 Sep 2021 00:27:41 GMT  
		Size: 2.1 MB (2051151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856ddc4bf6a58ca53ceb6444141995979c00718b20dae8c849231fcf9bfae27`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2117e19917ef5839774785d348adb2ff996bccac5f12d461ca21ecfd58283314`  
		Last Modified: Wed, 01 Sep 2021 00:27:51 GMT  
		Size: 61.3 MB (61284048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53eeb058f8c3c25c5b9f9d12769ab386c353b9f48506daae8fdebd88a33a21`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9223565313e3813eda94fc3641a51cdd88a37775e7b9817ada2a57bd45050906`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa82c493f72cf1d33f4a0bd90320bdb1923957f3cb3b0d36596f52bad68ecb4`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:cbad49f1637b08b224d3bb36e840cc869624bbe08b359763bd6ada7026165403
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60193296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51720a73bc2639cb36d62b9239b6db9903861e48a613e6202cfc1224065d5c3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 12:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 12:09:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 12:09:34 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 12:09:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 12:09:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 12:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:39 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a21b349a3936e2b00dec57a9db1f448fc4a1a7a3f4ce187cab93819f045fb35`  
		Last Modified: Wed, 01 Sep 2021 12:11:04 GMT  
		Size: 2.1 MB (2058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd93908d94fd730b48322ef41072abf6ba75634aeca40153ef133aae9700fbf4`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2566d8104302856d2cfd150c099a6c900ecc92f214478aa574d755afc6ce191`  
		Last Modified: Wed, 01 Sep 2021 12:11:11 GMT  
		Size: 55.4 MB (55420371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0dc4a2cf61d4525db0351dcde1cc47f8005d1f7260470032b1b731c75757f6`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90454e11d6bb4b836cd9f026908873ed60d1f7e76b2cbcde812fcabe652fa8d`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a170ef51809d6a08fc091d84fc936b83c0aa5c141c7d0cf8ec41c885a79808`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind`

```console
$ docker pull docker@sha256:930d9041e55d0be64f84cc1a83c75be5d0ae456732b731ee3787fbb5e1f54303
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind` - linux; amd64

```console
$ docker pull docker@sha256:d1c7515d7ba19c572b6f60ec904cf0a875b3bf60c427205845b5ab7b432b05ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72680575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dc41137f712d794c3471c40b56f946667cfe729e112ebc6f1a824bcc775f679`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:26:39 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 00:26:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:26:40 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 00:26:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 00:26:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 00:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:48 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 00:26:54 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 00:26:55 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 00:26:55 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 00:26:57 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 00:26:57 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:57 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 00:26:57 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 00:26:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:58 GMT
CMD []
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de31523ae09475f6d68e873b416f497c2bd9a92224d9dc9224e1ec4c0a6066e`  
		Last Modified: Wed, 01 Sep 2021 00:27:41 GMT  
		Size: 2.1 MB (2051151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856ddc4bf6a58ca53ceb6444141995979c00718b20dae8c849231fcf9bfae27`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2117e19917ef5839774785d348adb2ff996bccac5f12d461ca21ecfd58283314`  
		Last Modified: Wed, 01 Sep 2021 00:27:51 GMT  
		Size: 61.3 MB (61284048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53eeb058f8c3c25c5b9f9d12769ab386c353b9f48506daae8fdebd88a33a21`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9223565313e3813eda94fc3641a51cdd88a37775e7b9817ada2a57bd45050906`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa82c493f72cf1d33f4a0bd90320bdb1923957f3cb3b0d36596f52bad68ecb4`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5973cffe69ed6ec4ab2e2a3a191794cfba7339588cdbc4f3c6355e040c05fb`  
		Last Modified: Wed, 01 Sep 2021 00:28:13 GMT  
		Size: 6.5 MB (6524532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a47d00d0a33090100f0be8b5d564e20357fa60a275aba922aea6db6fb47531`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ba8a29d06b5993e5468f57fa6a9d0adff807919d6c664b785a96b1fb6a96d8`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 978.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6762b64189d2495a0856c3f7d465d7ad0f91a4e2db42b4093e70c7b55e571211`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e2c074f5bc12ca897de843ea2a4be80c932562a92fa388759a9e3ca0510f1ebe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66613965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da28e79c019f7bf9d228ccbf4537acc4f791b8c17d88df076532d28c63c57725`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 12:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 12:09:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 12:09:34 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 12:09:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 12:09:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 12:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:39 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 12:09:48 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 12:09:49 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 12:09:49 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 12:09:50 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 12:09:51 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:51 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 12:09:51 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 12:09:51 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:51 GMT
CMD []
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a21b349a3936e2b00dec57a9db1f448fc4a1a7a3f4ce187cab93819f045fb35`  
		Last Modified: Wed, 01 Sep 2021 12:11:04 GMT  
		Size: 2.1 MB (2058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd93908d94fd730b48322ef41072abf6ba75634aeca40153ef133aae9700fbf4`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2566d8104302856d2cfd150c099a6c900ecc92f214478aa574d755afc6ce191`  
		Last Modified: Wed, 01 Sep 2021 12:11:11 GMT  
		Size: 55.4 MB (55420371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0dc4a2cf61d4525db0351dcde1cc47f8005d1f7260470032b1b731c75757f6`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90454e11d6bb4b836cd9f026908873ed60d1f7e76b2cbcde812fcabe652fa8d`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a170ef51809d6a08fc091d84fc936b83c0aa5c141c7d0cf8ec41c885a79808`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0e2259beeaa75ad2e5d9a651083197a65f1cc00f81974fe83c51617cc4c723`  
		Last Modified: Wed, 01 Sep 2021 12:11:33 GMT  
		Size: 6.4 MB (6415767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c21d52d8c2e860c682d8f1c65d2ffdde59adc3fa8885afe8f7ce95d69ca2a25`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c880d1f23bb87b195c065ca4feb4801fded56bc304979b1b896202db7974a3`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 977.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c833ed3f15c1989d0149c5389b60b295a9fb2ab1050d01c3ac94605805737daa`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind-rootless`

```console
$ docker pull docker@sha256:e20d60287be95c73a224d658b455181367f0d6be7e7810cb94e721ad4cb411e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:33a0761966c87569be2a9763c8c477dd3e8981982c8abc4324c090f9d2478231
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.9 MB (92930272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5357717b590217cbd992209ed6e2fb34e8ba65a74d3a5324c9b916395a15cb1b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:26:39 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 00:26:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:26:40 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 00:26:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 00:26:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 00:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:48 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 00:26:54 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 00:26:55 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 00:26:55 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 00:26:57 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 00:26:57 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:57 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 00:26:57 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 00:26:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:58 GMT
CMD []
# Wed, 01 Sep 2021 00:27:03 GMT
RUN apk add --no-cache iproute2
# Wed, 01 Sep 2021 00:27:03 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Sep 2021 00:27:04 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Sep 2021 00:27:06 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Sep 2021 00:27:07 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Sep 2021 00:27:08 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Sep 2021 00:27:08 GMT
USER rootless
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de31523ae09475f6d68e873b416f497c2bd9a92224d9dc9224e1ec4c0a6066e`  
		Last Modified: Wed, 01 Sep 2021 00:27:41 GMT  
		Size: 2.1 MB (2051151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856ddc4bf6a58ca53ceb6444141995979c00718b20dae8c849231fcf9bfae27`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2117e19917ef5839774785d348adb2ff996bccac5f12d461ca21ecfd58283314`  
		Last Modified: Wed, 01 Sep 2021 00:27:51 GMT  
		Size: 61.3 MB (61284048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53eeb058f8c3c25c5b9f9d12769ab386c353b9f48506daae8fdebd88a33a21`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9223565313e3813eda94fc3641a51cdd88a37775e7b9817ada2a57bd45050906`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa82c493f72cf1d33f4a0bd90320bdb1923957f3cb3b0d36596f52bad68ecb4`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5973cffe69ed6ec4ab2e2a3a191794cfba7339588cdbc4f3c6355e040c05fb`  
		Last Modified: Wed, 01 Sep 2021 00:28:13 GMT  
		Size: 6.5 MB (6524532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a47d00d0a33090100f0be8b5d564e20357fa60a275aba922aea6db6fb47531`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ba8a29d06b5993e5468f57fa6a9d0adff807919d6c664b785a96b1fb6a96d8`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 978.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6762b64189d2495a0856c3f7d465d7ad0f91a4e2db42b4093e70c7b55e571211`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62dbc14ca68582d0028413d0826f71ced2423d092126de153c91bbf05e4c98fa`  
		Last Modified: Wed, 01 Sep 2021 00:28:35 GMT  
		Size: 1.1 MB (1131899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2498ce93d923f17fb67004858df28e840d729cf6e6fbdfa82ed3c82679ebe4`  
		Last Modified: Wed, 01 Sep 2021 00:28:34 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64015873fa22ddcd58c65fa437669d9153f1a1fd72fd3a43dbd6873f129461b9`  
		Last Modified: Wed, 01 Sep 2021 00:28:35 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcf73021c4287b49de963988902f36818158f72e0ccd6e3b93af6bb3f4e7ef9`  
		Last Modified: Wed, 01 Sep 2021 00:28:39 GMT  
		Size: 19.1 MB (19116093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57ea275b05bd4bf7a61d8bc934c3d72b3d30ae866ed920fdd7d0a5d06933c0d`  
		Last Modified: Wed, 01 Sep 2021 00:28:34 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:b598f87e3cc82f736a2eeca9070c755d210c1e07e781dab8d10b4de0f667f70e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.9 MB (88863616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fd63c6c9164195ca3489088ce1c8c64b49592ed1226e03c7d92022039060851`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 12:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 12:09:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 12:09:34 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 12:09:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 12:09:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 12:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:39 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 12:09:48 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 12:09:49 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 12:09:49 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 12:09:50 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 12:09:51 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:51 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 12:09:51 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 12:09:51 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:51 GMT
CMD []
# Wed, 01 Sep 2021 12:09:59 GMT
RUN apk add --no-cache iproute2
# Wed, 01 Sep 2021 12:10:00 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Sep 2021 12:10:00 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Sep 2021 12:10:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Sep 2021 12:10:04 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Sep 2021 12:10:04 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Sep 2021 12:10:04 GMT
USER rootless
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a21b349a3936e2b00dec57a9db1f448fc4a1a7a3f4ce187cab93819f045fb35`  
		Last Modified: Wed, 01 Sep 2021 12:11:04 GMT  
		Size: 2.1 MB (2058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd93908d94fd730b48322ef41072abf6ba75634aeca40153ef133aae9700fbf4`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2566d8104302856d2cfd150c099a6c900ecc92f214478aa574d755afc6ce191`  
		Last Modified: Wed, 01 Sep 2021 12:11:11 GMT  
		Size: 55.4 MB (55420371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0dc4a2cf61d4525db0351dcde1cc47f8005d1f7260470032b1b731c75757f6`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90454e11d6bb4b836cd9f026908873ed60d1f7e76b2cbcde812fcabe652fa8d`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a170ef51809d6a08fc091d84fc936b83c0aa5c141c7d0cf8ec41c885a79808`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0e2259beeaa75ad2e5d9a651083197a65f1cc00f81974fe83c51617cc4c723`  
		Last Modified: Wed, 01 Sep 2021 12:11:33 GMT  
		Size: 6.4 MB (6415767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c21d52d8c2e860c682d8f1c65d2ffdde59adc3fa8885afe8f7ce95d69ca2a25`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c880d1f23bb87b195c065ca4feb4801fded56bc304979b1b896202db7974a3`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 977.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c833ed3f15c1989d0149c5389b60b295a9fb2ab1050d01c3ac94605805737daa`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a3816659f3ed80691c2440a71c52b701b209b0312b20ab035de66138b7ace4`  
		Last Modified: Wed, 01 Sep 2021 12:11:57 GMT  
		Size: 1.2 MB (1153143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b263473a450858ffea4d4f20398e671f3aed33088ea2f024d5ca85b05d483bc5`  
		Last Modified: Wed, 01 Sep 2021 12:11:56 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5dd74bf9b8a1eeb40d1eb049b50f17d218b6a8d3cda03762604975431b4e3f4`  
		Last Modified: Wed, 01 Sep 2021 12:11:56 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8c4d3ed13e9425941dcc5ec5474591f125fd656353e50ed00a1c285976395d`  
		Last Modified: Wed, 01 Sep 2021 12:12:00 GMT  
		Size: 21.1 MB (21094799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba347b526ac690189b994abf8234c930775ca075b958c325f24ac2c1c4bcf0e`  
		Last Modified: Wed, 01 Sep 2021 12:11:56 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-git`

```console
$ docker pull docker@sha256:5924323fafec1818770a7b001524ff526ab1865223b214a19055b87195912734
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-git` - linux; amd64

```console
$ docker pull docker@sha256:709ceab8cd1164fbf0c03b1991f8f412a1543023548fa7a30de2268d399723aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72553637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d03657b093bb281e2bf0c19460dbf0f73fbf181780da767109363461960b6de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:26:39 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 00:26:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:26:40 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 00:26:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 00:26:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 00:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:48 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 00:27:13 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de31523ae09475f6d68e873b416f497c2bd9a92224d9dc9224e1ec4c0a6066e`  
		Last Modified: Wed, 01 Sep 2021 00:27:41 GMT  
		Size: 2.1 MB (2051151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856ddc4bf6a58ca53ceb6444141995979c00718b20dae8c849231fcf9bfae27`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2117e19917ef5839774785d348adb2ff996bccac5f12d461ca21ecfd58283314`  
		Last Modified: Wed, 01 Sep 2021 00:27:51 GMT  
		Size: 61.3 MB (61284048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53eeb058f8c3c25c5b9f9d12769ab386c353b9f48506daae8fdebd88a33a21`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9223565313e3813eda94fc3641a51cdd88a37775e7b9817ada2a57bd45050906`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa82c493f72cf1d33f4a0bd90320bdb1923957f3cb3b0d36596f52bad68ecb4`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8c9f33643fb8321012f52f6a1ec572b42b9f29dcd29c0dcf2635ad0c9d1911`  
		Last Modified: Wed, 01 Sep 2021 00:29:00 GMT  
		Size: 6.4 MB (6402499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f250afada2977e1734ed8c977b720466c1fbc738a1e0ccb85ee0e9bf115dbb9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66680653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6314b14754b6270ce0116f6d93d356dab16dcd7a402b233399d25307483f405`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 12:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 12:09:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 12:09:34 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 12:09:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 12:09:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 12:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:39 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 12:10:12 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a21b349a3936e2b00dec57a9db1f448fc4a1a7a3f4ce187cab93819f045fb35`  
		Last Modified: Wed, 01 Sep 2021 12:11:04 GMT  
		Size: 2.1 MB (2058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd93908d94fd730b48322ef41072abf6ba75634aeca40153ef133aae9700fbf4`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2566d8104302856d2cfd150c099a6c900ecc92f214478aa574d755afc6ce191`  
		Last Modified: Wed, 01 Sep 2021 12:11:11 GMT  
		Size: 55.4 MB (55420371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0dc4a2cf61d4525db0351dcde1cc47f8005d1f7260470032b1b731c75757f6`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90454e11d6bb4b836cd9f026908873ed60d1f7e76b2cbcde812fcabe652fa8d`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a170ef51809d6a08fc091d84fc936b83c0aa5c141c7d0cf8ec41c885a79808`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d37843d9fbf619a9dab1b56a4e2582d767a5106ed2fa0c97f5c1cc3c23e18b`  
		Last Modified: Wed, 01 Sep 2021 12:12:21 GMT  
		Size: 6.5 MB (6487357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore`

```console
$ docker pull docker@sha256:81d849a5208118837827efb4f0433db49a305260c37f83ff813590c03521247f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `docker:20.10-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull docker@sha256:a86536c27f22717fed9d5bcb2ff43eb82f0c2e7eb602d6b9c5d714cd0b706e9a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737269694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e594329f431fd456d89c771444f5e662730713ccd58a9d03b52796bd7fa42e35`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 24 Aug 2021 23:23:49 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 24 Aug 2021 23:23:52 GMT
ENV DOCKER_VERSION=20.10.8
# Tue, 24 Aug 2021 23:23:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Tue, 24 Aug 2021 23:24:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c4896faf56da9e635d1215c12a54c8734e695682b57d6e038ca62fd90b532b`  
		Last Modified: Tue, 24 Aug 2021 23:25:13 GMT  
		Size: 378.4 KB (378370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe49ef5983ec79b546f9ba4e76c016df80499c33627052d1101b851ffb7b4fde`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8baf6cf9c02dbd2217455c62d5ee255fd65036a9a442d0d4794abb2fa68c59`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0b72a29873171e2e2cfc43d555ef003e482ffe643396157ba76e4b22ab3017`  
		Last Modified: Tue, 24 Aug 2021 23:26:06 GMT  
		Size: 50.9 MB (50889387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-1809`

```console
$ docker pull docker@sha256:81d849a5208118837827efb4f0433db49a305260c37f83ff813590c03521247f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `docker:20.10-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull docker@sha256:a86536c27f22717fed9d5bcb2ff43eb82f0c2e7eb602d6b9c5d714cd0b706e9a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737269694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e594329f431fd456d89c771444f5e662730713ccd58a9d03b52796bd7fa42e35`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 24 Aug 2021 23:23:49 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 24 Aug 2021 23:23:52 GMT
ENV DOCKER_VERSION=20.10.8
# Tue, 24 Aug 2021 23:23:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Tue, 24 Aug 2021 23:24:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c4896faf56da9e635d1215c12a54c8734e695682b57d6e038ca62fd90b532b`  
		Last Modified: Tue, 24 Aug 2021 23:25:13 GMT  
		Size: 378.4 KB (378370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe49ef5983ec79b546f9ba4e76c016df80499c33627052d1101b851ffb7b4fde`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8baf6cf9c02dbd2217455c62d5ee255fd65036a9a442d0d4794abb2fa68c59`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0b72a29873171e2e2cfc43d555ef003e482ffe643396157ba76e4b22ab3017`  
		Last Modified: Tue, 24 Aug 2021 23:26:06 GMT  
		Size: 50.9 MB (50889387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8`

```console
$ docker pull docker@sha256:e496f1729171f76a9b1a9b2a99431003e8e89e67168ed411ad25b95a73445d13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.8` - linux; amd64

```console
$ docker pull docker@sha256:35f612c47195c6e7c1e9ecc80c1b1a00402f3c039e768dd08b2ddb237fd5d0ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66151138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f67ee0b7de2f5cca0d60fe996f082ee6795d35fdd0c7823325b0f7855f57c342`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:26:39 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 00:26:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:26:40 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 00:26:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 00:26:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 00:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:48 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de31523ae09475f6d68e873b416f497c2bd9a92224d9dc9224e1ec4c0a6066e`  
		Last Modified: Wed, 01 Sep 2021 00:27:41 GMT  
		Size: 2.1 MB (2051151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856ddc4bf6a58ca53ceb6444141995979c00718b20dae8c849231fcf9bfae27`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2117e19917ef5839774785d348adb2ff996bccac5f12d461ca21ecfd58283314`  
		Last Modified: Wed, 01 Sep 2021 00:27:51 GMT  
		Size: 61.3 MB (61284048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53eeb058f8c3c25c5b9f9d12769ab386c353b9f48506daae8fdebd88a33a21`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9223565313e3813eda94fc3641a51cdd88a37775e7b9817ada2a57bd45050906`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa82c493f72cf1d33f4a0bd90320bdb1923957f3cb3b0d36596f52bad68ecb4`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.8` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:cbad49f1637b08b224d3bb36e840cc869624bbe08b359763bd6ada7026165403
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60193296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51720a73bc2639cb36d62b9239b6db9903861e48a613e6202cfc1224065d5c3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 12:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 12:09:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 12:09:34 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 12:09:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 12:09:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 12:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:39 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a21b349a3936e2b00dec57a9db1f448fc4a1a7a3f4ce187cab93819f045fb35`  
		Last Modified: Wed, 01 Sep 2021 12:11:04 GMT  
		Size: 2.1 MB (2058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd93908d94fd730b48322ef41072abf6ba75634aeca40153ef133aae9700fbf4`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2566d8104302856d2cfd150c099a6c900ecc92f214478aa574d755afc6ce191`  
		Last Modified: Wed, 01 Sep 2021 12:11:11 GMT  
		Size: 55.4 MB (55420371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0dc4a2cf61d4525db0351dcde1cc47f8005d1f7260470032b1b731c75757f6`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90454e11d6bb4b836cd9f026908873ed60d1f7e76b2cbcde812fcabe652fa8d`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a170ef51809d6a08fc091d84fc936b83c0aa5c141c7d0cf8ec41c885a79808`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8-alpine3.13`

```console
$ docker pull docker@sha256:e496f1729171f76a9b1a9b2a99431003e8e89e67168ed411ad25b95a73445d13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.8-alpine3.13` - linux; amd64

```console
$ docker pull docker@sha256:35f612c47195c6e7c1e9ecc80c1b1a00402f3c039e768dd08b2ddb237fd5d0ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66151138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f67ee0b7de2f5cca0d60fe996f082ee6795d35fdd0c7823325b0f7855f57c342`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:26:39 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 00:26:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:26:40 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 00:26:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 00:26:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 00:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:48 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de31523ae09475f6d68e873b416f497c2bd9a92224d9dc9224e1ec4c0a6066e`  
		Last Modified: Wed, 01 Sep 2021 00:27:41 GMT  
		Size: 2.1 MB (2051151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856ddc4bf6a58ca53ceb6444141995979c00718b20dae8c849231fcf9bfae27`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2117e19917ef5839774785d348adb2ff996bccac5f12d461ca21ecfd58283314`  
		Last Modified: Wed, 01 Sep 2021 00:27:51 GMT  
		Size: 61.3 MB (61284048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53eeb058f8c3c25c5b9f9d12769ab386c353b9f48506daae8fdebd88a33a21`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9223565313e3813eda94fc3641a51cdd88a37775e7b9817ada2a57bd45050906`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa82c493f72cf1d33f4a0bd90320bdb1923957f3cb3b0d36596f52bad68ecb4`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.8-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:cbad49f1637b08b224d3bb36e840cc869624bbe08b359763bd6ada7026165403
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60193296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51720a73bc2639cb36d62b9239b6db9903861e48a613e6202cfc1224065d5c3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 12:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 12:09:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 12:09:34 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 12:09:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 12:09:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 12:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:39 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a21b349a3936e2b00dec57a9db1f448fc4a1a7a3f4ce187cab93819f045fb35`  
		Last Modified: Wed, 01 Sep 2021 12:11:04 GMT  
		Size: 2.1 MB (2058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd93908d94fd730b48322ef41072abf6ba75634aeca40153ef133aae9700fbf4`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2566d8104302856d2cfd150c099a6c900ecc92f214478aa574d755afc6ce191`  
		Last Modified: Wed, 01 Sep 2021 12:11:11 GMT  
		Size: 55.4 MB (55420371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0dc4a2cf61d4525db0351dcde1cc47f8005d1f7260470032b1b731c75757f6`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90454e11d6bb4b836cd9f026908873ed60d1f7e76b2cbcde812fcabe652fa8d`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a170ef51809d6a08fc091d84fc936b83c0aa5c141c7d0cf8ec41c885a79808`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8-dind`

```console
$ docker pull docker@sha256:930d9041e55d0be64f84cc1a83c75be5d0ae456732b731ee3787fbb5e1f54303
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.8-dind` - linux; amd64

```console
$ docker pull docker@sha256:d1c7515d7ba19c572b6f60ec904cf0a875b3bf60c427205845b5ab7b432b05ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72680575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dc41137f712d794c3471c40b56f946667cfe729e112ebc6f1a824bcc775f679`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:26:39 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 00:26:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:26:40 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 00:26:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 00:26:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 00:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:48 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 00:26:54 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 00:26:55 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 00:26:55 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 00:26:57 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 00:26:57 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:57 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 00:26:57 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 00:26:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:58 GMT
CMD []
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de31523ae09475f6d68e873b416f497c2bd9a92224d9dc9224e1ec4c0a6066e`  
		Last Modified: Wed, 01 Sep 2021 00:27:41 GMT  
		Size: 2.1 MB (2051151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856ddc4bf6a58ca53ceb6444141995979c00718b20dae8c849231fcf9bfae27`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2117e19917ef5839774785d348adb2ff996bccac5f12d461ca21ecfd58283314`  
		Last Modified: Wed, 01 Sep 2021 00:27:51 GMT  
		Size: 61.3 MB (61284048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53eeb058f8c3c25c5b9f9d12769ab386c353b9f48506daae8fdebd88a33a21`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9223565313e3813eda94fc3641a51cdd88a37775e7b9817ada2a57bd45050906`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa82c493f72cf1d33f4a0bd90320bdb1923957f3cb3b0d36596f52bad68ecb4`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5973cffe69ed6ec4ab2e2a3a191794cfba7339588cdbc4f3c6355e040c05fb`  
		Last Modified: Wed, 01 Sep 2021 00:28:13 GMT  
		Size: 6.5 MB (6524532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a47d00d0a33090100f0be8b5d564e20357fa60a275aba922aea6db6fb47531`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ba8a29d06b5993e5468f57fa6a9d0adff807919d6c664b785a96b1fb6a96d8`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 978.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6762b64189d2495a0856c3f7d465d7ad0f91a4e2db42b4093e70c7b55e571211`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.8-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e2c074f5bc12ca897de843ea2a4be80c932562a92fa388759a9e3ca0510f1ebe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66613965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da28e79c019f7bf9d228ccbf4537acc4f791b8c17d88df076532d28c63c57725`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 12:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 12:09:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 12:09:34 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 12:09:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 12:09:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 12:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:39 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 12:09:48 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 12:09:49 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 12:09:49 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 12:09:50 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 12:09:51 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:51 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 12:09:51 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 12:09:51 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:51 GMT
CMD []
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a21b349a3936e2b00dec57a9db1f448fc4a1a7a3f4ce187cab93819f045fb35`  
		Last Modified: Wed, 01 Sep 2021 12:11:04 GMT  
		Size: 2.1 MB (2058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd93908d94fd730b48322ef41072abf6ba75634aeca40153ef133aae9700fbf4`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2566d8104302856d2cfd150c099a6c900ecc92f214478aa574d755afc6ce191`  
		Last Modified: Wed, 01 Sep 2021 12:11:11 GMT  
		Size: 55.4 MB (55420371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0dc4a2cf61d4525db0351dcde1cc47f8005d1f7260470032b1b731c75757f6`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90454e11d6bb4b836cd9f026908873ed60d1f7e76b2cbcde812fcabe652fa8d`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a170ef51809d6a08fc091d84fc936b83c0aa5c141c7d0cf8ec41c885a79808`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0e2259beeaa75ad2e5d9a651083197a65f1cc00f81974fe83c51617cc4c723`  
		Last Modified: Wed, 01 Sep 2021 12:11:33 GMT  
		Size: 6.4 MB (6415767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c21d52d8c2e860c682d8f1c65d2ffdde59adc3fa8885afe8f7ce95d69ca2a25`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c880d1f23bb87b195c065ca4feb4801fded56bc304979b1b896202db7974a3`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 977.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c833ed3f15c1989d0149c5389b60b295a9fb2ab1050d01c3ac94605805737daa`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8-dind-alpine3.13`

```console
$ docker pull docker@sha256:930d9041e55d0be64f84cc1a83c75be5d0ae456732b731ee3787fbb5e1f54303
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.8-dind-alpine3.13` - linux; amd64

```console
$ docker pull docker@sha256:d1c7515d7ba19c572b6f60ec904cf0a875b3bf60c427205845b5ab7b432b05ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72680575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dc41137f712d794c3471c40b56f946667cfe729e112ebc6f1a824bcc775f679`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:26:39 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 00:26:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:26:40 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 00:26:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 00:26:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 00:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:48 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 00:26:54 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 00:26:55 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 00:26:55 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 00:26:57 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 00:26:57 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:57 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 00:26:57 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 00:26:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:58 GMT
CMD []
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de31523ae09475f6d68e873b416f497c2bd9a92224d9dc9224e1ec4c0a6066e`  
		Last Modified: Wed, 01 Sep 2021 00:27:41 GMT  
		Size: 2.1 MB (2051151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856ddc4bf6a58ca53ceb6444141995979c00718b20dae8c849231fcf9bfae27`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2117e19917ef5839774785d348adb2ff996bccac5f12d461ca21ecfd58283314`  
		Last Modified: Wed, 01 Sep 2021 00:27:51 GMT  
		Size: 61.3 MB (61284048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53eeb058f8c3c25c5b9f9d12769ab386c353b9f48506daae8fdebd88a33a21`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9223565313e3813eda94fc3641a51cdd88a37775e7b9817ada2a57bd45050906`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa82c493f72cf1d33f4a0bd90320bdb1923957f3cb3b0d36596f52bad68ecb4`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5973cffe69ed6ec4ab2e2a3a191794cfba7339588cdbc4f3c6355e040c05fb`  
		Last Modified: Wed, 01 Sep 2021 00:28:13 GMT  
		Size: 6.5 MB (6524532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a47d00d0a33090100f0be8b5d564e20357fa60a275aba922aea6db6fb47531`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ba8a29d06b5993e5468f57fa6a9d0adff807919d6c664b785a96b1fb6a96d8`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 978.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6762b64189d2495a0856c3f7d465d7ad0f91a4e2db42b4093e70c7b55e571211`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.8-dind-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e2c074f5bc12ca897de843ea2a4be80c932562a92fa388759a9e3ca0510f1ebe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66613965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da28e79c019f7bf9d228ccbf4537acc4f791b8c17d88df076532d28c63c57725`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 12:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 12:09:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 12:09:34 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 12:09:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 12:09:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 12:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:39 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 12:09:48 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 12:09:49 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 12:09:49 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 12:09:50 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 12:09:51 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:51 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 12:09:51 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 12:09:51 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:51 GMT
CMD []
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a21b349a3936e2b00dec57a9db1f448fc4a1a7a3f4ce187cab93819f045fb35`  
		Last Modified: Wed, 01 Sep 2021 12:11:04 GMT  
		Size: 2.1 MB (2058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd93908d94fd730b48322ef41072abf6ba75634aeca40153ef133aae9700fbf4`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2566d8104302856d2cfd150c099a6c900ecc92f214478aa574d755afc6ce191`  
		Last Modified: Wed, 01 Sep 2021 12:11:11 GMT  
		Size: 55.4 MB (55420371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0dc4a2cf61d4525db0351dcde1cc47f8005d1f7260470032b1b731c75757f6`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90454e11d6bb4b836cd9f026908873ed60d1f7e76b2cbcde812fcabe652fa8d`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a170ef51809d6a08fc091d84fc936b83c0aa5c141c7d0cf8ec41c885a79808`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0e2259beeaa75ad2e5d9a651083197a65f1cc00f81974fe83c51617cc4c723`  
		Last Modified: Wed, 01 Sep 2021 12:11:33 GMT  
		Size: 6.4 MB (6415767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c21d52d8c2e860c682d8f1c65d2ffdde59adc3fa8885afe8f7ce95d69ca2a25`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c880d1f23bb87b195c065ca4feb4801fded56bc304979b1b896202db7974a3`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 977.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c833ed3f15c1989d0149c5389b60b295a9fb2ab1050d01c3ac94605805737daa`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8-dind-rootless`

```console
$ docker pull docker@sha256:e20d60287be95c73a224d658b455181367f0d6be7e7810cb94e721ad4cb411e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.8-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:33a0761966c87569be2a9763c8c477dd3e8981982c8abc4324c090f9d2478231
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.9 MB (92930272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5357717b590217cbd992209ed6e2fb34e8ba65a74d3a5324c9b916395a15cb1b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:26:39 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 00:26:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:26:40 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 00:26:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 00:26:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 00:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:48 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 00:26:54 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 00:26:55 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 00:26:55 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 00:26:57 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 00:26:57 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:57 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 00:26:57 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 00:26:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:58 GMT
CMD []
# Wed, 01 Sep 2021 00:27:03 GMT
RUN apk add --no-cache iproute2
# Wed, 01 Sep 2021 00:27:03 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Sep 2021 00:27:04 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Sep 2021 00:27:06 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Sep 2021 00:27:07 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Sep 2021 00:27:08 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Sep 2021 00:27:08 GMT
USER rootless
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de31523ae09475f6d68e873b416f497c2bd9a92224d9dc9224e1ec4c0a6066e`  
		Last Modified: Wed, 01 Sep 2021 00:27:41 GMT  
		Size: 2.1 MB (2051151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856ddc4bf6a58ca53ceb6444141995979c00718b20dae8c849231fcf9bfae27`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2117e19917ef5839774785d348adb2ff996bccac5f12d461ca21ecfd58283314`  
		Last Modified: Wed, 01 Sep 2021 00:27:51 GMT  
		Size: 61.3 MB (61284048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53eeb058f8c3c25c5b9f9d12769ab386c353b9f48506daae8fdebd88a33a21`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9223565313e3813eda94fc3641a51cdd88a37775e7b9817ada2a57bd45050906`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa82c493f72cf1d33f4a0bd90320bdb1923957f3cb3b0d36596f52bad68ecb4`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5973cffe69ed6ec4ab2e2a3a191794cfba7339588cdbc4f3c6355e040c05fb`  
		Last Modified: Wed, 01 Sep 2021 00:28:13 GMT  
		Size: 6.5 MB (6524532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a47d00d0a33090100f0be8b5d564e20357fa60a275aba922aea6db6fb47531`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ba8a29d06b5993e5468f57fa6a9d0adff807919d6c664b785a96b1fb6a96d8`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 978.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6762b64189d2495a0856c3f7d465d7ad0f91a4e2db42b4093e70c7b55e571211`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62dbc14ca68582d0028413d0826f71ced2423d092126de153c91bbf05e4c98fa`  
		Last Modified: Wed, 01 Sep 2021 00:28:35 GMT  
		Size: 1.1 MB (1131899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2498ce93d923f17fb67004858df28e840d729cf6e6fbdfa82ed3c82679ebe4`  
		Last Modified: Wed, 01 Sep 2021 00:28:34 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64015873fa22ddcd58c65fa437669d9153f1a1fd72fd3a43dbd6873f129461b9`  
		Last Modified: Wed, 01 Sep 2021 00:28:35 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcf73021c4287b49de963988902f36818158f72e0ccd6e3b93af6bb3f4e7ef9`  
		Last Modified: Wed, 01 Sep 2021 00:28:39 GMT  
		Size: 19.1 MB (19116093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57ea275b05bd4bf7a61d8bc934c3d72b3d30ae866ed920fdd7d0a5d06933c0d`  
		Last Modified: Wed, 01 Sep 2021 00:28:34 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.8-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:b598f87e3cc82f736a2eeca9070c755d210c1e07e781dab8d10b4de0f667f70e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.9 MB (88863616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fd63c6c9164195ca3489088ce1c8c64b49592ed1226e03c7d92022039060851`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 12:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 12:09:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 12:09:34 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 12:09:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 12:09:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 12:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:39 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 12:09:48 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 12:09:49 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 12:09:49 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 12:09:50 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 12:09:51 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:51 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 12:09:51 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 12:09:51 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:51 GMT
CMD []
# Wed, 01 Sep 2021 12:09:59 GMT
RUN apk add --no-cache iproute2
# Wed, 01 Sep 2021 12:10:00 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Sep 2021 12:10:00 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Sep 2021 12:10:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Sep 2021 12:10:04 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Sep 2021 12:10:04 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Sep 2021 12:10:04 GMT
USER rootless
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a21b349a3936e2b00dec57a9db1f448fc4a1a7a3f4ce187cab93819f045fb35`  
		Last Modified: Wed, 01 Sep 2021 12:11:04 GMT  
		Size: 2.1 MB (2058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd93908d94fd730b48322ef41072abf6ba75634aeca40153ef133aae9700fbf4`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2566d8104302856d2cfd150c099a6c900ecc92f214478aa574d755afc6ce191`  
		Last Modified: Wed, 01 Sep 2021 12:11:11 GMT  
		Size: 55.4 MB (55420371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0dc4a2cf61d4525db0351dcde1cc47f8005d1f7260470032b1b731c75757f6`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90454e11d6bb4b836cd9f026908873ed60d1f7e76b2cbcde812fcabe652fa8d`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a170ef51809d6a08fc091d84fc936b83c0aa5c141c7d0cf8ec41c885a79808`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0e2259beeaa75ad2e5d9a651083197a65f1cc00f81974fe83c51617cc4c723`  
		Last Modified: Wed, 01 Sep 2021 12:11:33 GMT  
		Size: 6.4 MB (6415767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c21d52d8c2e860c682d8f1c65d2ffdde59adc3fa8885afe8f7ce95d69ca2a25`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c880d1f23bb87b195c065ca4feb4801fded56bc304979b1b896202db7974a3`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 977.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c833ed3f15c1989d0149c5389b60b295a9fb2ab1050d01c3ac94605805737daa`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a3816659f3ed80691c2440a71c52b701b209b0312b20ab035de66138b7ace4`  
		Last Modified: Wed, 01 Sep 2021 12:11:57 GMT  
		Size: 1.2 MB (1153143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b263473a450858ffea4d4f20398e671f3aed33088ea2f024d5ca85b05d483bc5`  
		Last Modified: Wed, 01 Sep 2021 12:11:56 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5dd74bf9b8a1eeb40d1eb049b50f17d218b6a8d3cda03762604975431b4e3f4`  
		Last Modified: Wed, 01 Sep 2021 12:11:56 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8c4d3ed13e9425941dcc5ec5474591f125fd656353e50ed00a1c285976395d`  
		Last Modified: Wed, 01 Sep 2021 12:12:00 GMT  
		Size: 21.1 MB (21094799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba347b526ac690189b994abf8234c930775ca075b958c325f24ac2c1c4bcf0e`  
		Last Modified: Wed, 01 Sep 2021 12:11:56 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8-git`

```console
$ docker pull docker@sha256:5924323fafec1818770a7b001524ff526ab1865223b214a19055b87195912734
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.8-git` - linux; amd64

```console
$ docker pull docker@sha256:709ceab8cd1164fbf0c03b1991f8f412a1543023548fa7a30de2268d399723aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72553637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d03657b093bb281e2bf0c19460dbf0f73fbf181780da767109363461960b6de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:26:39 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 00:26:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:26:40 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 00:26:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 00:26:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 00:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:48 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 00:27:13 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de31523ae09475f6d68e873b416f497c2bd9a92224d9dc9224e1ec4c0a6066e`  
		Last Modified: Wed, 01 Sep 2021 00:27:41 GMT  
		Size: 2.1 MB (2051151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856ddc4bf6a58ca53ceb6444141995979c00718b20dae8c849231fcf9bfae27`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2117e19917ef5839774785d348adb2ff996bccac5f12d461ca21ecfd58283314`  
		Last Modified: Wed, 01 Sep 2021 00:27:51 GMT  
		Size: 61.3 MB (61284048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53eeb058f8c3c25c5b9f9d12769ab386c353b9f48506daae8fdebd88a33a21`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9223565313e3813eda94fc3641a51cdd88a37775e7b9817ada2a57bd45050906`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa82c493f72cf1d33f4a0bd90320bdb1923957f3cb3b0d36596f52bad68ecb4`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8c9f33643fb8321012f52f6a1ec572b42b9f29dcd29c0dcf2635ad0c9d1911`  
		Last Modified: Wed, 01 Sep 2021 00:29:00 GMT  
		Size: 6.4 MB (6402499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.8-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f250afada2977e1734ed8c977b720466c1fbc738a1e0ccb85ee0e9bf115dbb9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66680653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6314b14754b6270ce0116f6d93d356dab16dcd7a402b233399d25307483f405`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 12:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 12:09:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 12:09:34 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 12:09:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 12:09:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 12:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:39 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 12:10:12 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a21b349a3936e2b00dec57a9db1f448fc4a1a7a3f4ce187cab93819f045fb35`  
		Last Modified: Wed, 01 Sep 2021 12:11:04 GMT  
		Size: 2.1 MB (2058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd93908d94fd730b48322ef41072abf6ba75634aeca40153ef133aae9700fbf4`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2566d8104302856d2cfd150c099a6c900ecc92f214478aa574d755afc6ce191`  
		Last Modified: Wed, 01 Sep 2021 12:11:11 GMT  
		Size: 55.4 MB (55420371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0dc4a2cf61d4525db0351dcde1cc47f8005d1f7260470032b1b731c75757f6`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90454e11d6bb4b836cd9f026908873ed60d1f7e76b2cbcde812fcabe652fa8d`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a170ef51809d6a08fc091d84fc936b83c0aa5c141c7d0cf8ec41c885a79808`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d37843d9fbf619a9dab1b56a4e2582d767a5106ed2fa0c97f5c1cc3c23e18b`  
		Last Modified: Wed, 01 Sep 2021 12:12:21 GMT  
		Size: 6.5 MB (6487357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8-windowsservercore`

```console
$ docker pull docker@sha256:81d849a5208118837827efb4f0433db49a305260c37f83ff813590c03521247f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `docker:20.10.8-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull docker@sha256:a86536c27f22717fed9d5bcb2ff43eb82f0c2e7eb602d6b9c5d714cd0b706e9a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737269694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e594329f431fd456d89c771444f5e662730713ccd58a9d03b52796bd7fa42e35`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 24 Aug 2021 23:23:49 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 24 Aug 2021 23:23:52 GMT
ENV DOCKER_VERSION=20.10.8
# Tue, 24 Aug 2021 23:23:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Tue, 24 Aug 2021 23:24:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c4896faf56da9e635d1215c12a54c8734e695682b57d6e038ca62fd90b532b`  
		Last Modified: Tue, 24 Aug 2021 23:25:13 GMT  
		Size: 378.4 KB (378370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe49ef5983ec79b546f9ba4e76c016df80499c33627052d1101b851ffb7b4fde`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8baf6cf9c02dbd2217455c62d5ee255fd65036a9a442d0d4794abb2fa68c59`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0b72a29873171e2e2cfc43d555ef003e482ffe643396157ba76e4b22ab3017`  
		Last Modified: Tue, 24 Aug 2021 23:26:06 GMT  
		Size: 50.9 MB (50889387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8-windowsservercore-1809`

```console
$ docker pull docker@sha256:81d849a5208118837827efb4f0433db49a305260c37f83ff813590c03521247f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `docker:20.10.8-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull docker@sha256:a86536c27f22717fed9d5bcb2ff43eb82f0c2e7eb602d6b9c5d714cd0b706e9a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737269694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e594329f431fd456d89c771444f5e662730713ccd58a9d03b52796bd7fa42e35`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 24 Aug 2021 23:23:49 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 24 Aug 2021 23:23:52 GMT
ENV DOCKER_VERSION=20.10.8
# Tue, 24 Aug 2021 23:23:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Tue, 24 Aug 2021 23:24:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c4896faf56da9e635d1215c12a54c8734e695682b57d6e038ca62fd90b532b`  
		Last Modified: Tue, 24 Aug 2021 23:25:13 GMT  
		Size: 378.4 KB (378370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe49ef5983ec79b546f9ba4e76c016df80499c33627052d1101b851ffb7b4fde`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8baf6cf9c02dbd2217455c62d5ee255fd65036a9a442d0d4794abb2fa68c59`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0b72a29873171e2e2cfc43d555ef003e482ffe643396157ba76e4b22ab3017`  
		Last Modified: Tue, 24 Aug 2021 23:26:06 GMT  
		Size: 50.9 MB (50889387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:930d9041e55d0be64f84cc1a83c75be5d0ae456732b731ee3787fbb5e1f54303
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:d1c7515d7ba19c572b6f60ec904cf0a875b3bf60c427205845b5ab7b432b05ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72680575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dc41137f712d794c3471c40b56f946667cfe729e112ebc6f1a824bcc775f679`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:26:39 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 00:26:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:26:40 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 00:26:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 00:26:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 00:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:48 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 00:26:54 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 00:26:55 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 00:26:55 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 00:26:57 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 00:26:57 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:57 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 00:26:57 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 00:26:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:58 GMT
CMD []
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de31523ae09475f6d68e873b416f497c2bd9a92224d9dc9224e1ec4c0a6066e`  
		Last Modified: Wed, 01 Sep 2021 00:27:41 GMT  
		Size: 2.1 MB (2051151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856ddc4bf6a58ca53ceb6444141995979c00718b20dae8c849231fcf9bfae27`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2117e19917ef5839774785d348adb2ff996bccac5f12d461ca21ecfd58283314`  
		Last Modified: Wed, 01 Sep 2021 00:27:51 GMT  
		Size: 61.3 MB (61284048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53eeb058f8c3c25c5b9f9d12769ab386c353b9f48506daae8fdebd88a33a21`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9223565313e3813eda94fc3641a51cdd88a37775e7b9817ada2a57bd45050906`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa82c493f72cf1d33f4a0bd90320bdb1923957f3cb3b0d36596f52bad68ecb4`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5973cffe69ed6ec4ab2e2a3a191794cfba7339588cdbc4f3c6355e040c05fb`  
		Last Modified: Wed, 01 Sep 2021 00:28:13 GMT  
		Size: 6.5 MB (6524532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a47d00d0a33090100f0be8b5d564e20357fa60a275aba922aea6db6fb47531`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ba8a29d06b5993e5468f57fa6a9d0adff807919d6c664b785a96b1fb6a96d8`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 978.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6762b64189d2495a0856c3f7d465d7ad0f91a4e2db42b4093e70c7b55e571211`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e2c074f5bc12ca897de843ea2a4be80c932562a92fa388759a9e3ca0510f1ebe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66613965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da28e79c019f7bf9d228ccbf4537acc4f791b8c17d88df076532d28c63c57725`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 12:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 12:09:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 12:09:34 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 12:09:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 12:09:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 12:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:39 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 12:09:48 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 12:09:49 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 12:09:49 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 12:09:50 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 12:09:51 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:51 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 12:09:51 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 12:09:51 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:51 GMT
CMD []
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a21b349a3936e2b00dec57a9db1f448fc4a1a7a3f4ce187cab93819f045fb35`  
		Last Modified: Wed, 01 Sep 2021 12:11:04 GMT  
		Size: 2.1 MB (2058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd93908d94fd730b48322ef41072abf6ba75634aeca40153ef133aae9700fbf4`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2566d8104302856d2cfd150c099a6c900ecc92f214478aa574d755afc6ce191`  
		Last Modified: Wed, 01 Sep 2021 12:11:11 GMT  
		Size: 55.4 MB (55420371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0dc4a2cf61d4525db0351dcde1cc47f8005d1f7260470032b1b731c75757f6`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90454e11d6bb4b836cd9f026908873ed60d1f7e76b2cbcde812fcabe652fa8d`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a170ef51809d6a08fc091d84fc936b83c0aa5c141c7d0cf8ec41c885a79808`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0e2259beeaa75ad2e5d9a651083197a65f1cc00f81974fe83c51617cc4c723`  
		Last Modified: Wed, 01 Sep 2021 12:11:33 GMT  
		Size: 6.4 MB (6415767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c21d52d8c2e860c682d8f1c65d2ffdde59adc3fa8885afe8f7ce95d69ca2a25`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c880d1f23bb87b195c065ca4feb4801fded56bc304979b1b896202db7974a3`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 977.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c833ed3f15c1989d0149c5389b60b295a9fb2ab1050d01c3ac94605805737daa`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:e20d60287be95c73a224d658b455181367f0d6be7e7810cb94e721ad4cb411e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:33a0761966c87569be2a9763c8c477dd3e8981982c8abc4324c090f9d2478231
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.9 MB (92930272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5357717b590217cbd992209ed6e2fb34e8ba65a74d3a5324c9b916395a15cb1b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:26:39 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 00:26:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:26:40 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 00:26:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 00:26:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 00:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:48 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 00:26:54 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 00:26:55 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 00:26:55 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 00:26:57 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 00:26:57 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:57 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 00:26:57 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 00:26:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:58 GMT
CMD []
# Wed, 01 Sep 2021 00:27:03 GMT
RUN apk add --no-cache iproute2
# Wed, 01 Sep 2021 00:27:03 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Sep 2021 00:27:04 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Sep 2021 00:27:06 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Sep 2021 00:27:07 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Sep 2021 00:27:08 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Sep 2021 00:27:08 GMT
USER rootless
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de31523ae09475f6d68e873b416f497c2bd9a92224d9dc9224e1ec4c0a6066e`  
		Last Modified: Wed, 01 Sep 2021 00:27:41 GMT  
		Size: 2.1 MB (2051151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856ddc4bf6a58ca53ceb6444141995979c00718b20dae8c849231fcf9bfae27`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2117e19917ef5839774785d348adb2ff996bccac5f12d461ca21ecfd58283314`  
		Last Modified: Wed, 01 Sep 2021 00:27:51 GMT  
		Size: 61.3 MB (61284048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53eeb058f8c3c25c5b9f9d12769ab386c353b9f48506daae8fdebd88a33a21`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9223565313e3813eda94fc3641a51cdd88a37775e7b9817ada2a57bd45050906`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa82c493f72cf1d33f4a0bd90320bdb1923957f3cb3b0d36596f52bad68ecb4`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5973cffe69ed6ec4ab2e2a3a191794cfba7339588cdbc4f3c6355e040c05fb`  
		Last Modified: Wed, 01 Sep 2021 00:28:13 GMT  
		Size: 6.5 MB (6524532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a47d00d0a33090100f0be8b5d564e20357fa60a275aba922aea6db6fb47531`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ba8a29d06b5993e5468f57fa6a9d0adff807919d6c664b785a96b1fb6a96d8`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 978.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6762b64189d2495a0856c3f7d465d7ad0f91a4e2db42b4093e70c7b55e571211`  
		Last Modified: Wed, 01 Sep 2021 00:28:11 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62dbc14ca68582d0028413d0826f71ced2423d092126de153c91bbf05e4c98fa`  
		Last Modified: Wed, 01 Sep 2021 00:28:35 GMT  
		Size: 1.1 MB (1131899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2498ce93d923f17fb67004858df28e840d729cf6e6fbdfa82ed3c82679ebe4`  
		Last Modified: Wed, 01 Sep 2021 00:28:34 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64015873fa22ddcd58c65fa437669d9153f1a1fd72fd3a43dbd6873f129461b9`  
		Last Modified: Wed, 01 Sep 2021 00:28:35 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcf73021c4287b49de963988902f36818158f72e0ccd6e3b93af6bb3f4e7ef9`  
		Last Modified: Wed, 01 Sep 2021 00:28:39 GMT  
		Size: 19.1 MB (19116093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57ea275b05bd4bf7a61d8bc934c3d72b3d30ae866ed920fdd7d0a5d06933c0d`  
		Last Modified: Wed, 01 Sep 2021 00:28:34 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:b598f87e3cc82f736a2eeca9070c755d210c1e07e781dab8d10b4de0f667f70e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.9 MB (88863616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fd63c6c9164195ca3489088ce1c8c64b49592ed1226e03c7d92022039060851`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 12:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 12:09:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 12:09:34 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 12:09:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 12:09:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 12:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:39 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 12:09:48 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 12:09:49 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 12:09:49 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 12:09:50 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 12:09:51 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:51 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 12:09:51 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 12:09:51 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:51 GMT
CMD []
# Wed, 01 Sep 2021 12:09:59 GMT
RUN apk add --no-cache iproute2
# Wed, 01 Sep 2021 12:10:00 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Sep 2021 12:10:00 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Sep 2021 12:10:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Sep 2021 12:10:04 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Sep 2021 12:10:04 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Sep 2021 12:10:04 GMT
USER rootless
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a21b349a3936e2b00dec57a9db1f448fc4a1a7a3f4ce187cab93819f045fb35`  
		Last Modified: Wed, 01 Sep 2021 12:11:04 GMT  
		Size: 2.1 MB (2058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd93908d94fd730b48322ef41072abf6ba75634aeca40153ef133aae9700fbf4`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2566d8104302856d2cfd150c099a6c900ecc92f214478aa574d755afc6ce191`  
		Last Modified: Wed, 01 Sep 2021 12:11:11 GMT  
		Size: 55.4 MB (55420371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0dc4a2cf61d4525db0351dcde1cc47f8005d1f7260470032b1b731c75757f6`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90454e11d6bb4b836cd9f026908873ed60d1f7e76b2cbcde812fcabe652fa8d`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a170ef51809d6a08fc091d84fc936b83c0aa5c141c7d0cf8ec41c885a79808`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0e2259beeaa75ad2e5d9a651083197a65f1cc00f81974fe83c51617cc4c723`  
		Last Modified: Wed, 01 Sep 2021 12:11:33 GMT  
		Size: 6.4 MB (6415767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c21d52d8c2e860c682d8f1c65d2ffdde59adc3fa8885afe8f7ce95d69ca2a25`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c880d1f23bb87b195c065ca4feb4801fded56bc304979b1b896202db7974a3`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 977.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c833ed3f15c1989d0149c5389b60b295a9fb2ab1050d01c3ac94605805737daa`  
		Last Modified: Wed, 01 Sep 2021 12:11:32 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a3816659f3ed80691c2440a71c52b701b209b0312b20ab035de66138b7ace4`  
		Last Modified: Wed, 01 Sep 2021 12:11:57 GMT  
		Size: 1.2 MB (1153143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b263473a450858ffea4d4f20398e671f3aed33088ea2f024d5ca85b05d483bc5`  
		Last Modified: Wed, 01 Sep 2021 12:11:56 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5dd74bf9b8a1eeb40d1eb049b50f17d218b6a8d3cda03762604975431b4e3f4`  
		Last Modified: Wed, 01 Sep 2021 12:11:56 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8c4d3ed13e9425941dcc5ec5474591f125fd656353e50ed00a1c285976395d`  
		Last Modified: Wed, 01 Sep 2021 12:12:00 GMT  
		Size: 21.1 MB (21094799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba347b526ac690189b994abf8234c930775ca075b958c325f24ac2c1c4bcf0e`  
		Last Modified: Wed, 01 Sep 2021 12:11:56 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:5924323fafec1818770a7b001524ff526ab1865223b214a19055b87195912734
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:709ceab8cd1164fbf0c03b1991f8f412a1543023548fa7a30de2268d399723aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72553637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d03657b093bb281e2bf0c19460dbf0f73fbf181780da767109363461960b6de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:26:39 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 00:26:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:26:40 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 00:26:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 00:26:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 00:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:48 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 00:27:13 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de31523ae09475f6d68e873b416f497c2bd9a92224d9dc9224e1ec4c0a6066e`  
		Last Modified: Wed, 01 Sep 2021 00:27:41 GMT  
		Size: 2.1 MB (2051151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856ddc4bf6a58ca53ceb6444141995979c00718b20dae8c849231fcf9bfae27`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2117e19917ef5839774785d348adb2ff996bccac5f12d461ca21ecfd58283314`  
		Last Modified: Wed, 01 Sep 2021 00:27:51 GMT  
		Size: 61.3 MB (61284048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53eeb058f8c3c25c5b9f9d12769ab386c353b9f48506daae8fdebd88a33a21`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9223565313e3813eda94fc3641a51cdd88a37775e7b9817ada2a57bd45050906`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa82c493f72cf1d33f4a0bd90320bdb1923957f3cb3b0d36596f52bad68ecb4`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8c9f33643fb8321012f52f6a1ec572b42b9f29dcd29c0dcf2635ad0c9d1911`  
		Last Modified: Wed, 01 Sep 2021 00:29:00 GMT  
		Size: 6.4 MB (6402499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f250afada2977e1734ed8c977b720466c1fbc738a1e0ccb85ee0e9bf115dbb9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66680653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6314b14754b6270ce0116f6d93d356dab16dcd7a402b233399d25307483f405`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 12:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 12:09:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 12:09:34 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 12:09:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 12:09:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 12:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:39 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 12:10:12 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a21b349a3936e2b00dec57a9db1f448fc4a1a7a3f4ce187cab93819f045fb35`  
		Last Modified: Wed, 01 Sep 2021 12:11:04 GMT  
		Size: 2.1 MB (2058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd93908d94fd730b48322ef41072abf6ba75634aeca40153ef133aae9700fbf4`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2566d8104302856d2cfd150c099a6c900ecc92f214478aa574d755afc6ce191`  
		Last Modified: Wed, 01 Sep 2021 12:11:11 GMT  
		Size: 55.4 MB (55420371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0dc4a2cf61d4525db0351dcde1cc47f8005d1f7260470032b1b731c75757f6`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90454e11d6bb4b836cd9f026908873ed60d1f7e76b2cbcde812fcabe652fa8d`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a170ef51809d6a08fc091d84fc936b83c0aa5c141c7d0cf8ec41c885a79808`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d37843d9fbf619a9dab1b56a4e2582d767a5106ed2fa0c97f5c1cc3c23e18b`  
		Last Modified: Wed, 01 Sep 2021 12:12:21 GMT  
		Size: 6.5 MB (6487357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:e496f1729171f76a9b1a9b2a99431003e8e89e67168ed411ad25b95a73445d13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:35f612c47195c6e7c1e9ecc80c1b1a00402f3c039e768dd08b2ddb237fd5d0ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66151138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f67ee0b7de2f5cca0d60fe996f082ee6795d35fdd0c7823325b0f7855f57c342`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:26:39 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 00:26:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:26:40 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 00:26:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 00:26:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 00:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:48 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de31523ae09475f6d68e873b416f497c2bd9a92224d9dc9224e1ec4c0a6066e`  
		Last Modified: Wed, 01 Sep 2021 00:27:41 GMT  
		Size: 2.1 MB (2051151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856ddc4bf6a58ca53ceb6444141995979c00718b20dae8c849231fcf9bfae27`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2117e19917ef5839774785d348adb2ff996bccac5f12d461ca21ecfd58283314`  
		Last Modified: Wed, 01 Sep 2021 00:27:51 GMT  
		Size: 61.3 MB (61284048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53eeb058f8c3c25c5b9f9d12769ab386c353b9f48506daae8fdebd88a33a21`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9223565313e3813eda94fc3641a51cdd88a37775e7b9817ada2a57bd45050906`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa82c493f72cf1d33f4a0bd90320bdb1923957f3cb3b0d36596f52bad68ecb4`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:cbad49f1637b08b224d3bb36e840cc869624bbe08b359763bd6ada7026165403
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60193296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51720a73bc2639cb36d62b9239b6db9903861e48a613e6202cfc1224065d5c3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 12:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 12:09:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 12:09:34 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 12:09:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 12:09:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 12:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:39 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a21b349a3936e2b00dec57a9db1f448fc4a1a7a3f4ce187cab93819f045fb35`  
		Last Modified: Wed, 01 Sep 2021 12:11:04 GMT  
		Size: 2.1 MB (2058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd93908d94fd730b48322ef41072abf6ba75634aeca40153ef133aae9700fbf4`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2566d8104302856d2cfd150c099a6c900ecc92f214478aa574d755afc6ce191`  
		Last Modified: Wed, 01 Sep 2021 12:11:11 GMT  
		Size: 55.4 MB (55420371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0dc4a2cf61d4525db0351dcde1cc47f8005d1f7260470032b1b731c75757f6`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90454e11d6bb4b836cd9f026908873ed60d1f7e76b2cbcde812fcabe652fa8d`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a170ef51809d6a08fc091d84fc936b83c0aa5c141c7d0cf8ec41c885a79808`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore`

```console
$ docker pull docker@sha256:81d849a5208118837827efb4f0433db49a305260c37f83ff813590c03521247f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `docker:windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull docker@sha256:a86536c27f22717fed9d5bcb2ff43eb82f0c2e7eb602d6b9c5d714cd0b706e9a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737269694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e594329f431fd456d89c771444f5e662730713ccd58a9d03b52796bd7fa42e35`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 24 Aug 2021 23:23:49 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 24 Aug 2021 23:23:52 GMT
ENV DOCKER_VERSION=20.10.8
# Tue, 24 Aug 2021 23:23:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Tue, 24 Aug 2021 23:24:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c4896faf56da9e635d1215c12a54c8734e695682b57d6e038ca62fd90b532b`  
		Last Modified: Tue, 24 Aug 2021 23:25:13 GMT  
		Size: 378.4 KB (378370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe49ef5983ec79b546f9ba4e76c016df80499c33627052d1101b851ffb7b4fde`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8baf6cf9c02dbd2217455c62d5ee255fd65036a9a442d0d4794abb2fa68c59`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0b72a29873171e2e2cfc43d555ef003e482ffe643396157ba76e4b22ab3017`  
		Last Modified: Tue, 24 Aug 2021 23:26:06 GMT  
		Size: 50.9 MB (50889387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:81d849a5208118837827efb4f0433db49a305260c37f83ff813590c03521247f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull docker@sha256:a86536c27f22717fed9d5bcb2ff43eb82f0c2e7eb602d6b9c5d714cd0b706e9a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737269694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e594329f431fd456d89c771444f5e662730713ccd58a9d03b52796bd7fa42e35`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 24 Aug 2021 23:23:49 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 24 Aug 2021 23:23:52 GMT
ENV DOCKER_VERSION=20.10.8
# Tue, 24 Aug 2021 23:23:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Tue, 24 Aug 2021 23:24:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c4896faf56da9e635d1215c12a54c8734e695682b57d6e038ca62fd90b532b`  
		Last Modified: Tue, 24 Aug 2021 23:25:13 GMT  
		Size: 378.4 KB (378370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe49ef5983ec79b546f9ba4e76c016df80499c33627052d1101b851ffb7b4fde`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8baf6cf9c02dbd2217455c62d5ee255fd65036a9a442d0d4794abb2fa68c59`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0b72a29873171e2e2cfc43d555ef003e482ffe643396157ba76e4b22ab3017`  
		Last Modified: Tue, 24 Aug 2021 23:26:06 GMT  
		Size: 50.9 MB (50889387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
