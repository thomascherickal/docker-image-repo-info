<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `docker`

-	[`docker:20`](#docker20)
-	[`docker:20-dind`](#docker20-dind)
-	[`docker:20-dind-rootless`](#docker20-dind-rootless)
-	[`docker:20-git`](#docker20-git)
-	[`docker:20-windowsservercore`](#docker20-windowsservercore)
-	[`docker:20-windowsservercore-1809`](#docker20-windowsservercore-1809)
-	[`docker:20-windowsservercore-ltsc2022`](#docker20-windowsservercore-ltsc2022)
-	[`docker:20.10`](#docker2010)
-	[`docker:20.10-dind`](#docker2010-dind)
-	[`docker:20.10-dind-rootless`](#docker2010-dind-rootless)
-	[`docker:20.10-git`](#docker2010-git)
-	[`docker:20.10-windowsservercore`](#docker2010-windowsservercore)
-	[`docker:20.10-windowsservercore-1809`](#docker2010-windowsservercore-1809)
-	[`docker:20.10-windowsservercore-ltsc2022`](#docker2010-windowsservercore-ltsc2022)
-	[`docker:20.10.13`](#docker201013)
-	[`docker:20.10.13-alpine3.15`](#docker201013-alpine315)
-	[`docker:20.10.13-dind`](#docker201013-dind)
-	[`docker:20.10.13-dind-alpine3.15`](#docker201013-dind-alpine315)
-	[`docker:20.10.13-dind-rootless`](#docker201013-dind-rootless)
-	[`docker:20.10.13-git`](#docker201013-git)
-	[`docker:20.10.13-windowsservercore`](#docker201013-windowsservercore)
-	[`docker:20.10.13-windowsservercore-1809`](#docker201013-windowsservercore-1809)
-	[`docker:20.10.13-windowsservercore-ltsc2022`](#docker201013-windowsservercore-ltsc2022)
-	[`docker:dind`](#dockerdind)
-	[`docker:dind-rootless`](#dockerdind-rootless)
-	[`docker:git`](#dockergit)
-	[`docker:latest`](#dockerlatest)
-	[`docker:windowsservercore`](#dockerwindowsservercore)
-	[`docker:windowsservercore-1809`](#dockerwindowsservercore-1809)
-	[`docker:windowsservercore-ltsc2022`](#dockerwindowsservercore-ltsc2022)

## `docker:20`

```console
$ docker pull docker@sha256:72e87d4f1d2ed054bf9ec48c77dfc546c7e6173fe9b6afd9e80716b9c5ade4bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20` - linux; amd64

```console
$ docker pull docker@sha256:338217655cdf830e6f659207f447776c8debaf1c3cbce0050645c2b621893d6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69413254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6816f070b2395d750ce78e4fbdb7e9df0af63b7686f3063c09e008c2ef1a0036`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Mar 2022 00:19:37 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:19:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Mar 2022 00:19:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Mar 2022 00:19:42 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:42 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Mar 2022 00:19:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Mar 2022 00:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:42 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea03e1895df432fba23ac2810a53a408fa25273ecf001276263d810107e1c81`  
		Last Modified: Wed, 15 Dec 2021 20:20:23 GMT  
		Size: 2.0 MB (1980404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff98835b05535c14c9bd8aa0449fd33d147a58c9a9fe7f21b76137065d0f4c5`  
		Last Modified: Wed, 15 Dec 2021 20:20:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbbd0a7b1dec526be119d73f0018052afa23e65ea79e09049a54a5954f2a374`  
		Last Modified: Fri, 11 Mar 2022 00:20:32 GMT  
		Size: 64.6 MB (64612571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317ecb07c86c68358ba3d763bea251b7baf1befde793d08f074abf2743a388dc`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52850491ed6a707afb12e76035b1a36f408c071e00d1de77b26ec2cb178c9a8a`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb2b84e11d9e63efd7d7cad8459ac6f5326f44d93991a59380b186824079bdf`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:576a187cf88c74c82b1cda12e206a8e20e24633499128894296909a44456f82a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63220789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51ae867936fd1dc5c38dab32635ffb031fba90112aaf70cd838fdf678922f0b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 06:44:43 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 17 Mar 2022 06:44:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 06:44:45 GMT
ENV DOCKER_VERSION=20.10.13
# Thu, 17 Mar 2022 06:44:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Mar 2022 06:44:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Mar 2022 06:44:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:44:51 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Mar 2022 06:44:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Mar 2022 06:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 06:44:54 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bd6b2d67571b28ebbe22152f5536e3cff37d4346bc02a444b2ede9b5d71c6`  
		Last Modified: Thu, 17 Mar 2022 06:46:18 GMT  
		Size: 1.9 MB (1938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadc398c63809a7b7b0d60cee36c1a95c7dd031fb5987cb99246b289df77d64f`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fce163fc9e7e1d8912203364c303838e60da953ed77812572633504c2bd014`  
		Last Modified: Thu, 17 Mar 2022 06:46:25 GMT  
		Size: 58.6 MB (58565248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a0a3a69cb84240c8270720f964d7155438567aa97bb868bfe1adc07b5b977`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8be56eb060db5cad28d2359c143a7a7de20610f090073f5cbd7f1cfeafbd4`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746be13a2cb02a7014e32f66ba9fb3bb10e14bd43af45b7890fb09464fe2a830`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind`

```console
$ docker pull docker@sha256:ca2744235df40f184843b2cb9f0245a6b64ae65065aad30285e80d5a266fe0c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind` - linux; amd64

```console
$ docker pull docker@sha256:34c594c12507d24f66789978a90240d4addf3eb8fce22a7a9157ca9701afd46d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76152892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c05a8c965912fe35df9cce58ddb7aed725fb34d81772761a4ef7a373fd3271c1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Mar 2022 00:19:37 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:19:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Mar 2022 00:19:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Mar 2022 00:19:42 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:42 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Mar 2022 00:19:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Mar 2022 00:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:42 GMT
CMD ["sh"]
# Fri, 11 Mar 2022 00:19:47 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Mar 2022 00:19:48 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Mar 2022 00:19:48 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 11 Mar 2022 00:19:48 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Mar 2022 00:19:48 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:48 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Mar 2022 00:19:49 GMT
EXPOSE 2375 2376
# Fri, 11 Mar 2022 00:19:49 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:49 GMT
CMD []
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea03e1895df432fba23ac2810a53a408fa25273ecf001276263d810107e1c81`  
		Last Modified: Wed, 15 Dec 2021 20:20:23 GMT  
		Size: 2.0 MB (1980404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff98835b05535c14c9bd8aa0449fd33d147a58c9a9fe7f21b76137065d0f4c5`  
		Last Modified: Wed, 15 Dec 2021 20:20:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbbd0a7b1dec526be119d73f0018052afa23e65ea79e09049a54a5954f2a374`  
		Last Modified: Fri, 11 Mar 2022 00:20:32 GMT  
		Size: 64.6 MB (64612571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317ecb07c86c68358ba3d763bea251b7baf1befde793d08f074abf2743a388dc`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52850491ed6a707afb12e76035b1a36f408c071e00d1de77b26ec2cb178c9a8a`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb2b84e11d9e63efd7d7cad8459ac6f5326f44d93991a59380b186824079bdf`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd217e3dc5c63b9a21276d1a8b9b2c0a19dd9aeecf5c242902d63e8dd7c251f`  
		Last Modified: Fri, 11 Mar 2022 00:20:50 GMT  
		Size: 6.7 MB (6734617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f85497bc6212a4fbd95757776ba9f0cfc449ba5ec26f58dc4b48718582d256`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63824672dbc4b8bf906bba2cabad90a9964a4de17f7df52debc99611d2782d66`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330cf4336db2c7c1846de44144ed6eb30ac0942792712aeca3f5b38acbd16933`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 2.7 KB (2747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e6222d4d8b30c439b883f691f52e8e405f6464852c86477f7b1577dee106ee6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69841345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ba71573c3cddc7fe6d1f68e3c7c55e13f7549be38cf07414563df801aa79e1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 06:44:43 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 17 Mar 2022 06:44:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 06:44:45 GMT
ENV DOCKER_VERSION=20.10.13
# Thu, 17 Mar 2022 06:44:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Mar 2022 06:44:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Mar 2022 06:44:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:44:51 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Mar 2022 06:44:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Mar 2022 06:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 06:44:54 GMT
CMD ["sh"]
# Thu, 17 Mar 2022 06:45:06 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 17 Mar 2022 06:45:07 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 17 Mar 2022 06:45:08 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 17 Mar 2022 06:45:09 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 17 Mar 2022 06:45:11 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:45:11 GMT
VOLUME [/var/lib/docker]
# Thu, 17 Mar 2022 06:45:12 GMT
EXPOSE 2375 2376
# Thu, 17 Mar 2022 06:45:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 17 Mar 2022 06:45:14 GMT
CMD []
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bd6b2d67571b28ebbe22152f5536e3cff37d4346bc02a444b2ede9b5d71c6`  
		Last Modified: Thu, 17 Mar 2022 06:46:18 GMT  
		Size: 1.9 MB (1938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadc398c63809a7b7b0d60cee36c1a95c7dd031fb5987cb99246b289df77d64f`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fce163fc9e7e1d8912203364c303838e60da953ed77812572633504c2bd014`  
		Last Modified: Thu, 17 Mar 2022 06:46:25 GMT  
		Size: 58.6 MB (58565248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a0a3a69cb84240c8270720f964d7155438567aa97bb868bfe1adc07b5b977`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8be56eb060db5cad28d2359c143a7a7de20610f090073f5cbd7f1cfeafbd4`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746be13a2cb02a7014e32f66ba9fb3bb10e14bd43af45b7890fb09464fe2a830`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb73bd4ce74defd0741f3f7922ffb261b2f91b45cf97e2225f65aaba2b4c42d6`  
		Last Modified: Thu, 17 Mar 2022 06:46:48 GMT  
		Size: 6.6 MB (6615563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e054635e9f383caa96af63cfbbc71098384c50f5c13efcc785d2a870ed8e4af9`  
		Last Modified: Thu, 17 Mar 2022 06:46:46 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791a50930d17375d4278a896defa85218b579b3efdd1455d1fa503e187676dfb`  
		Last Modified: Thu, 17 Mar 2022 06:46:46 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752ca04529521e0b4db8ded3d79d79f1629c7c725837b87fe79519f64bcb2e05`  
		Last Modified: Thu, 17 Mar 2022 06:46:47 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:e65462ff8bfe7c34478edfb354d6a1b5c03ecf7279212fc54fc54180d2663c2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:6a92617cb4df46747dc2fd832bae2ddda144ab9c1116ea2753df44cb211a55ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 MB (96448562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d466e72290286bcdfbc871e8561fae40d9eef80790216bb18f18b5313b6e088b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Mar 2022 00:19:37 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:19:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Mar 2022 00:19:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Mar 2022 00:19:42 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:42 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Mar 2022 00:19:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Mar 2022 00:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:42 GMT
CMD ["sh"]
# Fri, 11 Mar 2022 00:19:47 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Mar 2022 00:19:48 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Mar 2022 00:19:48 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 11 Mar 2022 00:19:48 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Mar 2022 00:19:48 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:48 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Mar 2022 00:19:49 GMT
EXPOSE 2375 2376
# Fri, 11 Mar 2022 00:19:49 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:49 GMT
CMD []
# Fri, 11 Mar 2022 00:19:52 GMT
RUN apk add --no-cache iproute2
# Fri, 11 Mar 2022 00:19:53 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 11 Mar 2022 00:19:53 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 11 Mar 2022 00:19:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 11 Mar 2022 00:19:57 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 11 Mar 2022 00:19:57 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 11 Mar 2022 00:19:57 GMT
USER rootless
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea03e1895df432fba23ac2810a53a408fa25273ecf001276263d810107e1c81`  
		Last Modified: Wed, 15 Dec 2021 20:20:23 GMT  
		Size: 2.0 MB (1980404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff98835b05535c14c9bd8aa0449fd33d147a58c9a9fe7f21b76137065d0f4c5`  
		Last Modified: Wed, 15 Dec 2021 20:20:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbbd0a7b1dec526be119d73f0018052afa23e65ea79e09049a54a5954f2a374`  
		Last Modified: Fri, 11 Mar 2022 00:20:32 GMT  
		Size: 64.6 MB (64612571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317ecb07c86c68358ba3d763bea251b7baf1befde793d08f074abf2743a388dc`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52850491ed6a707afb12e76035b1a36f408c071e00d1de77b26ec2cb178c9a8a`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb2b84e11d9e63efd7d7cad8459ac6f5326f44d93991a59380b186824079bdf`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd217e3dc5c63b9a21276d1a8b9b2c0a19dd9aeecf5c242902d63e8dd7c251f`  
		Last Modified: Fri, 11 Mar 2022 00:20:50 GMT  
		Size: 6.7 MB (6734617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f85497bc6212a4fbd95757776ba9f0cfc449ba5ec26f58dc4b48718582d256`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63824672dbc4b8bf906bba2cabad90a9964a4de17f7df52debc99611d2782d66`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330cf4336db2c7c1846de44144ed6eb30ac0942792712aeca3f5b38acbd16933`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 2.7 KB (2747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9243af40d6dedb8bec94753185a0e50302ceca90029164040a3c567cfe6649ed`  
		Last Modified: Fri, 11 Mar 2022 00:21:10 GMT  
		Size: 1.2 MB (1162145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad945e48854711031ed9581488dcd35e6a7281c7cef4273cc6c4fd49fb768ebd`  
		Last Modified: Fri, 11 Mar 2022 00:21:08 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dbac2c48de1cb6054512bc0b3967aa776ed177ce538b1901e10390d2e83250`  
		Last Modified: Fri, 11 Mar 2022 00:21:09 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2445b41c3397a2f9da27c43cc92a64a2e373b418307bc1a0322072b6f87096`  
		Last Modified: Fri, 11 Mar 2022 00:21:12 GMT  
		Size: 19.1 MB (19131808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ec68c91cc2997a8e6a4a961bc06b2a2af234d24e8f116a0ba3a2e0305beaf7`  
		Last Modified: Fri, 11 Mar 2022 00:21:08 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:fb00e978daa05ad0619ff4b0bbd52dd7c000a39954746498aadc6d94ac35194a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92132138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20955ed3fe29f7eca363024931545542a3e3bcaddd6de747255b806cb75f8c3d`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 06:44:43 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 17 Mar 2022 06:44:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 06:44:45 GMT
ENV DOCKER_VERSION=20.10.13
# Thu, 17 Mar 2022 06:44:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Mar 2022 06:44:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Mar 2022 06:44:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:44:51 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Mar 2022 06:44:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Mar 2022 06:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 06:44:54 GMT
CMD ["sh"]
# Thu, 17 Mar 2022 06:45:06 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 17 Mar 2022 06:45:07 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 17 Mar 2022 06:45:08 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 17 Mar 2022 06:45:09 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 17 Mar 2022 06:45:11 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:45:11 GMT
VOLUME [/var/lib/docker]
# Thu, 17 Mar 2022 06:45:12 GMT
EXPOSE 2375 2376
# Thu, 17 Mar 2022 06:45:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 17 Mar 2022 06:45:14 GMT
CMD []
# Thu, 17 Mar 2022 06:45:22 GMT
RUN apk add --no-cache iproute2
# Thu, 17 Mar 2022 06:45:23 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 17 Mar 2022 06:45:24 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 17 Mar 2022 06:45:27 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 17 Mar 2022 06:45:27 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 17 Mar 2022 06:45:28 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 17 Mar 2022 06:45:29 GMT
USER rootless
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bd6b2d67571b28ebbe22152f5536e3cff37d4346bc02a444b2ede9b5d71c6`  
		Last Modified: Thu, 17 Mar 2022 06:46:18 GMT  
		Size: 1.9 MB (1938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadc398c63809a7b7b0d60cee36c1a95c7dd031fb5987cb99246b289df77d64f`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fce163fc9e7e1d8912203364c303838e60da953ed77812572633504c2bd014`  
		Last Modified: Thu, 17 Mar 2022 06:46:25 GMT  
		Size: 58.6 MB (58565248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a0a3a69cb84240c8270720f964d7155438567aa97bb868bfe1adc07b5b977`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8be56eb060db5cad28d2359c143a7a7de20610f090073f5cbd7f1cfeafbd4`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746be13a2cb02a7014e32f66ba9fb3bb10e14bd43af45b7890fb09464fe2a830`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb73bd4ce74defd0741f3f7922ffb261b2f91b45cf97e2225f65aaba2b4c42d6`  
		Last Modified: Thu, 17 Mar 2022 06:46:48 GMT  
		Size: 6.6 MB (6615563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e054635e9f383caa96af63cfbbc71098384c50f5c13efcc785d2a870ed8e4af9`  
		Last Modified: Thu, 17 Mar 2022 06:46:46 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791a50930d17375d4278a896defa85218b579b3efdd1455d1fa503e187676dfb`  
		Last Modified: Thu, 17 Mar 2022 06:46:46 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752ca04529521e0b4db8ded3d79d79f1629c7c725837b87fe79519f64bcb2e05`  
		Last Modified: Thu, 17 Mar 2022 06:46:47 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b68e435beb33fd13cba08b839c86323a9ea7d3c280f4e09040d67dd21cfd835`  
		Last Modified: Thu, 17 Mar 2022 06:47:11 GMT  
		Size: 1.2 MB (1177952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f4ab31ae44292e2bfb84410de85f6a729607613d6dbef35902577fcbe78e4f`  
		Last Modified: Thu, 17 Mar 2022 06:47:10 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72e8ed3a93a11307aba41a4d0f7ffb6302f7de9886d46bf2562f06ab3e01e3f`  
		Last Modified: Thu, 17 Mar 2022 06:47:10 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768a72d3947b3532412cc42dd744996a22bf0574cebf60ac1119be3ca7530922`  
		Last Modified: Thu, 17 Mar 2022 06:47:14 GMT  
		Size: 21.1 MB (21111220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dec4d02116a97f8282cc9d24eaf55d48d469e3ad232980a8724940ba2a07ed3`  
		Last Modified: Thu, 17 Mar 2022 06:47:10 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-git`

```console
$ docker pull docker@sha256:5ec008af09dcdc65abc239b6f492af27f37a9c7ec94148f40703ca622a5faba5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-git` - linux; amd64

```console
$ docker pull docker@sha256:7383e8c2efcd6846670dd96ca1b6af84b7a4098fd778b85cee0ae2739301a79c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76237387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f328899fc7a17e58951f5523f603df43687ea162ad1f8f04eed66b876e9480ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Mar 2022 00:19:37 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:19:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Mar 2022 00:19:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Mar 2022 00:19:42 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:42 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Mar 2022 00:19:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Mar 2022 00:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:42 GMT
CMD ["sh"]
# Fri, 11 Mar 2022 00:20:00 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea03e1895df432fba23ac2810a53a408fa25273ecf001276263d810107e1c81`  
		Last Modified: Wed, 15 Dec 2021 20:20:23 GMT  
		Size: 2.0 MB (1980404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff98835b05535c14c9bd8aa0449fd33d147a58c9a9fe7f21b76137065d0f4c5`  
		Last Modified: Wed, 15 Dec 2021 20:20:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbbd0a7b1dec526be119d73f0018052afa23e65ea79e09049a54a5954f2a374`  
		Last Modified: Fri, 11 Mar 2022 00:20:32 GMT  
		Size: 64.6 MB (64612571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317ecb07c86c68358ba3d763bea251b7baf1befde793d08f074abf2743a388dc`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52850491ed6a707afb12e76035b1a36f408c071e00d1de77b26ec2cb178c9a8a`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb2b84e11d9e63efd7d7cad8459ac6f5326f44d93991a59380b186824079bdf`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc827496373a4a4176b9c5e48d8ea6bb5823b745c62a5ddd68e6b201ae7341d`  
		Last Modified: Fri, 11 Mar 2022 00:21:30 GMT  
		Size: 6.8 MB (6824133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:72b64e64f292fcc354064aff807584ba6aa24c62dcaacd0f4180974d732d7c33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70153837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a742244413c82313c84ffc8e2aae4a5e443443e2e7c6283b00bc9d89c10d767`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 06:44:43 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 17 Mar 2022 06:44:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 06:44:45 GMT
ENV DOCKER_VERSION=20.10.13
# Thu, 17 Mar 2022 06:44:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Mar 2022 06:44:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Mar 2022 06:44:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:44:51 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Mar 2022 06:44:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Mar 2022 06:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 06:44:54 GMT
CMD ["sh"]
# Thu, 17 Mar 2022 06:45:36 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bd6b2d67571b28ebbe22152f5536e3cff37d4346bc02a444b2ede9b5d71c6`  
		Last Modified: Thu, 17 Mar 2022 06:46:18 GMT  
		Size: 1.9 MB (1938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadc398c63809a7b7b0d60cee36c1a95c7dd031fb5987cb99246b289df77d64f`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fce163fc9e7e1d8912203364c303838e60da953ed77812572633504c2bd014`  
		Last Modified: Thu, 17 Mar 2022 06:46:25 GMT  
		Size: 58.6 MB (58565248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a0a3a69cb84240c8270720f964d7155438567aa97bb868bfe1adc07b5b977`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8be56eb060db5cad28d2359c143a7a7de20610f090073f5cbd7f1cfeafbd4`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746be13a2cb02a7014e32f66ba9fb3bb10e14bd43af45b7890fb09464fe2a830`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2716e163322a30318e4b5622ac98de0815fd95f93070ec60e4ee6ea3a3f85b59`  
		Last Modified: Thu, 17 Mar 2022 06:47:35 GMT  
		Size: 6.9 MB (6933048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore`

```console
$ docker pull docker@sha256:998f6c6a8ca0e9871ae959625b33ded24ef0dbf102278d815ca5c2ca91708e33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.587; amd64
	-	windows version 10.0.17763.2686; amd64

### `docker:20-windowsservercore` - windows version 10.0.20348.587; amd64

```console
$ docker pull docker@sha256:ef007d39e5aa17f57f4ad75825febf433ea51d70fde48d5b40fea73307ffe3e8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2275653963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b8f4e76e84e2dd1842160718087208b325a794ca03ff7f14aac4b0b7b4694e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 03 Mar 2022 05:02:11 GMT
RUN Install update ltsc2022-amd64
# Tue, 08 Mar 2022 19:26:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:55:44 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 11 Mar 2022 00:15:07 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:15:08 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.13.zip
# Fri, 11 Mar 2022 00:15:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:037d5740b40414bc505c21324142a1cd3eab10c176189a9a74d1a90354ac7cd4`  
		Size: 969.5 MB (969547968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d58ba398110c3f761c6307a5621ec218b8593ba8b07b734436bcdd8d07a23e08`  
		Last Modified: Tue, 08 Mar 2022 20:00:31 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfaa4c2639ecdc27410a570e2dcb2efe02bcbec37d6ad750d15a97aac6990236`  
		Last Modified: Wed, 09 Mar 2022 18:59:14 GMT  
		Size: 598.3 KB (598260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0e605541ab33ab5774f3b41805cecf36dffbc7d02428d5bed5cbd86e1a7a0e`  
		Last Modified: Fri, 11 Mar 2022 00:17:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d060c5ba2630e8637c44694ed52a53850d5dd01c5f55f7b49493d202f48a5565`  
		Last Modified: Fri, 11 Mar 2022 00:17:32 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01c70e5c0d32c6abc7141a56d515a00df83a0786489da36fe453fa7a2b67d6d`  
		Last Modified: Fri, 11 Mar 2022 00:18:31 GMT  
		Size: 53.8 MB (53804674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull docker@sha256:11fa18bbbc94e9342dea2f011d4ac7dc0e674553a427eeac46962b7fd3bb7654
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2769425405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57844be2857bef97ed862468dd3a51e9d0dea7c7b269a9efe192aa526df18835`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:57:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 11 Mar 2022 00:15:45 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:15:46 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.13.zip
# Fri, 11 Mar 2022 00:16:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc556e75fc2ee0a56749fd9ec604591d58c7dcfbf6ddd1389aedfe0faa926127`  
		Last Modified: Wed, 09 Mar 2022 19:00:27 GMT  
		Size: 353.8 KB (353787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fcaecf749d555a0d83fad08ace6a7998307b24f4fecf9632bbfe013d112577`  
		Last Modified: Fri, 11 Mar 2022 00:18:44 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d880c105cf28c98f7d9613f331846e631375f272f037491c61f85d4cac54220d`  
		Last Modified: Fri, 11 Mar 2022 00:18:44 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2570e437e8fcb2cb9d3d91f7edafcf34ff2c23106a9aacbea7701ba1fce8d2b`  
		Last Modified: Fri, 11 Mar 2022 00:18:56 GMT  
		Size: 53.6 MB (53615032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-1809`

```console
$ docker pull docker@sha256:2351bc67908336460d6d176ad7237bd4ce87e3906d102f82fa7b9464d08f8a83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `docker:20-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull docker@sha256:11fa18bbbc94e9342dea2f011d4ac7dc0e674553a427eeac46962b7fd3bb7654
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2769425405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57844be2857bef97ed862468dd3a51e9d0dea7c7b269a9efe192aa526df18835`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:57:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 11 Mar 2022 00:15:45 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:15:46 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.13.zip
# Fri, 11 Mar 2022 00:16:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc556e75fc2ee0a56749fd9ec604591d58c7dcfbf6ddd1389aedfe0faa926127`  
		Last Modified: Wed, 09 Mar 2022 19:00:27 GMT  
		Size: 353.8 KB (353787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fcaecf749d555a0d83fad08ace6a7998307b24f4fecf9632bbfe013d112577`  
		Last Modified: Fri, 11 Mar 2022 00:18:44 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d880c105cf28c98f7d9613f331846e631375f272f037491c61f85d4cac54220d`  
		Last Modified: Fri, 11 Mar 2022 00:18:44 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2570e437e8fcb2cb9d3d91f7edafcf34ff2c23106a9aacbea7701ba1fce8d2b`  
		Last Modified: Fri, 11 Mar 2022 00:18:56 GMT  
		Size: 53.6 MB (53615032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:cd6d6c06799b236d2301e7ad57c076023ac64080624866d62810e268f91217e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.587; amd64

### `docker:20-windowsservercore-ltsc2022` - windows version 10.0.20348.587; amd64

```console
$ docker pull docker@sha256:ef007d39e5aa17f57f4ad75825febf433ea51d70fde48d5b40fea73307ffe3e8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2275653963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b8f4e76e84e2dd1842160718087208b325a794ca03ff7f14aac4b0b7b4694e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 03 Mar 2022 05:02:11 GMT
RUN Install update ltsc2022-amd64
# Tue, 08 Mar 2022 19:26:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:55:44 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 11 Mar 2022 00:15:07 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:15:08 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.13.zip
# Fri, 11 Mar 2022 00:15:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:037d5740b40414bc505c21324142a1cd3eab10c176189a9a74d1a90354ac7cd4`  
		Size: 969.5 MB (969547968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d58ba398110c3f761c6307a5621ec218b8593ba8b07b734436bcdd8d07a23e08`  
		Last Modified: Tue, 08 Mar 2022 20:00:31 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfaa4c2639ecdc27410a570e2dcb2efe02bcbec37d6ad750d15a97aac6990236`  
		Last Modified: Wed, 09 Mar 2022 18:59:14 GMT  
		Size: 598.3 KB (598260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0e605541ab33ab5774f3b41805cecf36dffbc7d02428d5bed5cbd86e1a7a0e`  
		Last Modified: Fri, 11 Mar 2022 00:17:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d060c5ba2630e8637c44694ed52a53850d5dd01c5f55f7b49493d202f48a5565`  
		Last Modified: Fri, 11 Mar 2022 00:17:32 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01c70e5c0d32c6abc7141a56d515a00df83a0786489da36fe453fa7a2b67d6d`  
		Last Modified: Fri, 11 Mar 2022 00:18:31 GMT  
		Size: 53.8 MB (53804674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10`

```console
$ docker pull docker@sha256:72e87d4f1d2ed054bf9ec48c77dfc546c7e6173fe9b6afd9e80716b9c5ade4bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10` - linux; amd64

```console
$ docker pull docker@sha256:338217655cdf830e6f659207f447776c8debaf1c3cbce0050645c2b621893d6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69413254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6816f070b2395d750ce78e4fbdb7e9df0af63b7686f3063c09e008c2ef1a0036`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Mar 2022 00:19:37 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:19:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Mar 2022 00:19:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Mar 2022 00:19:42 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:42 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Mar 2022 00:19:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Mar 2022 00:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:42 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea03e1895df432fba23ac2810a53a408fa25273ecf001276263d810107e1c81`  
		Last Modified: Wed, 15 Dec 2021 20:20:23 GMT  
		Size: 2.0 MB (1980404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff98835b05535c14c9bd8aa0449fd33d147a58c9a9fe7f21b76137065d0f4c5`  
		Last Modified: Wed, 15 Dec 2021 20:20:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbbd0a7b1dec526be119d73f0018052afa23e65ea79e09049a54a5954f2a374`  
		Last Modified: Fri, 11 Mar 2022 00:20:32 GMT  
		Size: 64.6 MB (64612571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317ecb07c86c68358ba3d763bea251b7baf1befde793d08f074abf2743a388dc`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52850491ed6a707afb12e76035b1a36f408c071e00d1de77b26ec2cb178c9a8a`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb2b84e11d9e63efd7d7cad8459ac6f5326f44d93991a59380b186824079bdf`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:576a187cf88c74c82b1cda12e206a8e20e24633499128894296909a44456f82a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63220789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51ae867936fd1dc5c38dab32635ffb031fba90112aaf70cd838fdf678922f0b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 06:44:43 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 17 Mar 2022 06:44:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 06:44:45 GMT
ENV DOCKER_VERSION=20.10.13
# Thu, 17 Mar 2022 06:44:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Mar 2022 06:44:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Mar 2022 06:44:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:44:51 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Mar 2022 06:44:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Mar 2022 06:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 06:44:54 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bd6b2d67571b28ebbe22152f5536e3cff37d4346bc02a444b2ede9b5d71c6`  
		Last Modified: Thu, 17 Mar 2022 06:46:18 GMT  
		Size: 1.9 MB (1938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadc398c63809a7b7b0d60cee36c1a95c7dd031fb5987cb99246b289df77d64f`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fce163fc9e7e1d8912203364c303838e60da953ed77812572633504c2bd014`  
		Last Modified: Thu, 17 Mar 2022 06:46:25 GMT  
		Size: 58.6 MB (58565248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a0a3a69cb84240c8270720f964d7155438567aa97bb868bfe1adc07b5b977`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8be56eb060db5cad28d2359c143a7a7de20610f090073f5cbd7f1cfeafbd4`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746be13a2cb02a7014e32f66ba9fb3bb10e14bd43af45b7890fb09464fe2a830`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind`

```console
$ docker pull docker@sha256:ca2744235df40f184843b2cb9f0245a6b64ae65065aad30285e80d5a266fe0c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind` - linux; amd64

```console
$ docker pull docker@sha256:34c594c12507d24f66789978a90240d4addf3eb8fce22a7a9157ca9701afd46d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76152892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c05a8c965912fe35df9cce58ddb7aed725fb34d81772761a4ef7a373fd3271c1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Mar 2022 00:19:37 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:19:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Mar 2022 00:19:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Mar 2022 00:19:42 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:42 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Mar 2022 00:19:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Mar 2022 00:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:42 GMT
CMD ["sh"]
# Fri, 11 Mar 2022 00:19:47 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Mar 2022 00:19:48 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Mar 2022 00:19:48 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 11 Mar 2022 00:19:48 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Mar 2022 00:19:48 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:48 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Mar 2022 00:19:49 GMT
EXPOSE 2375 2376
# Fri, 11 Mar 2022 00:19:49 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:49 GMT
CMD []
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea03e1895df432fba23ac2810a53a408fa25273ecf001276263d810107e1c81`  
		Last Modified: Wed, 15 Dec 2021 20:20:23 GMT  
		Size: 2.0 MB (1980404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff98835b05535c14c9bd8aa0449fd33d147a58c9a9fe7f21b76137065d0f4c5`  
		Last Modified: Wed, 15 Dec 2021 20:20:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbbd0a7b1dec526be119d73f0018052afa23e65ea79e09049a54a5954f2a374`  
		Last Modified: Fri, 11 Mar 2022 00:20:32 GMT  
		Size: 64.6 MB (64612571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317ecb07c86c68358ba3d763bea251b7baf1befde793d08f074abf2743a388dc`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52850491ed6a707afb12e76035b1a36f408c071e00d1de77b26ec2cb178c9a8a`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb2b84e11d9e63efd7d7cad8459ac6f5326f44d93991a59380b186824079bdf`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd217e3dc5c63b9a21276d1a8b9b2c0a19dd9aeecf5c242902d63e8dd7c251f`  
		Last Modified: Fri, 11 Mar 2022 00:20:50 GMT  
		Size: 6.7 MB (6734617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f85497bc6212a4fbd95757776ba9f0cfc449ba5ec26f58dc4b48718582d256`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63824672dbc4b8bf906bba2cabad90a9964a4de17f7df52debc99611d2782d66`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330cf4336db2c7c1846de44144ed6eb30ac0942792712aeca3f5b38acbd16933`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 2.7 KB (2747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e6222d4d8b30c439b883f691f52e8e405f6464852c86477f7b1577dee106ee6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69841345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ba71573c3cddc7fe6d1f68e3c7c55e13f7549be38cf07414563df801aa79e1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 06:44:43 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 17 Mar 2022 06:44:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 06:44:45 GMT
ENV DOCKER_VERSION=20.10.13
# Thu, 17 Mar 2022 06:44:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Mar 2022 06:44:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Mar 2022 06:44:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:44:51 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Mar 2022 06:44:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Mar 2022 06:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 06:44:54 GMT
CMD ["sh"]
# Thu, 17 Mar 2022 06:45:06 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 17 Mar 2022 06:45:07 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 17 Mar 2022 06:45:08 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 17 Mar 2022 06:45:09 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 17 Mar 2022 06:45:11 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:45:11 GMT
VOLUME [/var/lib/docker]
# Thu, 17 Mar 2022 06:45:12 GMT
EXPOSE 2375 2376
# Thu, 17 Mar 2022 06:45:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 17 Mar 2022 06:45:14 GMT
CMD []
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bd6b2d67571b28ebbe22152f5536e3cff37d4346bc02a444b2ede9b5d71c6`  
		Last Modified: Thu, 17 Mar 2022 06:46:18 GMT  
		Size: 1.9 MB (1938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadc398c63809a7b7b0d60cee36c1a95c7dd031fb5987cb99246b289df77d64f`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fce163fc9e7e1d8912203364c303838e60da953ed77812572633504c2bd014`  
		Last Modified: Thu, 17 Mar 2022 06:46:25 GMT  
		Size: 58.6 MB (58565248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a0a3a69cb84240c8270720f964d7155438567aa97bb868bfe1adc07b5b977`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8be56eb060db5cad28d2359c143a7a7de20610f090073f5cbd7f1cfeafbd4`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746be13a2cb02a7014e32f66ba9fb3bb10e14bd43af45b7890fb09464fe2a830`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb73bd4ce74defd0741f3f7922ffb261b2f91b45cf97e2225f65aaba2b4c42d6`  
		Last Modified: Thu, 17 Mar 2022 06:46:48 GMT  
		Size: 6.6 MB (6615563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e054635e9f383caa96af63cfbbc71098384c50f5c13efcc785d2a870ed8e4af9`  
		Last Modified: Thu, 17 Mar 2022 06:46:46 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791a50930d17375d4278a896defa85218b579b3efdd1455d1fa503e187676dfb`  
		Last Modified: Thu, 17 Mar 2022 06:46:46 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752ca04529521e0b4db8ded3d79d79f1629c7c725837b87fe79519f64bcb2e05`  
		Last Modified: Thu, 17 Mar 2022 06:46:47 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind-rootless`

```console
$ docker pull docker@sha256:e65462ff8bfe7c34478edfb354d6a1b5c03ecf7279212fc54fc54180d2663c2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:6a92617cb4df46747dc2fd832bae2ddda144ab9c1116ea2753df44cb211a55ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 MB (96448562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d466e72290286bcdfbc871e8561fae40d9eef80790216bb18f18b5313b6e088b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Mar 2022 00:19:37 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:19:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Mar 2022 00:19:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Mar 2022 00:19:42 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:42 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Mar 2022 00:19:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Mar 2022 00:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:42 GMT
CMD ["sh"]
# Fri, 11 Mar 2022 00:19:47 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Mar 2022 00:19:48 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Mar 2022 00:19:48 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 11 Mar 2022 00:19:48 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Mar 2022 00:19:48 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:48 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Mar 2022 00:19:49 GMT
EXPOSE 2375 2376
# Fri, 11 Mar 2022 00:19:49 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:49 GMT
CMD []
# Fri, 11 Mar 2022 00:19:52 GMT
RUN apk add --no-cache iproute2
# Fri, 11 Mar 2022 00:19:53 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 11 Mar 2022 00:19:53 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 11 Mar 2022 00:19:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 11 Mar 2022 00:19:57 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 11 Mar 2022 00:19:57 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 11 Mar 2022 00:19:57 GMT
USER rootless
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea03e1895df432fba23ac2810a53a408fa25273ecf001276263d810107e1c81`  
		Last Modified: Wed, 15 Dec 2021 20:20:23 GMT  
		Size: 2.0 MB (1980404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff98835b05535c14c9bd8aa0449fd33d147a58c9a9fe7f21b76137065d0f4c5`  
		Last Modified: Wed, 15 Dec 2021 20:20:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbbd0a7b1dec526be119d73f0018052afa23e65ea79e09049a54a5954f2a374`  
		Last Modified: Fri, 11 Mar 2022 00:20:32 GMT  
		Size: 64.6 MB (64612571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317ecb07c86c68358ba3d763bea251b7baf1befde793d08f074abf2743a388dc`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52850491ed6a707afb12e76035b1a36f408c071e00d1de77b26ec2cb178c9a8a`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb2b84e11d9e63efd7d7cad8459ac6f5326f44d93991a59380b186824079bdf`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd217e3dc5c63b9a21276d1a8b9b2c0a19dd9aeecf5c242902d63e8dd7c251f`  
		Last Modified: Fri, 11 Mar 2022 00:20:50 GMT  
		Size: 6.7 MB (6734617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f85497bc6212a4fbd95757776ba9f0cfc449ba5ec26f58dc4b48718582d256`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63824672dbc4b8bf906bba2cabad90a9964a4de17f7df52debc99611d2782d66`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330cf4336db2c7c1846de44144ed6eb30ac0942792712aeca3f5b38acbd16933`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 2.7 KB (2747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9243af40d6dedb8bec94753185a0e50302ceca90029164040a3c567cfe6649ed`  
		Last Modified: Fri, 11 Mar 2022 00:21:10 GMT  
		Size: 1.2 MB (1162145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad945e48854711031ed9581488dcd35e6a7281c7cef4273cc6c4fd49fb768ebd`  
		Last Modified: Fri, 11 Mar 2022 00:21:08 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dbac2c48de1cb6054512bc0b3967aa776ed177ce538b1901e10390d2e83250`  
		Last Modified: Fri, 11 Mar 2022 00:21:09 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2445b41c3397a2f9da27c43cc92a64a2e373b418307bc1a0322072b6f87096`  
		Last Modified: Fri, 11 Mar 2022 00:21:12 GMT  
		Size: 19.1 MB (19131808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ec68c91cc2997a8e6a4a961bc06b2a2af234d24e8f116a0ba3a2e0305beaf7`  
		Last Modified: Fri, 11 Mar 2022 00:21:08 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:fb00e978daa05ad0619ff4b0bbd52dd7c000a39954746498aadc6d94ac35194a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92132138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20955ed3fe29f7eca363024931545542a3e3bcaddd6de747255b806cb75f8c3d`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 06:44:43 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 17 Mar 2022 06:44:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 06:44:45 GMT
ENV DOCKER_VERSION=20.10.13
# Thu, 17 Mar 2022 06:44:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Mar 2022 06:44:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Mar 2022 06:44:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:44:51 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Mar 2022 06:44:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Mar 2022 06:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 06:44:54 GMT
CMD ["sh"]
# Thu, 17 Mar 2022 06:45:06 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 17 Mar 2022 06:45:07 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 17 Mar 2022 06:45:08 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 17 Mar 2022 06:45:09 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 17 Mar 2022 06:45:11 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:45:11 GMT
VOLUME [/var/lib/docker]
# Thu, 17 Mar 2022 06:45:12 GMT
EXPOSE 2375 2376
# Thu, 17 Mar 2022 06:45:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 17 Mar 2022 06:45:14 GMT
CMD []
# Thu, 17 Mar 2022 06:45:22 GMT
RUN apk add --no-cache iproute2
# Thu, 17 Mar 2022 06:45:23 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 17 Mar 2022 06:45:24 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 17 Mar 2022 06:45:27 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 17 Mar 2022 06:45:27 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 17 Mar 2022 06:45:28 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 17 Mar 2022 06:45:29 GMT
USER rootless
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bd6b2d67571b28ebbe22152f5536e3cff37d4346bc02a444b2ede9b5d71c6`  
		Last Modified: Thu, 17 Mar 2022 06:46:18 GMT  
		Size: 1.9 MB (1938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadc398c63809a7b7b0d60cee36c1a95c7dd031fb5987cb99246b289df77d64f`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fce163fc9e7e1d8912203364c303838e60da953ed77812572633504c2bd014`  
		Last Modified: Thu, 17 Mar 2022 06:46:25 GMT  
		Size: 58.6 MB (58565248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a0a3a69cb84240c8270720f964d7155438567aa97bb868bfe1adc07b5b977`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8be56eb060db5cad28d2359c143a7a7de20610f090073f5cbd7f1cfeafbd4`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746be13a2cb02a7014e32f66ba9fb3bb10e14bd43af45b7890fb09464fe2a830`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb73bd4ce74defd0741f3f7922ffb261b2f91b45cf97e2225f65aaba2b4c42d6`  
		Last Modified: Thu, 17 Mar 2022 06:46:48 GMT  
		Size: 6.6 MB (6615563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e054635e9f383caa96af63cfbbc71098384c50f5c13efcc785d2a870ed8e4af9`  
		Last Modified: Thu, 17 Mar 2022 06:46:46 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791a50930d17375d4278a896defa85218b579b3efdd1455d1fa503e187676dfb`  
		Last Modified: Thu, 17 Mar 2022 06:46:46 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752ca04529521e0b4db8ded3d79d79f1629c7c725837b87fe79519f64bcb2e05`  
		Last Modified: Thu, 17 Mar 2022 06:46:47 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b68e435beb33fd13cba08b839c86323a9ea7d3c280f4e09040d67dd21cfd835`  
		Last Modified: Thu, 17 Mar 2022 06:47:11 GMT  
		Size: 1.2 MB (1177952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f4ab31ae44292e2bfb84410de85f6a729607613d6dbef35902577fcbe78e4f`  
		Last Modified: Thu, 17 Mar 2022 06:47:10 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72e8ed3a93a11307aba41a4d0f7ffb6302f7de9886d46bf2562f06ab3e01e3f`  
		Last Modified: Thu, 17 Mar 2022 06:47:10 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768a72d3947b3532412cc42dd744996a22bf0574cebf60ac1119be3ca7530922`  
		Last Modified: Thu, 17 Mar 2022 06:47:14 GMT  
		Size: 21.1 MB (21111220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dec4d02116a97f8282cc9d24eaf55d48d469e3ad232980a8724940ba2a07ed3`  
		Last Modified: Thu, 17 Mar 2022 06:47:10 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-git`

```console
$ docker pull docker@sha256:5ec008af09dcdc65abc239b6f492af27f37a9c7ec94148f40703ca622a5faba5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-git` - linux; amd64

```console
$ docker pull docker@sha256:7383e8c2efcd6846670dd96ca1b6af84b7a4098fd778b85cee0ae2739301a79c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76237387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f328899fc7a17e58951f5523f603df43687ea162ad1f8f04eed66b876e9480ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Mar 2022 00:19:37 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:19:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Mar 2022 00:19:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Mar 2022 00:19:42 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:42 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Mar 2022 00:19:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Mar 2022 00:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:42 GMT
CMD ["sh"]
# Fri, 11 Mar 2022 00:20:00 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea03e1895df432fba23ac2810a53a408fa25273ecf001276263d810107e1c81`  
		Last Modified: Wed, 15 Dec 2021 20:20:23 GMT  
		Size: 2.0 MB (1980404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff98835b05535c14c9bd8aa0449fd33d147a58c9a9fe7f21b76137065d0f4c5`  
		Last Modified: Wed, 15 Dec 2021 20:20:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbbd0a7b1dec526be119d73f0018052afa23e65ea79e09049a54a5954f2a374`  
		Last Modified: Fri, 11 Mar 2022 00:20:32 GMT  
		Size: 64.6 MB (64612571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317ecb07c86c68358ba3d763bea251b7baf1befde793d08f074abf2743a388dc`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52850491ed6a707afb12e76035b1a36f408c071e00d1de77b26ec2cb178c9a8a`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb2b84e11d9e63efd7d7cad8459ac6f5326f44d93991a59380b186824079bdf`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc827496373a4a4176b9c5e48d8ea6bb5823b745c62a5ddd68e6b201ae7341d`  
		Last Modified: Fri, 11 Mar 2022 00:21:30 GMT  
		Size: 6.8 MB (6824133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:72b64e64f292fcc354064aff807584ba6aa24c62dcaacd0f4180974d732d7c33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70153837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a742244413c82313c84ffc8e2aae4a5e443443e2e7c6283b00bc9d89c10d767`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 06:44:43 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 17 Mar 2022 06:44:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 06:44:45 GMT
ENV DOCKER_VERSION=20.10.13
# Thu, 17 Mar 2022 06:44:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Mar 2022 06:44:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Mar 2022 06:44:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:44:51 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Mar 2022 06:44:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Mar 2022 06:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 06:44:54 GMT
CMD ["sh"]
# Thu, 17 Mar 2022 06:45:36 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bd6b2d67571b28ebbe22152f5536e3cff37d4346bc02a444b2ede9b5d71c6`  
		Last Modified: Thu, 17 Mar 2022 06:46:18 GMT  
		Size: 1.9 MB (1938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadc398c63809a7b7b0d60cee36c1a95c7dd031fb5987cb99246b289df77d64f`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fce163fc9e7e1d8912203364c303838e60da953ed77812572633504c2bd014`  
		Last Modified: Thu, 17 Mar 2022 06:46:25 GMT  
		Size: 58.6 MB (58565248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a0a3a69cb84240c8270720f964d7155438567aa97bb868bfe1adc07b5b977`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8be56eb060db5cad28d2359c143a7a7de20610f090073f5cbd7f1cfeafbd4`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746be13a2cb02a7014e32f66ba9fb3bb10e14bd43af45b7890fb09464fe2a830`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2716e163322a30318e4b5622ac98de0815fd95f93070ec60e4ee6ea3a3f85b59`  
		Last Modified: Thu, 17 Mar 2022 06:47:35 GMT  
		Size: 6.9 MB (6933048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore`

```console
$ docker pull docker@sha256:998f6c6a8ca0e9871ae959625b33ded24ef0dbf102278d815ca5c2ca91708e33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.587; amd64
	-	windows version 10.0.17763.2686; amd64

### `docker:20.10-windowsservercore` - windows version 10.0.20348.587; amd64

```console
$ docker pull docker@sha256:ef007d39e5aa17f57f4ad75825febf433ea51d70fde48d5b40fea73307ffe3e8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2275653963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b8f4e76e84e2dd1842160718087208b325a794ca03ff7f14aac4b0b7b4694e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 03 Mar 2022 05:02:11 GMT
RUN Install update ltsc2022-amd64
# Tue, 08 Mar 2022 19:26:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:55:44 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 11 Mar 2022 00:15:07 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:15:08 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.13.zip
# Fri, 11 Mar 2022 00:15:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:037d5740b40414bc505c21324142a1cd3eab10c176189a9a74d1a90354ac7cd4`  
		Size: 969.5 MB (969547968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d58ba398110c3f761c6307a5621ec218b8593ba8b07b734436bcdd8d07a23e08`  
		Last Modified: Tue, 08 Mar 2022 20:00:31 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfaa4c2639ecdc27410a570e2dcb2efe02bcbec37d6ad750d15a97aac6990236`  
		Last Modified: Wed, 09 Mar 2022 18:59:14 GMT  
		Size: 598.3 KB (598260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0e605541ab33ab5774f3b41805cecf36dffbc7d02428d5bed5cbd86e1a7a0e`  
		Last Modified: Fri, 11 Mar 2022 00:17:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d060c5ba2630e8637c44694ed52a53850d5dd01c5f55f7b49493d202f48a5565`  
		Last Modified: Fri, 11 Mar 2022 00:17:32 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01c70e5c0d32c6abc7141a56d515a00df83a0786489da36fe453fa7a2b67d6d`  
		Last Modified: Fri, 11 Mar 2022 00:18:31 GMT  
		Size: 53.8 MB (53804674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull docker@sha256:11fa18bbbc94e9342dea2f011d4ac7dc0e674553a427eeac46962b7fd3bb7654
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2769425405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57844be2857bef97ed862468dd3a51e9d0dea7c7b269a9efe192aa526df18835`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:57:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 11 Mar 2022 00:15:45 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:15:46 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.13.zip
# Fri, 11 Mar 2022 00:16:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc556e75fc2ee0a56749fd9ec604591d58c7dcfbf6ddd1389aedfe0faa926127`  
		Last Modified: Wed, 09 Mar 2022 19:00:27 GMT  
		Size: 353.8 KB (353787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fcaecf749d555a0d83fad08ace6a7998307b24f4fecf9632bbfe013d112577`  
		Last Modified: Fri, 11 Mar 2022 00:18:44 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d880c105cf28c98f7d9613f331846e631375f272f037491c61f85d4cac54220d`  
		Last Modified: Fri, 11 Mar 2022 00:18:44 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2570e437e8fcb2cb9d3d91f7edafcf34ff2c23106a9aacbea7701ba1fce8d2b`  
		Last Modified: Fri, 11 Mar 2022 00:18:56 GMT  
		Size: 53.6 MB (53615032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-1809`

```console
$ docker pull docker@sha256:2351bc67908336460d6d176ad7237bd4ce87e3906d102f82fa7b9464d08f8a83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `docker:20.10-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull docker@sha256:11fa18bbbc94e9342dea2f011d4ac7dc0e674553a427eeac46962b7fd3bb7654
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2769425405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57844be2857bef97ed862468dd3a51e9d0dea7c7b269a9efe192aa526df18835`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:57:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 11 Mar 2022 00:15:45 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:15:46 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.13.zip
# Fri, 11 Mar 2022 00:16:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc556e75fc2ee0a56749fd9ec604591d58c7dcfbf6ddd1389aedfe0faa926127`  
		Last Modified: Wed, 09 Mar 2022 19:00:27 GMT  
		Size: 353.8 KB (353787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fcaecf749d555a0d83fad08ace6a7998307b24f4fecf9632bbfe013d112577`  
		Last Modified: Fri, 11 Mar 2022 00:18:44 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d880c105cf28c98f7d9613f331846e631375f272f037491c61f85d4cac54220d`  
		Last Modified: Fri, 11 Mar 2022 00:18:44 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2570e437e8fcb2cb9d3d91f7edafcf34ff2c23106a9aacbea7701ba1fce8d2b`  
		Last Modified: Fri, 11 Mar 2022 00:18:56 GMT  
		Size: 53.6 MB (53615032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:cd6d6c06799b236d2301e7ad57c076023ac64080624866d62810e268f91217e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.587; amd64

### `docker:20.10-windowsservercore-ltsc2022` - windows version 10.0.20348.587; amd64

```console
$ docker pull docker@sha256:ef007d39e5aa17f57f4ad75825febf433ea51d70fde48d5b40fea73307ffe3e8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2275653963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b8f4e76e84e2dd1842160718087208b325a794ca03ff7f14aac4b0b7b4694e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 03 Mar 2022 05:02:11 GMT
RUN Install update ltsc2022-amd64
# Tue, 08 Mar 2022 19:26:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:55:44 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 11 Mar 2022 00:15:07 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:15:08 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.13.zip
# Fri, 11 Mar 2022 00:15:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:037d5740b40414bc505c21324142a1cd3eab10c176189a9a74d1a90354ac7cd4`  
		Size: 969.5 MB (969547968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d58ba398110c3f761c6307a5621ec218b8593ba8b07b734436bcdd8d07a23e08`  
		Last Modified: Tue, 08 Mar 2022 20:00:31 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfaa4c2639ecdc27410a570e2dcb2efe02bcbec37d6ad750d15a97aac6990236`  
		Last Modified: Wed, 09 Mar 2022 18:59:14 GMT  
		Size: 598.3 KB (598260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0e605541ab33ab5774f3b41805cecf36dffbc7d02428d5bed5cbd86e1a7a0e`  
		Last Modified: Fri, 11 Mar 2022 00:17:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d060c5ba2630e8637c44694ed52a53850d5dd01c5f55f7b49493d202f48a5565`  
		Last Modified: Fri, 11 Mar 2022 00:17:32 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01c70e5c0d32c6abc7141a56d515a00df83a0786489da36fe453fa7a2b67d6d`  
		Last Modified: Fri, 11 Mar 2022 00:18:31 GMT  
		Size: 53.8 MB (53804674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.13`

```console
$ docker pull docker@sha256:72e87d4f1d2ed054bf9ec48c77dfc546c7e6173fe9b6afd9e80716b9c5ade4bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.13` - linux; amd64

```console
$ docker pull docker@sha256:338217655cdf830e6f659207f447776c8debaf1c3cbce0050645c2b621893d6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69413254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6816f070b2395d750ce78e4fbdb7e9df0af63b7686f3063c09e008c2ef1a0036`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Mar 2022 00:19:37 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:19:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Mar 2022 00:19:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Mar 2022 00:19:42 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:42 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Mar 2022 00:19:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Mar 2022 00:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:42 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea03e1895df432fba23ac2810a53a408fa25273ecf001276263d810107e1c81`  
		Last Modified: Wed, 15 Dec 2021 20:20:23 GMT  
		Size: 2.0 MB (1980404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff98835b05535c14c9bd8aa0449fd33d147a58c9a9fe7f21b76137065d0f4c5`  
		Last Modified: Wed, 15 Dec 2021 20:20:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbbd0a7b1dec526be119d73f0018052afa23e65ea79e09049a54a5954f2a374`  
		Last Modified: Fri, 11 Mar 2022 00:20:32 GMT  
		Size: 64.6 MB (64612571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317ecb07c86c68358ba3d763bea251b7baf1befde793d08f074abf2743a388dc`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52850491ed6a707afb12e76035b1a36f408c071e00d1de77b26ec2cb178c9a8a`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb2b84e11d9e63efd7d7cad8459ac6f5326f44d93991a59380b186824079bdf`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.13` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:576a187cf88c74c82b1cda12e206a8e20e24633499128894296909a44456f82a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63220789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51ae867936fd1dc5c38dab32635ffb031fba90112aaf70cd838fdf678922f0b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 06:44:43 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 17 Mar 2022 06:44:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 06:44:45 GMT
ENV DOCKER_VERSION=20.10.13
# Thu, 17 Mar 2022 06:44:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Mar 2022 06:44:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Mar 2022 06:44:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:44:51 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Mar 2022 06:44:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Mar 2022 06:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 06:44:54 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bd6b2d67571b28ebbe22152f5536e3cff37d4346bc02a444b2ede9b5d71c6`  
		Last Modified: Thu, 17 Mar 2022 06:46:18 GMT  
		Size: 1.9 MB (1938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadc398c63809a7b7b0d60cee36c1a95c7dd031fb5987cb99246b289df77d64f`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fce163fc9e7e1d8912203364c303838e60da953ed77812572633504c2bd014`  
		Last Modified: Thu, 17 Mar 2022 06:46:25 GMT  
		Size: 58.6 MB (58565248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a0a3a69cb84240c8270720f964d7155438567aa97bb868bfe1adc07b5b977`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8be56eb060db5cad28d2359c143a7a7de20610f090073f5cbd7f1cfeafbd4`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746be13a2cb02a7014e32f66ba9fb3bb10e14bd43af45b7890fb09464fe2a830`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.13-alpine3.15`

```console
$ docker pull docker@sha256:72e87d4f1d2ed054bf9ec48c77dfc546c7e6173fe9b6afd9e80716b9c5ade4bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.13-alpine3.15` - linux; amd64

```console
$ docker pull docker@sha256:338217655cdf830e6f659207f447776c8debaf1c3cbce0050645c2b621893d6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69413254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6816f070b2395d750ce78e4fbdb7e9df0af63b7686f3063c09e008c2ef1a0036`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Mar 2022 00:19:37 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:19:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Mar 2022 00:19:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Mar 2022 00:19:42 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:42 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Mar 2022 00:19:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Mar 2022 00:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:42 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea03e1895df432fba23ac2810a53a408fa25273ecf001276263d810107e1c81`  
		Last Modified: Wed, 15 Dec 2021 20:20:23 GMT  
		Size: 2.0 MB (1980404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff98835b05535c14c9bd8aa0449fd33d147a58c9a9fe7f21b76137065d0f4c5`  
		Last Modified: Wed, 15 Dec 2021 20:20:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbbd0a7b1dec526be119d73f0018052afa23e65ea79e09049a54a5954f2a374`  
		Last Modified: Fri, 11 Mar 2022 00:20:32 GMT  
		Size: 64.6 MB (64612571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317ecb07c86c68358ba3d763bea251b7baf1befde793d08f074abf2743a388dc`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52850491ed6a707afb12e76035b1a36f408c071e00d1de77b26ec2cb178c9a8a`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb2b84e11d9e63efd7d7cad8459ac6f5326f44d93991a59380b186824079bdf`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.13-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:576a187cf88c74c82b1cda12e206a8e20e24633499128894296909a44456f82a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63220789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51ae867936fd1dc5c38dab32635ffb031fba90112aaf70cd838fdf678922f0b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 06:44:43 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 17 Mar 2022 06:44:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 06:44:45 GMT
ENV DOCKER_VERSION=20.10.13
# Thu, 17 Mar 2022 06:44:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Mar 2022 06:44:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Mar 2022 06:44:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:44:51 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Mar 2022 06:44:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Mar 2022 06:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 06:44:54 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bd6b2d67571b28ebbe22152f5536e3cff37d4346bc02a444b2ede9b5d71c6`  
		Last Modified: Thu, 17 Mar 2022 06:46:18 GMT  
		Size: 1.9 MB (1938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadc398c63809a7b7b0d60cee36c1a95c7dd031fb5987cb99246b289df77d64f`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fce163fc9e7e1d8912203364c303838e60da953ed77812572633504c2bd014`  
		Last Modified: Thu, 17 Mar 2022 06:46:25 GMT  
		Size: 58.6 MB (58565248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a0a3a69cb84240c8270720f964d7155438567aa97bb868bfe1adc07b5b977`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8be56eb060db5cad28d2359c143a7a7de20610f090073f5cbd7f1cfeafbd4`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746be13a2cb02a7014e32f66ba9fb3bb10e14bd43af45b7890fb09464fe2a830`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.13-dind`

```console
$ docker pull docker@sha256:ca2744235df40f184843b2cb9f0245a6b64ae65065aad30285e80d5a266fe0c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.13-dind` - linux; amd64

```console
$ docker pull docker@sha256:34c594c12507d24f66789978a90240d4addf3eb8fce22a7a9157ca9701afd46d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76152892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c05a8c965912fe35df9cce58ddb7aed725fb34d81772761a4ef7a373fd3271c1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Mar 2022 00:19:37 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:19:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Mar 2022 00:19:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Mar 2022 00:19:42 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:42 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Mar 2022 00:19:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Mar 2022 00:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:42 GMT
CMD ["sh"]
# Fri, 11 Mar 2022 00:19:47 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Mar 2022 00:19:48 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Mar 2022 00:19:48 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 11 Mar 2022 00:19:48 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Mar 2022 00:19:48 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:48 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Mar 2022 00:19:49 GMT
EXPOSE 2375 2376
# Fri, 11 Mar 2022 00:19:49 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:49 GMT
CMD []
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea03e1895df432fba23ac2810a53a408fa25273ecf001276263d810107e1c81`  
		Last Modified: Wed, 15 Dec 2021 20:20:23 GMT  
		Size: 2.0 MB (1980404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff98835b05535c14c9bd8aa0449fd33d147a58c9a9fe7f21b76137065d0f4c5`  
		Last Modified: Wed, 15 Dec 2021 20:20:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbbd0a7b1dec526be119d73f0018052afa23e65ea79e09049a54a5954f2a374`  
		Last Modified: Fri, 11 Mar 2022 00:20:32 GMT  
		Size: 64.6 MB (64612571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317ecb07c86c68358ba3d763bea251b7baf1befde793d08f074abf2743a388dc`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52850491ed6a707afb12e76035b1a36f408c071e00d1de77b26ec2cb178c9a8a`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb2b84e11d9e63efd7d7cad8459ac6f5326f44d93991a59380b186824079bdf`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd217e3dc5c63b9a21276d1a8b9b2c0a19dd9aeecf5c242902d63e8dd7c251f`  
		Last Modified: Fri, 11 Mar 2022 00:20:50 GMT  
		Size: 6.7 MB (6734617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f85497bc6212a4fbd95757776ba9f0cfc449ba5ec26f58dc4b48718582d256`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63824672dbc4b8bf906bba2cabad90a9964a4de17f7df52debc99611d2782d66`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330cf4336db2c7c1846de44144ed6eb30ac0942792712aeca3f5b38acbd16933`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 2.7 KB (2747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.13-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e6222d4d8b30c439b883f691f52e8e405f6464852c86477f7b1577dee106ee6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69841345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ba71573c3cddc7fe6d1f68e3c7c55e13f7549be38cf07414563df801aa79e1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 06:44:43 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 17 Mar 2022 06:44:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 06:44:45 GMT
ENV DOCKER_VERSION=20.10.13
# Thu, 17 Mar 2022 06:44:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Mar 2022 06:44:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Mar 2022 06:44:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:44:51 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Mar 2022 06:44:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Mar 2022 06:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 06:44:54 GMT
CMD ["sh"]
# Thu, 17 Mar 2022 06:45:06 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 17 Mar 2022 06:45:07 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 17 Mar 2022 06:45:08 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 17 Mar 2022 06:45:09 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 17 Mar 2022 06:45:11 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:45:11 GMT
VOLUME [/var/lib/docker]
# Thu, 17 Mar 2022 06:45:12 GMT
EXPOSE 2375 2376
# Thu, 17 Mar 2022 06:45:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 17 Mar 2022 06:45:14 GMT
CMD []
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bd6b2d67571b28ebbe22152f5536e3cff37d4346bc02a444b2ede9b5d71c6`  
		Last Modified: Thu, 17 Mar 2022 06:46:18 GMT  
		Size: 1.9 MB (1938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadc398c63809a7b7b0d60cee36c1a95c7dd031fb5987cb99246b289df77d64f`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fce163fc9e7e1d8912203364c303838e60da953ed77812572633504c2bd014`  
		Last Modified: Thu, 17 Mar 2022 06:46:25 GMT  
		Size: 58.6 MB (58565248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a0a3a69cb84240c8270720f964d7155438567aa97bb868bfe1adc07b5b977`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8be56eb060db5cad28d2359c143a7a7de20610f090073f5cbd7f1cfeafbd4`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746be13a2cb02a7014e32f66ba9fb3bb10e14bd43af45b7890fb09464fe2a830`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb73bd4ce74defd0741f3f7922ffb261b2f91b45cf97e2225f65aaba2b4c42d6`  
		Last Modified: Thu, 17 Mar 2022 06:46:48 GMT  
		Size: 6.6 MB (6615563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e054635e9f383caa96af63cfbbc71098384c50f5c13efcc785d2a870ed8e4af9`  
		Last Modified: Thu, 17 Mar 2022 06:46:46 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791a50930d17375d4278a896defa85218b579b3efdd1455d1fa503e187676dfb`  
		Last Modified: Thu, 17 Mar 2022 06:46:46 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752ca04529521e0b4db8ded3d79d79f1629c7c725837b87fe79519f64bcb2e05`  
		Last Modified: Thu, 17 Mar 2022 06:46:47 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.13-dind-alpine3.15`

```console
$ docker pull docker@sha256:ca2744235df40f184843b2cb9f0245a6b64ae65065aad30285e80d5a266fe0c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.13-dind-alpine3.15` - linux; amd64

```console
$ docker pull docker@sha256:34c594c12507d24f66789978a90240d4addf3eb8fce22a7a9157ca9701afd46d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76152892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c05a8c965912fe35df9cce58ddb7aed725fb34d81772761a4ef7a373fd3271c1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Mar 2022 00:19:37 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:19:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Mar 2022 00:19:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Mar 2022 00:19:42 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:42 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Mar 2022 00:19:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Mar 2022 00:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:42 GMT
CMD ["sh"]
# Fri, 11 Mar 2022 00:19:47 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Mar 2022 00:19:48 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Mar 2022 00:19:48 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 11 Mar 2022 00:19:48 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Mar 2022 00:19:48 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:48 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Mar 2022 00:19:49 GMT
EXPOSE 2375 2376
# Fri, 11 Mar 2022 00:19:49 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:49 GMT
CMD []
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea03e1895df432fba23ac2810a53a408fa25273ecf001276263d810107e1c81`  
		Last Modified: Wed, 15 Dec 2021 20:20:23 GMT  
		Size: 2.0 MB (1980404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff98835b05535c14c9bd8aa0449fd33d147a58c9a9fe7f21b76137065d0f4c5`  
		Last Modified: Wed, 15 Dec 2021 20:20:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbbd0a7b1dec526be119d73f0018052afa23e65ea79e09049a54a5954f2a374`  
		Last Modified: Fri, 11 Mar 2022 00:20:32 GMT  
		Size: 64.6 MB (64612571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317ecb07c86c68358ba3d763bea251b7baf1befde793d08f074abf2743a388dc`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52850491ed6a707afb12e76035b1a36f408c071e00d1de77b26ec2cb178c9a8a`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb2b84e11d9e63efd7d7cad8459ac6f5326f44d93991a59380b186824079bdf`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd217e3dc5c63b9a21276d1a8b9b2c0a19dd9aeecf5c242902d63e8dd7c251f`  
		Last Modified: Fri, 11 Mar 2022 00:20:50 GMT  
		Size: 6.7 MB (6734617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f85497bc6212a4fbd95757776ba9f0cfc449ba5ec26f58dc4b48718582d256`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63824672dbc4b8bf906bba2cabad90a9964a4de17f7df52debc99611d2782d66`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330cf4336db2c7c1846de44144ed6eb30ac0942792712aeca3f5b38acbd16933`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 2.7 KB (2747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.13-dind-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e6222d4d8b30c439b883f691f52e8e405f6464852c86477f7b1577dee106ee6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69841345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ba71573c3cddc7fe6d1f68e3c7c55e13f7549be38cf07414563df801aa79e1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 06:44:43 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 17 Mar 2022 06:44:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 06:44:45 GMT
ENV DOCKER_VERSION=20.10.13
# Thu, 17 Mar 2022 06:44:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Mar 2022 06:44:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Mar 2022 06:44:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:44:51 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Mar 2022 06:44:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Mar 2022 06:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 06:44:54 GMT
CMD ["sh"]
# Thu, 17 Mar 2022 06:45:06 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 17 Mar 2022 06:45:07 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 17 Mar 2022 06:45:08 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 17 Mar 2022 06:45:09 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 17 Mar 2022 06:45:11 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:45:11 GMT
VOLUME [/var/lib/docker]
# Thu, 17 Mar 2022 06:45:12 GMT
EXPOSE 2375 2376
# Thu, 17 Mar 2022 06:45:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 17 Mar 2022 06:45:14 GMT
CMD []
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bd6b2d67571b28ebbe22152f5536e3cff37d4346bc02a444b2ede9b5d71c6`  
		Last Modified: Thu, 17 Mar 2022 06:46:18 GMT  
		Size: 1.9 MB (1938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadc398c63809a7b7b0d60cee36c1a95c7dd031fb5987cb99246b289df77d64f`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fce163fc9e7e1d8912203364c303838e60da953ed77812572633504c2bd014`  
		Last Modified: Thu, 17 Mar 2022 06:46:25 GMT  
		Size: 58.6 MB (58565248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a0a3a69cb84240c8270720f964d7155438567aa97bb868bfe1adc07b5b977`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8be56eb060db5cad28d2359c143a7a7de20610f090073f5cbd7f1cfeafbd4`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746be13a2cb02a7014e32f66ba9fb3bb10e14bd43af45b7890fb09464fe2a830`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb73bd4ce74defd0741f3f7922ffb261b2f91b45cf97e2225f65aaba2b4c42d6`  
		Last Modified: Thu, 17 Mar 2022 06:46:48 GMT  
		Size: 6.6 MB (6615563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e054635e9f383caa96af63cfbbc71098384c50f5c13efcc785d2a870ed8e4af9`  
		Last Modified: Thu, 17 Mar 2022 06:46:46 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791a50930d17375d4278a896defa85218b579b3efdd1455d1fa503e187676dfb`  
		Last Modified: Thu, 17 Mar 2022 06:46:46 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752ca04529521e0b4db8ded3d79d79f1629c7c725837b87fe79519f64bcb2e05`  
		Last Modified: Thu, 17 Mar 2022 06:46:47 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.13-dind-rootless`

```console
$ docker pull docker@sha256:e65462ff8bfe7c34478edfb354d6a1b5c03ecf7279212fc54fc54180d2663c2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.13-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:6a92617cb4df46747dc2fd832bae2ddda144ab9c1116ea2753df44cb211a55ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 MB (96448562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d466e72290286bcdfbc871e8561fae40d9eef80790216bb18f18b5313b6e088b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Mar 2022 00:19:37 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:19:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Mar 2022 00:19:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Mar 2022 00:19:42 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:42 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Mar 2022 00:19:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Mar 2022 00:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:42 GMT
CMD ["sh"]
# Fri, 11 Mar 2022 00:19:47 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Mar 2022 00:19:48 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Mar 2022 00:19:48 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 11 Mar 2022 00:19:48 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Mar 2022 00:19:48 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:48 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Mar 2022 00:19:49 GMT
EXPOSE 2375 2376
# Fri, 11 Mar 2022 00:19:49 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:49 GMT
CMD []
# Fri, 11 Mar 2022 00:19:52 GMT
RUN apk add --no-cache iproute2
# Fri, 11 Mar 2022 00:19:53 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 11 Mar 2022 00:19:53 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 11 Mar 2022 00:19:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 11 Mar 2022 00:19:57 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 11 Mar 2022 00:19:57 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 11 Mar 2022 00:19:57 GMT
USER rootless
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea03e1895df432fba23ac2810a53a408fa25273ecf001276263d810107e1c81`  
		Last Modified: Wed, 15 Dec 2021 20:20:23 GMT  
		Size: 2.0 MB (1980404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff98835b05535c14c9bd8aa0449fd33d147a58c9a9fe7f21b76137065d0f4c5`  
		Last Modified: Wed, 15 Dec 2021 20:20:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbbd0a7b1dec526be119d73f0018052afa23e65ea79e09049a54a5954f2a374`  
		Last Modified: Fri, 11 Mar 2022 00:20:32 GMT  
		Size: 64.6 MB (64612571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317ecb07c86c68358ba3d763bea251b7baf1befde793d08f074abf2743a388dc`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52850491ed6a707afb12e76035b1a36f408c071e00d1de77b26ec2cb178c9a8a`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb2b84e11d9e63efd7d7cad8459ac6f5326f44d93991a59380b186824079bdf`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd217e3dc5c63b9a21276d1a8b9b2c0a19dd9aeecf5c242902d63e8dd7c251f`  
		Last Modified: Fri, 11 Mar 2022 00:20:50 GMT  
		Size: 6.7 MB (6734617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f85497bc6212a4fbd95757776ba9f0cfc449ba5ec26f58dc4b48718582d256`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63824672dbc4b8bf906bba2cabad90a9964a4de17f7df52debc99611d2782d66`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330cf4336db2c7c1846de44144ed6eb30ac0942792712aeca3f5b38acbd16933`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 2.7 KB (2747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9243af40d6dedb8bec94753185a0e50302ceca90029164040a3c567cfe6649ed`  
		Last Modified: Fri, 11 Mar 2022 00:21:10 GMT  
		Size: 1.2 MB (1162145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad945e48854711031ed9581488dcd35e6a7281c7cef4273cc6c4fd49fb768ebd`  
		Last Modified: Fri, 11 Mar 2022 00:21:08 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dbac2c48de1cb6054512bc0b3967aa776ed177ce538b1901e10390d2e83250`  
		Last Modified: Fri, 11 Mar 2022 00:21:09 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2445b41c3397a2f9da27c43cc92a64a2e373b418307bc1a0322072b6f87096`  
		Last Modified: Fri, 11 Mar 2022 00:21:12 GMT  
		Size: 19.1 MB (19131808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ec68c91cc2997a8e6a4a961bc06b2a2af234d24e8f116a0ba3a2e0305beaf7`  
		Last Modified: Fri, 11 Mar 2022 00:21:08 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.13-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:fb00e978daa05ad0619ff4b0bbd52dd7c000a39954746498aadc6d94ac35194a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92132138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20955ed3fe29f7eca363024931545542a3e3bcaddd6de747255b806cb75f8c3d`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 06:44:43 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 17 Mar 2022 06:44:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 06:44:45 GMT
ENV DOCKER_VERSION=20.10.13
# Thu, 17 Mar 2022 06:44:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Mar 2022 06:44:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Mar 2022 06:44:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:44:51 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Mar 2022 06:44:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Mar 2022 06:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 06:44:54 GMT
CMD ["sh"]
# Thu, 17 Mar 2022 06:45:06 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 17 Mar 2022 06:45:07 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 17 Mar 2022 06:45:08 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 17 Mar 2022 06:45:09 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 17 Mar 2022 06:45:11 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:45:11 GMT
VOLUME [/var/lib/docker]
# Thu, 17 Mar 2022 06:45:12 GMT
EXPOSE 2375 2376
# Thu, 17 Mar 2022 06:45:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 17 Mar 2022 06:45:14 GMT
CMD []
# Thu, 17 Mar 2022 06:45:22 GMT
RUN apk add --no-cache iproute2
# Thu, 17 Mar 2022 06:45:23 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 17 Mar 2022 06:45:24 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 17 Mar 2022 06:45:27 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 17 Mar 2022 06:45:27 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 17 Mar 2022 06:45:28 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 17 Mar 2022 06:45:29 GMT
USER rootless
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bd6b2d67571b28ebbe22152f5536e3cff37d4346bc02a444b2ede9b5d71c6`  
		Last Modified: Thu, 17 Mar 2022 06:46:18 GMT  
		Size: 1.9 MB (1938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadc398c63809a7b7b0d60cee36c1a95c7dd031fb5987cb99246b289df77d64f`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fce163fc9e7e1d8912203364c303838e60da953ed77812572633504c2bd014`  
		Last Modified: Thu, 17 Mar 2022 06:46:25 GMT  
		Size: 58.6 MB (58565248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a0a3a69cb84240c8270720f964d7155438567aa97bb868bfe1adc07b5b977`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8be56eb060db5cad28d2359c143a7a7de20610f090073f5cbd7f1cfeafbd4`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746be13a2cb02a7014e32f66ba9fb3bb10e14bd43af45b7890fb09464fe2a830`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb73bd4ce74defd0741f3f7922ffb261b2f91b45cf97e2225f65aaba2b4c42d6`  
		Last Modified: Thu, 17 Mar 2022 06:46:48 GMT  
		Size: 6.6 MB (6615563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e054635e9f383caa96af63cfbbc71098384c50f5c13efcc785d2a870ed8e4af9`  
		Last Modified: Thu, 17 Mar 2022 06:46:46 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791a50930d17375d4278a896defa85218b579b3efdd1455d1fa503e187676dfb`  
		Last Modified: Thu, 17 Mar 2022 06:46:46 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752ca04529521e0b4db8ded3d79d79f1629c7c725837b87fe79519f64bcb2e05`  
		Last Modified: Thu, 17 Mar 2022 06:46:47 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b68e435beb33fd13cba08b839c86323a9ea7d3c280f4e09040d67dd21cfd835`  
		Last Modified: Thu, 17 Mar 2022 06:47:11 GMT  
		Size: 1.2 MB (1177952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f4ab31ae44292e2bfb84410de85f6a729607613d6dbef35902577fcbe78e4f`  
		Last Modified: Thu, 17 Mar 2022 06:47:10 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72e8ed3a93a11307aba41a4d0f7ffb6302f7de9886d46bf2562f06ab3e01e3f`  
		Last Modified: Thu, 17 Mar 2022 06:47:10 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768a72d3947b3532412cc42dd744996a22bf0574cebf60ac1119be3ca7530922`  
		Last Modified: Thu, 17 Mar 2022 06:47:14 GMT  
		Size: 21.1 MB (21111220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dec4d02116a97f8282cc9d24eaf55d48d469e3ad232980a8724940ba2a07ed3`  
		Last Modified: Thu, 17 Mar 2022 06:47:10 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.13-git`

```console
$ docker pull docker@sha256:5ec008af09dcdc65abc239b6f492af27f37a9c7ec94148f40703ca622a5faba5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.13-git` - linux; amd64

```console
$ docker pull docker@sha256:7383e8c2efcd6846670dd96ca1b6af84b7a4098fd778b85cee0ae2739301a79c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76237387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f328899fc7a17e58951f5523f603df43687ea162ad1f8f04eed66b876e9480ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Mar 2022 00:19:37 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:19:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Mar 2022 00:19:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Mar 2022 00:19:42 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:42 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Mar 2022 00:19:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Mar 2022 00:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:42 GMT
CMD ["sh"]
# Fri, 11 Mar 2022 00:20:00 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea03e1895df432fba23ac2810a53a408fa25273ecf001276263d810107e1c81`  
		Last Modified: Wed, 15 Dec 2021 20:20:23 GMT  
		Size: 2.0 MB (1980404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff98835b05535c14c9bd8aa0449fd33d147a58c9a9fe7f21b76137065d0f4c5`  
		Last Modified: Wed, 15 Dec 2021 20:20:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbbd0a7b1dec526be119d73f0018052afa23e65ea79e09049a54a5954f2a374`  
		Last Modified: Fri, 11 Mar 2022 00:20:32 GMT  
		Size: 64.6 MB (64612571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317ecb07c86c68358ba3d763bea251b7baf1befde793d08f074abf2743a388dc`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52850491ed6a707afb12e76035b1a36f408c071e00d1de77b26ec2cb178c9a8a`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb2b84e11d9e63efd7d7cad8459ac6f5326f44d93991a59380b186824079bdf`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc827496373a4a4176b9c5e48d8ea6bb5823b745c62a5ddd68e6b201ae7341d`  
		Last Modified: Fri, 11 Mar 2022 00:21:30 GMT  
		Size: 6.8 MB (6824133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.13-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:72b64e64f292fcc354064aff807584ba6aa24c62dcaacd0f4180974d732d7c33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70153837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a742244413c82313c84ffc8e2aae4a5e443443e2e7c6283b00bc9d89c10d767`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 06:44:43 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 17 Mar 2022 06:44:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 06:44:45 GMT
ENV DOCKER_VERSION=20.10.13
# Thu, 17 Mar 2022 06:44:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Mar 2022 06:44:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Mar 2022 06:44:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:44:51 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Mar 2022 06:44:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Mar 2022 06:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 06:44:54 GMT
CMD ["sh"]
# Thu, 17 Mar 2022 06:45:36 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bd6b2d67571b28ebbe22152f5536e3cff37d4346bc02a444b2ede9b5d71c6`  
		Last Modified: Thu, 17 Mar 2022 06:46:18 GMT  
		Size: 1.9 MB (1938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadc398c63809a7b7b0d60cee36c1a95c7dd031fb5987cb99246b289df77d64f`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fce163fc9e7e1d8912203364c303838e60da953ed77812572633504c2bd014`  
		Last Modified: Thu, 17 Mar 2022 06:46:25 GMT  
		Size: 58.6 MB (58565248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a0a3a69cb84240c8270720f964d7155438567aa97bb868bfe1adc07b5b977`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8be56eb060db5cad28d2359c143a7a7de20610f090073f5cbd7f1cfeafbd4`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746be13a2cb02a7014e32f66ba9fb3bb10e14bd43af45b7890fb09464fe2a830`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2716e163322a30318e4b5622ac98de0815fd95f93070ec60e4ee6ea3a3f85b59`  
		Last Modified: Thu, 17 Mar 2022 06:47:35 GMT  
		Size: 6.9 MB (6933048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.13-windowsservercore`

```console
$ docker pull docker@sha256:998f6c6a8ca0e9871ae959625b33ded24ef0dbf102278d815ca5c2ca91708e33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.587; amd64
	-	windows version 10.0.17763.2686; amd64

### `docker:20.10.13-windowsservercore` - windows version 10.0.20348.587; amd64

```console
$ docker pull docker@sha256:ef007d39e5aa17f57f4ad75825febf433ea51d70fde48d5b40fea73307ffe3e8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2275653963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b8f4e76e84e2dd1842160718087208b325a794ca03ff7f14aac4b0b7b4694e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 03 Mar 2022 05:02:11 GMT
RUN Install update ltsc2022-amd64
# Tue, 08 Mar 2022 19:26:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:55:44 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 11 Mar 2022 00:15:07 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:15:08 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.13.zip
# Fri, 11 Mar 2022 00:15:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:037d5740b40414bc505c21324142a1cd3eab10c176189a9a74d1a90354ac7cd4`  
		Size: 969.5 MB (969547968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d58ba398110c3f761c6307a5621ec218b8593ba8b07b734436bcdd8d07a23e08`  
		Last Modified: Tue, 08 Mar 2022 20:00:31 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfaa4c2639ecdc27410a570e2dcb2efe02bcbec37d6ad750d15a97aac6990236`  
		Last Modified: Wed, 09 Mar 2022 18:59:14 GMT  
		Size: 598.3 KB (598260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0e605541ab33ab5774f3b41805cecf36dffbc7d02428d5bed5cbd86e1a7a0e`  
		Last Modified: Fri, 11 Mar 2022 00:17:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d060c5ba2630e8637c44694ed52a53850d5dd01c5f55f7b49493d202f48a5565`  
		Last Modified: Fri, 11 Mar 2022 00:17:32 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01c70e5c0d32c6abc7141a56d515a00df83a0786489da36fe453fa7a2b67d6d`  
		Last Modified: Fri, 11 Mar 2022 00:18:31 GMT  
		Size: 53.8 MB (53804674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.13-windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull docker@sha256:11fa18bbbc94e9342dea2f011d4ac7dc0e674553a427eeac46962b7fd3bb7654
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2769425405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57844be2857bef97ed862468dd3a51e9d0dea7c7b269a9efe192aa526df18835`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:57:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 11 Mar 2022 00:15:45 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:15:46 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.13.zip
# Fri, 11 Mar 2022 00:16:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc556e75fc2ee0a56749fd9ec604591d58c7dcfbf6ddd1389aedfe0faa926127`  
		Last Modified: Wed, 09 Mar 2022 19:00:27 GMT  
		Size: 353.8 KB (353787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fcaecf749d555a0d83fad08ace6a7998307b24f4fecf9632bbfe013d112577`  
		Last Modified: Fri, 11 Mar 2022 00:18:44 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d880c105cf28c98f7d9613f331846e631375f272f037491c61f85d4cac54220d`  
		Last Modified: Fri, 11 Mar 2022 00:18:44 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2570e437e8fcb2cb9d3d91f7edafcf34ff2c23106a9aacbea7701ba1fce8d2b`  
		Last Modified: Fri, 11 Mar 2022 00:18:56 GMT  
		Size: 53.6 MB (53615032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.13-windowsservercore-1809`

```console
$ docker pull docker@sha256:2351bc67908336460d6d176ad7237bd4ce87e3906d102f82fa7b9464d08f8a83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `docker:20.10.13-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull docker@sha256:11fa18bbbc94e9342dea2f011d4ac7dc0e674553a427eeac46962b7fd3bb7654
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2769425405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57844be2857bef97ed862468dd3a51e9d0dea7c7b269a9efe192aa526df18835`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:57:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 11 Mar 2022 00:15:45 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:15:46 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.13.zip
# Fri, 11 Mar 2022 00:16:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc556e75fc2ee0a56749fd9ec604591d58c7dcfbf6ddd1389aedfe0faa926127`  
		Last Modified: Wed, 09 Mar 2022 19:00:27 GMT  
		Size: 353.8 KB (353787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fcaecf749d555a0d83fad08ace6a7998307b24f4fecf9632bbfe013d112577`  
		Last Modified: Fri, 11 Mar 2022 00:18:44 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d880c105cf28c98f7d9613f331846e631375f272f037491c61f85d4cac54220d`  
		Last Modified: Fri, 11 Mar 2022 00:18:44 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2570e437e8fcb2cb9d3d91f7edafcf34ff2c23106a9aacbea7701ba1fce8d2b`  
		Last Modified: Fri, 11 Mar 2022 00:18:56 GMT  
		Size: 53.6 MB (53615032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.13-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:cd6d6c06799b236d2301e7ad57c076023ac64080624866d62810e268f91217e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.587; amd64

### `docker:20.10.13-windowsservercore-ltsc2022` - windows version 10.0.20348.587; amd64

```console
$ docker pull docker@sha256:ef007d39e5aa17f57f4ad75825febf433ea51d70fde48d5b40fea73307ffe3e8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2275653963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b8f4e76e84e2dd1842160718087208b325a794ca03ff7f14aac4b0b7b4694e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 03 Mar 2022 05:02:11 GMT
RUN Install update ltsc2022-amd64
# Tue, 08 Mar 2022 19:26:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:55:44 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 11 Mar 2022 00:15:07 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:15:08 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.13.zip
# Fri, 11 Mar 2022 00:15:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:037d5740b40414bc505c21324142a1cd3eab10c176189a9a74d1a90354ac7cd4`  
		Size: 969.5 MB (969547968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d58ba398110c3f761c6307a5621ec218b8593ba8b07b734436bcdd8d07a23e08`  
		Last Modified: Tue, 08 Mar 2022 20:00:31 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfaa4c2639ecdc27410a570e2dcb2efe02bcbec37d6ad750d15a97aac6990236`  
		Last Modified: Wed, 09 Mar 2022 18:59:14 GMT  
		Size: 598.3 KB (598260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0e605541ab33ab5774f3b41805cecf36dffbc7d02428d5bed5cbd86e1a7a0e`  
		Last Modified: Fri, 11 Mar 2022 00:17:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d060c5ba2630e8637c44694ed52a53850d5dd01c5f55f7b49493d202f48a5565`  
		Last Modified: Fri, 11 Mar 2022 00:17:32 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01c70e5c0d32c6abc7141a56d515a00df83a0786489da36fe453fa7a2b67d6d`  
		Last Modified: Fri, 11 Mar 2022 00:18:31 GMT  
		Size: 53.8 MB (53804674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:ca2744235df40f184843b2cb9f0245a6b64ae65065aad30285e80d5a266fe0c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:34c594c12507d24f66789978a90240d4addf3eb8fce22a7a9157ca9701afd46d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76152892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c05a8c965912fe35df9cce58ddb7aed725fb34d81772761a4ef7a373fd3271c1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Mar 2022 00:19:37 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:19:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Mar 2022 00:19:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Mar 2022 00:19:42 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:42 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Mar 2022 00:19:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Mar 2022 00:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:42 GMT
CMD ["sh"]
# Fri, 11 Mar 2022 00:19:47 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Mar 2022 00:19:48 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Mar 2022 00:19:48 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 11 Mar 2022 00:19:48 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Mar 2022 00:19:48 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:48 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Mar 2022 00:19:49 GMT
EXPOSE 2375 2376
# Fri, 11 Mar 2022 00:19:49 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:49 GMT
CMD []
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea03e1895df432fba23ac2810a53a408fa25273ecf001276263d810107e1c81`  
		Last Modified: Wed, 15 Dec 2021 20:20:23 GMT  
		Size: 2.0 MB (1980404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff98835b05535c14c9bd8aa0449fd33d147a58c9a9fe7f21b76137065d0f4c5`  
		Last Modified: Wed, 15 Dec 2021 20:20:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbbd0a7b1dec526be119d73f0018052afa23e65ea79e09049a54a5954f2a374`  
		Last Modified: Fri, 11 Mar 2022 00:20:32 GMT  
		Size: 64.6 MB (64612571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317ecb07c86c68358ba3d763bea251b7baf1befde793d08f074abf2743a388dc`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52850491ed6a707afb12e76035b1a36f408c071e00d1de77b26ec2cb178c9a8a`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb2b84e11d9e63efd7d7cad8459ac6f5326f44d93991a59380b186824079bdf`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd217e3dc5c63b9a21276d1a8b9b2c0a19dd9aeecf5c242902d63e8dd7c251f`  
		Last Modified: Fri, 11 Mar 2022 00:20:50 GMT  
		Size: 6.7 MB (6734617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f85497bc6212a4fbd95757776ba9f0cfc449ba5ec26f58dc4b48718582d256`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63824672dbc4b8bf906bba2cabad90a9964a4de17f7df52debc99611d2782d66`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330cf4336db2c7c1846de44144ed6eb30ac0942792712aeca3f5b38acbd16933`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 2.7 KB (2747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e6222d4d8b30c439b883f691f52e8e405f6464852c86477f7b1577dee106ee6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69841345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ba71573c3cddc7fe6d1f68e3c7c55e13f7549be38cf07414563df801aa79e1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 06:44:43 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 17 Mar 2022 06:44:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 06:44:45 GMT
ENV DOCKER_VERSION=20.10.13
# Thu, 17 Mar 2022 06:44:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Mar 2022 06:44:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Mar 2022 06:44:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:44:51 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Mar 2022 06:44:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Mar 2022 06:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 06:44:54 GMT
CMD ["sh"]
# Thu, 17 Mar 2022 06:45:06 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 17 Mar 2022 06:45:07 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 17 Mar 2022 06:45:08 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 17 Mar 2022 06:45:09 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 17 Mar 2022 06:45:11 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:45:11 GMT
VOLUME [/var/lib/docker]
# Thu, 17 Mar 2022 06:45:12 GMT
EXPOSE 2375 2376
# Thu, 17 Mar 2022 06:45:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 17 Mar 2022 06:45:14 GMT
CMD []
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bd6b2d67571b28ebbe22152f5536e3cff37d4346bc02a444b2ede9b5d71c6`  
		Last Modified: Thu, 17 Mar 2022 06:46:18 GMT  
		Size: 1.9 MB (1938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadc398c63809a7b7b0d60cee36c1a95c7dd031fb5987cb99246b289df77d64f`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fce163fc9e7e1d8912203364c303838e60da953ed77812572633504c2bd014`  
		Last Modified: Thu, 17 Mar 2022 06:46:25 GMT  
		Size: 58.6 MB (58565248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a0a3a69cb84240c8270720f964d7155438567aa97bb868bfe1adc07b5b977`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8be56eb060db5cad28d2359c143a7a7de20610f090073f5cbd7f1cfeafbd4`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746be13a2cb02a7014e32f66ba9fb3bb10e14bd43af45b7890fb09464fe2a830`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb73bd4ce74defd0741f3f7922ffb261b2f91b45cf97e2225f65aaba2b4c42d6`  
		Last Modified: Thu, 17 Mar 2022 06:46:48 GMT  
		Size: 6.6 MB (6615563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e054635e9f383caa96af63cfbbc71098384c50f5c13efcc785d2a870ed8e4af9`  
		Last Modified: Thu, 17 Mar 2022 06:46:46 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791a50930d17375d4278a896defa85218b579b3efdd1455d1fa503e187676dfb`  
		Last Modified: Thu, 17 Mar 2022 06:46:46 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752ca04529521e0b4db8ded3d79d79f1629c7c725837b87fe79519f64bcb2e05`  
		Last Modified: Thu, 17 Mar 2022 06:46:47 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:e65462ff8bfe7c34478edfb354d6a1b5c03ecf7279212fc54fc54180d2663c2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:6a92617cb4df46747dc2fd832bae2ddda144ab9c1116ea2753df44cb211a55ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 MB (96448562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d466e72290286bcdfbc871e8561fae40d9eef80790216bb18f18b5313b6e088b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Mar 2022 00:19:37 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:19:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Mar 2022 00:19:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Mar 2022 00:19:42 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:42 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Mar 2022 00:19:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Mar 2022 00:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:42 GMT
CMD ["sh"]
# Fri, 11 Mar 2022 00:19:47 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Mar 2022 00:19:48 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Mar 2022 00:19:48 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 11 Mar 2022 00:19:48 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Mar 2022 00:19:48 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:48 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Mar 2022 00:19:49 GMT
EXPOSE 2375 2376
# Fri, 11 Mar 2022 00:19:49 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:49 GMT
CMD []
# Fri, 11 Mar 2022 00:19:52 GMT
RUN apk add --no-cache iproute2
# Fri, 11 Mar 2022 00:19:53 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 11 Mar 2022 00:19:53 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 11 Mar 2022 00:19:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 11 Mar 2022 00:19:57 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 11 Mar 2022 00:19:57 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 11 Mar 2022 00:19:57 GMT
USER rootless
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea03e1895df432fba23ac2810a53a408fa25273ecf001276263d810107e1c81`  
		Last Modified: Wed, 15 Dec 2021 20:20:23 GMT  
		Size: 2.0 MB (1980404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff98835b05535c14c9bd8aa0449fd33d147a58c9a9fe7f21b76137065d0f4c5`  
		Last Modified: Wed, 15 Dec 2021 20:20:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbbd0a7b1dec526be119d73f0018052afa23e65ea79e09049a54a5954f2a374`  
		Last Modified: Fri, 11 Mar 2022 00:20:32 GMT  
		Size: 64.6 MB (64612571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317ecb07c86c68358ba3d763bea251b7baf1befde793d08f074abf2743a388dc`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52850491ed6a707afb12e76035b1a36f408c071e00d1de77b26ec2cb178c9a8a`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb2b84e11d9e63efd7d7cad8459ac6f5326f44d93991a59380b186824079bdf`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd217e3dc5c63b9a21276d1a8b9b2c0a19dd9aeecf5c242902d63e8dd7c251f`  
		Last Modified: Fri, 11 Mar 2022 00:20:50 GMT  
		Size: 6.7 MB (6734617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f85497bc6212a4fbd95757776ba9f0cfc449ba5ec26f58dc4b48718582d256`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63824672dbc4b8bf906bba2cabad90a9964a4de17f7df52debc99611d2782d66`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330cf4336db2c7c1846de44144ed6eb30ac0942792712aeca3f5b38acbd16933`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 2.7 KB (2747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9243af40d6dedb8bec94753185a0e50302ceca90029164040a3c567cfe6649ed`  
		Last Modified: Fri, 11 Mar 2022 00:21:10 GMT  
		Size: 1.2 MB (1162145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad945e48854711031ed9581488dcd35e6a7281c7cef4273cc6c4fd49fb768ebd`  
		Last Modified: Fri, 11 Mar 2022 00:21:08 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dbac2c48de1cb6054512bc0b3967aa776ed177ce538b1901e10390d2e83250`  
		Last Modified: Fri, 11 Mar 2022 00:21:09 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2445b41c3397a2f9da27c43cc92a64a2e373b418307bc1a0322072b6f87096`  
		Last Modified: Fri, 11 Mar 2022 00:21:12 GMT  
		Size: 19.1 MB (19131808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ec68c91cc2997a8e6a4a961bc06b2a2af234d24e8f116a0ba3a2e0305beaf7`  
		Last Modified: Fri, 11 Mar 2022 00:21:08 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:fb00e978daa05ad0619ff4b0bbd52dd7c000a39954746498aadc6d94ac35194a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92132138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20955ed3fe29f7eca363024931545542a3e3bcaddd6de747255b806cb75f8c3d`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 06:44:43 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 17 Mar 2022 06:44:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 06:44:45 GMT
ENV DOCKER_VERSION=20.10.13
# Thu, 17 Mar 2022 06:44:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Mar 2022 06:44:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Mar 2022 06:44:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:44:51 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Mar 2022 06:44:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Mar 2022 06:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 06:44:54 GMT
CMD ["sh"]
# Thu, 17 Mar 2022 06:45:06 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 17 Mar 2022 06:45:07 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 17 Mar 2022 06:45:08 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 17 Mar 2022 06:45:09 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 17 Mar 2022 06:45:11 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:45:11 GMT
VOLUME [/var/lib/docker]
# Thu, 17 Mar 2022 06:45:12 GMT
EXPOSE 2375 2376
# Thu, 17 Mar 2022 06:45:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 17 Mar 2022 06:45:14 GMT
CMD []
# Thu, 17 Mar 2022 06:45:22 GMT
RUN apk add --no-cache iproute2
# Thu, 17 Mar 2022 06:45:23 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 17 Mar 2022 06:45:24 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 17 Mar 2022 06:45:27 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 17 Mar 2022 06:45:27 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 17 Mar 2022 06:45:28 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 17 Mar 2022 06:45:29 GMT
USER rootless
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bd6b2d67571b28ebbe22152f5536e3cff37d4346bc02a444b2ede9b5d71c6`  
		Last Modified: Thu, 17 Mar 2022 06:46:18 GMT  
		Size: 1.9 MB (1938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadc398c63809a7b7b0d60cee36c1a95c7dd031fb5987cb99246b289df77d64f`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fce163fc9e7e1d8912203364c303838e60da953ed77812572633504c2bd014`  
		Last Modified: Thu, 17 Mar 2022 06:46:25 GMT  
		Size: 58.6 MB (58565248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a0a3a69cb84240c8270720f964d7155438567aa97bb868bfe1adc07b5b977`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8be56eb060db5cad28d2359c143a7a7de20610f090073f5cbd7f1cfeafbd4`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746be13a2cb02a7014e32f66ba9fb3bb10e14bd43af45b7890fb09464fe2a830`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb73bd4ce74defd0741f3f7922ffb261b2f91b45cf97e2225f65aaba2b4c42d6`  
		Last Modified: Thu, 17 Mar 2022 06:46:48 GMT  
		Size: 6.6 MB (6615563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e054635e9f383caa96af63cfbbc71098384c50f5c13efcc785d2a870ed8e4af9`  
		Last Modified: Thu, 17 Mar 2022 06:46:46 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791a50930d17375d4278a896defa85218b579b3efdd1455d1fa503e187676dfb`  
		Last Modified: Thu, 17 Mar 2022 06:46:46 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752ca04529521e0b4db8ded3d79d79f1629c7c725837b87fe79519f64bcb2e05`  
		Last Modified: Thu, 17 Mar 2022 06:46:47 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b68e435beb33fd13cba08b839c86323a9ea7d3c280f4e09040d67dd21cfd835`  
		Last Modified: Thu, 17 Mar 2022 06:47:11 GMT  
		Size: 1.2 MB (1177952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f4ab31ae44292e2bfb84410de85f6a729607613d6dbef35902577fcbe78e4f`  
		Last Modified: Thu, 17 Mar 2022 06:47:10 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72e8ed3a93a11307aba41a4d0f7ffb6302f7de9886d46bf2562f06ab3e01e3f`  
		Last Modified: Thu, 17 Mar 2022 06:47:10 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768a72d3947b3532412cc42dd744996a22bf0574cebf60ac1119be3ca7530922`  
		Last Modified: Thu, 17 Mar 2022 06:47:14 GMT  
		Size: 21.1 MB (21111220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dec4d02116a97f8282cc9d24eaf55d48d469e3ad232980a8724940ba2a07ed3`  
		Last Modified: Thu, 17 Mar 2022 06:47:10 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:5ec008af09dcdc65abc239b6f492af27f37a9c7ec94148f40703ca622a5faba5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:7383e8c2efcd6846670dd96ca1b6af84b7a4098fd778b85cee0ae2739301a79c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76237387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f328899fc7a17e58951f5523f603df43687ea162ad1f8f04eed66b876e9480ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Mar 2022 00:19:37 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:19:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Mar 2022 00:19:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Mar 2022 00:19:42 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:42 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Mar 2022 00:19:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Mar 2022 00:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:42 GMT
CMD ["sh"]
# Fri, 11 Mar 2022 00:20:00 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea03e1895df432fba23ac2810a53a408fa25273ecf001276263d810107e1c81`  
		Last Modified: Wed, 15 Dec 2021 20:20:23 GMT  
		Size: 2.0 MB (1980404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff98835b05535c14c9bd8aa0449fd33d147a58c9a9fe7f21b76137065d0f4c5`  
		Last Modified: Wed, 15 Dec 2021 20:20:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbbd0a7b1dec526be119d73f0018052afa23e65ea79e09049a54a5954f2a374`  
		Last Modified: Fri, 11 Mar 2022 00:20:32 GMT  
		Size: 64.6 MB (64612571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317ecb07c86c68358ba3d763bea251b7baf1befde793d08f074abf2743a388dc`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52850491ed6a707afb12e76035b1a36f408c071e00d1de77b26ec2cb178c9a8a`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb2b84e11d9e63efd7d7cad8459ac6f5326f44d93991a59380b186824079bdf`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc827496373a4a4176b9c5e48d8ea6bb5823b745c62a5ddd68e6b201ae7341d`  
		Last Modified: Fri, 11 Mar 2022 00:21:30 GMT  
		Size: 6.8 MB (6824133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:72b64e64f292fcc354064aff807584ba6aa24c62dcaacd0f4180974d732d7c33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70153837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a742244413c82313c84ffc8e2aae4a5e443443e2e7c6283b00bc9d89c10d767`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 06:44:43 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 17 Mar 2022 06:44:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 06:44:45 GMT
ENV DOCKER_VERSION=20.10.13
# Thu, 17 Mar 2022 06:44:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Mar 2022 06:44:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Mar 2022 06:44:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:44:51 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Mar 2022 06:44:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Mar 2022 06:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 06:44:54 GMT
CMD ["sh"]
# Thu, 17 Mar 2022 06:45:36 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bd6b2d67571b28ebbe22152f5536e3cff37d4346bc02a444b2ede9b5d71c6`  
		Last Modified: Thu, 17 Mar 2022 06:46:18 GMT  
		Size: 1.9 MB (1938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadc398c63809a7b7b0d60cee36c1a95c7dd031fb5987cb99246b289df77d64f`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fce163fc9e7e1d8912203364c303838e60da953ed77812572633504c2bd014`  
		Last Modified: Thu, 17 Mar 2022 06:46:25 GMT  
		Size: 58.6 MB (58565248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a0a3a69cb84240c8270720f964d7155438567aa97bb868bfe1adc07b5b977`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8be56eb060db5cad28d2359c143a7a7de20610f090073f5cbd7f1cfeafbd4`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746be13a2cb02a7014e32f66ba9fb3bb10e14bd43af45b7890fb09464fe2a830`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2716e163322a30318e4b5622ac98de0815fd95f93070ec60e4ee6ea3a3f85b59`  
		Last Modified: Thu, 17 Mar 2022 06:47:35 GMT  
		Size: 6.9 MB (6933048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:72e87d4f1d2ed054bf9ec48c77dfc546c7e6173fe9b6afd9e80716b9c5ade4bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:338217655cdf830e6f659207f447776c8debaf1c3cbce0050645c2b621893d6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69413254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6816f070b2395d750ce78e4fbdb7e9df0af63b7686f3063c09e008c2ef1a0036`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Mar 2022 00:19:37 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:19:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Mar 2022 00:19:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Mar 2022 00:19:42 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:42 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Mar 2022 00:19:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Mar 2022 00:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:42 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea03e1895df432fba23ac2810a53a408fa25273ecf001276263d810107e1c81`  
		Last Modified: Wed, 15 Dec 2021 20:20:23 GMT  
		Size: 2.0 MB (1980404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff98835b05535c14c9bd8aa0449fd33d147a58c9a9fe7f21b76137065d0f4c5`  
		Last Modified: Wed, 15 Dec 2021 20:20:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbbd0a7b1dec526be119d73f0018052afa23e65ea79e09049a54a5954f2a374`  
		Last Modified: Fri, 11 Mar 2022 00:20:32 GMT  
		Size: 64.6 MB (64612571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317ecb07c86c68358ba3d763bea251b7baf1befde793d08f074abf2743a388dc`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52850491ed6a707afb12e76035b1a36f408c071e00d1de77b26ec2cb178c9a8a`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb2b84e11d9e63efd7d7cad8459ac6f5326f44d93991a59380b186824079bdf`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:576a187cf88c74c82b1cda12e206a8e20e24633499128894296909a44456f82a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63220789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51ae867936fd1dc5c38dab32635ffb031fba90112aaf70cd838fdf678922f0b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 06:44:43 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 17 Mar 2022 06:44:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 06:44:45 GMT
ENV DOCKER_VERSION=20.10.13
# Thu, 17 Mar 2022 06:44:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Mar 2022 06:44:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Mar 2022 06:44:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:44:51 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Mar 2022 06:44:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Mar 2022 06:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 06:44:54 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bd6b2d67571b28ebbe22152f5536e3cff37d4346bc02a444b2ede9b5d71c6`  
		Last Modified: Thu, 17 Mar 2022 06:46:18 GMT  
		Size: 1.9 MB (1938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadc398c63809a7b7b0d60cee36c1a95c7dd031fb5987cb99246b289df77d64f`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fce163fc9e7e1d8912203364c303838e60da953ed77812572633504c2bd014`  
		Last Modified: Thu, 17 Mar 2022 06:46:25 GMT  
		Size: 58.6 MB (58565248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a0a3a69cb84240c8270720f964d7155438567aa97bb868bfe1adc07b5b977`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8be56eb060db5cad28d2359c143a7a7de20610f090073f5cbd7f1cfeafbd4`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746be13a2cb02a7014e32f66ba9fb3bb10e14bd43af45b7890fb09464fe2a830`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore`

```console
$ docker pull docker@sha256:998f6c6a8ca0e9871ae959625b33ded24ef0dbf102278d815ca5c2ca91708e33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.587; amd64
	-	windows version 10.0.17763.2686; amd64

### `docker:windowsservercore` - windows version 10.0.20348.587; amd64

```console
$ docker pull docker@sha256:ef007d39e5aa17f57f4ad75825febf433ea51d70fde48d5b40fea73307ffe3e8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2275653963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b8f4e76e84e2dd1842160718087208b325a794ca03ff7f14aac4b0b7b4694e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 03 Mar 2022 05:02:11 GMT
RUN Install update ltsc2022-amd64
# Tue, 08 Mar 2022 19:26:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:55:44 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 11 Mar 2022 00:15:07 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:15:08 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.13.zip
# Fri, 11 Mar 2022 00:15:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:037d5740b40414bc505c21324142a1cd3eab10c176189a9a74d1a90354ac7cd4`  
		Size: 969.5 MB (969547968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d58ba398110c3f761c6307a5621ec218b8593ba8b07b734436bcdd8d07a23e08`  
		Last Modified: Tue, 08 Mar 2022 20:00:31 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfaa4c2639ecdc27410a570e2dcb2efe02bcbec37d6ad750d15a97aac6990236`  
		Last Modified: Wed, 09 Mar 2022 18:59:14 GMT  
		Size: 598.3 KB (598260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0e605541ab33ab5774f3b41805cecf36dffbc7d02428d5bed5cbd86e1a7a0e`  
		Last Modified: Fri, 11 Mar 2022 00:17:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d060c5ba2630e8637c44694ed52a53850d5dd01c5f55f7b49493d202f48a5565`  
		Last Modified: Fri, 11 Mar 2022 00:17:32 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01c70e5c0d32c6abc7141a56d515a00df83a0786489da36fe453fa7a2b67d6d`  
		Last Modified: Fri, 11 Mar 2022 00:18:31 GMT  
		Size: 53.8 MB (53804674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull docker@sha256:11fa18bbbc94e9342dea2f011d4ac7dc0e674553a427eeac46962b7fd3bb7654
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2769425405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57844be2857bef97ed862468dd3a51e9d0dea7c7b269a9efe192aa526df18835`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:57:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 11 Mar 2022 00:15:45 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:15:46 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.13.zip
# Fri, 11 Mar 2022 00:16:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc556e75fc2ee0a56749fd9ec604591d58c7dcfbf6ddd1389aedfe0faa926127`  
		Last Modified: Wed, 09 Mar 2022 19:00:27 GMT  
		Size: 353.8 KB (353787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fcaecf749d555a0d83fad08ace6a7998307b24f4fecf9632bbfe013d112577`  
		Last Modified: Fri, 11 Mar 2022 00:18:44 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d880c105cf28c98f7d9613f331846e631375f272f037491c61f85d4cac54220d`  
		Last Modified: Fri, 11 Mar 2022 00:18:44 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2570e437e8fcb2cb9d3d91f7edafcf34ff2c23106a9aacbea7701ba1fce8d2b`  
		Last Modified: Fri, 11 Mar 2022 00:18:56 GMT  
		Size: 53.6 MB (53615032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:2351bc67908336460d6d176ad7237bd4ce87e3906d102f82fa7b9464d08f8a83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull docker@sha256:11fa18bbbc94e9342dea2f011d4ac7dc0e674553a427eeac46962b7fd3bb7654
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2769425405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57844be2857bef97ed862468dd3a51e9d0dea7c7b269a9efe192aa526df18835`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:57:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 11 Mar 2022 00:15:45 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:15:46 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.13.zip
# Fri, 11 Mar 2022 00:16:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc556e75fc2ee0a56749fd9ec604591d58c7dcfbf6ddd1389aedfe0faa926127`  
		Last Modified: Wed, 09 Mar 2022 19:00:27 GMT  
		Size: 353.8 KB (353787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fcaecf749d555a0d83fad08ace6a7998307b24f4fecf9632bbfe013d112577`  
		Last Modified: Fri, 11 Mar 2022 00:18:44 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d880c105cf28c98f7d9613f331846e631375f272f037491c61f85d4cac54220d`  
		Last Modified: Fri, 11 Mar 2022 00:18:44 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2570e437e8fcb2cb9d3d91f7edafcf34ff2c23106a9aacbea7701ba1fce8d2b`  
		Last Modified: Fri, 11 Mar 2022 00:18:56 GMT  
		Size: 53.6 MB (53615032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:cd6d6c06799b236d2301e7ad57c076023ac64080624866d62810e268f91217e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.587; amd64

### `docker:windowsservercore-ltsc2022` - windows version 10.0.20348.587; amd64

```console
$ docker pull docker@sha256:ef007d39e5aa17f57f4ad75825febf433ea51d70fde48d5b40fea73307ffe3e8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2275653963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b8f4e76e84e2dd1842160718087208b325a794ca03ff7f14aac4b0b7b4694e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 03 Mar 2022 05:02:11 GMT
RUN Install update ltsc2022-amd64
# Tue, 08 Mar 2022 19:26:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:55:44 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 11 Mar 2022 00:15:07 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:15:08 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.13.zip
# Fri, 11 Mar 2022 00:15:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:037d5740b40414bc505c21324142a1cd3eab10c176189a9a74d1a90354ac7cd4`  
		Size: 969.5 MB (969547968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d58ba398110c3f761c6307a5621ec218b8593ba8b07b734436bcdd8d07a23e08`  
		Last Modified: Tue, 08 Mar 2022 20:00:31 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfaa4c2639ecdc27410a570e2dcb2efe02bcbec37d6ad750d15a97aac6990236`  
		Last Modified: Wed, 09 Mar 2022 18:59:14 GMT  
		Size: 598.3 KB (598260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0e605541ab33ab5774f3b41805cecf36dffbc7d02428d5bed5cbd86e1a7a0e`  
		Last Modified: Fri, 11 Mar 2022 00:17:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d060c5ba2630e8637c44694ed52a53850d5dd01c5f55f7b49493d202f48a5565`  
		Last Modified: Fri, 11 Mar 2022 00:17:32 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01c70e5c0d32c6abc7141a56d515a00df83a0786489da36fe453fa7a2b67d6d`  
		Last Modified: Fri, 11 Mar 2022 00:18:31 GMT  
		Size: 53.8 MB (53804674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
