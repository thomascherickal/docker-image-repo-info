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
-	[`docker:20.10.12`](#docker201012)
-	[`docker:20.10.12-alpine3.15`](#docker201012-alpine315)
-	[`docker:20.10.12-dind`](#docker201012-dind)
-	[`docker:20.10.12-dind-alpine3.15`](#docker201012-dind-alpine315)
-	[`docker:20.10.12-dind-rootless`](#docker201012-dind-rootless)
-	[`docker:20.10.12-git`](#docker201012-git)
-	[`docker:20.10.12-windowsservercore`](#docker201012-windowsservercore)
-	[`docker:20.10.12-windowsservercore-1809`](#docker201012-windowsservercore-1809)
-	[`docker:dind`](#dockerdind)
-	[`docker:dind-rootless`](#dockerdind-rootless)
-	[`docker:git`](#dockergit)
-	[`docker:latest`](#dockerlatest)
-	[`docker:windowsservercore`](#dockerwindowsservercore)
-	[`docker:windowsservercore-1809`](#dockerwindowsservercore-1809)

## `docker:20`

```console
$ docker pull docker@sha256:7576c1354d56ada47f1e52b9f5b9f472cb4bc85e299432b5508b5661228d3104
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20` - linux; amd64

```console
$ docker pull docker@sha256:09f8748c248001840cdb2a0ce93ccc3e20100a910e51158d3f74e708ad899f73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68480564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff1c1f4454a0a9a125b74d9850d4a79dd8973ff2a9ca39f9de2648b123750d4d`
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
# Tue, 14 Dec 2021 01:19:22 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:19:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:29 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:19:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:30 GMT
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
	-	`sha256:7f22bd4996264a086a8770f4f667d2fb7877b525951480e7121a1a4c3905e3a1`  
		Last Modified: Tue, 14 Dec 2021 01:20:27 GMT  
		Size: 63.7 MB (63718514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b00d1b5a23c849695e38cc1c8d7a9cca6d62f173982209441666d4c7cb25b`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6ad723338071334a09327bc602580ca713fa4ff41c9cba96b0682f9c96e752`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad69ecad074ceedac2158c71f1890d95dc421ceae190b0608170261ddad1c8fa`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:74e1492f3a3c1716347ce322bcae5838e7676eac8d0c53aa20615d7d056ee0db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62376713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3acd5d40f4879cbbb916d83836f8d66d4d60654671f2bc00f81597d31cb04771`
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
# Tue, 14 Dec 2021 01:39:30 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:39:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:39:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:39:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:39:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:40 GMT
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
	-	`sha256:efa29b56432c31c1ae3e3a198fd660fe24aad4f3c1bd2fcc41ec7bec1c86127a`  
		Last Modified: Tue, 14 Dec 2021 01:41:12 GMT  
		Size: 57.7 MB (57747212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03e69d0d3fb7491b603b26d6209129be9cc220a763e55d8f61e0f615dd67eec`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d00fe7a17c2f14d79be0e290f3f72bbfa899722f3136964137f41c55299faf0`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fdcc8ecc6967aea4440794a0fe37896acca35ad9541b1e91550a8cabaecc7b`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind`

```console
$ docker pull docker@sha256:f18cb807df96d3b9d4d096ddef6c800ed7c779964ea723d02b32b6fe2cee3e0a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind` - linux; amd64

```console
$ docker pull docker@sha256:9deffd6a4e57534f4a01eef1ac10a6017a301ec698e79603f8b8a13ab3ef33bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75008177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c15c97e82b6205f24eedbb8d68635967b13e48f8f3593083759febe9a9503a5`
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
# Tue, 14 Dec 2021 01:19:22 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:19:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:29 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:19:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:30 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:19:36 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 14 Dec 2021 01:19:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:19:37 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 14 Dec 2021 01:19:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 14 Dec 2021 01:19:39 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:39 GMT
VOLUME [/var/lib/docker]
# Tue, 14 Dec 2021 01:19:39 GMT
EXPOSE 2375 2376
# Tue, 14 Dec 2021 01:19:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:39 GMT
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
	-	`sha256:7f22bd4996264a086a8770f4f667d2fb7877b525951480e7121a1a4c3905e3a1`  
		Last Modified: Tue, 14 Dec 2021 01:20:27 GMT  
		Size: 63.7 MB (63718514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b00d1b5a23c849695e38cc1c8d7a9cca6d62f173982209441666d4c7cb25b`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6ad723338071334a09327bc602580ca713fa4ff41c9cba96b0682f9c96e752`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad69ecad074ceedac2158c71f1890d95dc421ceae190b0608170261ddad1c8fa`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f042b35272e657c8969916691d9d1bba7ae8851dc915f76b2c506e8a29c543df`  
		Last Modified: Tue, 14 Dec 2021 01:20:47 GMT  
		Size: 6.5 MB (6522717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc27002d71f82e23a7ff61b4b6a82e9e38226da406833f6addc45a85322ec39`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f75dc2db7d9c3b72573b7b542f56b99b99c33ef1318dfd7fd7052cb9e0e8c7`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd05b7cec7a24208dfc6bc6b1fd6d12fcbb6952bcea5d42b60ad5b3acf4f1211`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:36774fd5f0e105eaecea48094276b7c9553d87607d0409c57b8af57cf5aba8c7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68799974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbc79ed4af04a8cad8cec4f9176dbcb26b12c6c71e2d249aae088a3acdc7500a`
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
# Tue, 14 Dec 2021 01:39:30 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:39:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:39:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:39:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:39:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:40 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:39:50 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 14 Dec 2021 01:39:51 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:39:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 14 Dec 2021 01:39:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 14 Dec 2021 01:39:55 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:55 GMT
VOLUME [/var/lib/docker]
# Tue, 14 Dec 2021 01:39:56 GMT
EXPOSE 2375 2376
# Tue, 14 Dec 2021 01:39:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:58 GMT
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
	-	`sha256:efa29b56432c31c1ae3e3a198fd660fe24aad4f3c1bd2fcc41ec7bec1c86127a`  
		Last Modified: Tue, 14 Dec 2021 01:41:12 GMT  
		Size: 57.7 MB (57747212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03e69d0d3fb7491b603b26d6209129be9cc220a763e55d8f61e0f615dd67eec`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d00fe7a17c2f14d79be0e290f3f72bbfa899722f3136964137f41c55299faf0`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fdcc8ecc6967aea4440794a0fe37896acca35ad9541b1e91550a8cabaecc7b`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6139c50bbab98e9bb1d1aa2396b4c1e18b2861015efe52da5cbd4660705e38`  
		Last Modified: Tue, 14 Dec 2021 01:41:33 GMT  
		Size: 6.4 MB (6418394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36036b817024bbc3edcaff34d3688363c0659efe28a2ae890783ea074bc121e2`  
		Last Modified: Tue, 14 Dec 2021 01:41:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923c1073ccef6aa80d889d9bb29d6ad6226a6c76e4d8425233d62af225d270b0`  
		Last Modified: Tue, 14 Dec 2021 01:41:33 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e05effd75ccd7827a2c37694bc29f407143b4b4ffdb8ef6b0a7a9205aead834`  
		Last Modified: Tue, 14 Dec 2021 01:41:32 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:01b992491884cd0dca76675926097d3534b00f5ee9e60cfd195c5e4a764a4534
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:5e9deaaf38b027b5a5f033c548da2296ec0429bd21d3db137069e7a3add1712c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95290953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43c1e14ca17cb3d66246538810f34e4df5854eced27d3bb833f453db0cb53e6c`
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
# Tue, 14 Dec 2021 01:19:22 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:19:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:29 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:19:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:30 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:19:36 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 14 Dec 2021 01:19:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:19:37 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 14 Dec 2021 01:19:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 14 Dec 2021 01:19:39 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:39 GMT
VOLUME [/var/lib/docker]
# Tue, 14 Dec 2021 01:19:39 GMT
EXPOSE 2375 2376
# Tue, 14 Dec 2021 01:19:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:39 GMT
CMD []
# Tue, 14 Dec 2021 01:19:43 GMT
RUN apk add --no-cache iproute2
# Tue, 14 Dec 2021 01:19:44 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 14 Dec 2021 01:19:45 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:19:47 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 14 Dec 2021 01:19:48 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 14 Dec 2021 01:19:48 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 14 Dec 2021 01:19:48 GMT
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
	-	`sha256:7f22bd4996264a086a8770f4f667d2fb7877b525951480e7121a1a4c3905e3a1`  
		Last Modified: Tue, 14 Dec 2021 01:20:27 GMT  
		Size: 63.7 MB (63718514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b00d1b5a23c849695e38cc1c8d7a9cca6d62f173982209441666d4c7cb25b`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6ad723338071334a09327bc602580ca713fa4ff41c9cba96b0682f9c96e752`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad69ecad074ceedac2158c71f1890d95dc421ceae190b0608170261ddad1c8fa`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f042b35272e657c8969916691d9d1bba7ae8851dc915f76b2c506e8a29c543df`  
		Last Modified: Tue, 14 Dec 2021 01:20:47 GMT  
		Size: 6.5 MB (6522717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc27002d71f82e23a7ff61b4b6a82e9e38226da406833f6addc45a85322ec39`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f75dc2db7d9c3b72573b7b542f56b99b99c33ef1318dfd7fd7052cb9e0e8c7`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd05b7cec7a24208dfc6bc6b1fd6d12fcbb6952bcea5d42b60ad5b3acf4f1211`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895786101537dd46ede9b73a7e9aeda41de46cd664d0bc7372d98337de961ab3`  
		Last Modified: Tue, 14 Dec 2021 01:21:07 GMT  
		Size: 1.1 MB (1149119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3069ef522e1061f2cf66d656ed079481ea603e6cd482656f4c1d4f89b87677a`  
		Last Modified: Tue, 14 Dec 2021 01:21:07 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd05514682855814f146fd143e50fccb168ba0211450583daaba94900dc2032f`  
		Last Modified: Tue, 14 Dec 2021 01:21:07 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a912066e38c030b9897a347cc9dffb6f3df2ce002b7b9eeec1d6dff74e8ba275`  
		Last Modified: Tue, 14 Dec 2021 01:21:10 GMT  
		Size: 19.1 MB (19131942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfc994d0a45d0f7ccc0175ae21d2c32b2d70e0e1ac2f05fb7d9e6f60ae37de1`  
		Last Modified: Tue, 14 Dec 2021 01:21:07 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:d8cbc56394ae3dcb2152c14f1abb85a50262b05a02ca6db21a8f566c60a2c151
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91075410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e14b610229d453c957535c435f52080c651f1dd2f59919d9051c4e695a1dd16`
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
# Tue, 14 Dec 2021 01:39:30 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:39:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:39:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:39:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:39:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:40 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:39:50 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 14 Dec 2021 01:39:51 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:39:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 14 Dec 2021 01:39:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 14 Dec 2021 01:39:55 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:55 GMT
VOLUME [/var/lib/docker]
# Tue, 14 Dec 2021 01:39:56 GMT
EXPOSE 2375 2376
# Tue, 14 Dec 2021 01:39:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:58 GMT
CMD []
# Tue, 14 Dec 2021 01:40:06 GMT
RUN apk add --no-cache iproute2
# Tue, 14 Dec 2021 01:40:07 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 14 Dec 2021 01:40:08 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:40:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 14 Dec 2021 01:40:12 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 14 Dec 2021 01:40:13 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 14 Dec 2021 01:40:14 GMT
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
	-	`sha256:efa29b56432c31c1ae3e3a198fd660fe24aad4f3c1bd2fcc41ec7bec1c86127a`  
		Last Modified: Tue, 14 Dec 2021 01:41:12 GMT  
		Size: 57.7 MB (57747212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03e69d0d3fb7491b603b26d6209129be9cc220a763e55d8f61e0f615dd67eec`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d00fe7a17c2f14d79be0e290f3f72bbfa899722f3136964137f41c55299faf0`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fdcc8ecc6967aea4440794a0fe37896acca35ad9541b1e91550a8cabaecc7b`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6139c50bbab98e9bb1d1aa2396b4c1e18b2861015efe52da5cbd4660705e38`  
		Last Modified: Tue, 14 Dec 2021 01:41:33 GMT  
		Size: 6.4 MB (6418394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36036b817024bbc3edcaff34d3688363c0659efe28a2ae890783ea074bc121e2`  
		Last Modified: Tue, 14 Dec 2021 01:41:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923c1073ccef6aa80d889d9bb29d6ad6226a6c76e4d8425233d62af225d270b0`  
		Last Modified: Tue, 14 Dec 2021 01:41:33 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e05effd75ccd7827a2c37694bc29f407143b4b4ffdb8ef6b0a7a9205aead834`  
		Last Modified: Tue, 14 Dec 2021 01:41:32 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e512c70c3e7c936e32ce6b40f81a8b1fe652a867b1052540fce9d592b8d57c2`  
		Last Modified: Tue, 14 Dec 2021 01:41:55 GMT  
		Size: 1.2 MB (1168597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f629c942ca98a178333071f9e485fd5fc62c9f95f3eaf124dfa919ecd59b06`  
		Last Modified: Tue, 14 Dec 2021 01:41:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac41d51e834ca86a8b9f559608abda6fbb9a25d331a91ca14351a54c0072ea7`  
		Last Modified: Tue, 14 Dec 2021 01:41:55 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f721865855552d187017d6a733b602cc288bb0f67e75e786d42975c2f96b1ae`  
		Last Modified: Tue, 14 Dec 2021 01:41:58 GMT  
		Size: 21.1 MB (21105216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad8303f5f8549cce863da24719c3251898d720cdbe18479d95f2f06bde15606`  
		Last Modified: Tue, 14 Dec 2021 01:41:55 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-git`

```console
$ docker pull docker@sha256:20ca38ca6e5f9b2389b832053e090ff5160120c7b2365326599a1b1f55bd935a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-git` - linux; amd64

```console
$ docker pull docker@sha256:5e0b8727e8f439bfeb7cc9ece341e1627b38475aea43aeb78bdf7f1ce78b4d00
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75111302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e508e51d27b39da3d198527a2fe2eb1020b4c4a22186a889f5b08ebcd0a8ba73`
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
# Tue, 14 Dec 2021 01:19:22 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:19:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:29 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:19:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:30 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:19:52 GMT
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
	-	`sha256:7f22bd4996264a086a8770f4f667d2fb7877b525951480e7121a1a4c3905e3a1`  
		Last Modified: Tue, 14 Dec 2021 01:20:27 GMT  
		Size: 63.7 MB (63718514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b00d1b5a23c849695e38cc1c8d7a9cca6d62f173982209441666d4c7cb25b`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6ad723338071334a09327bc602580ca713fa4ff41c9cba96b0682f9c96e752`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad69ecad074ceedac2158c71f1890d95dc421ceae190b0608170261ddad1c8fa`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90cf0bd28b7a98109de7f7f39709740eccdb39470fc6df3d5ef6e47b77d6862`  
		Last Modified: Tue, 14 Dec 2021 01:21:34 GMT  
		Size: 6.6 MB (6630738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:fc0c35f685a42162c84f28e67392a2df8d905dcf8c266bd75623c50a2efc62e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69116887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfa2d5809f71991954f14c210580ffe0abac8bcc10dbabae3265ca6bf8356cd1`
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
# Tue, 14 Dec 2021 01:39:30 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:39:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:39:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:39:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:39:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:40 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:40:22 GMT
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
	-	`sha256:efa29b56432c31c1ae3e3a198fd660fe24aad4f3c1bd2fcc41ec7bec1c86127a`  
		Last Modified: Tue, 14 Dec 2021 01:41:12 GMT  
		Size: 57.7 MB (57747212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03e69d0d3fb7491b603b26d6209129be9cc220a763e55d8f61e0f615dd67eec`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d00fe7a17c2f14d79be0e290f3f72bbfa899722f3136964137f41c55299faf0`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fdcc8ecc6967aea4440794a0fe37896acca35ad9541b1e91550a8cabaecc7b`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d111a24a972eb73f8f7928da3ce21c28424a6fd6db2041fcdf541808cef53742`  
		Last Modified: Tue, 14 Dec 2021 01:42:19 GMT  
		Size: 6.7 MB (6740174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore`

```console
$ docker pull docker@sha256:aeae5d99fe3dc85006d347bcd0f0209b8350fbba00fff026ddd2927a9927bca3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `docker:20-windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull docker@sha256:bddeba547b89b83f3504923c518755dcefbd6d6af21e3b880b342c9fd632a75d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2759710145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c7db75db2732a0bbca809e17a72de80fae5ff7722bdce5cbc4b7f34dfaeb01`
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
# Tue, 14 Dec 2021 01:14:53 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:14:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.12.zip
# Tue, 14 Dec 2021 01:16:12 GMT
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
	-	`sha256:e2dca1c227843d13b5eed8f547ee009f1c0a3f31cee57cd0478d6a5187c0565c`  
		Last Modified: Tue, 14 Dec 2021 01:16:37 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be433795619099d6fd71321a47a80e03c2c381ae57b9d90b92b45627ff7f6d96`  
		Last Modified: Tue, 14 Dec 2021 01:16:37 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66d67f0ea287b8dd2ba1e3a70e2ce53cce0b193f44a01bdc569ed2688465f5a`  
		Last Modified: Tue, 14 Dec 2021 01:16:48 GMT  
		Size: 53.2 MB (53228223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-1809`

```console
$ docker pull docker@sha256:aeae5d99fe3dc85006d347bcd0f0209b8350fbba00fff026ddd2927a9927bca3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `docker:20-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull docker@sha256:bddeba547b89b83f3504923c518755dcefbd6d6af21e3b880b342c9fd632a75d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2759710145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c7db75db2732a0bbca809e17a72de80fae5ff7722bdce5cbc4b7f34dfaeb01`
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
# Tue, 14 Dec 2021 01:14:53 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:14:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.12.zip
# Tue, 14 Dec 2021 01:16:12 GMT
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
	-	`sha256:e2dca1c227843d13b5eed8f547ee009f1c0a3f31cee57cd0478d6a5187c0565c`  
		Last Modified: Tue, 14 Dec 2021 01:16:37 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be433795619099d6fd71321a47a80e03c2c381ae57b9d90b92b45627ff7f6d96`  
		Last Modified: Tue, 14 Dec 2021 01:16:37 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66d67f0ea287b8dd2ba1e3a70e2ce53cce0b193f44a01bdc569ed2688465f5a`  
		Last Modified: Tue, 14 Dec 2021 01:16:48 GMT  
		Size: 53.2 MB (53228223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10`

```console
$ docker pull docker@sha256:7576c1354d56ada47f1e52b9f5b9f472cb4bc85e299432b5508b5661228d3104
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10` - linux; amd64

```console
$ docker pull docker@sha256:09f8748c248001840cdb2a0ce93ccc3e20100a910e51158d3f74e708ad899f73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68480564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff1c1f4454a0a9a125b74d9850d4a79dd8973ff2a9ca39f9de2648b123750d4d`
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
# Tue, 14 Dec 2021 01:19:22 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:19:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:29 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:19:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:30 GMT
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
	-	`sha256:7f22bd4996264a086a8770f4f667d2fb7877b525951480e7121a1a4c3905e3a1`  
		Last Modified: Tue, 14 Dec 2021 01:20:27 GMT  
		Size: 63.7 MB (63718514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b00d1b5a23c849695e38cc1c8d7a9cca6d62f173982209441666d4c7cb25b`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6ad723338071334a09327bc602580ca713fa4ff41c9cba96b0682f9c96e752`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad69ecad074ceedac2158c71f1890d95dc421ceae190b0608170261ddad1c8fa`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:74e1492f3a3c1716347ce322bcae5838e7676eac8d0c53aa20615d7d056ee0db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62376713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3acd5d40f4879cbbb916d83836f8d66d4d60654671f2bc00f81597d31cb04771`
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
# Tue, 14 Dec 2021 01:39:30 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:39:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:39:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:39:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:39:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:40 GMT
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
	-	`sha256:efa29b56432c31c1ae3e3a198fd660fe24aad4f3c1bd2fcc41ec7bec1c86127a`  
		Last Modified: Tue, 14 Dec 2021 01:41:12 GMT  
		Size: 57.7 MB (57747212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03e69d0d3fb7491b603b26d6209129be9cc220a763e55d8f61e0f615dd67eec`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d00fe7a17c2f14d79be0e290f3f72bbfa899722f3136964137f41c55299faf0`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fdcc8ecc6967aea4440794a0fe37896acca35ad9541b1e91550a8cabaecc7b`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind`

```console
$ docker pull docker@sha256:f18cb807df96d3b9d4d096ddef6c800ed7c779964ea723d02b32b6fe2cee3e0a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind` - linux; amd64

```console
$ docker pull docker@sha256:9deffd6a4e57534f4a01eef1ac10a6017a301ec698e79603f8b8a13ab3ef33bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75008177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c15c97e82b6205f24eedbb8d68635967b13e48f8f3593083759febe9a9503a5`
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
# Tue, 14 Dec 2021 01:19:22 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:19:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:29 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:19:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:30 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:19:36 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 14 Dec 2021 01:19:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:19:37 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 14 Dec 2021 01:19:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 14 Dec 2021 01:19:39 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:39 GMT
VOLUME [/var/lib/docker]
# Tue, 14 Dec 2021 01:19:39 GMT
EXPOSE 2375 2376
# Tue, 14 Dec 2021 01:19:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:39 GMT
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
	-	`sha256:7f22bd4996264a086a8770f4f667d2fb7877b525951480e7121a1a4c3905e3a1`  
		Last Modified: Tue, 14 Dec 2021 01:20:27 GMT  
		Size: 63.7 MB (63718514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b00d1b5a23c849695e38cc1c8d7a9cca6d62f173982209441666d4c7cb25b`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6ad723338071334a09327bc602580ca713fa4ff41c9cba96b0682f9c96e752`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad69ecad074ceedac2158c71f1890d95dc421ceae190b0608170261ddad1c8fa`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f042b35272e657c8969916691d9d1bba7ae8851dc915f76b2c506e8a29c543df`  
		Last Modified: Tue, 14 Dec 2021 01:20:47 GMT  
		Size: 6.5 MB (6522717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc27002d71f82e23a7ff61b4b6a82e9e38226da406833f6addc45a85322ec39`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f75dc2db7d9c3b72573b7b542f56b99b99c33ef1318dfd7fd7052cb9e0e8c7`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd05b7cec7a24208dfc6bc6b1fd6d12fcbb6952bcea5d42b60ad5b3acf4f1211`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:36774fd5f0e105eaecea48094276b7c9553d87607d0409c57b8af57cf5aba8c7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68799974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbc79ed4af04a8cad8cec4f9176dbcb26b12c6c71e2d249aae088a3acdc7500a`
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
# Tue, 14 Dec 2021 01:39:30 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:39:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:39:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:39:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:39:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:40 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:39:50 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 14 Dec 2021 01:39:51 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:39:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 14 Dec 2021 01:39:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 14 Dec 2021 01:39:55 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:55 GMT
VOLUME [/var/lib/docker]
# Tue, 14 Dec 2021 01:39:56 GMT
EXPOSE 2375 2376
# Tue, 14 Dec 2021 01:39:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:58 GMT
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
	-	`sha256:efa29b56432c31c1ae3e3a198fd660fe24aad4f3c1bd2fcc41ec7bec1c86127a`  
		Last Modified: Tue, 14 Dec 2021 01:41:12 GMT  
		Size: 57.7 MB (57747212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03e69d0d3fb7491b603b26d6209129be9cc220a763e55d8f61e0f615dd67eec`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d00fe7a17c2f14d79be0e290f3f72bbfa899722f3136964137f41c55299faf0`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fdcc8ecc6967aea4440794a0fe37896acca35ad9541b1e91550a8cabaecc7b`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6139c50bbab98e9bb1d1aa2396b4c1e18b2861015efe52da5cbd4660705e38`  
		Last Modified: Tue, 14 Dec 2021 01:41:33 GMT  
		Size: 6.4 MB (6418394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36036b817024bbc3edcaff34d3688363c0659efe28a2ae890783ea074bc121e2`  
		Last Modified: Tue, 14 Dec 2021 01:41:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923c1073ccef6aa80d889d9bb29d6ad6226a6c76e4d8425233d62af225d270b0`  
		Last Modified: Tue, 14 Dec 2021 01:41:33 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e05effd75ccd7827a2c37694bc29f407143b4b4ffdb8ef6b0a7a9205aead834`  
		Last Modified: Tue, 14 Dec 2021 01:41:32 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind-rootless`

```console
$ docker pull docker@sha256:01b992491884cd0dca76675926097d3534b00f5ee9e60cfd195c5e4a764a4534
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:5e9deaaf38b027b5a5f033c548da2296ec0429bd21d3db137069e7a3add1712c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95290953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43c1e14ca17cb3d66246538810f34e4df5854eced27d3bb833f453db0cb53e6c`
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
# Tue, 14 Dec 2021 01:19:22 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:19:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:29 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:19:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:30 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:19:36 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 14 Dec 2021 01:19:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:19:37 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 14 Dec 2021 01:19:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 14 Dec 2021 01:19:39 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:39 GMT
VOLUME [/var/lib/docker]
# Tue, 14 Dec 2021 01:19:39 GMT
EXPOSE 2375 2376
# Tue, 14 Dec 2021 01:19:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:39 GMT
CMD []
# Tue, 14 Dec 2021 01:19:43 GMT
RUN apk add --no-cache iproute2
# Tue, 14 Dec 2021 01:19:44 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 14 Dec 2021 01:19:45 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:19:47 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 14 Dec 2021 01:19:48 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 14 Dec 2021 01:19:48 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 14 Dec 2021 01:19:48 GMT
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
	-	`sha256:7f22bd4996264a086a8770f4f667d2fb7877b525951480e7121a1a4c3905e3a1`  
		Last Modified: Tue, 14 Dec 2021 01:20:27 GMT  
		Size: 63.7 MB (63718514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b00d1b5a23c849695e38cc1c8d7a9cca6d62f173982209441666d4c7cb25b`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6ad723338071334a09327bc602580ca713fa4ff41c9cba96b0682f9c96e752`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad69ecad074ceedac2158c71f1890d95dc421ceae190b0608170261ddad1c8fa`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f042b35272e657c8969916691d9d1bba7ae8851dc915f76b2c506e8a29c543df`  
		Last Modified: Tue, 14 Dec 2021 01:20:47 GMT  
		Size: 6.5 MB (6522717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc27002d71f82e23a7ff61b4b6a82e9e38226da406833f6addc45a85322ec39`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f75dc2db7d9c3b72573b7b542f56b99b99c33ef1318dfd7fd7052cb9e0e8c7`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd05b7cec7a24208dfc6bc6b1fd6d12fcbb6952bcea5d42b60ad5b3acf4f1211`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895786101537dd46ede9b73a7e9aeda41de46cd664d0bc7372d98337de961ab3`  
		Last Modified: Tue, 14 Dec 2021 01:21:07 GMT  
		Size: 1.1 MB (1149119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3069ef522e1061f2cf66d656ed079481ea603e6cd482656f4c1d4f89b87677a`  
		Last Modified: Tue, 14 Dec 2021 01:21:07 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd05514682855814f146fd143e50fccb168ba0211450583daaba94900dc2032f`  
		Last Modified: Tue, 14 Dec 2021 01:21:07 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a912066e38c030b9897a347cc9dffb6f3df2ce002b7b9eeec1d6dff74e8ba275`  
		Last Modified: Tue, 14 Dec 2021 01:21:10 GMT  
		Size: 19.1 MB (19131942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfc994d0a45d0f7ccc0175ae21d2c32b2d70e0e1ac2f05fb7d9e6f60ae37de1`  
		Last Modified: Tue, 14 Dec 2021 01:21:07 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:d8cbc56394ae3dcb2152c14f1abb85a50262b05a02ca6db21a8f566c60a2c151
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91075410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e14b610229d453c957535c435f52080c651f1dd2f59919d9051c4e695a1dd16`
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
# Tue, 14 Dec 2021 01:39:30 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:39:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:39:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:39:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:39:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:40 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:39:50 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 14 Dec 2021 01:39:51 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:39:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 14 Dec 2021 01:39:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 14 Dec 2021 01:39:55 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:55 GMT
VOLUME [/var/lib/docker]
# Tue, 14 Dec 2021 01:39:56 GMT
EXPOSE 2375 2376
# Tue, 14 Dec 2021 01:39:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:58 GMT
CMD []
# Tue, 14 Dec 2021 01:40:06 GMT
RUN apk add --no-cache iproute2
# Tue, 14 Dec 2021 01:40:07 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 14 Dec 2021 01:40:08 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:40:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 14 Dec 2021 01:40:12 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 14 Dec 2021 01:40:13 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 14 Dec 2021 01:40:14 GMT
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
	-	`sha256:efa29b56432c31c1ae3e3a198fd660fe24aad4f3c1bd2fcc41ec7bec1c86127a`  
		Last Modified: Tue, 14 Dec 2021 01:41:12 GMT  
		Size: 57.7 MB (57747212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03e69d0d3fb7491b603b26d6209129be9cc220a763e55d8f61e0f615dd67eec`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d00fe7a17c2f14d79be0e290f3f72bbfa899722f3136964137f41c55299faf0`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fdcc8ecc6967aea4440794a0fe37896acca35ad9541b1e91550a8cabaecc7b`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6139c50bbab98e9bb1d1aa2396b4c1e18b2861015efe52da5cbd4660705e38`  
		Last Modified: Tue, 14 Dec 2021 01:41:33 GMT  
		Size: 6.4 MB (6418394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36036b817024bbc3edcaff34d3688363c0659efe28a2ae890783ea074bc121e2`  
		Last Modified: Tue, 14 Dec 2021 01:41:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923c1073ccef6aa80d889d9bb29d6ad6226a6c76e4d8425233d62af225d270b0`  
		Last Modified: Tue, 14 Dec 2021 01:41:33 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e05effd75ccd7827a2c37694bc29f407143b4b4ffdb8ef6b0a7a9205aead834`  
		Last Modified: Tue, 14 Dec 2021 01:41:32 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e512c70c3e7c936e32ce6b40f81a8b1fe652a867b1052540fce9d592b8d57c2`  
		Last Modified: Tue, 14 Dec 2021 01:41:55 GMT  
		Size: 1.2 MB (1168597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f629c942ca98a178333071f9e485fd5fc62c9f95f3eaf124dfa919ecd59b06`  
		Last Modified: Tue, 14 Dec 2021 01:41:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac41d51e834ca86a8b9f559608abda6fbb9a25d331a91ca14351a54c0072ea7`  
		Last Modified: Tue, 14 Dec 2021 01:41:55 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f721865855552d187017d6a733b602cc288bb0f67e75e786d42975c2f96b1ae`  
		Last Modified: Tue, 14 Dec 2021 01:41:58 GMT  
		Size: 21.1 MB (21105216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad8303f5f8549cce863da24719c3251898d720cdbe18479d95f2f06bde15606`  
		Last Modified: Tue, 14 Dec 2021 01:41:55 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-git`

```console
$ docker pull docker@sha256:20ca38ca6e5f9b2389b832053e090ff5160120c7b2365326599a1b1f55bd935a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-git` - linux; amd64

```console
$ docker pull docker@sha256:5e0b8727e8f439bfeb7cc9ece341e1627b38475aea43aeb78bdf7f1ce78b4d00
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75111302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e508e51d27b39da3d198527a2fe2eb1020b4c4a22186a889f5b08ebcd0a8ba73`
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
# Tue, 14 Dec 2021 01:19:22 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:19:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:29 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:19:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:30 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:19:52 GMT
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
	-	`sha256:7f22bd4996264a086a8770f4f667d2fb7877b525951480e7121a1a4c3905e3a1`  
		Last Modified: Tue, 14 Dec 2021 01:20:27 GMT  
		Size: 63.7 MB (63718514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b00d1b5a23c849695e38cc1c8d7a9cca6d62f173982209441666d4c7cb25b`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6ad723338071334a09327bc602580ca713fa4ff41c9cba96b0682f9c96e752`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad69ecad074ceedac2158c71f1890d95dc421ceae190b0608170261ddad1c8fa`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90cf0bd28b7a98109de7f7f39709740eccdb39470fc6df3d5ef6e47b77d6862`  
		Last Modified: Tue, 14 Dec 2021 01:21:34 GMT  
		Size: 6.6 MB (6630738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:fc0c35f685a42162c84f28e67392a2df8d905dcf8c266bd75623c50a2efc62e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69116887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfa2d5809f71991954f14c210580ffe0abac8bcc10dbabae3265ca6bf8356cd1`
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
# Tue, 14 Dec 2021 01:39:30 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:39:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:39:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:39:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:39:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:40 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:40:22 GMT
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
	-	`sha256:efa29b56432c31c1ae3e3a198fd660fe24aad4f3c1bd2fcc41ec7bec1c86127a`  
		Last Modified: Tue, 14 Dec 2021 01:41:12 GMT  
		Size: 57.7 MB (57747212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03e69d0d3fb7491b603b26d6209129be9cc220a763e55d8f61e0f615dd67eec`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d00fe7a17c2f14d79be0e290f3f72bbfa899722f3136964137f41c55299faf0`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fdcc8ecc6967aea4440794a0fe37896acca35ad9541b1e91550a8cabaecc7b`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d111a24a972eb73f8f7928da3ce21c28424a6fd6db2041fcdf541808cef53742`  
		Last Modified: Tue, 14 Dec 2021 01:42:19 GMT  
		Size: 6.7 MB (6740174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore`

```console
$ docker pull docker@sha256:aeae5d99fe3dc85006d347bcd0f0209b8350fbba00fff026ddd2927a9927bca3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `docker:20.10-windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull docker@sha256:bddeba547b89b83f3504923c518755dcefbd6d6af21e3b880b342c9fd632a75d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2759710145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c7db75db2732a0bbca809e17a72de80fae5ff7722bdce5cbc4b7f34dfaeb01`
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
# Tue, 14 Dec 2021 01:14:53 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:14:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.12.zip
# Tue, 14 Dec 2021 01:16:12 GMT
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
	-	`sha256:e2dca1c227843d13b5eed8f547ee009f1c0a3f31cee57cd0478d6a5187c0565c`  
		Last Modified: Tue, 14 Dec 2021 01:16:37 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be433795619099d6fd71321a47a80e03c2c381ae57b9d90b92b45627ff7f6d96`  
		Last Modified: Tue, 14 Dec 2021 01:16:37 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66d67f0ea287b8dd2ba1e3a70e2ce53cce0b193f44a01bdc569ed2688465f5a`  
		Last Modified: Tue, 14 Dec 2021 01:16:48 GMT  
		Size: 53.2 MB (53228223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-1809`

```console
$ docker pull docker@sha256:aeae5d99fe3dc85006d347bcd0f0209b8350fbba00fff026ddd2927a9927bca3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `docker:20.10-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull docker@sha256:bddeba547b89b83f3504923c518755dcefbd6d6af21e3b880b342c9fd632a75d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2759710145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c7db75db2732a0bbca809e17a72de80fae5ff7722bdce5cbc4b7f34dfaeb01`
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
# Tue, 14 Dec 2021 01:14:53 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:14:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.12.zip
# Tue, 14 Dec 2021 01:16:12 GMT
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
	-	`sha256:e2dca1c227843d13b5eed8f547ee009f1c0a3f31cee57cd0478d6a5187c0565c`  
		Last Modified: Tue, 14 Dec 2021 01:16:37 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be433795619099d6fd71321a47a80e03c2c381ae57b9d90b92b45627ff7f6d96`  
		Last Modified: Tue, 14 Dec 2021 01:16:37 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66d67f0ea287b8dd2ba1e3a70e2ce53cce0b193f44a01bdc569ed2688465f5a`  
		Last Modified: Tue, 14 Dec 2021 01:16:48 GMT  
		Size: 53.2 MB (53228223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.12`

```console
$ docker pull docker@sha256:7576c1354d56ada47f1e52b9f5b9f472cb4bc85e299432b5508b5661228d3104
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.12` - linux; amd64

```console
$ docker pull docker@sha256:09f8748c248001840cdb2a0ce93ccc3e20100a910e51158d3f74e708ad899f73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68480564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff1c1f4454a0a9a125b74d9850d4a79dd8973ff2a9ca39f9de2648b123750d4d`
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
# Tue, 14 Dec 2021 01:19:22 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:19:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:29 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:19:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:30 GMT
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
	-	`sha256:7f22bd4996264a086a8770f4f667d2fb7877b525951480e7121a1a4c3905e3a1`  
		Last Modified: Tue, 14 Dec 2021 01:20:27 GMT  
		Size: 63.7 MB (63718514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b00d1b5a23c849695e38cc1c8d7a9cca6d62f173982209441666d4c7cb25b`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6ad723338071334a09327bc602580ca713fa4ff41c9cba96b0682f9c96e752`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad69ecad074ceedac2158c71f1890d95dc421ceae190b0608170261ddad1c8fa`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.12` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:74e1492f3a3c1716347ce322bcae5838e7676eac8d0c53aa20615d7d056ee0db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62376713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3acd5d40f4879cbbb916d83836f8d66d4d60654671f2bc00f81597d31cb04771`
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
# Tue, 14 Dec 2021 01:39:30 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:39:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:39:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:39:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:39:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:40 GMT
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
	-	`sha256:efa29b56432c31c1ae3e3a198fd660fe24aad4f3c1bd2fcc41ec7bec1c86127a`  
		Last Modified: Tue, 14 Dec 2021 01:41:12 GMT  
		Size: 57.7 MB (57747212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03e69d0d3fb7491b603b26d6209129be9cc220a763e55d8f61e0f615dd67eec`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d00fe7a17c2f14d79be0e290f3f72bbfa899722f3136964137f41c55299faf0`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fdcc8ecc6967aea4440794a0fe37896acca35ad9541b1e91550a8cabaecc7b`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.12-alpine3.15`

**does not exist** (yet?)

## `docker:20.10.12-dind`

```console
$ docker pull docker@sha256:f18cb807df96d3b9d4d096ddef6c800ed7c779964ea723d02b32b6fe2cee3e0a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.12-dind` - linux; amd64

```console
$ docker pull docker@sha256:9deffd6a4e57534f4a01eef1ac10a6017a301ec698e79603f8b8a13ab3ef33bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75008177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c15c97e82b6205f24eedbb8d68635967b13e48f8f3593083759febe9a9503a5`
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
# Tue, 14 Dec 2021 01:19:22 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:19:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:29 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:19:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:30 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:19:36 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 14 Dec 2021 01:19:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:19:37 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 14 Dec 2021 01:19:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 14 Dec 2021 01:19:39 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:39 GMT
VOLUME [/var/lib/docker]
# Tue, 14 Dec 2021 01:19:39 GMT
EXPOSE 2375 2376
# Tue, 14 Dec 2021 01:19:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:39 GMT
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
	-	`sha256:7f22bd4996264a086a8770f4f667d2fb7877b525951480e7121a1a4c3905e3a1`  
		Last Modified: Tue, 14 Dec 2021 01:20:27 GMT  
		Size: 63.7 MB (63718514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b00d1b5a23c849695e38cc1c8d7a9cca6d62f173982209441666d4c7cb25b`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6ad723338071334a09327bc602580ca713fa4ff41c9cba96b0682f9c96e752`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad69ecad074ceedac2158c71f1890d95dc421ceae190b0608170261ddad1c8fa`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f042b35272e657c8969916691d9d1bba7ae8851dc915f76b2c506e8a29c543df`  
		Last Modified: Tue, 14 Dec 2021 01:20:47 GMT  
		Size: 6.5 MB (6522717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc27002d71f82e23a7ff61b4b6a82e9e38226da406833f6addc45a85322ec39`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f75dc2db7d9c3b72573b7b542f56b99b99c33ef1318dfd7fd7052cb9e0e8c7`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd05b7cec7a24208dfc6bc6b1fd6d12fcbb6952bcea5d42b60ad5b3acf4f1211`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.12-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:36774fd5f0e105eaecea48094276b7c9553d87607d0409c57b8af57cf5aba8c7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68799974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbc79ed4af04a8cad8cec4f9176dbcb26b12c6c71e2d249aae088a3acdc7500a`
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
# Tue, 14 Dec 2021 01:39:30 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:39:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:39:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:39:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:39:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:40 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:39:50 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 14 Dec 2021 01:39:51 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:39:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 14 Dec 2021 01:39:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 14 Dec 2021 01:39:55 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:55 GMT
VOLUME [/var/lib/docker]
# Tue, 14 Dec 2021 01:39:56 GMT
EXPOSE 2375 2376
# Tue, 14 Dec 2021 01:39:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:58 GMT
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
	-	`sha256:efa29b56432c31c1ae3e3a198fd660fe24aad4f3c1bd2fcc41ec7bec1c86127a`  
		Last Modified: Tue, 14 Dec 2021 01:41:12 GMT  
		Size: 57.7 MB (57747212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03e69d0d3fb7491b603b26d6209129be9cc220a763e55d8f61e0f615dd67eec`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d00fe7a17c2f14d79be0e290f3f72bbfa899722f3136964137f41c55299faf0`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fdcc8ecc6967aea4440794a0fe37896acca35ad9541b1e91550a8cabaecc7b`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6139c50bbab98e9bb1d1aa2396b4c1e18b2861015efe52da5cbd4660705e38`  
		Last Modified: Tue, 14 Dec 2021 01:41:33 GMT  
		Size: 6.4 MB (6418394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36036b817024bbc3edcaff34d3688363c0659efe28a2ae890783ea074bc121e2`  
		Last Modified: Tue, 14 Dec 2021 01:41:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923c1073ccef6aa80d889d9bb29d6ad6226a6c76e4d8425233d62af225d270b0`  
		Last Modified: Tue, 14 Dec 2021 01:41:33 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e05effd75ccd7827a2c37694bc29f407143b4b4ffdb8ef6b0a7a9205aead834`  
		Last Modified: Tue, 14 Dec 2021 01:41:32 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.12-dind-alpine3.15`

**does not exist** (yet?)

## `docker:20.10.12-dind-rootless`

```console
$ docker pull docker@sha256:01b992491884cd0dca76675926097d3534b00f5ee9e60cfd195c5e4a764a4534
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.12-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:5e9deaaf38b027b5a5f033c548da2296ec0429bd21d3db137069e7a3add1712c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95290953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43c1e14ca17cb3d66246538810f34e4df5854eced27d3bb833f453db0cb53e6c`
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
# Tue, 14 Dec 2021 01:19:22 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:19:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:29 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:19:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:30 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:19:36 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 14 Dec 2021 01:19:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:19:37 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 14 Dec 2021 01:19:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 14 Dec 2021 01:19:39 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:39 GMT
VOLUME [/var/lib/docker]
# Tue, 14 Dec 2021 01:19:39 GMT
EXPOSE 2375 2376
# Tue, 14 Dec 2021 01:19:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:39 GMT
CMD []
# Tue, 14 Dec 2021 01:19:43 GMT
RUN apk add --no-cache iproute2
# Tue, 14 Dec 2021 01:19:44 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 14 Dec 2021 01:19:45 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:19:47 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 14 Dec 2021 01:19:48 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 14 Dec 2021 01:19:48 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 14 Dec 2021 01:19:48 GMT
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
	-	`sha256:7f22bd4996264a086a8770f4f667d2fb7877b525951480e7121a1a4c3905e3a1`  
		Last Modified: Tue, 14 Dec 2021 01:20:27 GMT  
		Size: 63.7 MB (63718514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b00d1b5a23c849695e38cc1c8d7a9cca6d62f173982209441666d4c7cb25b`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6ad723338071334a09327bc602580ca713fa4ff41c9cba96b0682f9c96e752`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad69ecad074ceedac2158c71f1890d95dc421ceae190b0608170261ddad1c8fa`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f042b35272e657c8969916691d9d1bba7ae8851dc915f76b2c506e8a29c543df`  
		Last Modified: Tue, 14 Dec 2021 01:20:47 GMT  
		Size: 6.5 MB (6522717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc27002d71f82e23a7ff61b4b6a82e9e38226da406833f6addc45a85322ec39`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f75dc2db7d9c3b72573b7b542f56b99b99c33ef1318dfd7fd7052cb9e0e8c7`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd05b7cec7a24208dfc6bc6b1fd6d12fcbb6952bcea5d42b60ad5b3acf4f1211`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895786101537dd46ede9b73a7e9aeda41de46cd664d0bc7372d98337de961ab3`  
		Last Modified: Tue, 14 Dec 2021 01:21:07 GMT  
		Size: 1.1 MB (1149119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3069ef522e1061f2cf66d656ed079481ea603e6cd482656f4c1d4f89b87677a`  
		Last Modified: Tue, 14 Dec 2021 01:21:07 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd05514682855814f146fd143e50fccb168ba0211450583daaba94900dc2032f`  
		Last Modified: Tue, 14 Dec 2021 01:21:07 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a912066e38c030b9897a347cc9dffb6f3df2ce002b7b9eeec1d6dff74e8ba275`  
		Last Modified: Tue, 14 Dec 2021 01:21:10 GMT  
		Size: 19.1 MB (19131942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfc994d0a45d0f7ccc0175ae21d2c32b2d70e0e1ac2f05fb7d9e6f60ae37de1`  
		Last Modified: Tue, 14 Dec 2021 01:21:07 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.12-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:d8cbc56394ae3dcb2152c14f1abb85a50262b05a02ca6db21a8f566c60a2c151
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91075410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e14b610229d453c957535c435f52080c651f1dd2f59919d9051c4e695a1dd16`
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
# Tue, 14 Dec 2021 01:39:30 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:39:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:39:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:39:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:39:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:40 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:39:50 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 14 Dec 2021 01:39:51 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:39:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 14 Dec 2021 01:39:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 14 Dec 2021 01:39:55 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:55 GMT
VOLUME [/var/lib/docker]
# Tue, 14 Dec 2021 01:39:56 GMT
EXPOSE 2375 2376
# Tue, 14 Dec 2021 01:39:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:58 GMT
CMD []
# Tue, 14 Dec 2021 01:40:06 GMT
RUN apk add --no-cache iproute2
# Tue, 14 Dec 2021 01:40:07 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 14 Dec 2021 01:40:08 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:40:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 14 Dec 2021 01:40:12 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 14 Dec 2021 01:40:13 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 14 Dec 2021 01:40:14 GMT
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
	-	`sha256:efa29b56432c31c1ae3e3a198fd660fe24aad4f3c1bd2fcc41ec7bec1c86127a`  
		Last Modified: Tue, 14 Dec 2021 01:41:12 GMT  
		Size: 57.7 MB (57747212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03e69d0d3fb7491b603b26d6209129be9cc220a763e55d8f61e0f615dd67eec`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d00fe7a17c2f14d79be0e290f3f72bbfa899722f3136964137f41c55299faf0`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fdcc8ecc6967aea4440794a0fe37896acca35ad9541b1e91550a8cabaecc7b`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6139c50bbab98e9bb1d1aa2396b4c1e18b2861015efe52da5cbd4660705e38`  
		Last Modified: Tue, 14 Dec 2021 01:41:33 GMT  
		Size: 6.4 MB (6418394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36036b817024bbc3edcaff34d3688363c0659efe28a2ae890783ea074bc121e2`  
		Last Modified: Tue, 14 Dec 2021 01:41:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923c1073ccef6aa80d889d9bb29d6ad6226a6c76e4d8425233d62af225d270b0`  
		Last Modified: Tue, 14 Dec 2021 01:41:33 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e05effd75ccd7827a2c37694bc29f407143b4b4ffdb8ef6b0a7a9205aead834`  
		Last Modified: Tue, 14 Dec 2021 01:41:32 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e512c70c3e7c936e32ce6b40f81a8b1fe652a867b1052540fce9d592b8d57c2`  
		Last Modified: Tue, 14 Dec 2021 01:41:55 GMT  
		Size: 1.2 MB (1168597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f629c942ca98a178333071f9e485fd5fc62c9f95f3eaf124dfa919ecd59b06`  
		Last Modified: Tue, 14 Dec 2021 01:41:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac41d51e834ca86a8b9f559608abda6fbb9a25d331a91ca14351a54c0072ea7`  
		Last Modified: Tue, 14 Dec 2021 01:41:55 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f721865855552d187017d6a733b602cc288bb0f67e75e786d42975c2f96b1ae`  
		Last Modified: Tue, 14 Dec 2021 01:41:58 GMT  
		Size: 21.1 MB (21105216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad8303f5f8549cce863da24719c3251898d720cdbe18479d95f2f06bde15606`  
		Last Modified: Tue, 14 Dec 2021 01:41:55 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.12-git`

```console
$ docker pull docker@sha256:20ca38ca6e5f9b2389b832053e090ff5160120c7b2365326599a1b1f55bd935a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.12-git` - linux; amd64

```console
$ docker pull docker@sha256:5e0b8727e8f439bfeb7cc9ece341e1627b38475aea43aeb78bdf7f1ce78b4d00
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75111302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e508e51d27b39da3d198527a2fe2eb1020b4c4a22186a889f5b08ebcd0a8ba73`
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
# Tue, 14 Dec 2021 01:19:22 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:19:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:29 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:19:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:30 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:19:52 GMT
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
	-	`sha256:7f22bd4996264a086a8770f4f667d2fb7877b525951480e7121a1a4c3905e3a1`  
		Last Modified: Tue, 14 Dec 2021 01:20:27 GMT  
		Size: 63.7 MB (63718514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b00d1b5a23c849695e38cc1c8d7a9cca6d62f173982209441666d4c7cb25b`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6ad723338071334a09327bc602580ca713fa4ff41c9cba96b0682f9c96e752`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad69ecad074ceedac2158c71f1890d95dc421ceae190b0608170261ddad1c8fa`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90cf0bd28b7a98109de7f7f39709740eccdb39470fc6df3d5ef6e47b77d6862`  
		Last Modified: Tue, 14 Dec 2021 01:21:34 GMT  
		Size: 6.6 MB (6630738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.12-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:fc0c35f685a42162c84f28e67392a2df8d905dcf8c266bd75623c50a2efc62e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69116887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfa2d5809f71991954f14c210580ffe0abac8bcc10dbabae3265ca6bf8356cd1`
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
# Tue, 14 Dec 2021 01:39:30 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:39:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:39:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:39:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:39:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:40 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:40:22 GMT
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
	-	`sha256:efa29b56432c31c1ae3e3a198fd660fe24aad4f3c1bd2fcc41ec7bec1c86127a`  
		Last Modified: Tue, 14 Dec 2021 01:41:12 GMT  
		Size: 57.7 MB (57747212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03e69d0d3fb7491b603b26d6209129be9cc220a763e55d8f61e0f615dd67eec`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d00fe7a17c2f14d79be0e290f3f72bbfa899722f3136964137f41c55299faf0`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fdcc8ecc6967aea4440794a0fe37896acca35ad9541b1e91550a8cabaecc7b`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d111a24a972eb73f8f7928da3ce21c28424a6fd6db2041fcdf541808cef53742`  
		Last Modified: Tue, 14 Dec 2021 01:42:19 GMT  
		Size: 6.7 MB (6740174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.12-windowsservercore`

```console
$ docker pull docker@sha256:aeae5d99fe3dc85006d347bcd0f0209b8350fbba00fff026ddd2927a9927bca3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `docker:20.10.12-windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull docker@sha256:bddeba547b89b83f3504923c518755dcefbd6d6af21e3b880b342c9fd632a75d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2759710145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c7db75db2732a0bbca809e17a72de80fae5ff7722bdce5cbc4b7f34dfaeb01`
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
# Tue, 14 Dec 2021 01:14:53 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:14:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.12.zip
# Tue, 14 Dec 2021 01:16:12 GMT
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
	-	`sha256:e2dca1c227843d13b5eed8f547ee009f1c0a3f31cee57cd0478d6a5187c0565c`  
		Last Modified: Tue, 14 Dec 2021 01:16:37 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be433795619099d6fd71321a47a80e03c2c381ae57b9d90b92b45627ff7f6d96`  
		Last Modified: Tue, 14 Dec 2021 01:16:37 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66d67f0ea287b8dd2ba1e3a70e2ce53cce0b193f44a01bdc569ed2688465f5a`  
		Last Modified: Tue, 14 Dec 2021 01:16:48 GMT  
		Size: 53.2 MB (53228223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.12-windowsservercore-1809`

```console
$ docker pull docker@sha256:aeae5d99fe3dc85006d347bcd0f0209b8350fbba00fff026ddd2927a9927bca3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `docker:20.10.12-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull docker@sha256:bddeba547b89b83f3504923c518755dcefbd6d6af21e3b880b342c9fd632a75d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2759710145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c7db75db2732a0bbca809e17a72de80fae5ff7722bdce5cbc4b7f34dfaeb01`
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
# Tue, 14 Dec 2021 01:14:53 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:14:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.12.zip
# Tue, 14 Dec 2021 01:16:12 GMT
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
	-	`sha256:e2dca1c227843d13b5eed8f547ee009f1c0a3f31cee57cd0478d6a5187c0565c`  
		Last Modified: Tue, 14 Dec 2021 01:16:37 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be433795619099d6fd71321a47a80e03c2c381ae57b9d90b92b45627ff7f6d96`  
		Last Modified: Tue, 14 Dec 2021 01:16:37 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66d67f0ea287b8dd2ba1e3a70e2ce53cce0b193f44a01bdc569ed2688465f5a`  
		Last Modified: Tue, 14 Dec 2021 01:16:48 GMT  
		Size: 53.2 MB (53228223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:f18cb807df96d3b9d4d096ddef6c800ed7c779964ea723d02b32b6fe2cee3e0a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:9deffd6a4e57534f4a01eef1ac10a6017a301ec698e79603f8b8a13ab3ef33bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75008177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c15c97e82b6205f24eedbb8d68635967b13e48f8f3593083759febe9a9503a5`
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
# Tue, 14 Dec 2021 01:19:22 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:19:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:29 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:19:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:30 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:19:36 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 14 Dec 2021 01:19:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:19:37 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 14 Dec 2021 01:19:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 14 Dec 2021 01:19:39 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:39 GMT
VOLUME [/var/lib/docker]
# Tue, 14 Dec 2021 01:19:39 GMT
EXPOSE 2375 2376
# Tue, 14 Dec 2021 01:19:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:39 GMT
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
	-	`sha256:7f22bd4996264a086a8770f4f667d2fb7877b525951480e7121a1a4c3905e3a1`  
		Last Modified: Tue, 14 Dec 2021 01:20:27 GMT  
		Size: 63.7 MB (63718514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b00d1b5a23c849695e38cc1c8d7a9cca6d62f173982209441666d4c7cb25b`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6ad723338071334a09327bc602580ca713fa4ff41c9cba96b0682f9c96e752`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad69ecad074ceedac2158c71f1890d95dc421ceae190b0608170261ddad1c8fa`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f042b35272e657c8969916691d9d1bba7ae8851dc915f76b2c506e8a29c543df`  
		Last Modified: Tue, 14 Dec 2021 01:20:47 GMT  
		Size: 6.5 MB (6522717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc27002d71f82e23a7ff61b4b6a82e9e38226da406833f6addc45a85322ec39`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f75dc2db7d9c3b72573b7b542f56b99b99c33ef1318dfd7fd7052cb9e0e8c7`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd05b7cec7a24208dfc6bc6b1fd6d12fcbb6952bcea5d42b60ad5b3acf4f1211`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:36774fd5f0e105eaecea48094276b7c9553d87607d0409c57b8af57cf5aba8c7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68799974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbc79ed4af04a8cad8cec4f9176dbcb26b12c6c71e2d249aae088a3acdc7500a`
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
# Tue, 14 Dec 2021 01:39:30 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:39:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:39:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:39:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:39:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:40 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:39:50 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 14 Dec 2021 01:39:51 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:39:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 14 Dec 2021 01:39:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 14 Dec 2021 01:39:55 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:55 GMT
VOLUME [/var/lib/docker]
# Tue, 14 Dec 2021 01:39:56 GMT
EXPOSE 2375 2376
# Tue, 14 Dec 2021 01:39:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:58 GMT
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
	-	`sha256:efa29b56432c31c1ae3e3a198fd660fe24aad4f3c1bd2fcc41ec7bec1c86127a`  
		Last Modified: Tue, 14 Dec 2021 01:41:12 GMT  
		Size: 57.7 MB (57747212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03e69d0d3fb7491b603b26d6209129be9cc220a763e55d8f61e0f615dd67eec`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d00fe7a17c2f14d79be0e290f3f72bbfa899722f3136964137f41c55299faf0`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fdcc8ecc6967aea4440794a0fe37896acca35ad9541b1e91550a8cabaecc7b`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6139c50bbab98e9bb1d1aa2396b4c1e18b2861015efe52da5cbd4660705e38`  
		Last Modified: Tue, 14 Dec 2021 01:41:33 GMT  
		Size: 6.4 MB (6418394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36036b817024bbc3edcaff34d3688363c0659efe28a2ae890783ea074bc121e2`  
		Last Modified: Tue, 14 Dec 2021 01:41:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923c1073ccef6aa80d889d9bb29d6ad6226a6c76e4d8425233d62af225d270b0`  
		Last Modified: Tue, 14 Dec 2021 01:41:33 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e05effd75ccd7827a2c37694bc29f407143b4b4ffdb8ef6b0a7a9205aead834`  
		Last Modified: Tue, 14 Dec 2021 01:41:32 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:01b992491884cd0dca76675926097d3534b00f5ee9e60cfd195c5e4a764a4534
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:5e9deaaf38b027b5a5f033c548da2296ec0429bd21d3db137069e7a3add1712c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95290953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43c1e14ca17cb3d66246538810f34e4df5854eced27d3bb833f453db0cb53e6c`
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
# Tue, 14 Dec 2021 01:19:22 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:19:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:29 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:19:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:30 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:19:36 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 14 Dec 2021 01:19:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:19:37 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 14 Dec 2021 01:19:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 14 Dec 2021 01:19:39 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:39 GMT
VOLUME [/var/lib/docker]
# Tue, 14 Dec 2021 01:19:39 GMT
EXPOSE 2375 2376
# Tue, 14 Dec 2021 01:19:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:39 GMT
CMD []
# Tue, 14 Dec 2021 01:19:43 GMT
RUN apk add --no-cache iproute2
# Tue, 14 Dec 2021 01:19:44 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 14 Dec 2021 01:19:45 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:19:47 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 14 Dec 2021 01:19:48 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 14 Dec 2021 01:19:48 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 14 Dec 2021 01:19:48 GMT
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
	-	`sha256:7f22bd4996264a086a8770f4f667d2fb7877b525951480e7121a1a4c3905e3a1`  
		Last Modified: Tue, 14 Dec 2021 01:20:27 GMT  
		Size: 63.7 MB (63718514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b00d1b5a23c849695e38cc1c8d7a9cca6d62f173982209441666d4c7cb25b`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6ad723338071334a09327bc602580ca713fa4ff41c9cba96b0682f9c96e752`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad69ecad074ceedac2158c71f1890d95dc421ceae190b0608170261ddad1c8fa`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f042b35272e657c8969916691d9d1bba7ae8851dc915f76b2c506e8a29c543df`  
		Last Modified: Tue, 14 Dec 2021 01:20:47 GMT  
		Size: 6.5 MB (6522717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc27002d71f82e23a7ff61b4b6a82e9e38226da406833f6addc45a85322ec39`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f75dc2db7d9c3b72573b7b542f56b99b99c33ef1318dfd7fd7052cb9e0e8c7`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd05b7cec7a24208dfc6bc6b1fd6d12fcbb6952bcea5d42b60ad5b3acf4f1211`  
		Last Modified: Tue, 14 Dec 2021 01:20:46 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895786101537dd46ede9b73a7e9aeda41de46cd664d0bc7372d98337de961ab3`  
		Last Modified: Tue, 14 Dec 2021 01:21:07 GMT  
		Size: 1.1 MB (1149119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3069ef522e1061f2cf66d656ed079481ea603e6cd482656f4c1d4f89b87677a`  
		Last Modified: Tue, 14 Dec 2021 01:21:07 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd05514682855814f146fd143e50fccb168ba0211450583daaba94900dc2032f`  
		Last Modified: Tue, 14 Dec 2021 01:21:07 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a912066e38c030b9897a347cc9dffb6f3df2ce002b7b9eeec1d6dff74e8ba275`  
		Last Modified: Tue, 14 Dec 2021 01:21:10 GMT  
		Size: 19.1 MB (19131942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfc994d0a45d0f7ccc0175ae21d2c32b2d70e0e1ac2f05fb7d9e6f60ae37de1`  
		Last Modified: Tue, 14 Dec 2021 01:21:07 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:d8cbc56394ae3dcb2152c14f1abb85a50262b05a02ca6db21a8f566c60a2c151
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91075410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e14b610229d453c957535c435f52080c651f1dd2f59919d9051c4e695a1dd16`
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
# Tue, 14 Dec 2021 01:39:30 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:39:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:39:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:39:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:39:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:40 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:39:50 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 14 Dec 2021 01:39:51 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:39:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 14 Dec 2021 01:39:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 14 Dec 2021 01:39:55 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:55 GMT
VOLUME [/var/lib/docker]
# Tue, 14 Dec 2021 01:39:56 GMT
EXPOSE 2375 2376
# Tue, 14 Dec 2021 01:39:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:58 GMT
CMD []
# Tue, 14 Dec 2021 01:40:06 GMT
RUN apk add --no-cache iproute2
# Tue, 14 Dec 2021 01:40:07 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 14 Dec 2021 01:40:08 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 14 Dec 2021 01:40:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 14 Dec 2021 01:40:12 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 14 Dec 2021 01:40:13 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 14 Dec 2021 01:40:14 GMT
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
	-	`sha256:efa29b56432c31c1ae3e3a198fd660fe24aad4f3c1bd2fcc41ec7bec1c86127a`  
		Last Modified: Tue, 14 Dec 2021 01:41:12 GMT  
		Size: 57.7 MB (57747212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03e69d0d3fb7491b603b26d6209129be9cc220a763e55d8f61e0f615dd67eec`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d00fe7a17c2f14d79be0e290f3f72bbfa899722f3136964137f41c55299faf0`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fdcc8ecc6967aea4440794a0fe37896acca35ad9541b1e91550a8cabaecc7b`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6139c50bbab98e9bb1d1aa2396b4c1e18b2861015efe52da5cbd4660705e38`  
		Last Modified: Tue, 14 Dec 2021 01:41:33 GMT  
		Size: 6.4 MB (6418394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36036b817024bbc3edcaff34d3688363c0659efe28a2ae890783ea074bc121e2`  
		Last Modified: Tue, 14 Dec 2021 01:41:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923c1073ccef6aa80d889d9bb29d6ad6226a6c76e4d8425233d62af225d270b0`  
		Last Modified: Tue, 14 Dec 2021 01:41:33 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e05effd75ccd7827a2c37694bc29f407143b4b4ffdb8ef6b0a7a9205aead834`  
		Last Modified: Tue, 14 Dec 2021 01:41:32 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e512c70c3e7c936e32ce6b40f81a8b1fe652a867b1052540fce9d592b8d57c2`  
		Last Modified: Tue, 14 Dec 2021 01:41:55 GMT  
		Size: 1.2 MB (1168597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f629c942ca98a178333071f9e485fd5fc62c9f95f3eaf124dfa919ecd59b06`  
		Last Modified: Tue, 14 Dec 2021 01:41:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac41d51e834ca86a8b9f559608abda6fbb9a25d331a91ca14351a54c0072ea7`  
		Last Modified: Tue, 14 Dec 2021 01:41:55 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f721865855552d187017d6a733b602cc288bb0f67e75e786d42975c2f96b1ae`  
		Last Modified: Tue, 14 Dec 2021 01:41:58 GMT  
		Size: 21.1 MB (21105216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad8303f5f8549cce863da24719c3251898d720cdbe18479d95f2f06bde15606`  
		Last Modified: Tue, 14 Dec 2021 01:41:55 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:20ca38ca6e5f9b2389b832053e090ff5160120c7b2365326599a1b1f55bd935a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:5e0b8727e8f439bfeb7cc9ece341e1627b38475aea43aeb78bdf7f1ce78b4d00
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75111302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e508e51d27b39da3d198527a2fe2eb1020b4c4a22186a889f5b08ebcd0a8ba73`
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
# Tue, 14 Dec 2021 01:19:22 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:19:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:29 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:19:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:30 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:19:52 GMT
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
	-	`sha256:7f22bd4996264a086a8770f4f667d2fb7877b525951480e7121a1a4c3905e3a1`  
		Last Modified: Tue, 14 Dec 2021 01:20:27 GMT  
		Size: 63.7 MB (63718514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b00d1b5a23c849695e38cc1c8d7a9cca6d62f173982209441666d4c7cb25b`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6ad723338071334a09327bc602580ca713fa4ff41c9cba96b0682f9c96e752`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad69ecad074ceedac2158c71f1890d95dc421ceae190b0608170261ddad1c8fa`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90cf0bd28b7a98109de7f7f39709740eccdb39470fc6df3d5ef6e47b77d6862`  
		Last Modified: Tue, 14 Dec 2021 01:21:34 GMT  
		Size: 6.6 MB (6630738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:fc0c35f685a42162c84f28e67392a2df8d905dcf8c266bd75623c50a2efc62e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69116887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfa2d5809f71991954f14c210580ffe0abac8bcc10dbabae3265ca6bf8356cd1`
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
# Tue, 14 Dec 2021 01:39:30 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:39:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:39:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:39:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:39:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:40 GMT
CMD ["sh"]
# Tue, 14 Dec 2021 01:40:22 GMT
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
	-	`sha256:efa29b56432c31c1ae3e3a198fd660fe24aad4f3c1bd2fcc41ec7bec1c86127a`  
		Last Modified: Tue, 14 Dec 2021 01:41:12 GMT  
		Size: 57.7 MB (57747212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03e69d0d3fb7491b603b26d6209129be9cc220a763e55d8f61e0f615dd67eec`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d00fe7a17c2f14d79be0e290f3f72bbfa899722f3136964137f41c55299faf0`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fdcc8ecc6967aea4440794a0fe37896acca35ad9541b1e91550a8cabaecc7b`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d111a24a972eb73f8f7928da3ce21c28424a6fd6db2041fcdf541808cef53742`  
		Last Modified: Tue, 14 Dec 2021 01:42:19 GMT  
		Size: 6.7 MB (6740174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:7576c1354d56ada47f1e52b9f5b9f472cb4bc85e299432b5508b5661228d3104
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:09f8748c248001840cdb2a0ce93ccc3e20100a910e51158d3f74e708ad899f73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68480564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff1c1f4454a0a9a125b74d9850d4a79dd8973ff2a9ca39f9de2648b123750d4d`
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
# Tue, 14 Dec 2021 01:19:22 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:19:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:19:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:19:29 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:19:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:19:30 GMT
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
	-	`sha256:7f22bd4996264a086a8770f4f667d2fb7877b525951480e7121a1a4c3905e3a1`  
		Last Modified: Tue, 14 Dec 2021 01:20:27 GMT  
		Size: 63.7 MB (63718514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b00d1b5a23c849695e38cc1c8d7a9cca6d62f173982209441666d4c7cb25b`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6ad723338071334a09327bc602580ca713fa4ff41c9cba96b0682f9c96e752`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad69ecad074ceedac2158c71f1890d95dc421ceae190b0608170261ddad1c8fa`  
		Last Modified: Tue, 14 Dec 2021 01:20:16 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:74e1492f3a3c1716347ce322bcae5838e7676eac8d0c53aa20615d7d056ee0db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62376713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3acd5d40f4879cbbb916d83836f8d66d4d60654671f2bc00f81597d31cb04771`
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
# Tue, 14 Dec 2021 01:39:30 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:39:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 14 Dec 2021 01:39:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 14 Dec 2021 01:39:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 14 Dec 2021 01:39:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 14 Dec 2021 01:39:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 14 Dec 2021 01:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 01:39:40 GMT
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
	-	`sha256:efa29b56432c31c1ae3e3a198fd660fe24aad4f3c1bd2fcc41ec7bec1c86127a`  
		Last Modified: Tue, 14 Dec 2021 01:41:12 GMT  
		Size: 57.7 MB (57747212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03e69d0d3fb7491b603b26d6209129be9cc220a763e55d8f61e0f615dd67eec`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d00fe7a17c2f14d79be0e290f3f72bbfa899722f3136964137f41c55299faf0`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fdcc8ecc6967aea4440794a0fe37896acca35ad9541b1e91550a8cabaecc7b`  
		Last Modified: Tue, 14 Dec 2021 01:41:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore`

```console
$ docker pull docker@sha256:aeae5d99fe3dc85006d347bcd0f0209b8350fbba00fff026ddd2927a9927bca3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `docker:windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull docker@sha256:bddeba547b89b83f3504923c518755dcefbd6d6af21e3b880b342c9fd632a75d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2759710145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c7db75db2732a0bbca809e17a72de80fae5ff7722bdce5cbc4b7f34dfaeb01`
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
# Tue, 14 Dec 2021 01:14:53 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:14:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.12.zip
# Tue, 14 Dec 2021 01:16:12 GMT
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
	-	`sha256:e2dca1c227843d13b5eed8f547ee009f1c0a3f31cee57cd0478d6a5187c0565c`  
		Last Modified: Tue, 14 Dec 2021 01:16:37 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be433795619099d6fd71321a47a80e03c2c381ae57b9d90b92b45627ff7f6d96`  
		Last Modified: Tue, 14 Dec 2021 01:16:37 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66d67f0ea287b8dd2ba1e3a70e2ce53cce0b193f44a01bdc569ed2688465f5a`  
		Last Modified: Tue, 14 Dec 2021 01:16:48 GMT  
		Size: 53.2 MB (53228223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:aeae5d99fe3dc85006d347bcd0f0209b8350fbba00fff026ddd2927a9927bca3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull docker@sha256:bddeba547b89b83f3504923c518755dcefbd6d6af21e3b880b342c9fd632a75d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2759710145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c7db75db2732a0bbca809e17a72de80fae5ff7722bdce5cbc4b7f34dfaeb01`
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
# Tue, 14 Dec 2021 01:14:53 GMT
ENV DOCKER_VERSION=20.10.12
# Tue, 14 Dec 2021 01:14:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.12.zip
# Tue, 14 Dec 2021 01:16:12 GMT
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
	-	`sha256:e2dca1c227843d13b5eed8f547ee009f1c0a3f31cee57cd0478d6a5187c0565c`  
		Last Modified: Tue, 14 Dec 2021 01:16:37 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be433795619099d6fd71321a47a80e03c2c381ae57b9d90b92b45627ff7f6d96`  
		Last Modified: Tue, 14 Dec 2021 01:16:37 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66d67f0ea287b8dd2ba1e3a70e2ce53cce0b193f44a01bdc569ed2688465f5a`  
		Last Modified: Tue, 14 Dec 2021 01:16:48 GMT  
		Size: 53.2 MB (53228223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
