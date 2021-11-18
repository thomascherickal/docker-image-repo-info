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
-	[`docker:20.10.11`](#docker201011)
-	[`docker:20.10.11-alpine3.14`](#docker201011-alpine314)
-	[`docker:20.10.11-dind`](#docker201011-dind)
-	[`docker:20.10.11-dind-alpine3.14`](#docker201011-dind-alpine314)
-	[`docker:20.10.11-dind-rootless`](#docker201011-dind-rootless)
-	[`docker:20.10.11-git`](#docker201011-git)
-	[`docker:20.10.11-windowsservercore`](#docker201011-windowsservercore)
-	[`docker:20.10.11-windowsservercore-1809`](#docker201011-windowsservercore-1809)
-	[`docker:dind`](#dockerdind)
-	[`docker:dind-rootless`](#dockerdind-rootless)
-	[`docker:git`](#dockergit)
-	[`docker:latest`](#dockerlatest)
-	[`docker:windowsservercore`](#dockerwindowsservercore)
-	[`docker:windowsservercore-1809`](#dockerwindowsservercore-1809)

## `docker:20`

```console
$ docker pull docker@sha256:ff4fcc30e7c20f33c021e82683aedd1fe66654363eb1ff61065e0628f5bbf107
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20` - linux; amd64

```console
$ docker pull docker@sha256:0cd49922b08a5b66239fc764abe872f4799e291922e21a31d9490a10278a5a02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68479082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c655f708b2a86c4b241e80a784479ee098833dc55d9d3929e1e35e1cb0297c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:00:59 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 12 Nov 2021 22:01:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 16:02:11 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 16:02:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 16:02:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 16:02:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:19 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b81e4bf1fdc42d15e4c1cfd4aa82e5fe027cf88bd858b5be7681ef621c617`  
		Last Modified: Fri, 12 Nov 2021 22:02:42 GMT  
		Size: 1.9 MB (1937203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da79b3d4ea6e72fe17974fcd737705b6da38e9063e5bbb26cea5a9fa7465bae`  
		Last Modified: Fri, 12 Nov 2021 22:02:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9433235d3590c575f74cf6c833b63c7e5fd2c2ebf7017a086421fb465c67327`  
		Last Modified: Thu, 18 Nov 2021 16:03:22 GMT  
		Size: 63.7 MB (63717036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a370fc1bfda2f2192e17db23cd29f495b5c0b6ab9f36d73ec07a9dbdae1310`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c0972549c69874ec2e53b7534184e975853ec9602f9a7ba7466bb1a231db9`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a0159d8a68d2886d05e662c609ac1dc10a9e3b73244d73106b8888a3bddfbb`  
		Last Modified: Thu, 18 Nov 2021 16:03:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8aef5b543363230546c03371e8b3c857285ffdad566b676c3657cf64fedd9299
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62375513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0836e8a2fd6d55074387335d0a134d329cedce53561a1b6fc6eefe44cf1cf487`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:12:04 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Sat, 13 Nov 2021 11:12:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 09:17:16 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 09:17:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 09:17:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 09:17:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:25 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 09:17:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 09:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:28 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233f664f6e365c4259a38e7cfe3c14e234ab45f15847cc874a88b510f66a132f`  
		Last Modified: Sat, 13 Nov 2021 11:13:40 GMT  
		Size: 1.9 MB (1909969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c7cbdd3e377ff292e68f9ced99315b84c85398591633343352948bbc291`  
		Last Modified: Sat, 13 Nov 2021 11:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b50fed93df89351d596ab08fab482a174aa37a86d61cdeef150162665a67a80`  
		Last Modified: Thu, 18 Nov 2021 09:18:59 GMT  
		Size: 57.7 MB (57746015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21638a3c07c5ebd6977bcc9c75e0ac36c2a82b761fc51a8aee313c9a9d7ed46`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e37a1bae185ca8552a00efd7984a74bc595d0dac82ab81e945615f5a0b29af`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81c4e38c2d1b6603791a26f4dad582d554c306fb4c8c4218e0d537da3b8af6a`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind`

```console
$ docker pull docker@sha256:79d0c6e997920e71e96571ef434defcca1364d693d5b937232decf1ee7524a9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind` - linux; amd64

```console
$ docker pull docker@sha256:1ff5e500e2d42048923c1243ad26691c83c65406a33086f56e02e4fb2d43ecd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75006729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5261796049dd8a51b9e1c9ab5fa3e06960de7a813e7414dcc218022a6eb48680`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:00:59 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 12 Nov 2021 22:01:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 16:02:11 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 16:02:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 16:02:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 16:02:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:19 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 16:02:26 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 18 Nov 2021 16:02:27 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 18 Nov 2021 16:02:27 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 18 Nov 2021 16:02:28 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 18 Nov 2021 16:02:28 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:28 GMT
VOLUME [/var/lib/docker]
# Thu, 18 Nov 2021 16:02:29 GMT
EXPOSE 2375 2376
# Thu, 18 Nov 2021 16:02:29 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:29 GMT
CMD []
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b81e4bf1fdc42d15e4c1cfd4aa82e5fe027cf88bd858b5be7681ef621c617`  
		Last Modified: Fri, 12 Nov 2021 22:02:42 GMT  
		Size: 1.9 MB (1937203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da79b3d4ea6e72fe17974fcd737705b6da38e9063e5bbb26cea5a9fa7465bae`  
		Last Modified: Fri, 12 Nov 2021 22:02:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9433235d3590c575f74cf6c833b63c7e5fd2c2ebf7017a086421fb465c67327`  
		Last Modified: Thu, 18 Nov 2021 16:03:22 GMT  
		Size: 63.7 MB (63717036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a370fc1bfda2f2192e17db23cd29f495b5c0b6ab9f36d73ec07a9dbdae1310`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c0972549c69874ec2e53b7534184e975853ec9602f9a7ba7466bb1a231db9`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a0159d8a68d2886d05e662c609ac1dc10a9e3b73244d73106b8888a3bddfbb`  
		Last Modified: Thu, 18 Nov 2021 16:03:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2667e9a1d0ba047230eab7daedb7556a9d2204adebca9d7439ecaae6dbc1e3`  
		Last Modified: Thu, 18 Nov 2021 16:03:48 GMT  
		Size: 6.5 MB (6522755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f72da5423b84bdb2e04379edb8747ff161388fe38280eb242ef4d802008bf96`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b9fb6f0baf688ba32368dc395c50842182a9a4cadafd2cc0964570f740cd9a`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd10f5a3a8ed006ba472a52473be2b1f099d4b3b4cc8cdf52bae991cac915e0`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:6b91496cd8473f8f0412be846318dcf073a41e5c02fea27a75a657376c55e83b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68798719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9280bbaf2b20c01dbbcd50930cb5862adc44e531d88f54d157358d16f7de8a5f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:12:04 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Sat, 13 Nov 2021 11:12:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 09:17:16 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 09:17:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 09:17:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 09:17:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:25 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 09:17:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 09:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:28 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 09:17:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 18 Nov 2021 09:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 18 Nov 2021 09:17:40 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 18 Nov 2021 09:17:41 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 18 Nov 2021 09:17:43 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:43 GMT
VOLUME [/var/lib/docker]
# Thu, 18 Nov 2021 09:17:44 GMT
EXPOSE 2375 2376
# Thu, 18 Nov 2021 09:17:45 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:46 GMT
CMD []
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233f664f6e365c4259a38e7cfe3c14e234ab45f15847cc874a88b510f66a132f`  
		Last Modified: Sat, 13 Nov 2021 11:13:40 GMT  
		Size: 1.9 MB (1909969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c7cbdd3e377ff292e68f9ced99315b84c85398591633343352948bbc291`  
		Last Modified: Sat, 13 Nov 2021 11:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b50fed93df89351d596ab08fab482a174aa37a86d61cdeef150162665a67a80`  
		Last Modified: Thu, 18 Nov 2021 09:18:59 GMT  
		Size: 57.7 MB (57746015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21638a3c07c5ebd6977bcc9c75e0ac36c2a82b761fc51a8aee313c9a9d7ed46`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e37a1bae185ca8552a00efd7984a74bc595d0dac82ab81e945615f5a0b29af`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81c4e38c2d1b6603791a26f4dad582d554c306fb4c8c4218e0d537da3b8af6a`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc29a86f7ed1b15ec5c146abf64a41609779eb5b0e2a668d274b1b28c14c37e3`  
		Last Modified: Thu, 18 Nov 2021 09:19:20 GMT  
		Size: 6.4 MB (6418345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce285f2fd3dbcbe5e58749e817ef3a3e60fa1dbf82bc51eaff0f20f8e151d3f`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeabdc4aba67b4850e7e5c118e6409d59a161d11f5be536341a4e9f40ed017bf`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd2d42122e3f199551259bf3db06d2c446c725eb3ae3239f2692f3fa57804b5`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:154d9287cc128b8c4820b8d412652064cccd1466a61a50af871062b82cc05f6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:165b8b4bb284183bb67f3cb4617d84032b4d31d2a537e2bce63d016044a438c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95282418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:956ab016b037de2042fec25d130ac6a9aaa029a8183fff6512e356e2d44b205f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:00:59 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 12 Nov 2021 22:01:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 16:02:11 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 16:02:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 16:02:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 16:02:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:19 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 16:02:26 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 18 Nov 2021 16:02:27 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 18 Nov 2021 16:02:27 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 18 Nov 2021 16:02:28 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 18 Nov 2021 16:02:28 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:28 GMT
VOLUME [/var/lib/docker]
# Thu, 18 Nov 2021 16:02:29 GMT
EXPOSE 2375 2376
# Thu, 18 Nov 2021 16:02:29 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:29 GMT
CMD []
# Thu, 18 Nov 2021 16:02:33 GMT
RUN apk add --no-cache iproute2
# Thu, 18 Nov 2021 16:02:34 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 18 Nov 2021 16:02:35 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 18 Nov 2021 16:02:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 18 Nov 2021 16:02:38 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 18 Nov 2021 16:02:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 18 Nov 2021 16:02:39 GMT
USER rootless
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b81e4bf1fdc42d15e4c1cfd4aa82e5fe027cf88bd858b5be7681ef621c617`  
		Last Modified: Fri, 12 Nov 2021 22:02:42 GMT  
		Size: 1.9 MB (1937203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da79b3d4ea6e72fe17974fcd737705b6da38e9063e5bbb26cea5a9fa7465bae`  
		Last Modified: Fri, 12 Nov 2021 22:02:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9433235d3590c575f74cf6c833b63c7e5fd2c2ebf7017a086421fb465c67327`  
		Last Modified: Thu, 18 Nov 2021 16:03:22 GMT  
		Size: 63.7 MB (63717036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a370fc1bfda2f2192e17db23cd29f495b5c0b6ab9f36d73ec07a9dbdae1310`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c0972549c69874ec2e53b7534184e975853ec9602f9a7ba7466bb1a231db9`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a0159d8a68d2886d05e662c609ac1dc10a9e3b73244d73106b8888a3bddfbb`  
		Last Modified: Thu, 18 Nov 2021 16:03:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2667e9a1d0ba047230eab7daedb7556a9d2204adebca9d7439ecaae6dbc1e3`  
		Last Modified: Thu, 18 Nov 2021 16:03:48 GMT  
		Size: 6.5 MB (6522755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f72da5423b84bdb2e04379edb8747ff161388fe38280eb242ef4d802008bf96`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b9fb6f0baf688ba32368dc395c50842182a9a4cadafd2cc0964570f740cd9a`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd10f5a3a8ed006ba472a52473be2b1f099d4b3b4cc8cdf52bae991cac915e0`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e11d3f7e286c938d26bbb186acb5479276df6361d8df2dcd69411be8e3a69d7`  
		Last Modified: Thu, 18 Nov 2021 16:04:10 GMT  
		Size: 1.1 MB (1149116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f294faaf6353a52c03a2b9dcfa622a83436f037202b20fb7683021db79e775`  
		Last Modified: Thu, 18 Nov 2021 16:04:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b662b3e60558d88a695d82eff536d1ce83c74cca00618f4a905ed756ca05f241`  
		Last Modified: Thu, 18 Nov 2021 16:04:10 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45688b3cc691166b57c28f4fadfe415eb8c9bdf22e92e43a60b0c7e50071a3ac`  
		Last Modified: Thu, 18 Nov 2021 16:04:15 GMT  
		Size: 19.1 MB (19124859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1ee7128b0e98cd946608ca63e413eeb9b68f68eedd4f1d58ff71fed621291b`  
		Last Modified: Thu, 18 Nov 2021 16:04:10 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:2441b89586372dc59c8fce28fc3fa0a6141193ad158d18482597187a7e1c9eeb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91070455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c509ba52a7374da993e6cf01a7147518857077192831cf839078772fa27881b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:12:04 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Sat, 13 Nov 2021 11:12:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 09:17:16 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 09:17:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 09:17:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 09:17:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:25 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 09:17:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 09:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:28 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 09:17:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 18 Nov 2021 09:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 18 Nov 2021 09:17:40 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 18 Nov 2021 09:17:41 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 18 Nov 2021 09:17:43 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:43 GMT
VOLUME [/var/lib/docker]
# Thu, 18 Nov 2021 09:17:44 GMT
EXPOSE 2375 2376
# Thu, 18 Nov 2021 09:17:45 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:46 GMT
CMD []
# Thu, 18 Nov 2021 09:17:54 GMT
RUN apk add --no-cache iproute2
# Thu, 18 Nov 2021 09:17:55 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 18 Nov 2021 09:17:56 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 18 Nov 2021 09:17:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 18 Nov 2021 09:18:00 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 18 Nov 2021 09:18:01 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 18 Nov 2021 09:18:02 GMT
USER rootless
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233f664f6e365c4259a38e7cfe3c14e234ab45f15847cc874a88b510f66a132f`  
		Last Modified: Sat, 13 Nov 2021 11:13:40 GMT  
		Size: 1.9 MB (1909969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c7cbdd3e377ff292e68f9ced99315b84c85398591633343352948bbc291`  
		Last Modified: Sat, 13 Nov 2021 11:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b50fed93df89351d596ab08fab482a174aa37a86d61cdeef150162665a67a80`  
		Last Modified: Thu, 18 Nov 2021 09:18:59 GMT  
		Size: 57.7 MB (57746015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21638a3c07c5ebd6977bcc9c75e0ac36c2a82b761fc51a8aee313c9a9d7ed46`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e37a1bae185ca8552a00efd7984a74bc595d0dac82ab81e945615f5a0b29af`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81c4e38c2d1b6603791a26f4dad582d554c306fb4c8c4218e0d537da3b8af6a`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc29a86f7ed1b15ec5c146abf64a41609779eb5b0e2a668d274b1b28c14c37e3`  
		Last Modified: Thu, 18 Nov 2021 09:19:20 GMT  
		Size: 6.4 MB (6418345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce285f2fd3dbcbe5e58749e817ef3a3e60fa1dbf82bc51eaff0f20f8e151d3f`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeabdc4aba67b4850e7e5c118e6409d59a161d11f5be536341a4e9f40ed017bf`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd2d42122e3f199551259bf3db06d2c446c725eb3ae3239f2692f3fa57804b5`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230963f6db0e75d3a58bc46d5b33ea4f67e6b1f0300e99ba12497c89f68ce855`  
		Last Modified: Thu, 18 Nov 2021 09:19:41 GMT  
		Size: 1.2 MB (1168585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66cc595973e50f8d3e25c628464cfa45436824aab478bda61c9ac4232d822c3`  
		Last Modified: Thu, 18 Nov 2021 09:19:40 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55af54131c4a2bf83efebe4e4fec2d50bd4c99ffbca5aa5ccfa29c167f4c16ce`  
		Last Modified: Thu, 18 Nov 2021 09:19:40 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cab39e5c6b0a896c570c0218f29e0600936018957c487e7b439c9ecf14ad8e`  
		Last Modified: Thu, 18 Nov 2021 09:19:44 GMT  
		Size: 21.1 MB (21101528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365691e2dffd5c75fa3b86bd4ccd1b11a4beae986f511ce5400a6a3d69b550c`  
		Last Modified: Thu, 18 Nov 2021 09:19:40 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-git`

```console
$ docker pull docker@sha256:50fdfef2982984d5f587a8274e932da365b322388804a9f1b30ef5eac2524527
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-git` - linux; amd64

```console
$ docker pull docker@sha256:dd201d3335196a559cdc166592a7acfbe9545e25aa83baa8c7e90fbee9353172
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75109809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26ae7c6d74e81d7ec18428ac5cdf0879073d8e746c341bf389aad8593a235e83`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:00:59 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 12 Nov 2021 22:01:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 16:02:11 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 16:02:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 16:02:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 16:02:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:19 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 16:02:43 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b81e4bf1fdc42d15e4c1cfd4aa82e5fe027cf88bd858b5be7681ef621c617`  
		Last Modified: Fri, 12 Nov 2021 22:02:42 GMT  
		Size: 1.9 MB (1937203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da79b3d4ea6e72fe17974fcd737705b6da38e9063e5bbb26cea5a9fa7465bae`  
		Last Modified: Fri, 12 Nov 2021 22:02:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9433235d3590c575f74cf6c833b63c7e5fd2c2ebf7017a086421fb465c67327`  
		Last Modified: Thu, 18 Nov 2021 16:03:22 GMT  
		Size: 63.7 MB (63717036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a370fc1bfda2f2192e17db23cd29f495b5c0b6ab9f36d73ec07a9dbdae1310`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c0972549c69874ec2e53b7534184e975853ec9602f9a7ba7466bb1a231db9`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a0159d8a68d2886d05e662c609ac1dc10a9e3b73244d73106b8888a3bddfbb`  
		Last Modified: Thu, 18 Nov 2021 16:03:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f4768f31acf9871e50a178b839a569a05c1b6a8923f4644db556da09776dbb`  
		Last Modified: Thu, 18 Nov 2021 16:04:34 GMT  
		Size: 6.6 MB (6630727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:abd4f25a749ebaac21635348b5e8db17d1d7cc5bcfa3b437e730b4178177cd2f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69115687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eb4264b475ad1b401f8776fd4d94293173ddd396cf1a88a5fb4372947b3ef3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:12:04 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Sat, 13 Nov 2021 11:12:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 09:17:16 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 09:17:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 09:17:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 09:17:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:25 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 09:17:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 09:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:28 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 09:18:09 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233f664f6e365c4259a38e7cfe3c14e234ab45f15847cc874a88b510f66a132f`  
		Last Modified: Sat, 13 Nov 2021 11:13:40 GMT  
		Size: 1.9 MB (1909969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c7cbdd3e377ff292e68f9ced99315b84c85398591633343352948bbc291`  
		Last Modified: Sat, 13 Nov 2021 11:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b50fed93df89351d596ab08fab482a174aa37a86d61cdeef150162665a67a80`  
		Last Modified: Thu, 18 Nov 2021 09:18:59 GMT  
		Size: 57.7 MB (57746015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21638a3c07c5ebd6977bcc9c75e0ac36c2a82b761fc51a8aee313c9a9d7ed46`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e37a1bae185ca8552a00efd7984a74bc595d0dac82ab81e945615f5a0b29af`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81c4e38c2d1b6603791a26f4dad582d554c306fb4c8c4218e0d537da3b8af6a`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d06f8877e01ae57a21f32e8cdd5b66ffc3fdf70cfb5c8036a429db1ed15e12`  
		Last Modified: Thu, 18 Nov 2021 09:20:04 GMT  
		Size: 6.7 MB (6740174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore`

```console
$ docker pull docker@sha256:280e2bfd85a1840bc5220777f9d70a85a6bf7fb35a3d8a03275043b5bdd07fb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `docker:20-windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull docker@sha256:f9935026e3d4f01f6ffe7c97d63ee7f286c77f52f80e2f1be8afe7de69ba531c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2757389706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feec87f6f82e9966337409c1601a519ee1ddc39fb68c10dbfbbb4cc6328de03d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 19:07:02 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 18 Nov 2021 04:13:52 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 04:13:53 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.11.zip
# Thu, 18 Nov 2021 04:15:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e42405e6d7d9caeb7c5a114493eca7f34351fae0fc2b77118957003b2f6c5f`  
		Last Modified: Wed, 10 Nov 2021 19:08:27 GMT  
		Size: 356.8 KB (356764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568ddc925a63c78da177f9676136448290dfbb54e31f140f98a3d4e0f3cfdc6d`  
		Last Modified: Thu, 18 Nov 2021 04:15:36 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a4753c3e1103c5a6292410a73e0d9eeeaa777557870a6d95dae8c80d822305`  
		Last Modified: Thu, 18 Nov 2021 04:15:36 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc58abb4c9cd5805540f354d6ba7931a7afec3062b7f8ff918c78378ac5d876f`  
		Last Modified: Thu, 18 Nov 2021 04:16:34 GMT  
		Size: 50.9 MB (50907794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-1809`

```console
$ docker pull docker@sha256:280e2bfd85a1840bc5220777f9d70a85a6bf7fb35a3d8a03275043b5bdd07fb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `docker:20-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull docker@sha256:f9935026e3d4f01f6ffe7c97d63ee7f286c77f52f80e2f1be8afe7de69ba531c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2757389706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feec87f6f82e9966337409c1601a519ee1ddc39fb68c10dbfbbb4cc6328de03d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 19:07:02 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 18 Nov 2021 04:13:52 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 04:13:53 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.11.zip
# Thu, 18 Nov 2021 04:15:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e42405e6d7d9caeb7c5a114493eca7f34351fae0fc2b77118957003b2f6c5f`  
		Last Modified: Wed, 10 Nov 2021 19:08:27 GMT  
		Size: 356.8 KB (356764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568ddc925a63c78da177f9676136448290dfbb54e31f140f98a3d4e0f3cfdc6d`  
		Last Modified: Thu, 18 Nov 2021 04:15:36 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a4753c3e1103c5a6292410a73e0d9eeeaa777557870a6d95dae8c80d822305`  
		Last Modified: Thu, 18 Nov 2021 04:15:36 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc58abb4c9cd5805540f354d6ba7931a7afec3062b7f8ff918c78378ac5d876f`  
		Last Modified: Thu, 18 Nov 2021 04:16:34 GMT  
		Size: 50.9 MB (50907794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10`

```console
$ docker pull docker@sha256:ff4fcc30e7c20f33c021e82683aedd1fe66654363eb1ff61065e0628f5bbf107
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10` - linux; amd64

```console
$ docker pull docker@sha256:0cd49922b08a5b66239fc764abe872f4799e291922e21a31d9490a10278a5a02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68479082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c655f708b2a86c4b241e80a784479ee098833dc55d9d3929e1e35e1cb0297c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:00:59 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 12 Nov 2021 22:01:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 16:02:11 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 16:02:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 16:02:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 16:02:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:19 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b81e4bf1fdc42d15e4c1cfd4aa82e5fe027cf88bd858b5be7681ef621c617`  
		Last Modified: Fri, 12 Nov 2021 22:02:42 GMT  
		Size: 1.9 MB (1937203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da79b3d4ea6e72fe17974fcd737705b6da38e9063e5bbb26cea5a9fa7465bae`  
		Last Modified: Fri, 12 Nov 2021 22:02:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9433235d3590c575f74cf6c833b63c7e5fd2c2ebf7017a086421fb465c67327`  
		Last Modified: Thu, 18 Nov 2021 16:03:22 GMT  
		Size: 63.7 MB (63717036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a370fc1bfda2f2192e17db23cd29f495b5c0b6ab9f36d73ec07a9dbdae1310`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c0972549c69874ec2e53b7534184e975853ec9602f9a7ba7466bb1a231db9`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a0159d8a68d2886d05e662c609ac1dc10a9e3b73244d73106b8888a3bddfbb`  
		Last Modified: Thu, 18 Nov 2021 16:03:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8aef5b543363230546c03371e8b3c857285ffdad566b676c3657cf64fedd9299
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62375513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0836e8a2fd6d55074387335d0a134d329cedce53561a1b6fc6eefe44cf1cf487`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:12:04 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Sat, 13 Nov 2021 11:12:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 09:17:16 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 09:17:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 09:17:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 09:17:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:25 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 09:17:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 09:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:28 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233f664f6e365c4259a38e7cfe3c14e234ab45f15847cc874a88b510f66a132f`  
		Last Modified: Sat, 13 Nov 2021 11:13:40 GMT  
		Size: 1.9 MB (1909969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c7cbdd3e377ff292e68f9ced99315b84c85398591633343352948bbc291`  
		Last Modified: Sat, 13 Nov 2021 11:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b50fed93df89351d596ab08fab482a174aa37a86d61cdeef150162665a67a80`  
		Last Modified: Thu, 18 Nov 2021 09:18:59 GMT  
		Size: 57.7 MB (57746015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21638a3c07c5ebd6977bcc9c75e0ac36c2a82b761fc51a8aee313c9a9d7ed46`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e37a1bae185ca8552a00efd7984a74bc595d0dac82ab81e945615f5a0b29af`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81c4e38c2d1b6603791a26f4dad582d554c306fb4c8c4218e0d537da3b8af6a`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind`

```console
$ docker pull docker@sha256:79d0c6e997920e71e96571ef434defcca1364d693d5b937232decf1ee7524a9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind` - linux; amd64

```console
$ docker pull docker@sha256:1ff5e500e2d42048923c1243ad26691c83c65406a33086f56e02e4fb2d43ecd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75006729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5261796049dd8a51b9e1c9ab5fa3e06960de7a813e7414dcc218022a6eb48680`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:00:59 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 12 Nov 2021 22:01:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 16:02:11 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 16:02:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 16:02:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 16:02:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:19 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 16:02:26 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 18 Nov 2021 16:02:27 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 18 Nov 2021 16:02:27 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 18 Nov 2021 16:02:28 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 18 Nov 2021 16:02:28 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:28 GMT
VOLUME [/var/lib/docker]
# Thu, 18 Nov 2021 16:02:29 GMT
EXPOSE 2375 2376
# Thu, 18 Nov 2021 16:02:29 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:29 GMT
CMD []
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b81e4bf1fdc42d15e4c1cfd4aa82e5fe027cf88bd858b5be7681ef621c617`  
		Last Modified: Fri, 12 Nov 2021 22:02:42 GMT  
		Size: 1.9 MB (1937203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da79b3d4ea6e72fe17974fcd737705b6da38e9063e5bbb26cea5a9fa7465bae`  
		Last Modified: Fri, 12 Nov 2021 22:02:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9433235d3590c575f74cf6c833b63c7e5fd2c2ebf7017a086421fb465c67327`  
		Last Modified: Thu, 18 Nov 2021 16:03:22 GMT  
		Size: 63.7 MB (63717036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a370fc1bfda2f2192e17db23cd29f495b5c0b6ab9f36d73ec07a9dbdae1310`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c0972549c69874ec2e53b7534184e975853ec9602f9a7ba7466bb1a231db9`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a0159d8a68d2886d05e662c609ac1dc10a9e3b73244d73106b8888a3bddfbb`  
		Last Modified: Thu, 18 Nov 2021 16:03:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2667e9a1d0ba047230eab7daedb7556a9d2204adebca9d7439ecaae6dbc1e3`  
		Last Modified: Thu, 18 Nov 2021 16:03:48 GMT  
		Size: 6.5 MB (6522755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f72da5423b84bdb2e04379edb8747ff161388fe38280eb242ef4d802008bf96`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b9fb6f0baf688ba32368dc395c50842182a9a4cadafd2cc0964570f740cd9a`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd10f5a3a8ed006ba472a52473be2b1f099d4b3b4cc8cdf52bae991cac915e0`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:6b91496cd8473f8f0412be846318dcf073a41e5c02fea27a75a657376c55e83b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68798719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9280bbaf2b20c01dbbcd50930cb5862adc44e531d88f54d157358d16f7de8a5f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:12:04 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Sat, 13 Nov 2021 11:12:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 09:17:16 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 09:17:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 09:17:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 09:17:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:25 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 09:17:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 09:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:28 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 09:17:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 18 Nov 2021 09:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 18 Nov 2021 09:17:40 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 18 Nov 2021 09:17:41 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 18 Nov 2021 09:17:43 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:43 GMT
VOLUME [/var/lib/docker]
# Thu, 18 Nov 2021 09:17:44 GMT
EXPOSE 2375 2376
# Thu, 18 Nov 2021 09:17:45 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:46 GMT
CMD []
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233f664f6e365c4259a38e7cfe3c14e234ab45f15847cc874a88b510f66a132f`  
		Last Modified: Sat, 13 Nov 2021 11:13:40 GMT  
		Size: 1.9 MB (1909969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c7cbdd3e377ff292e68f9ced99315b84c85398591633343352948bbc291`  
		Last Modified: Sat, 13 Nov 2021 11:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b50fed93df89351d596ab08fab482a174aa37a86d61cdeef150162665a67a80`  
		Last Modified: Thu, 18 Nov 2021 09:18:59 GMT  
		Size: 57.7 MB (57746015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21638a3c07c5ebd6977bcc9c75e0ac36c2a82b761fc51a8aee313c9a9d7ed46`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e37a1bae185ca8552a00efd7984a74bc595d0dac82ab81e945615f5a0b29af`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81c4e38c2d1b6603791a26f4dad582d554c306fb4c8c4218e0d537da3b8af6a`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc29a86f7ed1b15ec5c146abf64a41609779eb5b0e2a668d274b1b28c14c37e3`  
		Last Modified: Thu, 18 Nov 2021 09:19:20 GMT  
		Size: 6.4 MB (6418345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce285f2fd3dbcbe5e58749e817ef3a3e60fa1dbf82bc51eaff0f20f8e151d3f`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeabdc4aba67b4850e7e5c118e6409d59a161d11f5be536341a4e9f40ed017bf`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd2d42122e3f199551259bf3db06d2c446c725eb3ae3239f2692f3fa57804b5`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind-rootless`

```console
$ docker pull docker@sha256:154d9287cc128b8c4820b8d412652064cccd1466a61a50af871062b82cc05f6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:165b8b4bb284183bb67f3cb4617d84032b4d31d2a537e2bce63d016044a438c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95282418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:956ab016b037de2042fec25d130ac6a9aaa029a8183fff6512e356e2d44b205f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:00:59 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 12 Nov 2021 22:01:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 16:02:11 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 16:02:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 16:02:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 16:02:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:19 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 16:02:26 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 18 Nov 2021 16:02:27 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 18 Nov 2021 16:02:27 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 18 Nov 2021 16:02:28 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 18 Nov 2021 16:02:28 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:28 GMT
VOLUME [/var/lib/docker]
# Thu, 18 Nov 2021 16:02:29 GMT
EXPOSE 2375 2376
# Thu, 18 Nov 2021 16:02:29 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:29 GMT
CMD []
# Thu, 18 Nov 2021 16:02:33 GMT
RUN apk add --no-cache iproute2
# Thu, 18 Nov 2021 16:02:34 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 18 Nov 2021 16:02:35 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 18 Nov 2021 16:02:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 18 Nov 2021 16:02:38 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 18 Nov 2021 16:02:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 18 Nov 2021 16:02:39 GMT
USER rootless
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b81e4bf1fdc42d15e4c1cfd4aa82e5fe027cf88bd858b5be7681ef621c617`  
		Last Modified: Fri, 12 Nov 2021 22:02:42 GMT  
		Size: 1.9 MB (1937203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da79b3d4ea6e72fe17974fcd737705b6da38e9063e5bbb26cea5a9fa7465bae`  
		Last Modified: Fri, 12 Nov 2021 22:02:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9433235d3590c575f74cf6c833b63c7e5fd2c2ebf7017a086421fb465c67327`  
		Last Modified: Thu, 18 Nov 2021 16:03:22 GMT  
		Size: 63.7 MB (63717036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a370fc1bfda2f2192e17db23cd29f495b5c0b6ab9f36d73ec07a9dbdae1310`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c0972549c69874ec2e53b7534184e975853ec9602f9a7ba7466bb1a231db9`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a0159d8a68d2886d05e662c609ac1dc10a9e3b73244d73106b8888a3bddfbb`  
		Last Modified: Thu, 18 Nov 2021 16:03:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2667e9a1d0ba047230eab7daedb7556a9d2204adebca9d7439ecaae6dbc1e3`  
		Last Modified: Thu, 18 Nov 2021 16:03:48 GMT  
		Size: 6.5 MB (6522755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f72da5423b84bdb2e04379edb8747ff161388fe38280eb242ef4d802008bf96`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b9fb6f0baf688ba32368dc395c50842182a9a4cadafd2cc0964570f740cd9a`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd10f5a3a8ed006ba472a52473be2b1f099d4b3b4cc8cdf52bae991cac915e0`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e11d3f7e286c938d26bbb186acb5479276df6361d8df2dcd69411be8e3a69d7`  
		Last Modified: Thu, 18 Nov 2021 16:04:10 GMT  
		Size: 1.1 MB (1149116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f294faaf6353a52c03a2b9dcfa622a83436f037202b20fb7683021db79e775`  
		Last Modified: Thu, 18 Nov 2021 16:04:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b662b3e60558d88a695d82eff536d1ce83c74cca00618f4a905ed756ca05f241`  
		Last Modified: Thu, 18 Nov 2021 16:04:10 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45688b3cc691166b57c28f4fadfe415eb8c9bdf22e92e43a60b0c7e50071a3ac`  
		Last Modified: Thu, 18 Nov 2021 16:04:15 GMT  
		Size: 19.1 MB (19124859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1ee7128b0e98cd946608ca63e413eeb9b68f68eedd4f1d58ff71fed621291b`  
		Last Modified: Thu, 18 Nov 2021 16:04:10 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:2441b89586372dc59c8fce28fc3fa0a6141193ad158d18482597187a7e1c9eeb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91070455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c509ba52a7374da993e6cf01a7147518857077192831cf839078772fa27881b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:12:04 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Sat, 13 Nov 2021 11:12:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 09:17:16 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 09:17:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 09:17:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 09:17:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:25 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 09:17:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 09:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:28 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 09:17:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 18 Nov 2021 09:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 18 Nov 2021 09:17:40 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 18 Nov 2021 09:17:41 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 18 Nov 2021 09:17:43 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:43 GMT
VOLUME [/var/lib/docker]
# Thu, 18 Nov 2021 09:17:44 GMT
EXPOSE 2375 2376
# Thu, 18 Nov 2021 09:17:45 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:46 GMT
CMD []
# Thu, 18 Nov 2021 09:17:54 GMT
RUN apk add --no-cache iproute2
# Thu, 18 Nov 2021 09:17:55 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 18 Nov 2021 09:17:56 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 18 Nov 2021 09:17:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 18 Nov 2021 09:18:00 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 18 Nov 2021 09:18:01 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 18 Nov 2021 09:18:02 GMT
USER rootless
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233f664f6e365c4259a38e7cfe3c14e234ab45f15847cc874a88b510f66a132f`  
		Last Modified: Sat, 13 Nov 2021 11:13:40 GMT  
		Size: 1.9 MB (1909969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c7cbdd3e377ff292e68f9ced99315b84c85398591633343352948bbc291`  
		Last Modified: Sat, 13 Nov 2021 11:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b50fed93df89351d596ab08fab482a174aa37a86d61cdeef150162665a67a80`  
		Last Modified: Thu, 18 Nov 2021 09:18:59 GMT  
		Size: 57.7 MB (57746015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21638a3c07c5ebd6977bcc9c75e0ac36c2a82b761fc51a8aee313c9a9d7ed46`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e37a1bae185ca8552a00efd7984a74bc595d0dac82ab81e945615f5a0b29af`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81c4e38c2d1b6603791a26f4dad582d554c306fb4c8c4218e0d537da3b8af6a`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc29a86f7ed1b15ec5c146abf64a41609779eb5b0e2a668d274b1b28c14c37e3`  
		Last Modified: Thu, 18 Nov 2021 09:19:20 GMT  
		Size: 6.4 MB (6418345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce285f2fd3dbcbe5e58749e817ef3a3e60fa1dbf82bc51eaff0f20f8e151d3f`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeabdc4aba67b4850e7e5c118e6409d59a161d11f5be536341a4e9f40ed017bf`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd2d42122e3f199551259bf3db06d2c446c725eb3ae3239f2692f3fa57804b5`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230963f6db0e75d3a58bc46d5b33ea4f67e6b1f0300e99ba12497c89f68ce855`  
		Last Modified: Thu, 18 Nov 2021 09:19:41 GMT  
		Size: 1.2 MB (1168585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66cc595973e50f8d3e25c628464cfa45436824aab478bda61c9ac4232d822c3`  
		Last Modified: Thu, 18 Nov 2021 09:19:40 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55af54131c4a2bf83efebe4e4fec2d50bd4c99ffbca5aa5ccfa29c167f4c16ce`  
		Last Modified: Thu, 18 Nov 2021 09:19:40 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cab39e5c6b0a896c570c0218f29e0600936018957c487e7b439c9ecf14ad8e`  
		Last Modified: Thu, 18 Nov 2021 09:19:44 GMT  
		Size: 21.1 MB (21101528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365691e2dffd5c75fa3b86bd4ccd1b11a4beae986f511ce5400a6a3d69b550c`  
		Last Modified: Thu, 18 Nov 2021 09:19:40 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-git`

```console
$ docker pull docker@sha256:50fdfef2982984d5f587a8274e932da365b322388804a9f1b30ef5eac2524527
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-git` - linux; amd64

```console
$ docker pull docker@sha256:dd201d3335196a559cdc166592a7acfbe9545e25aa83baa8c7e90fbee9353172
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75109809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26ae7c6d74e81d7ec18428ac5cdf0879073d8e746c341bf389aad8593a235e83`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:00:59 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 12 Nov 2021 22:01:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 16:02:11 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 16:02:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 16:02:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 16:02:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:19 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 16:02:43 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b81e4bf1fdc42d15e4c1cfd4aa82e5fe027cf88bd858b5be7681ef621c617`  
		Last Modified: Fri, 12 Nov 2021 22:02:42 GMT  
		Size: 1.9 MB (1937203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da79b3d4ea6e72fe17974fcd737705b6da38e9063e5bbb26cea5a9fa7465bae`  
		Last Modified: Fri, 12 Nov 2021 22:02:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9433235d3590c575f74cf6c833b63c7e5fd2c2ebf7017a086421fb465c67327`  
		Last Modified: Thu, 18 Nov 2021 16:03:22 GMT  
		Size: 63.7 MB (63717036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a370fc1bfda2f2192e17db23cd29f495b5c0b6ab9f36d73ec07a9dbdae1310`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c0972549c69874ec2e53b7534184e975853ec9602f9a7ba7466bb1a231db9`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a0159d8a68d2886d05e662c609ac1dc10a9e3b73244d73106b8888a3bddfbb`  
		Last Modified: Thu, 18 Nov 2021 16:03:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f4768f31acf9871e50a178b839a569a05c1b6a8923f4644db556da09776dbb`  
		Last Modified: Thu, 18 Nov 2021 16:04:34 GMT  
		Size: 6.6 MB (6630727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:abd4f25a749ebaac21635348b5e8db17d1d7cc5bcfa3b437e730b4178177cd2f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69115687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eb4264b475ad1b401f8776fd4d94293173ddd396cf1a88a5fb4372947b3ef3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:12:04 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Sat, 13 Nov 2021 11:12:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 09:17:16 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 09:17:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 09:17:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 09:17:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:25 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 09:17:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 09:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:28 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 09:18:09 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233f664f6e365c4259a38e7cfe3c14e234ab45f15847cc874a88b510f66a132f`  
		Last Modified: Sat, 13 Nov 2021 11:13:40 GMT  
		Size: 1.9 MB (1909969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c7cbdd3e377ff292e68f9ced99315b84c85398591633343352948bbc291`  
		Last Modified: Sat, 13 Nov 2021 11:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b50fed93df89351d596ab08fab482a174aa37a86d61cdeef150162665a67a80`  
		Last Modified: Thu, 18 Nov 2021 09:18:59 GMT  
		Size: 57.7 MB (57746015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21638a3c07c5ebd6977bcc9c75e0ac36c2a82b761fc51a8aee313c9a9d7ed46`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e37a1bae185ca8552a00efd7984a74bc595d0dac82ab81e945615f5a0b29af`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81c4e38c2d1b6603791a26f4dad582d554c306fb4c8c4218e0d537da3b8af6a`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d06f8877e01ae57a21f32e8cdd5b66ffc3fdf70cfb5c8036a429db1ed15e12`  
		Last Modified: Thu, 18 Nov 2021 09:20:04 GMT  
		Size: 6.7 MB (6740174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore`

```console
$ docker pull docker@sha256:280e2bfd85a1840bc5220777f9d70a85a6bf7fb35a3d8a03275043b5bdd07fb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `docker:20.10-windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull docker@sha256:f9935026e3d4f01f6ffe7c97d63ee7f286c77f52f80e2f1be8afe7de69ba531c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2757389706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feec87f6f82e9966337409c1601a519ee1ddc39fb68c10dbfbbb4cc6328de03d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 19:07:02 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 18 Nov 2021 04:13:52 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 04:13:53 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.11.zip
# Thu, 18 Nov 2021 04:15:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e42405e6d7d9caeb7c5a114493eca7f34351fae0fc2b77118957003b2f6c5f`  
		Last Modified: Wed, 10 Nov 2021 19:08:27 GMT  
		Size: 356.8 KB (356764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568ddc925a63c78da177f9676136448290dfbb54e31f140f98a3d4e0f3cfdc6d`  
		Last Modified: Thu, 18 Nov 2021 04:15:36 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a4753c3e1103c5a6292410a73e0d9eeeaa777557870a6d95dae8c80d822305`  
		Last Modified: Thu, 18 Nov 2021 04:15:36 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc58abb4c9cd5805540f354d6ba7931a7afec3062b7f8ff918c78378ac5d876f`  
		Last Modified: Thu, 18 Nov 2021 04:16:34 GMT  
		Size: 50.9 MB (50907794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-1809`

```console
$ docker pull docker@sha256:280e2bfd85a1840bc5220777f9d70a85a6bf7fb35a3d8a03275043b5bdd07fb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `docker:20.10-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull docker@sha256:f9935026e3d4f01f6ffe7c97d63ee7f286c77f52f80e2f1be8afe7de69ba531c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2757389706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feec87f6f82e9966337409c1601a519ee1ddc39fb68c10dbfbbb4cc6328de03d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 19:07:02 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 18 Nov 2021 04:13:52 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 04:13:53 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.11.zip
# Thu, 18 Nov 2021 04:15:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e42405e6d7d9caeb7c5a114493eca7f34351fae0fc2b77118957003b2f6c5f`  
		Last Modified: Wed, 10 Nov 2021 19:08:27 GMT  
		Size: 356.8 KB (356764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568ddc925a63c78da177f9676136448290dfbb54e31f140f98a3d4e0f3cfdc6d`  
		Last Modified: Thu, 18 Nov 2021 04:15:36 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a4753c3e1103c5a6292410a73e0d9eeeaa777557870a6d95dae8c80d822305`  
		Last Modified: Thu, 18 Nov 2021 04:15:36 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc58abb4c9cd5805540f354d6ba7931a7afec3062b7f8ff918c78378ac5d876f`  
		Last Modified: Thu, 18 Nov 2021 04:16:34 GMT  
		Size: 50.9 MB (50907794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.11`

```console
$ docker pull docker@sha256:ff4fcc30e7c20f33c021e82683aedd1fe66654363eb1ff61065e0628f5bbf107
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.11` - linux; amd64

```console
$ docker pull docker@sha256:0cd49922b08a5b66239fc764abe872f4799e291922e21a31d9490a10278a5a02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68479082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c655f708b2a86c4b241e80a784479ee098833dc55d9d3929e1e35e1cb0297c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:00:59 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 12 Nov 2021 22:01:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 16:02:11 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 16:02:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 16:02:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 16:02:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:19 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b81e4bf1fdc42d15e4c1cfd4aa82e5fe027cf88bd858b5be7681ef621c617`  
		Last Modified: Fri, 12 Nov 2021 22:02:42 GMT  
		Size: 1.9 MB (1937203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da79b3d4ea6e72fe17974fcd737705b6da38e9063e5bbb26cea5a9fa7465bae`  
		Last Modified: Fri, 12 Nov 2021 22:02:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9433235d3590c575f74cf6c833b63c7e5fd2c2ebf7017a086421fb465c67327`  
		Last Modified: Thu, 18 Nov 2021 16:03:22 GMT  
		Size: 63.7 MB (63717036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a370fc1bfda2f2192e17db23cd29f495b5c0b6ab9f36d73ec07a9dbdae1310`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c0972549c69874ec2e53b7534184e975853ec9602f9a7ba7466bb1a231db9`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a0159d8a68d2886d05e662c609ac1dc10a9e3b73244d73106b8888a3bddfbb`  
		Last Modified: Thu, 18 Nov 2021 16:03:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.11` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8aef5b543363230546c03371e8b3c857285ffdad566b676c3657cf64fedd9299
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62375513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0836e8a2fd6d55074387335d0a134d329cedce53561a1b6fc6eefe44cf1cf487`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:12:04 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Sat, 13 Nov 2021 11:12:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 09:17:16 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 09:17:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 09:17:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 09:17:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:25 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 09:17:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 09:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:28 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233f664f6e365c4259a38e7cfe3c14e234ab45f15847cc874a88b510f66a132f`  
		Last Modified: Sat, 13 Nov 2021 11:13:40 GMT  
		Size: 1.9 MB (1909969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c7cbdd3e377ff292e68f9ced99315b84c85398591633343352948bbc291`  
		Last Modified: Sat, 13 Nov 2021 11:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b50fed93df89351d596ab08fab482a174aa37a86d61cdeef150162665a67a80`  
		Last Modified: Thu, 18 Nov 2021 09:18:59 GMT  
		Size: 57.7 MB (57746015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21638a3c07c5ebd6977bcc9c75e0ac36c2a82b761fc51a8aee313c9a9d7ed46`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e37a1bae185ca8552a00efd7984a74bc595d0dac82ab81e945615f5a0b29af`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81c4e38c2d1b6603791a26f4dad582d554c306fb4c8c4218e0d537da3b8af6a`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.11-alpine3.14`

```console
$ docker pull docker@sha256:ff4fcc30e7c20f33c021e82683aedd1fe66654363eb1ff61065e0628f5bbf107
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.11-alpine3.14` - linux; amd64

```console
$ docker pull docker@sha256:0cd49922b08a5b66239fc764abe872f4799e291922e21a31d9490a10278a5a02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68479082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c655f708b2a86c4b241e80a784479ee098833dc55d9d3929e1e35e1cb0297c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:00:59 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 12 Nov 2021 22:01:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 16:02:11 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 16:02:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 16:02:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 16:02:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:19 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b81e4bf1fdc42d15e4c1cfd4aa82e5fe027cf88bd858b5be7681ef621c617`  
		Last Modified: Fri, 12 Nov 2021 22:02:42 GMT  
		Size: 1.9 MB (1937203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da79b3d4ea6e72fe17974fcd737705b6da38e9063e5bbb26cea5a9fa7465bae`  
		Last Modified: Fri, 12 Nov 2021 22:02:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9433235d3590c575f74cf6c833b63c7e5fd2c2ebf7017a086421fb465c67327`  
		Last Modified: Thu, 18 Nov 2021 16:03:22 GMT  
		Size: 63.7 MB (63717036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a370fc1bfda2f2192e17db23cd29f495b5c0b6ab9f36d73ec07a9dbdae1310`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c0972549c69874ec2e53b7534184e975853ec9602f9a7ba7466bb1a231db9`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a0159d8a68d2886d05e662c609ac1dc10a9e3b73244d73106b8888a3bddfbb`  
		Last Modified: Thu, 18 Nov 2021 16:03:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.11-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8aef5b543363230546c03371e8b3c857285ffdad566b676c3657cf64fedd9299
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62375513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0836e8a2fd6d55074387335d0a134d329cedce53561a1b6fc6eefe44cf1cf487`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:12:04 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Sat, 13 Nov 2021 11:12:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 09:17:16 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 09:17:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 09:17:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 09:17:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:25 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 09:17:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 09:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:28 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233f664f6e365c4259a38e7cfe3c14e234ab45f15847cc874a88b510f66a132f`  
		Last Modified: Sat, 13 Nov 2021 11:13:40 GMT  
		Size: 1.9 MB (1909969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c7cbdd3e377ff292e68f9ced99315b84c85398591633343352948bbc291`  
		Last Modified: Sat, 13 Nov 2021 11:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b50fed93df89351d596ab08fab482a174aa37a86d61cdeef150162665a67a80`  
		Last Modified: Thu, 18 Nov 2021 09:18:59 GMT  
		Size: 57.7 MB (57746015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21638a3c07c5ebd6977bcc9c75e0ac36c2a82b761fc51a8aee313c9a9d7ed46`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e37a1bae185ca8552a00efd7984a74bc595d0dac82ab81e945615f5a0b29af`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81c4e38c2d1b6603791a26f4dad582d554c306fb4c8c4218e0d537da3b8af6a`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.11-dind`

```console
$ docker pull docker@sha256:79d0c6e997920e71e96571ef434defcca1364d693d5b937232decf1ee7524a9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.11-dind` - linux; amd64

```console
$ docker pull docker@sha256:1ff5e500e2d42048923c1243ad26691c83c65406a33086f56e02e4fb2d43ecd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75006729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5261796049dd8a51b9e1c9ab5fa3e06960de7a813e7414dcc218022a6eb48680`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:00:59 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 12 Nov 2021 22:01:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 16:02:11 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 16:02:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 16:02:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 16:02:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:19 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 16:02:26 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 18 Nov 2021 16:02:27 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 18 Nov 2021 16:02:27 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 18 Nov 2021 16:02:28 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 18 Nov 2021 16:02:28 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:28 GMT
VOLUME [/var/lib/docker]
# Thu, 18 Nov 2021 16:02:29 GMT
EXPOSE 2375 2376
# Thu, 18 Nov 2021 16:02:29 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:29 GMT
CMD []
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b81e4bf1fdc42d15e4c1cfd4aa82e5fe027cf88bd858b5be7681ef621c617`  
		Last Modified: Fri, 12 Nov 2021 22:02:42 GMT  
		Size: 1.9 MB (1937203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da79b3d4ea6e72fe17974fcd737705b6da38e9063e5bbb26cea5a9fa7465bae`  
		Last Modified: Fri, 12 Nov 2021 22:02:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9433235d3590c575f74cf6c833b63c7e5fd2c2ebf7017a086421fb465c67327`  
		Last Modified: Thu, 18 Nov 2021 16:03:22 GMT  
		Size: 63.7 MB (63717036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a370fc1bfda2f2192e17db23cd29f495b5c0b6ab9f36d73ec07a9dbdae1310`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c0972549c69874ec2e53b7534184e975853ec9602f9a7ba7466bb1a231db9`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a0159d8a68d2886d05e662c609ac1dc10a9e3b73244d73106b8888a3bddfbb`  
		Last Modified: Thu, 18 Nov 2021 16:03:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2667e9a1d0ba047230eab7daedb7556a9d2204adebca9d7439ecaae6dbc1e3`  
		Last Modified: Thu, 18 Nov 2021 16:03:48 GMT  
		Size: 6.5 MB (6522755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f72da5423b84bdb2e04379edb8747ff161388fe38280eb242ef4d802008bf96`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b9fb6f0baf688ba32368dc395c50842182a9a4cadafd2cc0964570f740cd9a`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd10f5a3a8ed006ba472a52473be2b1f099d4b3b4cc8cdf52bae991cac915e0`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.11-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:6b91496cd8473f8f0412be846318dcf073a41e5c02fea27a75a657376c55e83b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68798719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9280bbaf2b20c01dbbcd50930cb5862adc44e531d88f54d157358d16f7de8a5f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:12:04 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Sat, 13 Nov 2021 11:12:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 09:17:16 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 09:17:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 09:17:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 09:17:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:25 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 09:17:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 09:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:28 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 09:17:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 18 Nov 2021 09:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 18 Nov 2021 09:17:40 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 18 Nov 2021 09:17:41 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 18 Nov 2021 09:17:43 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:43 GMT
VOLUME [/var/lib/docker]
# Thu, 18 Nov 2021 09:17:44 GMT
EXPOSE 2375 2376
# Thu, 18 Nov 2021 09:17:45 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:46 GMT
CMD []
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233f664f6e365c4259a38e7cfe3c14e234ab45f15847cc874a88b510f66a132f`  
		Last Modified: Sat, 13 Nov 2021 11:13:40 GMT  
		Size: 1.9 MB (1909969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c7cbdd3e377ff292e68f9ced99315b84c85398591633343352948bbc291`  
		Last Modified: Sat, 13 Nov 2021 11:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b50fed93df89351d596ab08fab482a174aa37a86d61cdeef150162665a67a80`  
		Last Modified: Thu, 18 Nov 2021 09:18:59 GMT  
		Size: 57.7 MB (57746015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21638a3c07c5ebd6977bcc9c75e0ac36c2a82b761fc51a8aee313c9a9d7ed46`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e37a1bae185ca8552a00efd7984a74bc595d0dac82ab81e945615f5a0b29af`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81c4e38c2d1b6603791a26f4dad582d554c306fb4c8c4218e0d537da3b8af6a`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc29a86f7ed1b15ec5c146abf64a41609779eb5b0e2a668d274b1b28c14c37e3`  
		Last Modified: Thu, 18 Nov 2021 09:19:20 GMT  
		Size: 6.4 MB (6418345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce285f2fd3dbcbe5e58749e817ef3a3e60fa1dbf82bc51eaff0f20f8e151d3f`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeabdc4aba67b4850e7e5c118e6409d59a161d11f5be536341a4e9f40ed017bf`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd2d42122e3f199551259bf3db06d2c446c725eb3ae3239f2692f3fa57804b5`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.11-dind-alpine3.14`

```console
$ docker pull docker@sha256:79d0c6e997920e71e96571ef434defcca1364d693d5b937232decf1ee7524a9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.11-dind-alpine3.14` - linux; amd64

```console
$ docker pull docker@sha256:1ff5e500e2d42048923c1243ad26691c83c65406a33086f56e02e4fb2d43ecd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75006729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5261796049dd8a51b9e1c9ab5fa3e06960de7a813e7414dcc218022a6eb48680`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:00:59 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 12 Nov 2021 22:01:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 16:02:11 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 16:02:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 16:02:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 16:02:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:19 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 16:02:26 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 18 Nov 2021 16:02:27 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 18 Nov 2021 16:02:27 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 18 Nov 2021 16:02:28 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 18 Nov 2021 16:02:28 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:28 GMT
VOLUME [/var/lib/docker]
# Thu, 18 Nov 2021 16:02:29 GMT
EXPOSE 2375 2376
# Thu, 18 Nov 2021 16:02:29 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:29 GMT
CMD []
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b81e4bf1fdc42d15e4c1cfd4aa82e5fe027cf88bd858b5be7681ef621c617`  
		Last Modified: Fri, 12 Nov 2021 22:02:42 GMT  
		Size: 1.9 MB (1937203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da79b3d4ea6e72fe17974fcd737705b6da38e9063e5bbb26cea5a9fa7465bae`  
		Last Modified: Fri, 12 Nov 2021 22:02:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9433235d3590c575f74cf6c833b63c7e5fd2c2ebf7017a086421fb465c67327`  
		Last Modified: Thu, 18 Nov 2021 16:03:22 GMT  
		Size: 63.7 MB (63717036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a370fc1bfda2f2192e17db23cd29f495b5c0b6ab9f36d73ec07a9dbdae1310`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c0972549c69874ec2e53b7534184e975853ec9602f9a7ba7466bb1a231db9`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a0159d8a68d2886d05e662c609ac1dc10a9e3b73244d73106b8888a3bddfbb`  
		Last Modified: Thu, 18 Nov 2021 16:03:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2667e9a1d0ba047230eab7daedb7556a9d2204adebca9d7439ecaae6dbc1e3`  
		Last Modified: Thu, 18 Nov 2021 16:03:48 GMT  
		Size: 6.5 MB (6522755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f72da5423b84bdb2e04379edb8747ff161388fe38280eb242ef4d802008bf96`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b9fb6f0baf688ba32368dc395c50842182a9a4cadafd2cc0964570f740cd9a`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd10f5a3a8ed006ba472a52473be2b1f099d4b3b4cc8cdf52bae991cac915e0`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.11-dind-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:6b91496cd8473f8f0412be846318dcf073a41e5c02fea27a75a657376c55e83b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68798719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9280bbaf2b20c01dbbcd50930cb5862adc44e531d88f54d157358d16f7de8a5f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:12:04 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Sat, 13 Nov 2021 11:12:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 09:17:16 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 09:17:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 09:17:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 09:17:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:25 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 09:17:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 09:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:28 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 09:17:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 18 Nov 2021 09:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 18 Nov 2021 09:17:40 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 18 Nov 2021 09:17:41 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 18 Nov 2021 09:17:43 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:43 GMT
VOLUME [/var/lib/docker]
# Thu, 18 Nov 2021 09:17:44 GMT
EXPOSE 2375 2376
# Thu, 18 Nov 2021 09:17:45 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:46 GMT
CMD []
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233f664f6e365c4259a38e7cfe3c14e234ab45f15847cc874a88b510f66a132f`  
		Last Modified: Sat, 13 Nov 2021 11:13:40 GMT  
		Size: 1.9 MB (1909969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c7cbdd3e377ff292e68f9ced99315b84c85398591633343352948bbc291`  
		Last Modified: Sat, 13 Nov 2021 11:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b50fed93df89351d596ab08fab482a174aa37a86d61cdeef150162665a67a80`  
		Last Modified: Thu, 18 Nov 2021 09:18:59 GMT  
		Size: 57.7 MB (57746015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21638a3c07c5ebd6977bcc9c75e0ac36c2a82b761fc51a8aee313c9a9d7ed46`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e37a1bae185ca8552a00efd7984a74bc595d0dac82ab81e945615f5a0b29af`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81c4e38c2d1b6603791a26f4dad582d554c306fb4c8c4218e0d537da3b8af6a`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc29a86f7ed1b15ec5c146abf64a41609779eb5b0e2a668d274b1b28c14c37e3`  
		Last Modified: Thu, 18 Nov 2021 09:19:20 GMT  
		Size: 6.4 MB (6418345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce285f2fd3dbcbe5e58749e817ef3a3e60fa1dbf82bc51eaff0f20f8e151d3f`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeabdc4aba67b4850e7e5c118e6409d59a161d11f5be536341a4e9f40ed017bf`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd2d42122e3f199551259bf3db06d2c446c725eb3ae3239f2692f3fa57804b5`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.11-dind-rootless`

```console
$ docker pull docker@sha256:154d9287cc128b8c4820b8d412652064cccd1466a61a50af871062b82cc05f6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.11-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:165b8b4bb284183bb67f3cb4617d84032b4d31d2a537e2bce63d016044a438c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95282418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:956ab016b037de2042fec25d130ac6a9aaa029a8183fff6512e356e2d44b205f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:00:59 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 12 Nov 2021 22:01:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 16:02:11 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 16:02:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 16:02:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 16:02:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:19 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 16:02:26 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 18 Nov 2021 16:02:27 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 18 Nov 2021 16:02:27 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 18 Nov 2021 16:02:28 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 18 Nov 2021 16:02:28 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:28 GMT
VOLUME [/var/lib/docker]
# Thu, 18 Nov 2021 16:02:29 GMT
EXPOSE 2375 2376
# Thu, 18 Nov 2021 16:02:29 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:29 GMT
CMD []
# Thu, 18 Nov 2021 16:02:33 GMT
RUN apk add --no-cache iproute2
# Thu, 18 Nov 2021 16:02:34 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 18 Nov 2021 16:02:35 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 18 Nov 2021 16:02:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 18 Nov 2021 16:02:38 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 18 Nov 2021 16:02:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 18 Nov 2021 16:02:39 GMT
USER rootless
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b81e4bf1fdc42d15e4c1cfd4aa82e5fe027cf88bd858b5be7681ef621c617`  
		Last Modified: Fri, 12 Nov 2021 22:02:42 GMT  
		Size: 1.9 MB (1937203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da79b3d4ea6e72fe17974fcd737705b6da38e9063e5bbb26cea5a9fa7465bae`  
		Last Modified: Fri, 12 Nov 2021 22:02:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9433235d3590c575f74cf6c833b63c7e5fd2c2ebf7017a086421fb465c67327`  
		Last Modified: Thu, 18 Nov 2021 16:03:22 GMT  
		Size: 63.7 MB (63717036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a370fc1bfda2f2192e17db23cd29f495b5c0b6ab9f36d73ec07a9dbdae1310`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c0972549c69874ec2e53b7534184e975853ec9602f9a7ba7466bb1a231db9`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a0159d8a68d2886d05e662c609ac1dc10a9e3b73244d73106b8888a3bddfbb`  
		Last Modified: Thu, 18 Nov 2021 16:03:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2667e9a1d0ba047230eab7daedb7556a9d2204adebca9d7439ecaae6dbc1e3`  
		Last Modified: Thu, 18 Nov 2021 16:03:48 GMT  
		Size: 6.5 MB (6522755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f72da5423b84bdb2e04379edb8747ff161388fe38280eb242ef4d802008bf96`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b9fb6f0baf688ba32368dc395c50842182a9a4cadafd2cc0964570f740cd9a`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd10f5a3a8ed006ba472a52473be2b1f099d4b3b4cc8cdf52bae991cac915e0`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e11d3f7e286c938d26bbb186acb5479276df6361d8df2dcd69411be8e3a69d7`  
		Last Modified: Thu, 18 Nov 2021 16:04:10 GMT  
		Size: 1.1 MB (1149116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f294faaf6353a52c03a2b9dcfa622a83436f037202b20fb7683021db79e775`  
		Last Modified: Thu, 18 Nov 2021 16:04:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b662b3e60558d88a695d82eff536d1ce83c74cca00618f4a905ed756ca05f241`  
		Last Modified: Thu, 18 Nov 2021 16:04:10 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45688b3cc691166b57c28f4fadfe415eb8c9bdf22e92e43a60b0c7e50071a3ac`  
		Last Modified: Thu, 18 Nov 2021 16:04:15 GMT  
		Size: 19.1 MB (19124859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1ee7128b0e98cd946608ca63e413eeb9b68f68eedd4f1d58ff71fed621291b`  
		Last Modified: Thu, 18 Nov 2021 16:04:10 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.11-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:2441b89586372dc59c8fce28fc3fa0a6141193ad158d18482597187a7e1c9eeb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91070455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c509ba52a7374da993e6cf01a7147518857077192831cf839078772fa27881b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:12:04 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Sat, 13 Nov 2021 11:12:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 09:17:16 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 09:17:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 09:17:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 09:17:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:25 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 09:17:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 09:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:28 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 09:17:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 18 Nov 2021 09:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 18 Nov 2021 09:17:40 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 18 Nov 2021 09:17:41 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 18 Nov 2021 09:17:43 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:43 GMT
VOLUME [/var/lib/docker]
# Thu, 18 Nov 2021 09:17:44 GMT
EXPOSE 2375 2376
# Thu, 18 Nov 2021 09:17:45 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:46 GMT
CMD []
# Thu, 18 Nov 2021 09:17:54 GMT
RUN apk add --no-cache iproute2
# Thu, 18 Nov 2021 09:17:55 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 18 Nov 2021 09:17:56 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 18 Nov 2021 09:17:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 18 Nov 2021 09:18:00 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 18 Nov 2021 09:18:01 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 18 Nov 2021 09:18:02 GMT
USER rootless
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233f664f6e365c4259a38e7cfe3c14e234ab45f15847cc874a88b510f66a132f`  
		Last Modified: Sat, 13 Nov 2021 11:13:40 GMT  
		Size: 1.9 MB (1909969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c7cbdd3e377ff292e68f9ced99315b84c85398591633343352948bbc291`  
		Last Modified: Sat, 13 Nov 2021 11:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b50fed93df89351d596ab08fab482a174aa37a86d61cdeef150162665a67a80`  
		Last Modified: Thu, 18 Nov 2021 09:18:59 GMT  
		Size: 57.7 MB (57746015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21638a3c07c5ebd6977bcc9c75e0ac36c2a82b761fc51a8aee313c9a9d7ed46`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e37a1bae185ca8552a00efd7984a74bc595d0dac82ab81e945615f5a0b29af`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81c4e38c2d1b6603791a26f4dad582d554c306fb4c8c4218e0d537da3b8af6a`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc29a86f7ed1b15ec5c146abf64a41609779eb5b0e2a668d274b1b28c14c37e3`  
		Last Modified: Thu, 18 Nov 2021 09:19:20 GMT  
		Size: 6.4 MB (6418345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce285f2fd3dbcbe5e58749e817ef3a3e60fa1dbf82bc51eaff0f20f8e151d3f`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeabdc4aba67b4850e7e5c118e6409d59a161d11f5be536341a4e9f40ed017bf`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd2d42122e3f199551259bf3db06d2c446c725eb3ae3239f2692f3fa57804b5`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230963f6db0e75d3a58bc46d5b33ea4f67e6b1f0300e99ba12497c89f68ce855`  
		Last Modified: Thu, 18 Nov 2021 09:19:41 GMT  
		Size: 1.2 MB (1168585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66cc595973e50f8d3e25c628464cfa45436824aab478bda61c9ac4232d822c3`  
		Last Modified: Thu, 18 Nov 2021 09:19:40 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55af54131c4a2bf83efebe4e4fec2d50bd4c99ffbca5aa5ccfa29c167f4c16ce`  
		Last Modified: Thu, 18 Nov 2021 09:19:40 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cab39e5c6b0a896c570c0218f29e0600936018957c487e7b439c9ecf14ad8e`  
		Last Modified: Thu, 18 Nov 2021 09:19:44 GMT  
		Size: 21.1 MB (21101528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365691e2dffd5c75fa3b86bd4ccd1b11a4beae986f511ce5400a6a3d69b550c`  
		Last Modified: Thu, 18 Nov 2021 09:19:40 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.11-git`

```console
$ docker pull docker@sha256:50fdfef2982984d5f587a8274e932da365b322388804a9f1b30ef5eac2524527
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.11-git` - linux; amd64

```console
$ docker pull docker@sha256:dd201d3335196a559cdc166592a7acfbe9545e25aa83baa8c7e90fbee9353172
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75109809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26ae7c6d74e81d7ec18428ac5cdf0879073d8e746c341bf389aad8593a235e83`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:00:59 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 12 Nov 2021 22:01:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 16:02:11 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 16:02:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 16:02:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 16:02:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:19 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 16:02:43 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b81e4bf1fdc42d15e4c1cfd4aa82e5fe027cf88bd858b5be7681ef621c617`  
		Last Modified: Fri, 12 Nov 2021 22:02:42 GMT  
		Size: 1.9 MB (1937203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da79b3d4ea6e72fe17974fcd737705b6da38e9063e5bbb26cea5a9fa7465bae`  
		Last Modified: Fri, 12 Nov 2021 22:02:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9433235d3590c575f74cf6c833b63c7e5fd2c2ebf7017a086421fb465c67327`  
		Last Modified: Thu, 18 Nov 2021 16:03:22 GMT  
		Size: 63.7 MB (63717036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a370fc1bfda2f2192e17db23cd29f495b5c0b6ab9f36d73ec07a9dbdae1310`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c0972549c69874ec2e53b7534184e975853ec9602f9a7ba7466bb1a231db9`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a0159d8a68d2886d05e662c609ac1dc10a9e3b73244d73106b8888a3bddfbb`  
		Last Modified: Thu, 18 Nov 2021 16:03:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f4768f31acf9871e50a178b839a569a05c1b6a8923f4644db556da09776dbb`  
		Last Modified: Thu, 18 Nov 2021 16:04:34 GMT  
		Size: 6.6 MB (6630727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.11-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:abd4f25a749ebaac21635348b5e8db17d1d7cc5bcfa3b437e730b4178177cd2f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69115687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eb4264b475ad1b401f8776fd4d94293173ddd396cf1a88a5fb4372947b3ef3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:12:04 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Sat, 13 Nov 2021 11:12:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 09:17:16 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 09:17:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 09:17:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 09:17:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:25 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 09:17:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 09:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:28 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 09:18:09 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233f664f6e365c4259a38e7cfe3c14e234ab45f15847cc874a88b510f66a132f`  
		Last Modified: Sat, 13 Nov 2021 11:13:40 GMT  
		Size: 1.9 MB (1909969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c7cbdd3e377ff292e68f9ced99315b84c85398591633343352948bbc291`  
		Last Modified: Sat, 13 Nov 2021 11:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b50fed93df89351d596ab08fab482a174aa37a86d61cdeef150162665a67a80`  
		Last Modified: Thu, 18 Nov 2021 09:18:59 GMT  
		Size: 57.7 MB (57746015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21638a3c07c5ebd6977bcc9c75e0ac36c2a82b761fc51a8aee313c9a9d7ed46`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e37a1bae185ca8552a00efd7984a74bc595d0dac82ab81e945615f5a0b29af`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81c4e38c2d1b6603791a26f4dad582d554c306fb4c8c4218e0d537da3b8af6a`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d06f8877e01ae57a21f32e8cdd5b66ffc3fdf70cfb5c8036a429db1ed15e12`  
		Last Modified: Thu, 18 Nov 2021 09:20:04 GMT  
		Size: 6.7 MB (6740174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.11-windowsservercore`

```console
$ docker pull docker@sha256:280e2bfd85a1840bc5220777f9d70a85a6bf7fb35a3d8a03275043b5bdd07fb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `docker:20.10.11-windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull docker@sha256:f9935026e3d4f01f6ffe7c97d63ee7f286c77f52f80e2f1be8afe7de69ba531c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2757389706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feec87f6f82e9966337409c1601a519ee1ddc39fb68c10dbfbbb4cc6328de03d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 19:07:02 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 18 Nov 2021 04:13:52 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 04:13:53 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.11.zip
# Thu, 18 Nov 2021 04:15:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e42405e6d7d9caeb7c5a114493eca7f34351fae0fc2b77118957003b2f6c5f`  
		Last Modified: Wed, 10 Nov 2021 19:08:27 GMT  
		Size: 356.8 KB (356764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568ddc925a63c78da177f9676136448290dfbb54e31f140f98a3d4e0f3cfdc6d`  
		Last Modified: Thu, 18 Nov 2021 04:15:36 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a4753c3e1103c5a6292410a73e0d9eeeaa777557870a6d95dae8c80d822305`  
		Last Modified: Thu, 18 Nov 2021 04:15:36 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc58abb4c9cd5805540f354d6ba7931a7afec3062b7f8ff918c78378ac5d876f`  
		Last Modified: Thu, 18 Nov 2021 04:16:34 GMT  
		Size: 50.9 MB (50907794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.11-windowsservercore-1809`

```console
$ docker pull docker@sha256:280e2bfd85a1840bc5220777f9d70a85a6bf7fb35a3d8a03275043b5bdd07fb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `docker:20.10.11-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull docker@sha256:f9935026e3d4f01f6ffe7c97d63ee7f286c77f52f80e2f1be8afe7de69ba531c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2757389706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feec87f6f82e9966337409c1601a519ee1ddc39fb68c10dbfbbb4cc6328de03d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 19:07:02 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 18 Nov 2021 04:13:52 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 04:13:53 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.11.zip
# Thu, 18 Nov 2021 04:15:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e42405e6d7d9caeb7c5a114493eca7f34351fae0fc2b77118957003b2f6c5f`  
		Last Modified: Wed, 10 Nov 2021 19:08:27 GMT  
		Size: 356.8 KB (356764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568ddc925a63c78da177f9676136448290dfbb54e31f140f98a3d4e0f3cfdc6d`  
		Last Modified: Thu, 18 Nov 2021 04:15:36 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a4753c3e1103c5a6292410a73e0d9eeeaa777557870a6d95dae8c80d822305`  
		Last Modified: Thu, 18 Nov 2021 04:15:36 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc58abb4c9cd5805540f354d6ba7931a7afec3062b7f8ff918c78378ac5d876f`  
		Last Modified: Thu, 18 Nov 2021 04:16:34 GMT  
		Size: 50.9 MB (50907794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:79d0c6e997920e71e96571ef434defcca1364d693d5b937232decf1ee7524a9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:1ff5e500e2d42048923c1243ad26691c83c65406a33086f56e02e4fb2d43ecd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75006729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5261796049dd8a51b9e1c9ab5fa3e06960de7a813e7414dcc218022a6eb48680`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:00:59 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 12 Nov 2021 22:01:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 16:02:11 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 16:02:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 16:02:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 16:02:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:19 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 16:02:26 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 18 Nov 2021 16:02:27 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 18 Nov 2021 16:02:27 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 18 Nov 2021 16:02:28 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 18 Nov 2021 16:02:28 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:28 GMT
VOLUME [/var/lib/docker]
# Thu, 18 Nov 2021 16:02:29 GMT
EXPOSE 2375 2376
# Thu, 18 Nov 2021 16:02:29 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:29 GMT
CMD []
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b81e4bf1fdc42d15e4c1cfd4aa82e5fe027cf88bd858b5be7681ef621c617`  
		Last Modified: Fri, 12 Nov 2021 22:02:42 GMT  
		Size: 1.9 MB (1937203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da79b3d4ea6e72fe17974fcd737705b6da38e9063e5bbb26cea5a9fa7465bae`  
		Last Modified: Fri, 12 Nov 2021 22:02:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9433235d3590c575f74cf6c833b63c7e5fd2c2ebf7017a086421fb465c67327`  
		Last Modified: Thu, 18 Nov 2021 16:03:22 GMT  
		Size: 63.7 MB (63717036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a370fc1bfda2f2192e17db23cd29f495b5c0b6ab9f36d73ec07a9dbdae1310`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c0972549c69874ec2e53b7534184e975853ec9602f9a7ba7466bb1a231db9`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a0159d8a68d2886d05e662c609ac1dc10a9e3b73244d73106b8888a3bddfbb`  
		Last Modified: Thu, 18 Nov 2021 16:03:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2667e9a1d0ba047230eab7daedb7556a9d2204adebca9d7439ecaae6dbc1e3`  
		Last Modified: Thu, 18 Nov 2021 16:03:48 GMT  
		Size: 6.5 MB (6522755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f72da5423b84bdb2e04379edb8747ff161388fe38280eb242ef4d802008bf96`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b9fb6f0baf688ba32368dc395c50842182a9a4cadafd2cc0964570f740cd9a`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd10f5a3a8ed006ba472a52473be2b1f099d4b3b4cc8cdf52bae991cac915e0`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:6b91496cd8473f8f0412be846318dcf073a41e5c02fea27a75a657376c55e83b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68798719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9280bbaf2b20c01dbbcd50930cb5862adc44e531d88f54d157358d16f7de8a5f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:12:04 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Sat, 13 Nov 2021 11:12:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 09:17:16 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 09:17:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 09:17:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 09:17:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:25 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 09:17:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 09:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:28 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 09:17:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 18 Nov 2021 09:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 18 Nov 2021 09:17:40 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 18 Nov 2021 09:17:41 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 18 Nov 2021 09:17:43 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:43 GMT
VOLUME [/var/lib/docker]
# Thu, 18 Nov 2021 09:17:44 GMT
EXPOSE 2375 2376
# Thu, 18 Nov 2021 09:17:45 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:46 GMT
CMD []
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233f664f6e365c4259a38e7cfe3c14e234ab45f15847cc874a88b510f66a132f`  
		Last Modified: Sat, 13 Nov 2021 11:13:40 GMT  
		Size: 1.9 MB (1909969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c7cbdd3e377ff292e68f9ced99315b84c85398591633343352948bbc291`  
		Last Modified: Sat, 13 Nov 2021 11:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b50fed93df89351d596ab08fab482a174aa37a86d61cdeef150162665a67a80`  
		Last Modified: Thu, 18 Nov 2021 09:18:59 GMT  
		Size: 57.7 MB (57746015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21638a3c07c5ebd6977bcc9c75e0ac36c2a82b761fc51a8aee313c9a9d7ed46`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e37a1bae185ca8552a00efd7984a74bc595d0dac82ab81e945615f5a0b29af`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81c4e38c2d1b6603791a26f4dad582d554c306fb4c8c4218e0d537da3b8af6a`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc29a86f7ed1b15ec5c146abf64a41609779eb5b0e2a668d274b1b28c14c37e3`  
		Last Modified: Thu, 18 Nov 2021 09:19:20 GMT  
		Size: 6.4 MB (6418345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce285f2fd3dbcbe5e58749e817ef3a3e60fa1dbf82bc51eaff0f20f8e151d3f`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeabdc4aba67b4850e7e5c118e6409d59a161d11f5be536341a4e9f40ed017bf`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd2d42122e3f199551259bf3db06d2c446c725eb3ae3239f2692f3fa57804b5`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:154d9287cc128b8c4820b8d412652064cccd1466a61a50af871062b82cc05f6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:165b8b4bb284183bb67f3cb4617d84032b4d31d2a537e2bce63d016044a438c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95282418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:956ab016b037de2042fec25d130ac6a9aaa029a8183fff6512e356e2d44b205f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:00:59 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 12 Nov 2021 22:01:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 16:02:11 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 16:02:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 16:02:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 16:02:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:19 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 16:02:26 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 18 Nov 2021 16:02:27 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 18 Nov 2021 16:02:27 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 18 Nov 2021 16:02:28 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 18 Nov 2021 16:02:28 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:28 GMT
VOLUME [/var/lib/docker]
# Thu, 18 Nov 2021 16:02:29 GMT
EXPOSE 2375 2376
# Thu, 18 Nov 2021 16:02:29 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:29 GMT
CMD []
# Thu, 18 Nov 2021 16:02:33 GMT
RUN apk add --no-cache iproute2
# Thu, 18 Nov 2021 16:02:34 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 18 Nov 2021 16:02:35 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 18 Nov 2021 16:02:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 18 Nov 2021 16:02:38 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 18 Nov 2021 16:02:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 18 Nov 2021 16:02:39 GMT
USER rootless
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b81e4bf1fdc42d15e4c1cfd4aa82e5fe027cf88bd858b5be7681ef621c617`  
		Last Modified: Fri, 12 Nov 2021 22:02:42 GMT  
		Size: 1.9 MB (1937203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da79b3d4ea6e72fe17974fcd737705b6da38e9063e5bbb26cea5a9fa7465bae`  
		Last Modified: Fri, 12 Nov 2021 22:02:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9433235d3590c575f74cf6c833b63c7e5fd2c2ebf7017a086421fb465c67327`  
		Last Modified: Thu, 18 Nov 2021 16:03:22 GMT  
		Size: 63.7 MB (63717036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a370fc1bfda2f2192e17db23cd29f495b5c0b6ab9f36d73ec07a9dbdae1310`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c0972549c69874ec2e53b7534184e975853ec9602f9a7ba7466bb1a231db9`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a0159d8a68d2886d05e662c609ac1dc10a9e3b73244d73106b8888a3bddfbb`  
		Last Modified: Thu, 18 Nov 2021 16:03:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2667e9a1d0ba047230eab7daedb7556a9d2204adebca9d7439ecaae6dbc1e3`  
		Last Modified: Thu, 18 Nov 2021 16:03:48 GMT  
		Size: 6.5 MB (6522755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f72da5423b84bdb2e04379edb8747ff161388fe38280eb242ef4d802008bf96`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b9fb6f0baf688ba32368dc395c50842182a9a4cadafd2cc0964570f740cd9a`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd10f5a3a8ed006ba472a52473be2b1f099d4b3b4cc8cdf52bae991cac915e0`  
		Last Modified: Thu, 18 Nov 2021 16:03:47 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e11d3f7e286c938d26bbb186acb5479276df6361d8df2dcd69411be8e3a69d7`  
		Last Modified: Thu, 18 Nov 2021 16:04:10 GMT  
		Size: 1.1 MB (1149116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f294faaf6353a52c03a2b9dcfa622a83436f037202b20fb7683021db79e775`  
		Last Modified: Thu, 18 Nov 2021 16:04:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b662b3e60558d88a695d82eff536d1ce83c74cca00618f4a905ed756ca05f241`  
		Last Modified: Thu, 18 Nov 2021 16:04:10 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45688b3cc691166b57c28f4fadfe415eb8c9bdf22e92e43a60b0c7e50071a3ac`  
		Last Modified: Thu, 18 Nov 2021 16:04:15 GMT  
		Size: 19.1 MB (19124859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1ee7128b0e98cd946608ca63e413eeb9b68f68eedd4f1d58ff71fed621291b`  
		Last Modified: Thu, 18 Nov 2021 16:04:10 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:2441b89586372dc59c8fce28fc3fa0a6141193ad158d18482597187a7e1c9eeb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91070455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c509ba52a7374da993e6cf01a7147518857077192831cf839078772fa27881b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:12:04 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Sat, 13 Nov 2021 11:12:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 09:17:16 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 09:17:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 09:17:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 09:17:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:25 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 09:17:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 09:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:28 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 09:17:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 18 Nov 2021 09:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 18 Nov 2021 09:17:40 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 18 Nov 2021 09:17:41 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 18 Nov 2021 09:17:43 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:43 GMT
VOLUME [/var/lib/docker]
# Thu, 18 Nov 2021 09:17:44 GMT
EXPOSE 2375 2376
# Thu, 18 Nov 2021 09:17:45 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:46 GMT
CMD []
# Thu, 18 Nov 2021 09:17:54 GMT
RUN apk add --no-cache iproute2
# Thu, 18 Nov 2021 09:17:55 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 18 Nov 2021 09:17:56 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 18 Nov 2021 09:17:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 18 Nov 2021 09:18:00 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 18 Nov 2021 09:18:01 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 18 Nov 2021 09:18:02 GMT
USER rootless
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233f664f6e365c4259a38e7cfe3c14e234ab45f15847cc874a88b510f66a132f`  
		Last Modified: Sat, 13 Nov 2021 11:13:40 GMT  
		Size: 1.9 MB (1909969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c7cbdd3e377ff292e68f9ced99315b84c85398591633343352948bbc291`  
		Last Modified: Sat, 13 Nov 2021 11:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b50fed93df89351d596ab08fab482a174aa37a86d61cdeef150162665a67a80`  
		Last Modified: Thu, 18 Nov 2021 09:18:59 GMT  
		Size: 57.7 MB (57746015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21638a3c07c5ebd6977bcc9c75e0ac36c2a82b761fc51a8aee313c9a9d7ed46`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e37a1bae185ca8552a00efd7984a74bc595d0dac82ab81e945615f5a0b29af`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81c4e38c2d1b6603791a26f4dad582d554c306fb4c8c4218e0d537da3b8af6a`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc29a86f7ed1b15ec5c146abf64a41609779eb5b0e2a668d274b1b28c14c37e3`  
		Last Modified: Thu, 18 Nov 2021 09:19:20 GMT  
		Size: 6.4 MB (6418345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce285f2fd3dbcbe5e58749e817ef3a3e60fa1dbf82bc51eaff0f20f8e151d3f`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeabdc4aba67b4850e7e5c118e6409d59a161d11f5be536341a4e9f40ed017bf`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd2d42122e3f199551259bf3db06d2c446c725eb3ae3239f2692f3fa57804b5`  
		Last Modified: Thu, 18 Nov 2021 09:19:18 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230963f6db0e75d3a58bc46d5b33ea4f67e6b1f0300e99ba12497c89f68ce855`  
		Last Modified: Thu, 18 Nov 2021 09:19:41 GMT  
		Size: 1.2 MB (1168585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66cc595973e50f8d3e25c628464cfa45436824aab478bda61c9ac4232d822c3`  
		Last Modified: Thu, 18 Nov 2021 09:19:40 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55af54131c4a2bf83efebe4e4fec2d50bd4c99ffbca5aa5ccfa29c167f4c16ce`  
		Last Modified: Thu, 18 Nov 2021 09:19:40 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cab39e5c6b0a896c570c0218f29e0600936018957c487e7b439c9ecf14ad8e`  
		Last Modified: Thu, 18 Nov 2021 09:19:44 GMT  
		Size: 21.1 MB (21101528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365691e2dffd5c75fa3b86bd4ccd1b11a4beae986f511ce5400a6a3d69b550c`  
		Last Modified: Thu, 18 Nov 2021 09:19:40 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:50fdfef2982984d5f587a8274e932da365b322388804a9f1b30ef5eac2524527
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:dd201d3335196a559cdc166592a7acfbe9545e25aa83baa8c7e90fbee9353172
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75109809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26ae7c6d74e81d7ec18428ac5cdf0879073d8e746c341bf389aad8593a235e83`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:00:59 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 12 Nov 2021 22:01:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 16:02:11 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 16:02:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 16:02:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 16:02:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:19 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 16:02:43 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b81e4bf1fdc42d15e4c1cfd4aa82e5fe027cf88bd858b5be7681ef621c617`  
		Last Modified: Fri, 12 Nov 2021 22:02:42 GMT  
		Size: 1.9 MB (1937203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da79b3d4ea6e72fe17974fcd737705b6da38e9063e5bbb26cea5a9fa7465bae`  
		Last Modified: Fri, 12 Nov 2021 22:02:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9433235d3590c575f74cf6c833b63c7e5fd2c2ebf7017a086421fb465c67327`  
		Last Modified: Thu, 18 Nov 2021 16:03:22 GMT  
		Size: 63.7 MB (63717036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a370fc1bfda2f2192e17db23cd29f495b5c0b6ab9f36d73ec07a9dbdae1310`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c0972549c69874ec2e53b7534184e975853ec9602f9a7ba7466bb1a231db9`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a0159d8a68d2886d05e662c609ac1dc10a9e3b73244d73106b8888a3bddfbb`  
		Last Modified: Thu, 18 Nov 2021 16:03:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f4768f31acf9871e50a178b839a569a05c1b6a8923f4644db556da09776dbb`  
		Last Modified: Thu, 18 Nov 2021 16:04:34 GMT  
		Size: 6.6 MB (6630727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:abd4f25a749ebaac21635348b5e8db17d1d7cc5bcfa3b437e730b4178177cd2f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69115687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eb4264b475ad1b401f8776fd4d94293173ddd396cf1a88a5fb4372947b3ef3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:12:04 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Sat, 13 Nov 2021 11:12:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 09:17:16 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 09:17:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 09:17:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 09:17:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:25 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 09:17:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 09:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:28 GMT
CMD ["sh"]
# Thu, 18 Nov 2021 09:18:09 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233f664f6e365c4259a38e7cfe3c14e234ab45f15847cc874a88b510f66a132f`  
		Last Modified: Sat, 13 Nov 2021 11:13:40 GMT  
		Size: 1.9 MB (1909969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c7cbdd3e377ff292e68f9ced99315b84c85398591633343352948bbc291`  
		Last Modified: Sat, 13 Nov 2021 11:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b50fed93df89351d596ab08fab482a174aa37a86d61cdeef150162665a67a80`  
		Last Modified: Thu, 18 Nov 2021 09:18:59 GMT  
		Size: 57.7 MB (57746015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21638a3c07c5ebd6977bcc9c75e0ac36c2a82b761fc51a8aee313c9a9d7ed46`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e37a1bae185ca8552a00efd7984a74bc595d0dac82ab81e945615f5a0b29af`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81c4e38c2d1b6603791a26f4dad582d554c306fb4c8c4218e0d537da3b8af6a`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d06f8877e01ae57a21f32e8cdd5b66ffc3fdf70cfb5c8036a429db1ed15e12`  
		Last Modified: Thu, 18 Nov 2021 09:20:04 GMT  
		Size: 6.7 MB (6740174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:ff4fcc30e7c20f33c021e82683aedd1fe66654363eb1ff61065e0628f5bbf107
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:0cd49922b08a5b66239fc764abe872f4799e291922e21a31d9490a10278a5a02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68479082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c655f708b2a86c4b241e80a784479ee098833dc55d9d3929e1e35e1cb0297c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:00:59 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 12 Nov 2021 22:01:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 16:02:11 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 16:02:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 16:02:18 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:02:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 16:02:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 16:02:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 16:02:19 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b81e4bf1fdc42d15e4c1cfd4aa82e5fe027cf88bd858b5be7681ef621c617`  
		Last Modified: Fri, 12 Nov 2021 22:02:42 GMT  
		Size: 1.9 MB (1937203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da79b3d4ea6e72fe17974fcd737705b6da38e9063e5bbb26cea5a9fa7465bae`  
		Last Modified: Fri, 12 Nov 2021 22:02:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9433235d3590c575f74cf6c833b63c7e5fd2c2ebf7017a086421fb465c67327`  
		Last Modified: Thu, 18 Nov 2021 16:03:22 GMT  
		Size: 63.7 MB (63717036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a370fc1bfda2f2192e17db23cd29f495b5c0b6ab9f36d73ec07a9dbdae1310`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c0972549c69874ec2e53b7534184e975853ec9602f9a7ba7466bb1a231db9`  
		Last Modified: Thu, 18 Nov 2021 16:03:10 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a0159d8a68d2886d05e662c609ac1dc10a9e3b73244d73106b8888a3bddfbb`  
		Last Modified: Thu, 18 Nov 2021 16:03:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8aef5b543363230546c03371e8b3c857285ffdad566b676c3657cf64fedd9299
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62375513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0836e8a2fd6d55074387335d0a134d329cedce53561a1b6fc6eefe44cf1cf487`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:12:04 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Sat, 13 Nov 2021 11:12:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Nov 2021 09:17:16 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 09:17:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.11.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.11.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.11.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.11.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 18 Nov 2021 09:17:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 18 Nov 2021 09:17:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:17:25 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 18 Nov 2021 09:17:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 18 Nov 2021 09:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 09:17:28 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233f664f6e365c4259a38e7cfe3c14e234ab45f15847cc874a88b510f66a132f`  
		Last Modified: Sat, 13 Nov 2021 11:13:40 GMT  
		Size: 1.9 MB (1909969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c7cbdd3e377ff292e68f9ced99315b84c85398591633343352948bbc291`  
		Last Modified: Sat, 13 Nov 2021 11:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b50fed93df89351d596ab08fab482a174aa37a86d61cdeef150162665a67a80`  
		Last Modified: Thu, 18 Nov 2021 09:18:59 GMT  
		Size: 57.7 MB (57746015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21638a3c07c5ebd6977bcc9c75e0ac36c2a82b761fc51a8aee313c9a9d7ed46`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e37a1bae185ca8552a00efd7984a74bc595d0dac82ab81e945615f5a0b29af`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81c4e38c2d1b6603791a26f4dad582d554c306fb4c8c4218e0d537da3b8af6a`  
		Last Modified: Thu, 18 Nov 2021 09:18:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore`

```console
$ docker pull docker@sha256:280e2bfd85a1840bc5220777f9d70a85a6bf7fb35a3d8a03275043b5bdd07fb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `docker:windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull docker@sha256:f9935026e3d4f01f6ffe7c97d63ee7f286c77f52f80e2f1be8afe7de69ba531c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2757389706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feec87f6f82e9966337409c1601a519ee1ddc39fb68c10dbfbbb4cc6328de03d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 19:07:02 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 18 Nov 2021 04:13:52 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 04:13:53 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.11.zip
# Thu, 18 Nov 2021 04:15:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e42405e6d7d9caeb7c5a114493eca7f34351fae0fc2b77118957003b2f6c5f`  
		Last Modified: Wed, 10 Nov 2021 19:08:27 GMT  
		Size: 356.8 KB (356764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568ddc925a63c78da177f9676136448290dfbb54e31f140f98a3d4e0f3cfdc6d`  
		Last Modified: Thu, 18 Nov 2021 04:15:36 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a4753c3e1103c5a6292410a73e0d9eeeaa777557870a6d95dae8c80d822305`  
		Last Modified: Thu, 18 Nov 2021 04:15:36 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc58abb4c9cd5805540f354d6ba7931a7afec3062b7f8ff918c78378ac5d876f`  
		Last Modified: Thu, 18 Nov 2021 04:16:34 GMT  
		Size: 50.9 MB (50907794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:280e2bfd85a1840bc5220777f9d70a85a6bf7fb35a3d8a03275043b5bdd07fb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull docker@sha256:f9935026e3d4f01f6ffe7c97d63ee7f286c77f52f80e2f1be8afe7de69ba531c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2757389706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feec87f6f82e9966337409c1601a519ee1ddc39fb68c10dbfbbb4cc6328de03d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 19:07:02 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 18 Nov 2021 04:13:52 GMT
ENV DOCKER_VERSION=20.10.11
# Thu, 18 Nov 2021 04:13:53 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.11.zip
# Thu, 18 Nov 2021 04:15:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e42405e6d7d9caeb7c5a114493eca7f34351fae0fc2b77118957003b2f6c5f`  
		Last Modified: Wed, 10 Nov 2021 19:08:27 GMT  
		Size: 356.8 KB (356764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568ddc925a63c78da177f9676136448290dfbb54e31f140f98a3d4e0f3cfdc6d`  
		Last Modified: Thu, 18 Nov 2021 04:15:36 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a4753c3e1103c5a6292410a73e0d9eeeaa777557870a6d95dae8c80d822305`  
		Last Modified: Thu, 18 Nov 2021 04:15:36 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc58abb4c9cd5805540f354d6ba7931a7afec3062b7f8ff918c78378ac5d876f`  
		Last Modified: Thu, 18 Nov 2021 04:16:34 GMT  
		Size: 50.9 MB (50907794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
