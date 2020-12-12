<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `docker`

-	[`docker:19`](#docker19)
-	[`docker:19.03`](#docker1903)
-	[`docker:19.03.14`](#docker190314)
-	[`docker:19.03.14-dind`](#docker190314-dind)
-	[`docker:19.03.14-dind-rootless`](#docker190314-dind-rootless)
-	[`docker:19.03.14-git`](#docker190314-git)
-	[`docker:19.03-dind`](#docker1903-dind)
-	[`docker:19.03-dind-rootless`](#docker1903-dind-rootless)
-	[`docker:19.03-git`](#docker1903-git)
-	[`docker:19-dind`](#docker19-dind)
-	[`docker:19-dind-rootless`](#docker19-dind-rootless)
-	[`docker:19-git`](#docker19-git)
-	[`docker:20`](#docker20)
-	[`docker:20.10`](#docker2010)
-	[`docker:20.10.0`](#docker20100)
-	[`docker:20.10.0-dind`](#docker20100-dind)
-	[`docker:20.10.0-dind-rootless`](#docker20100-dind-rootless)
-	[`docker:20.10.0-git`](#docker20100-git)
-	[`docker:20.10-dind`](#docker2010-dind)
-	[`docker:20.10-dind-rootless`](#docker2010-dind-rootless)
-	[`docker:20.10-git`](#docker2010-git)
-	[`docker:20-dind`](#docker20-dind)
-	[`docker:20-dind-rootless`](#docker20-dind-rootless)
-	[`docker:20-git`](#docker20-git)
-	[`docker:dind`](#dockerdind)
-	[`docker:dind-rootless`](#dockerdind-rootless)
-	[`docker:git`](#dockergit)
-	[`docker:latest`](#dockerlatest)

## `docker:19`

```console
$ docker pull docker@sha256:5e79065f99d94d4b75d7fcfd870973d65860db5635a32d4dfff50b9e07c97d2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19` - linux; amd64

```console
$ docker pull docker@sha256:91d69c044e7fb58727751d735a8b1ec4d4e94a20ed0922af5103b7f098b7122f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67728526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52cb15f6b716bd4b2763e2fa701707675774ff5e92d9959b952270e61abc2ad2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:30:20 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 05:30:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:30:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:30:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:30:27 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:30:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:30:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:30:28 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70334c77c8527b221cde2e0e99359cce5c9cb5457b65a88e8de902f18fa993cb`  
		Last Modified: Fri, 11 Dec 2020 05:32:42 GMT  
		Size: 62.9 MB (62890703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa7fdb08ac5140b5cd81c000edc16d1acbb3c78b722d1b15ac81a866cf6de0d`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f150ffb925c000212dfa35dbdfeef8ea564438f2e6d7fe1bfa9eb4fda29378d8`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5098a8250e99dce60ef1d8768af0300a6f0445ea10caf4e2eebf3ce5ed75a848`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19` - linux; arm variant v6

```console
$ docker pull docker@sha256:18d39b6848cecae067cc0d94c554029bfc88d3069c80bb5049d54da659249b94
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64475654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3106fcafb44a465ee4e0efadc103e5018d57587bd5d5ba6f465846bf7c3844`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:12:47 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 23 Apr 2020 17:12:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 17:12:50 GMT
ENV DOCKER_CHANNEL=stable
# Thu, 23 Apr 2020 17:12:51 GMT
ENV DOCKER_VERSION=19.03.8
# Thu, 23 Apr 2020 17:13:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 23 Apr 2020 17:13:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 23 Apr 2020 17:13:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:13:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 23 Apr 2020 17:13:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 23 Apr 2020 17:13:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 17:13:07 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcb342235c0ef85c7b7836ba057f513df540f983f4dbe5587035824aec248ab`  
		Last Modified: Thu, 23 Apr 2020 17:14:04 GMT  
		Size: 1.9 MB (1926703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94018ec82f0af1c26efba50dc99b07f2db1d2fbfab94f814ca9e1b5147c73e56`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593e1c01de3a8ad095d83439f0112c9a534fe764682e7a0f99d0a5794f914591`  
		Last Modified: Thu, 23 Apr 2020 17:14:22 GMT  
		Size: 59.9 MB (59927152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3737124780efb66a0753c8acdb04e12dad9a04b3362b1496cfe1e1dcf2d60b`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a76f66eab7a2e5314dd5973bcbb4ab91a025072e77fd14a83ab87d5ed8cc39`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e1037ca5d5c489e9b1a5f1433e4d8be4b012c29ef660e05769c63bfbd63812`  
		Last Modified: Thu, 23 Apr 2020 17:14:02 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19` - linux; arm variant v7

```console
$ docker pull docker@sha256:ce46ea18798c578f8923e0ced4c9996c30363fc35edd1b1c40e5e542407818ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64173697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81a685736103d7a1e988f52fb20b130a353e545dff4ccd52c9b075d5ead6f11d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:03:44 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 24 Apr 2020 02:03:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 02:03:47 GMT
ENV DOCKER_CHANNEL=stable
# Fri, 24 Apr 2020 02:03:48 GMT
ENV DOCKER_VERSION=19.03.8
# Fri, 24 Apr 2020 02:03:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 24 Apr 2020 02:04:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 24 Apr 2020 02:04:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 24 Apr 2020 02:04:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 24 Apr 2020 02:04:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 24 Apr 2020 02:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 02:04:05 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c2ce1bf627500ac9aec72c466865536bbff375e04a4e409655bbdf2827c1a`  
		Last Modified: Fri, 24 Apr 2020 02:04:53 GMT  
		Size: 1.8 MB (1822716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14a8989d4305a13a6c1fbfab29671cacd99035dd4291710ba978fd29283481`  
		Last Modified: Fri, 24 Apr 2020 02:04:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0b1f8e9eedb57e967305efe997babe0185ba6f7fe9eb7f4cbed6ee3d3f4dbe`  
		Last Modified: Fri, 24 Apr 2020 02:05:12 GMT  
		Size: 59.9 MB (59927054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc59092f5c3af9ff086a7203470a39d43b9ba5593cdd2eb494796a245ce8ecd4`  
		Last Modified: Fri, 24 Apr 2020 02:04:52 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f54a6c116900f095c4bce429f827a4dcc0af52c0634e42b3f83a9f5ea321d39`  
		Last Modified: Fri, 24 Apr 2020 02:04:51 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb98a21ac35e0dd075007407e66183792d9dbc8c997513d6592918018b5312a`  
		Last Modified: Fri, 24 Apr 2020 02:04:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8eb49538a5ae25e1dcee16953ef182cf19d8c9d117300173ede2b7d88f173bbb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60762670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:354327cb1b46abd394f47d0bd564e5018f821a33e8edfadce8114b879d30f9f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:43:16 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 03:43:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:43:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:43:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:43:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:43:31 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:43:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:43:33 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44406ea375713a15815e70d9f67caccd9d24e3edb888eb33765a7855947a57dd`  
		Last Modified: Fri, 11 Dec 2020 03:46:07 GMT  
		Size: 56.0 MB (55992945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da9e082087083b4fa5ee2804222088c41668d42a3cda42a0358add93cfbfed2`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd11a145516582d37d1ac882ec6ced4d65ad928b3f5923c73b16211995c42da6`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961068b01d86e33d4e09c9fa6829e3ff7bdb7d3b6a60449681cdf49519058265`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03`

```console
$ docker pull docker@sha256:5e79065f99d94d4b75d7fcfd870973d65860db5635a32d4dfff50b9e07c97d2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03` - linux; amd64

```console
$ docker pull docker@sha256:91d69c044e7fb58727751d735a8b1ec4d4e94a20ed0922af5103b7f098b7122f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67728526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52cb15f6b716bd4b2763e2fa701707675774ff5e92d9959b952270e61abc2ad2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:30:20 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 05:30:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:30:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:30:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:30:27 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:30:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:30:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:30:28 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70334c77c8527b221cde2e0e99359cce5c9cb5457b65a88e8de902f18fa993cb`  
		Last Modified: Fri, 11 Dec 2020 05:32:42 GMT  
		Size: 62.9 MB (62890703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa7fdb08ac5140b5cd81c000edc16d1acbb3c78b722d1b15ac81a866cf6de0d`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f150ffb925c000212dfa35dbdfeef8ea564438f2e6d7fe1bfa9eb4fda29378d8`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5098a8250e99dce60ef1d8768af0300a6f0445ea10caf4e2eebf3ce5ed75a848`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03` - linux; arm variant v6

```console
$ docker pull docker@sha256:18d39b6848cecae067cc0d94c554029bfc88d3069c80bb5049d54da659249b94
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64475654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3106fcafb44a465ee4e0efadc103e5018d57587bd5d5ba6f465846bf7c3844`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:12:47 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 23 Apr 2020 17:12:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 17:12:50 GMT
ENV DOCKER_CHANNEL=stable
# Thu, 23 Apr 2020 17:12:51 GMT
ENV DOCKER_VERSION=19.03.8
# Thu, 23 Apr 2020 17:13:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 23 Apr 2020 17:13:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 23 Apr 2020 17:13:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:13:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 23 Apr 2020 17:13:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 23 Apr 2020 17:13:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 17:13:07 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcb342235c0ef85c7b7836ba057f513df540f983f4dbe5587035824aec248ab`  
		Last Modified: Thu, 23 Apr 2020 17:14:04 GMT  
		Size: 1.9 MB (1926703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94018ec82f0af1c26efba50dc99b07f2db1d2fbfab94f814ca9e1b5147c73e56`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593e1c01de3a8ad095d83439f0112c9a534fe764682e7a0f99d0a5794f914591`  
		Last Modified: Thu, 23 Apr 2020 17:14:22 GMT  
		Size: 59.9 MB (59927152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3737124780efb66a0753c8acdb04e12dad9a04b3362b1496cfe1e1dcf2d60b`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a76f66eab7a2e5314dd5973bcbb4ab91a025072e77fd14a83ab87d5ed8cc39`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e1037ca5d5c489e9b1a5f1433e4d8be4b012c29ef660e05769c63bfbd63812`  
		Last Modified: Thu, 23 Apr 2020 17:14:02 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03` - linux; arm variant v7

```console
$ docker pull docker@sha256:ce46ea18798c578f8923e0ced4c9996c30363fc35edd1b1c40e5e542407818ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64173697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81a685736103d7a1e988f52fb20b130a353e545dff4ccd52c9b075d5ead6f11d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:03:44 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 24 Apr 2020 02:03:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 02:03:47 GMT
ENV DOCKER_CHANNEL=stable
# Fri, 24 Apr 2020 02:03:48 GMT
ENV DOCKER_VERSION=19.03.8
# Fri, 24 Apr 2020 02:03:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 24 Apr 2020 02:04:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 24 Apr 2020 02:04:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 24 Apr 2020 02:04:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 24 Apr 2020 02:04:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 24 Apr 2020 02:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 02:04:05 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c2ce1bf627500ac9aec72c466865536bbff375e04a4e409655bbdf2827c1a`  
		Last Modified: Fri, 24 Apr 2020 02:04:53 GMT  
		Size: 1.8 MB (1822716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14a8989d4305a13a6c1fbfab29671cacd99035dd4291710ba978fd29283481`  
		Last Modified: Fri, 24 Apr 2020 02:04:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0b1f8e9eedb57e967305efe997babe0185ba6f7fe9eb7f4cbed6ee3d3f4dbe`  
		Last Modified: Fri, 24 Apr 2020 02:05:12 GMT  
		Size: 59.9 MB (59927054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc59092f5c3af9ff086a7203470a39d43b9ba5593cdd2eb494796a245ce8ecd4`  
		Last Modified: Fri, 24 Apr 2020 02:04:52 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f54a6c116900f095c4bce429f827a4dcc0af52c0634e42b3f83a9f5ea321d39`  
		Last Modified: Fri, 24 Apr 2020 02:04:51 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb98a21ac35e0dd075007407e66183792d9dbc8c997513d6592918018b5312a`  
		Last Modified: Fri, 24 Apr 2020 02:04:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8eb49538a5ae25e1dcee16953ef182cf19d8c9d117300173ede2b7d88f173bbb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60762670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:354327cb1b46abd394f47d0bd564e5018f821a33e8edfadce8114b879d30f9f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:43:16 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 03:43:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:43:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:43:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:43:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:43:31 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:43:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:43:33 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44406ea375713a15815e70d9f67caccd9d24e3edb888eb33765a7855947a57dd`  
		Last Modified: Fri, 11 Dec 2020 03:46:07 GMT  
		Size: 56.0 MB (55992945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da9e082087083b4fa5ee2804222088c41668d42a3cda42a0358add93cfbfed2`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd11a145516582d37d1ac882ec6ced4d65ad928b3f5923c73b16211995c42da6`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961068b01d86e33d4e09c9fa6829e3ff7bdb7d3b6a60449681cdf49519058265`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.14`

```console
$ docker pull docker@sha256:1fc8317b79cbf8c9279a0d982dce981f57582c8946c44abc113f0133cd360fe7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:19.03.14` - linux; amd64

```console
$ docker pull docker@sha256:91d69c044e7fb58727751d735a8b1ec4d4e94a20ed0922af5103b7f098b7122f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67728526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52cb15f6b716bd4b2763e2fa701707675774ff5e92d9959b952270e61abc2ad2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:30:20 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 05:30:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:30:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:30:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:30:27 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:30:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:30:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:30:28 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70334c77c8527b221cde2e0e99359cce5c9cb5457b65a88e8de902f18fa993cb`  
		Last Modified: Fri, 11 Dec 2020 05:32:42 GMT  
		Size: 62.9 MB (62890703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa7fdb08ac5140b5cd81c000edc16d1acbb3c78b722d1b15ac81a866cf6de0d`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f150ffb925c000212dfa35dbdfeef8ea564438f2e6d7fe1bfa9eb4fda29378d8`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5098a8250e99dce60ef1d8768af0300a6f0445ea10caf4e2eebf3ce5ed75a848`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.14` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8eb49538a5ae25e1dcee16953ef182cf19d8c9d117300173ede2b7d88f173bbb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60762670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:354327cb1b46abd394f47d0bd564e5018f821a33e8edfadce8114b879d30f9f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:43:16 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 03:43:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:43:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:43:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:43:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:43:31 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:43:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:43:33 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44406ea375713a15815e70d9f67caccd9d24e3edb888eb33765a7855947a57dd`  
		Last Modified: Fri, 11 Dec 2020 03:46:07 GMT  
		Size: 56.0 MB (55992945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da9e082087083b4fa5ee2804222088c41668d42a3cda42a0358add93cfbfed2`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd11a145516582d37d1ac882ec6ced4d65ad928b3f5923c73b16211995c42da6`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961068b01d86e33d4e09c9fa6829e3ff7bdb7d3b6a60449681cdf49519058265`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.14-dind`

```console
$ docker pull docker@sha256:501c77d7474b5be4817d28178b34d15450e7f68d7c29e9b5f820798d9d8d8537
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:19.03.14-dind` - linux; amd64

```console
$ docker pull docker@sha256:24b8c9c132a93ec29c3ecac861c7b2657dc565f04dfbfa40c63372dbb2d03419
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73691996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:979576cc90c025f20b83960a7f40b56030cd89d4757ec42c66dd88fb246b2e42`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:30:20 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 05:30:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:30:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:30:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:30:27 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:30:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:30:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:30:28 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:30:36 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Dec 2020 05:30:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:30:37 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 11 Dec 2020 05:30:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Dec 2020 05:30:40 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:30:40 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Dec 2020 05:30:40 GMT
EXPOSE 2375 2376
# Fri, 11 Dec 2020 05:30:40 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Dec 2020 05:30:40 GMT
CMD []
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70334c77c8527b221cde2e0e99359cce5c9cb5457b65a88e8de902f18fa993cb`  
		Last Modified: Fri, 11 Dec 2020 05:32:42 GMT  
		Size: 62.9 MB (62890703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa7fdb08ac5140b5cd81c000edc16d1acbb3c78b722d1b15ac81a866cf6de0d`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f150ffb925c000212dfa35dbdfeef8ea564438f2e6d7fe1bfa9eb4fda29378d8`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5098a8250e99dce60ef1d8768af0300a6f0445ea10caf4e2eebf3ce5ed75a848`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2416ba3463b18b0c83da91150211585ef657b5e5a4efb611846618dce5519ccb`  
		Last Modified: Fri, 11 Dec 2020 05:32:50 GMT  
		Size: 6.0 MB (5958753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc1d0e72e9ecb1fb9e0720e47b64137e3e0ab13c39535af6b17407fc0f9830`  
		Last Modified: Fri, 11 Dec 2020 05:32:49 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc0000bd7996fdaad1cd606eef1ddb78c249ed6065160d04959cb3a4e41cd34`  
		Last Modified: Fri, 11 Dec 2020 05:32:48 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a56ce7b22c289f5576aaf0f2b4244e8507be53c619319fce1585728883407c1`  
		Last Modified: Fri, 11 Dec 2020 05:32:49 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.14-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4f02c4ad7f9483dee2ebc9efe3c66633691504e4c3734fa38b657bb6beb22047
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66714139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c275ab420e15e0f0d3fe6e88b30424974332da758bf2804e204b73dc7a3ddb7`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:43:16 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 03:43:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:43:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:43:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:43:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:43:31 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:43:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:43:33 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 03:43:45 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Dec 2020 03:43:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Dec 2020 03:43:52 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 11 Dec 2020 03:43:56 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Dec 2020 03:43:58 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:43:59 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Dec 2020 03:44:01 GMT
EXPOSE 2375 2376
# Fri, 11 Dec 2020 03:44:04 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Dec 2020 03:44:05 GMT
CMD []
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44406ea375713a15815e70d9f67caccd9d24e3edb888eb33765a7855947a57dd`  
		Last Modified: Fri, 11 Dec 2020 03:46:07 GMT  
		Size: 56.0 MB (55992945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da9e082087083b4fa5ee2804222088c41668d42a3cda42a0358add93cfbfed2`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd11a145516582d37d1ac882ec6ced4d65ad928b3f5923c73b16211995c42da6`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961068b01d86e33d4e09c9fa6829e3ff7bdb7d3b6a60449681cdf49519058265`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52bcec35351af8539981ca3f0097a0d3b02517a030e2fd5e2c52cd30c72ad66`  
		Last Modified: Fri, 11 Dec 2020 03:46:19 GMT  
		Size: 5.9 MB (5946714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ba61fc8445e0471f06d03123c54a76ac7d5d292c0f9983e7021df62400b2d1`  
		Last Modified: Fri, 11 Dec 2020 03:46:19 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28426d0cbfd272b6cb9a64a8b6a1a41033edeae5823a4a809d71f5c1435d7a4`  
		Last Modified: Fri, 11 Dec 2020 03:46:17 GMT  
		Size: 933.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1827aa166b927762754e480784c7ca687bf2acf61142c2a4e9667cf203a63614`  
		Last Modified: Fri, 11 Dec 2020 03:46:18 GMT  
		Size: 2.5 KB (2512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.14-dind-rootless`

```console
$ docker pull docker@sha256:8853e15e167d7e28afc759b9d08c387de504c149f58d009b35c234e953c2328b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19.03.14-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:1fef5d7f95e2d0616a2610badc9d9fd5a6122bb75a2804fe0696ac8aecffdee4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94208960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cf71f951fc9b03cab529aeaf8e9fa85201eacb20f96e4080a649eb8f86e3b75`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:30:20 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 05:30:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:30:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:30:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:30:27 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:30:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:30:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:30:28 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:30:36 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Dec 2020 05:30:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:30:37 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 11 Dec 2020 05:30:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Dec 2020 05:30:40 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:30:40 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Dec 2020 05:30:40 GMT
EXPOSE 2375 2376
# Fri, 11 Dec 2020 05:30:40 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Dec 2020 05:30:40 GMT
CMD []
# Fri, 11 Dec 2020 05:30:46 GMT
RUN apk add --no-cache iproute2
# Fri, 11 Dec 2020 05:30:47 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 11 Dec 2020 05:30:48 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:30:50 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 11 Dec 2020 05:30:51 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 11 Dec 2020 05:30:52 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 11 Dec 2020 05:30:52 GMT
USER rootless
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70334c77c8527b221cde2e0e99359cce5c9cb5457b65a88e8de902f18fa993cb`  
		Last Modified: Fri, 11 Dec 2020 05:32:42 GMT  
		Size: 62.9 MB (62890703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa7fdb08ac5140b5cd81c000edc16d1acbb3c78b722d1b15ac81a866cf6de0d`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f150ffb925c000212dfa35dbdfeef8ea564438f2e6d7fe1bfa9eb4fda29378d8`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5098a8250e99dce60ef1d8768af0300a6f0445ea10caf4e2eebf3ce5ed75a848`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2416ba3463b18b0c83da91150211585ef657b5e5a4efb611846618dce5519ccb`  
		Last Modified: Fri, 11 Dec 2020 05:32:50 GMT  
		Size: 6.0 MB (5958753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc1d0e72e9ecb1fb9e0720e47b64137e3e0ab13c39535af6b17407fc0f9830`  
		Last Modified: Fri, 11 Dec 2020 05:32:49 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc0000bd7996fdaad1cd606eef1ddb78c249ed6065160d04959cb3a4e41cd34`  
		Last Modified: Fri, 11 Dec 2020 05:32:48 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a56ce7b22c289f5576aaf0f2b4244e8507be53c619319fce1585728883407c1`  
		Last Modified: Fri, 11 Dec 2020 05:32:49 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae09a432442ae7c3b89b670bf9046d02628a622b863e4f6ceda0935ad1e5b0ce`  
		Last Modified: Fri, 11 Dec 2020 05:32:56 GMT  
		Size: 1.1 MB (1092669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1164c9f7543f20bceba64a87c109532fb467074d62c1c9dfde4e541f0b888121`  
		Last Modified: Fri, 11 Dec 2020 05:32:56 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57070d6bdb6eb102a9060f82c30b35246a59871253dd891a749389ca3c95a0ac`  
		Last Modified: Fri, 11 Dec 2020 05:32:56 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1009bf87802d243e7e232ccc8467592825b3cd847fc06c2310908840ee557612`  
		Last Modified: Fri, 11 Dec 2020 05:33:00 GMT  
		Size: 19.4 MB (19422680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceaa992d3405cd49893b8fa63378cf828bc40c291339f12dd01bb3f8b62844cf`  
		Last Modified: Fri, 11 Dec 2020 05:32:56 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.14-git`

```console
$ docker pull docker@sha256:26ea6dd65cb0b9befffd091bb08c9cb01c2d7fe2fa10fe9a5594936283f56277
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:19.03.14-git` - linux; amd64

```console
$ docker pull docker@sha256:ee6aee276f2be958681d31282993ef964180ef559730a5e6bed76d3668d328bc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (76040639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:183e97bebf36f6cad44bc7c0dce5103bcf992d95c9de726740cdd765204c538f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:30:20 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 05:30:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:30:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:30:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:30:27 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:30:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:30:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:30:28 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:30:58 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70334c77c8527b221cde2e0e99359cce5c9cb5457b65a88e8de902f18fa993cb`  
		Last Modified: Fri, 11 Dec 2020 05:32:42 GMT  
		Size: 62.9 MB (62890703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa7fdb08ac5140b5cd81c000edc16d1acbb3c78b722d1b15ac81a866cf6de0d`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f150ffb925c000212dfa35dbdfeef8ea564438f2e6d7fe1bfa9eb4fda29378d8`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5098a8250e99dce60ef1d8768af0300a6f0445ea10caf4e2eebf3ce5ed75a848`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7db262911d375a7fb6ea2b749ae3bf51300886f5da87d6240fd06875475d1cc`  
		Last Modified: Fri, 11 Dec 2020 05:33:09 GMT  
		Size: 8.3 MB (8312113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.14-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:31c852882a88e4c35ea2f1802f10d116fccbbe7101071d921c12e15beedd4cc4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69266142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae9478277bd44d0819627464380f1048579954877b0e7645ac34d954b63ab20`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:43:16 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 03:43:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:43:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:43:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:43:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:43:31 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:43:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:43:33 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 03:44:19 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44406ea375713a15815e70d9f67caccd9d24e3edb888eb33765a7855947a57dd`  
		Last Modified: Fri, 11 Dec 2020 03:46:07 GMT  
		Size: 56.0 MB (55992945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da9e082087083b4fa5ee2804222088c41668d42a3cda42a0358add93cfbfed2`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd11a145516582d37d1ac882ec6ced4d65ad928b3f5923c73b16211995c42da6`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961068b01d86e33d4e09c9fa6829e3ff7bdb7d3b6a60449681cdf49519058265`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72293c133127a3af2438e9fdec9f0453dd61056d294aec4c7c40b00a74c2e110`  
		Last Modified: Fri, 11 Dec 2020 03:46:31 GMT  
		Size: 8.5 MB (8503472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-dind`

```console
$ docker pull docker@sha256:e26923926850691a667caba2273dc5b021ec8a883417a017ad323c35cb1f2ffa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03-dind` - linux; amd64

```console
$ docker pull docker@sha256:24b8c9c132a93ec29c3ecac861c7b2657dc565f04dfbfa40c63372dbb2d03419
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73691996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:979576cc90c025f20b83960a7f40b56030cd89d4757ec42c66dd88fb246b2e42`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:30:20 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 05:30:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:30:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:30:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:30:27 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:30:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:30:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:30:28 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:30:36 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Dec 2020 05:30:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:30:37 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 11 Dec 2020 05:30:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Dec 2020 05:30:40 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:30:40 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Dec 2020 05:30:40 GMT
EXPOSE 2375 2376
# Fri, 11 Dec 2020 05:30:40 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Dec 2020 05:30:40 GMT
CMD []
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70334c77c8527b221cde2e0e99359cce5c9cb5457b65a88e8de902f18fa993cb`  
		Last Modified: Fri, 11 Dec 2020 05:32:42 GMT  
		Size: 62.9 MB (62890703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa7fdb08ac5140b5cd81c000edc16d1acbb3c78b722d1b15ac81a866cf6de0d`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f150ffb925c000212dfa35dbdfeef8ea564438f2e6d7fe1bfa9eb4fda29378d8`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5098a8250e99dce60ef1d8768af0300a6f0445ea10caf4e2eebf3ce5ed75a848`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2416ba3463b18b0c83da91150211585ef657b5e5a4efb611846618dce5519ccb`  
		Last Modified: Fri, 11 Dec 2020 05:32:50 GMT  
		Size: 6.0 MB (5958753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc1d0e72e9ecb1fb9e0720e47b64137e3e0ab13c39535af6b17407fc0f9830`  
		Last Modified: Fri, 11 Dec 2020 05:32:49 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc0000bd7996fdaad1cd606eef1ddb78c249ed6065160d04959cb3a4e41cd34`  
		Last Modified: Fri, 11 Dec 2020 05:32:48 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a56ce7b22c289f5576aaf0f2b4244e8507be53c619319fce1585728883407c1`  
		Last Modified: Fri, 11 Dec 2020 05:32:49 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:a6b0193cbf4d3c304f3bf6c6c253d88c25a22c6ffe6847fd57a6269e4324745f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67641153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50a37c38067d51b4185a04675f81f45209b82449ce8bbbec68b31d639ba45cd5`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:12:47 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 23 Apr 2020 17:12:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 17:12:50 GMT
ENV DOCKER_CHANNEL=stable
# Thu, 23 Apr 2020 17:12:51 GMT
ENV DOCKER_VERSION=19.03.8
# Thu, 23 Apr 2020 17:13:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 23 Apr 2020 17:13:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 23 Apr 2020 17:13:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:13:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 23 Apr 2020 17:13:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 23 Apr 2020 17:13:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 17:13:07 GMT
CMD ["sh"]
# Thu, 23 Apr 2020 17:13:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 23 Apr 2020 17:13:24 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 23 Apr 2020 17:13:25 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Thu, 23 Apr 2020 17:13:29 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 06 May 2020 00:49:37 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Wed, 06 May 2020 00:49:38 GMT
VOLUME [/var/lib/docker]
# Wed, 06 May 2020 00:49:38 GMT
EXPOSE 2375 2376
# Wed, 06 May 2020 00:49:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 06 May 2020 00:49:39 GMT
CMD []
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcb342235c0ef85c7b7836ba057f513df540f983f4dbe5587035824aec248ab`  
		Last Modified: Thu, 23 Apr 2020 17:14:04 GMT  
		Size: 1.9 MB (1926703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94018ec82f0af1c26efba50dc99b07f2db1d2fbfab94f814ca9e1b5147c73e56`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593e1c01de3a8ad095d83439f0112c9a534fe764682e7a0f99d0a5794f914591`  
		Last Modified: Thu, 23 Apr 2020 17:14:22 GMT  
		Size: 59.9 MB (59927152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3737124780efb66a0753c8acdb04e12dad9a04b3362b1496cfe1e1dcf2d60b`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a76f66eab7a2e5314dd5973bcbb4ab91a025072e77fd14a83ab87d5ed8cc39`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e1037ca5d5c489e9b1a5f1433e4d8be4b012c29ef660e05769c63bfbd63812`  
		Last Modified: Thu, 23 Apr 2020 17:14:02 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0227df4100f67814d05f04e139a5e9dca37299fd9d096c7574e16fe632211d4`  
		Last Modified: Thu, 23 Apr 2020 17:14:37 GMT  
		Size: 3.2 MB (3160940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a2483e804c9900710b0cfa9c5cad284336a14d95ec28dc1049dc1b3cc10de4`  
		Last Modified: Thu, 23 Apr 2020 17:14:36 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e906e300d3ad75b25c6513f466d68c5a2dc89ce9663dd6526821b9994ceef549`  
		Last Modified: Thu, 23 Apr 2020 17:14:36 GMT  
		Size: 753.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1dd819080e27b055eaa67e449dc1475fa02b89c7eb8406d4fd558c817df9ea`  
		Last Modified: Wed, 06 May 2020 00:50:04 GMT  
		Size: 2.5 KB (2501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:f998921d365053bf7e3f98794f6c23ca44e6809832d78105bc4d2da6bb8521ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67003102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e220c6648aa1a61c12d4f11dd3c99b4385828e8c4d9823a5656f4f40294c1d41`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:03:44 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 24 Apr 2020 02:03:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 02:03:47 GMT
ENV DOCKER_CHANNEL=stable
# Fri, 24 Apr 2020 02:03:48 GMT
ENV DOCKER_VERSION=19.03.8
# Fri, 24 Apr 2020 02:03:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 24 Apr 2020 02:04:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 24 Apr 2020 02:04:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 24 Apr 2020 02:04:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 24 Apr 2020 02:04:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 24 Apr 2020 02:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 02:04:05 GMT
CMD ["sh"]
# Fri, 24 Apr 2020 02:04:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 24 Apr 2020 02:04:18 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 24 Apr 2020 02:04:18 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 24 Apr 2020 02:04:21 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 06 May 2020 00:57:36 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Wed, 06 May 2020 00:57:37 GMT
VOLUME [/var/lib/docker]
# Wed, 06 May 2020 00:57:38 GMT
EXPOSE 2375 2376
# Wed, 06 May 2020 00:57:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 06 May 2020 00:57:39 GMT
CMD []
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c2ce1bf627500ac9aec72c466865536bbff375e04a4e409655bbdf2827c1a`  
		Last Modified: Fri, 24 Apr 2020 02:04:53 GMT  
		Size: 1.8 MB (1822716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14a8989d4305a13a6c1fbfab29671cacd99035dd4291710ba978fd29283481`  
		Last Modified: Fri, 24 Apr 2020 02:04:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0b1f8e9eedb57e967305efe997babe0185ba6f7fe9eb7f4cbed6ee3d3f4dbe`  
		Last Modified: Fri, 24 Apr 2020 02:05:12 GMT  
		Size: 59.9 MB (59927054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc59092f5c3af9ff086a7203470a39d43b9ba5593cdd2eb494796a245ce8ecd4`  
		Last Modified: Fri, 24 Apr 2020 02:04:52 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f54a6c116900f095c4bce429f827a4dcc0af52c0634e42b3f83a9f5ea321d39`  
		Last Modified: Fri, 24 Apr 2020 02:04:51 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb98a21ac35e0dd075007407e66183792d9dbc8c997513d6592918018b5312a`  
		Last Modified: Fri, 24 Apr 2020 02:04:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bec2c432e5c5b4a7f698ed4b9ae252a67bf63604d41a06f871228065ded28a0`  
		Last Modified: Fri, 24 Apr 2020 02:05:28 GMT  
		Size: 2.8 MB (2824842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75c0882dce0c322a151afe082f0005164734b3df8b685891a1796351c2c8155`  
		Last Modified: Fri, 24 Apr 2020 02:05:28 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53c8f90da7135b8a7bd1382287287fc0a77f5671a336d4e82b2d9bd7bfee975`  
		Last Modified: Fri, 24 Apr 2020 02:05:28 GMT  
		Size: 750.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd7687b9e4e3e2a29a9e10fda7c4e188a5f92507110c037afc83048a374ebb7`  
		Last Modified: Wed, 06 May 2020 00:58:02 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4f02c4ad7f9483dee2ebc9efe3c66633691504e4c3734fa38b657bb6beb22047
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66714139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c275ab420e15e0f0d3fe6e88b30424974332da758bf2804e204b73dc7a3ddb7`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:43:16 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 03:43:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:43:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:43:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:43:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:43:31 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:43:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:43:33 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 03:43:45 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Dec 2020 03:43:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Dec 2020 03:43:52 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 11 Dec 2020 03:43:56 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Dec 2020 03:43:58 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:43:59 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Dec 2020 03:44:01 GMT
EXPOSE 2375 2376
# Fri, 11 Dec 2020 03:44:04 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Dec 2020 03:44:05 GMT
CMD []
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44406ea375713a15815e70d9f67caccd9d24e3edb888eb33765a7855947a57dd`  
		Last Modified: Fri, 11 Dec 2020 03:46:07 GMT  
		Size: 56.0 MB (55992945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da9e082087083b4fa5ee2804222088c41668d42a3cda42a0358add93cfbfed2`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd11a145516582d37d1ac882ec6ced4d65ad928b3f5923c73b16211995c42da6`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961068b01d86e33d4e09c9fa6829e3ff7bdb7d3b6a60449681cdf49519058265`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52bcec35351af8539981ca3f0097a0d3b02517a030e2fd5e2c52cd30c72ad66`  
		Last Modified: Fri, 11 Dec 2020 03:46:19 GMT  
		Size: 5.9 MB (5946714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ba61fc8445e0471f06d03123c54a76ac7d5d292c0f9983e7021df62400b2d1`  
		Last Modified: Fri, 11 Dec 2020 03:46:19 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28426d0cbfd272b6cb9a64a8b6a1a41033edeae5823a4a809d71f5c1435d7a4`  
		Last Modified: Fri, 11 Dec 2020 03:46:17 GMT  
		Size: 933.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1827aa166b927762754e480784c7ca687bf2acf61142c2a4e9667cf203a63614`  
		Last Modified: Fri, 11 Dec 2020 03:46:18 GMT  
		Size: 2.5 KB (2512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-dind-rootless`

```console
$ docker pull docker@sha256:8853e15e167d7e28afc759b9d08c387de504c149f58d009b35c234e953c2328b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19.03-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:1fef5d7f95e2d0616a2610badc9d9fd5a6122bb75a2804fe0696ac8aecffdee4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94208960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cf71f951fc9b03cab529aeaf8e9fa85201eacb20f96e4080a649eb8f86e3b75`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:30:20 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 05:30:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:30:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:30:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:30:27 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:30:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:30:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:30:28 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:30:36 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Dec 2020 05:30:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:30:37 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 11 Dec 2020 05:30:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Dec 2020 05:30:40 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:30:40 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Dec 2020 05:30:40 GMT
EXPOSE 2375 2376
# Fri, 11 Dec 2020 05:30:40 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Dec 2020 05:30:40 GMT
CMD []
# Fri, 11 Dec 2020 05:30:46 GMT
RUN apk add --no-cache iproute2
# Fri, 11 Dec 2020 05:30:47 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 11 Dec 2020 05:30:48 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:30:50 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 11 Dec 2020 05:30:51 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 11 Dec 2020 05:30:52 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 11 Dec 2020 05:30:52 GMT
USER rootless
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70334c77c8527b221cde2e0e99359cce5c9cb5457b65a88e8de902f18fa993cb`  
		Last Modified: Fri, 11 Dec 2020 05:32:42 GMT  
		Size: 62.9 MB (62890703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa7fdb08ac5140b5cd81c000edc16d1acbb3c78b722d1b15ac81a866cf6de0d`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f150ffb925c000212dfa35dbdfeef8ea564438f2e6d7fe1bfa9eb4fda29378d8`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5098a8250e99dce60ef1d8768af0300a6f0445ea10caf4e2eebf3ce5ed75a848`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2416ba3463b18b0c83da91150211585ef657b5e5a4efb611846618dce5519ccb`  
		Last Modified: Fri, 11 Dec 2020 05:32:50 GMT  
		Size: 6.0 MB (5958753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc1d0e72e9ecb1fb9e0720e47b64137e3e0ab13c39535af6b17407fc0f9830`  
		Last Modified: Fri, 11 Dec 2020 05:32:49 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc0000bd7996fdaad1cd606eef1ddb78c249ed6065160d04959cb3a4e41cd34`  
		Last Modified: Fri, 11 Dec 2020 05:32:48 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a56ce7b22c289f5576aaf0f2b4244e8507be53c619319fce1585728883407c1`  
		Last Modified: Fri, 11 Dec 2020 05:32:49 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae09a432442ae7c3b89b670bf9046d02628a622b863e4f6ceda0935ad1e5b0ce`  
		Last Modified: Fri, 11 Dec 2020 05:32:56 GMT  
		Size: 1.1 MB (1092669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1164c9f7543f20bceba64a87c109532fb467074d62c1c9dfde4e541f0b888121`  
		Last Modified: Fri, 11 Dec 2020 05:32:56 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57070d6bdb6eb102a9060f82c30b35246a59871253dd891a749389ca3c95a0ac`  
		Last Modified: Fri, 11 Dec 2020 05:32:56 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1009bf87802d243e7e232ccc8467592825b3cd847fc06c2310908840ee557612`  
		Last Modified: Fri, 11 Dec 2020 05:33:00 GMT  
		Size: 19.4 MB (19422680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceaa992d3405cd49893b8fa63378cf828bc40c291339f12dd01bb3f8b62844cf`  
		Last Modified: Fri, 11 Dec 2020 05:32:56 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-git`

```console
$ docker pull docker@sha256:7ea1cab980be8e686d5dc26dccc8e177113d30a159db0307c7ee402a93024b76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03-git` - linux; amd64

```console
$ docker pull docker@sha256:ee6aee276f2be958681d31282993ef964180ef559730a5e6bed76d3668d328bc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (76040639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:183e97bebf36f6cad44bc7c0dce5103bcf992d95c9de726740cdd765204c538f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:30:20 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 05:30:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:30:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:30:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:30:27 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:30:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:30:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:30:28 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:30:58 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70334c77c8527b221cde2e0e99359cce5c9cb5457b65a88e8de902f18fa993cb`  
		Last Modified: Fri, 11 Dec 2020 05:32:42 GMT  
		Size: 62.9 MB (62890703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa7fdb08ac5140b5cd81c000edc16d1acbb3c78b722d1b15ac81a866cf6de0d`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f150ffb925c000212dfa35dbdfeef8ea564438f2e6d7fe1bfa9eb4fda29378d8`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5098a8250e99dce60ef1d8768af0300a6f0445ea10caf4e2eebf3ce5ed75a848`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7db262911d375a7fb6ea2b749ae3bf51300886f5da87d6240fd06875475d1cc`  
		Last Modified: Fri, 11 Dec 2020 05:33:09 GMT  
		Size: 8.3 MB (8312113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:bc0b0d405c1e2c6b365d09246756d2d4df5863ead71ff37cde0395e18832b525
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72273342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:124c69c34b8489345075587336e4f61de4c56072dd09e3f5d4a9ba6d2f9f4f5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:12:47 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 23 Apr 2020 17:12:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 17:12:50 GMT
ENV DOCKER_CHANNEL=stable
# Thu, 23 Apr 2020 17:12:51 GMT
ENV DOCKER_VERSION=19.03.8
# Thu, 23 Apr 2020 17:13:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 23 Apr 2020 17:13:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 23 Apr 2020 17:13:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:13:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 23 Apr 2020 17:13:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 23 Apr 2020 17:13:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 17:13:07 GMT
CMD ["sh"]
# Thu, 23 Apr 2020 17:13:45 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcb342235c0ef85c7b7836ba057f513df540f983f4dbe5587035824aec248ab`  
		Last Modified: Thu, 23 Apr 2020 17:14:04 GMT  
		Size: 1.9 MB (1926703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94018ec82f0af1c26efba50dc99b07f2db1d2fbfab94f814ca9e1b5147c73e56`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593e1c01de3a8ad095d83439f0112c9a534fe764682e7a0f99d0a5794f914591`  
		Last Modified: Thu, 23 Apr 2020 17:14:22 GMT  
		Size: 59.9 MB (59927152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3737124780efb66a0753c8acdb04e12dad9a04b3362b1496cfe1e1dcf2d60b`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a76f66eab7a2e5314dd5973bcbb4ab91a025072e77fd14a83ab87d5ed8cc39`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e1037ca5d5c489e9b1a5f1433e4d8be4b012c29ef660e05769c63bfbd63812`  
		Last Modified: Thu, 23 Apr 2020 17:14:02 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b7cb0ba4509eedc92c81006ddcf0e45d6676a0750dc0867dec331c7d6feb44`  
		Last Modified: Thu, 23 Apr 2020 17:14:54 GMT  
		Size: 7.8 MB (7797688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:e89d2f422796bb472a3f6c301076f8f64fb9f6c3078ff96a8cc7918121a9130f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.2 MB (71205027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba101ef968406449d45b9bf5373293c6f08f400cea9e947b6158777032233591`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:03:44 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 24 Apr 2020 02:03:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 02:03:47 GMT
ENV DOCKER_CHANNEL=stable
# Fri, 24 Apr 2020 02:03:48 GMT
ENV DOCKER_VERSION=19.03.8
# Fri, 24 Apr 2020 02:03:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 24 Apr 2020 02:04:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 24 Apr 2020 02:04:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 24 Apr 2020 02:04:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 24 Apr 2020 02:04:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 24 Apr 2020 02:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 02:04:05 GMT
CMD ["sh"]
# Fri, 24 Apr 2020 02:04:35 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c2ce1bf627500ac9aec72c466865536bbff375e04a4e409655bbdf2827c1a`  
		Last Modified: Fri, 24 Apr 2020 02:04:53 GMT  
		Size: 1.8 MB (1822716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14a8989d4305a13a6c1fbfab29671cacd99035dd4291710ba978fd29283481`  
		Last Modified: Fri, 24 Apr 2020 02:04:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0b1f8e9eedb57e967305efe997babe0185ba6f7fe9eb7f4cbed6ee3d3f4dbe`  
		Last Modified: Fri, 24 Apr 2020 02:05:12 GMT  
		Size: 59.9 MB (59927054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc59092f5c3af9ff086a7203470a39d43b9ba5593cdd2eb494796a245ce8ecd4`  
		Last Modified: Fri, 24 Apr 2020 02:04:52 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f54a6c116900f095c4bce429f827a4dcc0af52c0634e42b3f83a9f5ea321d39`  
		Last Modified: Fri, 24 Apr 2020 02:04:51 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb98a21ac35e0dd075007407e66183792d9dbc8c997513d6592918018b5312a`  
		Last Modified: Fri, 24 Apr 2020 02:04:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2b175115645c91b877c5783ddd6faf72ccddb1584eabd8187f8f8def8c2e17`  
		Last Modified: Fri, 24 Apr 2020 02:05:44 GMT  
		Size: 7.0 MB (7031330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:31c852882a88e4c35ea2f1802f10d116fccbbe7101071d921c12e15beedd4cc4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69266142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae9478277bd44d0819627464380f1048579954877b0e7645ac34d954b63ab20`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:43:16 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 03:43:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:43:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:43:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:43:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:43:31 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:43:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:43:33 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 03:44:19 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44406ea375713a15815e70d9f67caccd9d24e3edb888eb33765a7855947a57dd`  
		Last Modified: Fri, 11 Dec 2020 03:46:07 GMT  
		Size: 56.0 MB (55992945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da9e082087083b4fa5ee2804222088c41668d42a3cda42a0358add93cfbfed2`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd11a145516582d37d1ac882ec6ced4d65ad928b3f5923c73b16211995c42da6`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961068b01d86e33d4e09c9fa6829e3ff7bdb7d3b6a60449681cdf49519058265`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72293c133127a3af2438e9fdec9f0453dd61056d294aec4c7c40b00a74c2e110`  
		Last Modified: Fri, 11 Dec 2020 03:46:31 GMT  
		Size: 8.5 MB (8503472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19-dind`

```console
$ docker pull docker@sha256:e26923926850691a667caba2273dc5b021ec8a883417a017ad323c35cb1f2ffa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19-dind` - linux; amd64

```console
$ docker pull docker@sha256:24b8c9c132a93ec29c3ecac861c7b2657dc565f04dfbfa40c63372dbb2d03419
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73691996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:979576cc90c025f20b83960a7f40b56030cd89d4757ec42c66dd88fb246b2e42`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:30:20 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 05:30:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:30:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:30:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:30:27 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:30:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:30:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:30:28 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:30:36 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Dec 2020 05:30:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:30:37 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 11 Dec 2020 05:30:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Dec 2020 05:30:40 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:30:40 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Dec 2020 05:30:40 GMT
EXPOSE 2375 2376
# Fri, 11 Dec 2020 05:30:40 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Dec 2020 05:30:40 GMT
CMD []
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70334c77c8527b221cde2e0e99359cce5c9cb5457b65a88e8de902f18fa993cb`  
		Last Modified: Fri, 11 Dec 2020 05:32:42 GMT  
		Size: 62.9 MB (62890703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa7fdb08ac5140b5cd81c000edc16d1acbb3c78b722d1b15ac81a866cf6de0d`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f150ffb925c000212dfa35dbdfeef8ea564438f2e6d7fe1bfa9eb4fda29378d8`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5098a8250e99dce60ef1d8768af0300a6f0445ea10caf4e2eebf3ce5ed75a848`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2416ba3463b18b0c83da91150211585ef657b5e5a4efb611846618dce5519ccb`  
		Last Modified: Fri, 11 Dec 2020 05:32:50 GMT  
		Size: 6.0 MB (5958753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc1d0e72e9ecb1fb9e0720e47b64137e3e0ab13c39535af6b17407fc0f9830`  
		Last Modified: Fri, 11 Dec 2020 05:32:49 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc0000bd7996fdaad1cd606eef1ddb78c249ed6065160d04959cb3a4e41cd34`  
		Last Modified: Fri, 11 Dec 2020 05:32:48 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a56ce7b22c289f5576aaf0f2b4244e8507be53c619319fce1585728883407c1`  
		Last Modified: Fri, 11 Dec 2020 05:32:49 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:a6b0193cbf4d3c304f3bf6c6c253d88c25a22c6ffe6847fd57a6269e4324745f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67641153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50a37c38067d51b4185a04675f81f45209b82449ce8bbbec68b31d639ba45cd5`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:12:47 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 23 Apr 2020 17:12:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 17:12:50 GMT
ENV DOCKER_CHANNEL=stable
# Thu, 23 Apr 2020 17:12:51 GMT
ENV DOCKER_VERSION=19.03.8
# Thu, 23 Apr 2020 17:13:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 23 Apr 2020 17:13:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 23 Apr 2020 17:13:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:13:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 23 Apr 2020 17:13:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 23 Apr 2020 17:13:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 17:13:07 GMT
CMD ["sh"]
# Thu, 23 Apr 2020 17:13:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 23 Apr 2020 17:13:24 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 23 Apr 2020 17:13:25 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Thu, 23 Apr 2020 17:13:29 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 06 May 2020 00:49:37 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Wed, 06 May 2020 00:49:38 GMT
VOLUME [/var/lib/docker]
# Wed, 06 May 2020 00:49:38 GMT
EXPOSE 2375 2376
# Wed, 06 May 2020 00:49:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 06 May 2020 00:49:39 GMT
CMD []
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcb342235c0ef85c7b7836ba057f513df540f983f4dbe5587035824aec248ab`  
		Last Modified: Thu, 23 Apr 2020 17:14:04 GMT  
		Size: 1.9 MB (1926703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94018ec82f0af1c26efba50dc99b07f2db1d2fbfab94f814ca9e1b5147c73e56`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593e1c01de3a8ad095d83439f0112c9a534fe764682e7a0f99d0a5794f914591`  
		Last Modified: Thu, 23 Apr 2020 17:14:22 GMT  
		Size: 59.9 MB (59927152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3737124780efb66a0753c8acdb04e12dad9a04b3362b1496cfe1e1dcf2d60b`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a76f66eab7a2e5314dd5973bcbb4ab91a025072e77fd14a83ab87d5ed8cc39`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e1037ca5d5c489e9b1a5f1433e4d8be4b012c29ef660e05769c63bfbd63812`  
		Last Modified: Thu, 23 Apr 2020 17:14:02 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0227df4100f67814d05f04e139a5e9dca37299fd9d096c7574e16fe632211d4`  
		Last Modified: Thu, 23 Apr 2020 17:14:37 GMT  
		Size: 3.2 MB (3160940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a2483e804c9900710b0cfa9c5cad284336a14d95ec28dc1049dc1b3cc10de4`  
		Last Modified: Thu, 23 Apr 2020 17:14:36 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e906e300d3ad75b25c6513f466d68c5a2dc89ce9663dd6526821b9994ceef549`  
		Last Modified: Thu, 23 Apr 2020 17:14:36 GMT  
		Size: 753.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1dd819080e27b055eaa67e449dc1475fa02b89c7eb8406d4fd558c817df9ea`  
		Last Modified: Wed, 06 May 2020 00:50:04 GMT  
		Size: 2.5 KB (2501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:f998921d365053bf7e3f98794f6c23ca44e6809832d78105bc4d2da6bb8521ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67003102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e220c6648aa1a61c12d4f11dd3c99b4385828e8c4d9823a5656f4f40294c1d41`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:03:44 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 24 Apr 2020 02:03:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 02:03:47 GMT
ENV DOCKER_CHANNEL=stable
# Fri, 24 Apr 2020 02:03:48 GMT
ENV DOCKER_VERSION=19.03.8
# Fri, 24 Apr 2020 02:03:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 24 Apr 2020 02:04:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 24 Apr 2020 02:04:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 24 Apr 2020 02:04:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 24 Apr 2020 02:04:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 24 Apr 2020 02:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 02:04:05 GMT
CMD ["sh"]
# Fri, 24 Apr 2020 02:04:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 24 Apr 2020 02:04:18 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 24 Apr 2020 02:04:18 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 24 Apr 2020 02:04:21 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 06 May 2020 00:57:36 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Wed, 06 May 2020 00:57:37 GMT
VOLUME [/var/lib/docker]
# Wed, 06 May 2020 00:57:38 GMT
EXPOSE 2375 2376
# Wed, 06 May 2020 00:57:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 06 May 2020 00:57:39 GMT
CMD []
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c2ce1bf627500ac9aec72c466865536bbff375e04a4e409655bbdf2827c1a`  
		Last Modified: Fri, 24 Apr 2020 02:04:53 GMT  
		Size: 1.8 MB (1822716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14a8989d4305a13a6c1fbfab29671cacd99035dd4291710ba978fd29283481`  
		Last Modified: Fri, 24 Apr 2020 02:04:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0b1f8e9eedb57e967305efe997babe0185ba6f7fe9eb7f4cbed6ee3d3f4dbe`  
		Last Modified: Fri, 24 Apr 2020 02:05:12 GMT  
		Size: 59.9 MB (59927054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc59092f5c3af9ff086a7203470a39d43b9ba5593cdd2eb494796a245ce8ecd4`  
		Last Modified: Fri, 24 Apr 2020 02:04:52 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f54a6c116900f095c4bce429f827a4dcc0af52c0634e42b3f83a9f5ea321d39`  
		Last Modified: Fri, 24 Apr 2020 02:04:51 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb98a21ac35e0dd075007407e66183792d9dbc8c997513d6592918018b5312a`  
		Last Modified: Fri, 24 Apr 2020 02:04:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bec2c432e5c5b4a7f698ed4b9ae252a67bf63604d41a06f871228065ded28a0`  
		Last Modified: Fri, 24 Apr 2020 02:05:28 GMT  
		Size: 2.8 MB (2824842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75c0882dce0c322a151afe082f0005164734b3df8b685891a1796351c2c8155`  
		Last Modified: Fri, 24 Apr 2020 02:05:28 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53c8f90da7135b8a7bd1382287287fc0a77f5671a336d4e82b2d9bd7bfee975`  
		Last Modified: Fri, 24 Apr 2020 02:05:28 GMT  
		Size: 750.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd7687b9e4e3e2a29a9e10fda7c4e188a5f92507110c037afc83048a374ebb7`  
		Last Modified: Wed, 06 May 2020 00:58:02 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4f02c4ad7f9483dee2ebc9efe3c66633691504e4c3734fa38b657bb6beb22047
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66714139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c275ab420e15e0f0d3fe6e88b30424974332da758bf2804e204b73dc7a3ddb7`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:43:16 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 03:43:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:43:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:43:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:43:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:43:31 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:43:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:43:33 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 03:43:45 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Dec 2020 03:43:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Dec 2020 03:43:52 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 11 Dec 2020 03:43:56 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Dec 2020 03:43:58 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:43:59 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Dec 2020 03:44:01 GMT
EXPOSE 2375 2376
# Fri, 11 Dec 2020 03:44:04 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Dec 2020 03:44:05 GMT
CMD []
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44406ea375713a15815e70d9f67caccd9d24e3edb888eb33765a7855947a57dd`  
		Last Modified: Fri, 11 Dec 2020 03:46:07 GMT  
		Size: 56.0 MB (55992945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da9e082087083b4fa5ee2804222088c41668d42a3cda42a0358add93cfbfed2`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd11a145516582d37d1ac882ec6ced4d65ad928b3f5923c73b16211995c42da6`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961068b01d86e33d4e09c9fa6829e3ff7bdb7d3b6a60449681cdf49519058265`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52bcec35351af8539981ca3f0097a0d3b02517a030e2fd5e2c52cd30c72ad66`  
		Last Modified: Fri, 11 Dec 2020 03:46:19 GMT  
		Size: 5.9 MB (5946714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ba61fc8445e0471f06d03123c54a76ac7d5d292c0f9983e7021df62400b2d1`  
		Last Modified: Fri, 11 Dec 2020 03:46:19 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28426d0cbfd272b6cb9a64a8b6a1a41033edeae5823a4a809d71f5c1435d7a4`  
		Last Modified: Fri, 11 Dec 2020 03:46:17 GMT  
		Size: 933.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1827aa166b927762754e480784c7ca687bf2acf61142c2a4e9667cf203a63614`  
		Last Modified: Fri, 11 Dec 2020 03:46:18 GMT  
		Size: 2.5 KB (2512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19-dind-rootless`

```console
$ docker pull docker@sha256:8853e15e167d7e28afc759b9d08c387de504c149f58d009b35c234e953c2328b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:1fef5d7f95e2d0616a2610badc9d9fd5a6122bb75a2804fe0696ac8aecffdee4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94208960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cf71f951fc9b03cab529aeaf8e9fa85201eacb20f96e4080a649eb8f86e3b75`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:30:20 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 05:30:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:30:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:30:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:30:27 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:30:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:30:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:30:28 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:30:36 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Dec 2020 05:30:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:30:37 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 11 Dec 2020 05:30:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Dec 2020 05:30:40 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:30:40 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Dec 2020 05:30:40 GMT
EXPOSE 2375 2376
# Fri, 11 Dec 2020 05:30:40 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Dec 2020 05:30:40 GMT
CMD []
# Fri, 11 Dec 2020 05:30:46 GMT
RUN apk add --no-cache iproute2
# Fri, 11 Dec 2020 05:30:47 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 11 Dec 2020 05:30:48 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:30:50 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 11 Dec 2020 05:30:51 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 11 Dec 2020 05:30:52 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 11 Dec 2020 05:30:52 GMT
USER rootless
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70334c77c8527b221cde2e0e99359cce5c9cb5457b65a88e8de902f18fa993cb`  
		Last Modified: Fri, 11 Dec 2020 05:32:42 GMT  
		Size: 62.9 MB (62890703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa7fdb08ac5140b5cd81c000edc16d1acbb3c78b722d1b15ac81a866cf6de0d`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f150ffb925c000212dfa35dbdfeef8ea564438f2e6d7fe1bfa9eb4fda29378d8`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5098a8250e99dce60ef1d8768af0300a6f0445ea10caf4e2eebf3ce5ed75a848`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2416ba3463b18b0c83da91150211585ef657b5e5a4efb611846618dce5519ccb`  
		Last Modified: Fri, 11 Dec 2020 05:32:50 GMT  
		Size: 6.0 MB (5958753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc1d0e72e9ecb1fb9e0720e47b64137e3e0ab13c39535af6b17407fc0f9830`  
		Last Modified: Fri, 11 Dec 2020 05:32:49 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc0000bd7996fdaad1cd606eef1ddb78c249ed6065160d04959cb3a4e41cd34`  
		Last Modified: Fri, 11 Dec 2020 05:32:48 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a56ce7b22c289f5576aaf0f2b4244e8507be53c619319fce1585728883407c1`  
		Last Modified: Fri, 11 Dec 2020 05:32:49 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae09a432442ae7c3b89b670bf9046d02628a622b863e4f6ceda0935ad1e5b0ce`  
		Last Modified: Fri, 11 Dec 2020 05:32:56 GMT  
		Size: 1.1 MB (1092669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1164c9f7543f20bceba64a87c109532fb467074d62c1c9dfde4e541f0b888121`  
		Last Modified: Fri, 11 Dec 2020 05:32:56 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57070d6bdb6eb102a9060f82c30b35246a59871253dd891a749389ca3c95a0ac`  
		Last Modified: Fri, 11 Dec 2020 05:32:56 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1009bf87802d243e7e232ccc8467592825b3cd847fc06c2310908840ee557612`  
		Last Modified: Fri, 11 Dec 2020 05:33:00 GMT  
		Size: 19.4 MB (19422680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceaa992d3405cd49893b8fa63378cf828bc40c291339f12dd01bb3f8b62844cf`  
		Last Modified: Fri, 11 Dec 2020 05:32:56 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19-git`

```console
$ docker pull docker@sha256:7ea1cab980be8e686d5dc26dccc8e177113d30a159db0307c7ee402a93024b76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19-git` - linux; amd64

```console
$ docker pull docker@sha256:ee6aee276f2be958681d31282993ef964180ef559730a5e6bed76d3668d328bc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (76040639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:183e97bebf36f6cad44bc7c0dce5103bcf992d95c9de726740cdd765204c538f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:30:20 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 05:30:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:30:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:30:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:30:27 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:30:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:30:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:30:28 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:30:58 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70334c77c8527b221cde2e0e99359cce5c9cb5457b65a88e8de902f18fa993cb`  
		Last Modified: Fri, 11 Dec 2020 05:32:42 GMT  
		Size: 62.9 MB (62890703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa7fdb08ac5140b5cd81c000edc16d1acbb3c78b722d1b15ac81a866cf6de0d`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f150ffb925c000212dfa35dbdfeef8ea564438f2e6d7fe1bfa9eb4fda29378d8`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5098a8250e99dce60ef1d8768af0300a6f0445ea10caf4e2eebf3ce5ed75a848`  
		Last Modified: Fri, 11 Dec 2020 05:32:28 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7db262911d375a7fb6ea2b749ae3bf51300886f5da87d6240fd06875475d1cc`  
		Last Modified: Fri, 11 Dec 2020 05:33:09 GMT  
		Size: 8.3 MB (8312113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:bc0b0d405c1e2c6b365d09246756d2d4df5863ead71ff37cde0395e18832b525
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72273342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:124c69c34b8489345075587336e4f61de4c56072dd09e3f5d4a9ba6d2f9f4f5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:12:47 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 23 Apr 2020 17:12:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 17:12:50 GMT
ENV DOCKER_CHANNEL=stable
# Thu, 23 Apr 2020 17:12:51 GMT
ENV DOCKER_VERSION=19.03.8
# Thu, 23 Apr 2020 17:13:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 23 Apr 2020 17:13:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 23 Apr 2020 17:13:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:13:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 23 Apr 2020 17:13:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 23 Apr 2020 17:13:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 17:13:07 GMT
CMD ["sh"]
# Thu, 23 Apr 2020 17:13:45 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcb342235c0ef85c7b7836ba057f513df540f983f4dbe5587035824aec248ab`  
		Last Modified: Thu, 23 Apr 2020 17:14:04 GMT  
		Size: 1.9 MB (1926703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94018ec82f0af1c26efba50dc99b07f2db1d2fbfab94f814ca9e1b5147c73e56`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593e1c01de3a8ad095d83439f0112c9a534fe764682e7a0f99d0a5794f914591`  
		Last Modified: Thu, 23 Apr 2020 17:14:22 GMT  
		Size: 59.9 MB (59927152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3737124780efb66a0753c8acdb04e12dad9a04b3362b1496cfe1e1dcf2d60b`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a76f66eab7a2e5314dd5973bcbb4ab91a025072e77fd14a83ab87d5ed8cc39`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e1037ca5d5c489e9b1a5f1433e4d8be4b012c29ef660e05769c63bfbd63812`  
		Last Modified: Thu, 23 Apr 2020 17:14:02 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b7cb0ba4509eedc92c81006ddcf0e45d6676a0750dc0867dec331c7d6feb44`  
		Last Modified: Thu, 23 Apr 2020 17:14:54 GMT  
		Size: 7.8 MB (7797688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:e89d2f422796bb472a3f6c301076f8f64fb9f6c3078ff96a8cc7918121a9130f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.2 MB (71205027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba101ef968406449d45b9bf5373293c6f08f400cea9e947b6158777032233591`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:03:44 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 24 Apr 2020 02:03:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 02:03:47 GMT
ENV DOCKER_CHANNEL=stable
# Fri, 24 Apr 2020 02:03:48 GMT
ENV DOCKER_VERSION=19.03.8
# Fri, 24 Apr 2020 02:03:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 24 Apr 2020 02:04:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 24 Apr 2020 02:04:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 24 Apr 2020 02:04:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 24 Apr 2020 02:04:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 24 Apr 2020 02:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 02:04:05 GMT
CMD ["sh"]
# Fri, 24 Apr 2020 02:04:35 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c2ce1bf627500ac9aec72c466865536bbff375e04a4e409655bbdf2827c1a`  
		Last Modified: Fri, 24 Apr 2020 02:04:53 GMT  
		Size: 1.8 MB (1822716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14a8989d4305a13a6c1fbfab29671cacd99035dd4291710ba978fd29283481`  
		Last Modified: Fri, 24 Apr 2020 02:04:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0b1f8e9eedb57e967305efe997babe0185ba6f7fe9eb7f4cbed6ee3d3f4dbe`  
		Last Modified: Fri, 24 Apr 2020 02:05:12 GMT  
		Size: 59.9 MB (59927054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc59092f5c3af9ff086a7203470a39d43b9ba5593cdd2eb494796a245ce8ecd4`  
		Last Modified: Fri, 24 Apr 2020 02:04:52 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f54a6c116900f095c4bce429f827a4dcc0af52c0634e42b3f83a9f5ea321d39`  
		Last Modified: Fri, 24 Apr 2020 02:04:51 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb98a21ac35e0dd075007407e66183792d9dbc8c997513d6592918018b5312a`  
		Last Modified: Fri, 24 Apr 2020 02:04:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2b175115645c91b877c5783ddd6faf72ccddb1584eabd8187f8f8def8c2e17`  
		Last Modified: Fri, 24 Apr 2020 02:05:44 GMT  
		Size: 7.0 MB (7031330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:31c852882a88e4c35ea2f1802f10d116fccbbe7101071d921c12e15beedd4cc4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69266142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae9478277bd44d0819627464380f1048579954877b0e7645ac34d954b63ab20`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:43:16 GMT
ENV DOCKER_VERSION=19.03.14
# Fri, 11 Dec 2020 03:43:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:43:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:43:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:43:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:43:31 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:43:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:43:33 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 03:44:19 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44406ea375713a15815e70d9f67caccd9d24e3edb888eb33765a7855947a57dd`  
		Last Modified: Fri, 11 Dec 2020 03:46:07 GMT  
		Size: 56.0 MB (55992945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da9e082087083b4fa5ee2804222088c41668d42a3cda42a0358add93cfbfed2`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd11a145516582d37d1ac882ec6ced4d65ad928b3f5923c73b16211995c42da6`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961068b01d86e33d4e09c9fa6829e3ff7bdb7d3b6a60449681cdf49519058265`  
		Last Modified: Fri, 11 Dec 2020 03:45:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72293c133127a3af2438e9fdec9f0453dd61056d294aec4c7c40b00a74c2e110`  
		Last Modified: Fri, 11 Dec 2020 03:46:31 GMT  
		Size: 8.5 MB (8503472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20`

```console
$ docker pull docker@sha256:fefd2a66e0543621b3e022b34b504cb41c2e72e6098fb6239f1e3d6fd1edefd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20` - linux; amd64

```console
$ docker pull docker@sha256:48c45a5da08acef9293e5fa4d6527d1ba39689a498df135e8f5e0d90fa4b7f33
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74295694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aefe523efa57aaf5952272f1f3b1d4ccecd638bdfe3719304a9f7b5e464ec1cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:29:34 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 05:29:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:29:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:29:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:42 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e060f4bd70b333ccaa7ae441b42f1068621b39bbe8eb9c71b5a4e06d10b4ff3`  
		Last Modified: Fri, 11 Dec 2020 05:31:46 GMT  
		Size: 69.5 MB (69457871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e8d568a22304aafab5a456040525abd0b705efad0b6e60e64847ebe1c6e4e6`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc6ef1a942a0f6b2ab0993eecb7ce30d31f06af50a2ae40893e1a160c9a0892`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2312dd95470aa8eaccef80bbca7892390ca777559b50fab574e65147a35107fc`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f65a8021b3332e2cfe3498c23cf10ccd0010db66f6f0bc1fb65dff8d280b9ab8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68327992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeaf43b927733dcfd7b87c5a733c444df7c3d364e065dbebfdc2271d9caaa502`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:42:09 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 03:42:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:42:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:42:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:42:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:42:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:42:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:42:32 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330b718f631fe67ed5c2ddee0ac1f74cb77a1211022efb33aa66f6f5d6d2f05f`  
		Last Modified: Fri, 11 Dec 2020 03:45:09 GMT  
		Size: 63.6 MB (63558264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a938160415222146a455ed7ddae6e01d0c41f91a764f77ac05ed9794d08adf6a`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb6da89ff942a1c917a6a29653eb45dfc3826f334b16e17bc82207ce1193cc4`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a70c0c122f402fb4ee26f6661b037f3e6ee30e639f710e4f318dbf908e60a65`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10`

```console
$ docker pull docker@sha256:fefd2a66e0543621b3e022b34b504cb41c2e72e6098fb6239f1e3d6fd1edefd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10` - linux; amd64

```console
$ docker pull docker@sha256:48c45a5da08acef9293e5fa4d6527d1ba39689a498df135e8f5e0d90fa4b7f33
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74295694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aefe523efa57aaf5952272f1f3b1d4ccecd638bdfe3719304a9f7b5e464ec1cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:29:34 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 05:29:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:29:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:29:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:42 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e060f4bd70b333ccaa7ae441b42f1068621b39bbe8eb9c71b5a4e06d10b4ff3`  
		Last Modified: Fri, 11 Dec 2020 05:31:46 GMT  
		Size: 69.5 MB (69457871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e8d568a22304aafab5a456040525abd0b705efad0b6e60e64847ebe1c6e4e6`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc6ef1a942a0f6b2ab0993eecb7ce30d31f06af50a2ae40893e1a160c9a0892`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2312dd95470aa8eaccef80bbca7892390ca777559b50fab574e65147a35107fc`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f65a8021b3332e2cfe3498c23cf10ccd0010db66f6f0bc1fb65dff8d280b9ab8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68327992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeaf43b927733dcfd7b87c5a733c444df7c3d364e065dbebfdc2271d9caaa502`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:42:09 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 03:42:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:42:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:42:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:42:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:42:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:42:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:42:32 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330b718f631fe67ed5c2ddee0ac1f74cb77a1211022efb33aa66f6f5d6d2f05f`  
		Last Modified: Fri, 11 Dec 2020 03:45:09 GMT  
		Size: 63.6 MB (63558264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a938160415222146a455ed7ddae6e01d0c41f91a764f77ac05ed9794d08adf6a`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb6da89ff942a1c917a6a29653eb45dfc3826f334b16e17bc82207ce1193cc4`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a70c0c122f402fb4ee26f6661b037f3e6ee30e639f710e4f318dbf908e60a65`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.0`

```console
$ docker pull docker@sha256:fefd2a66e0543621b3e022b34b504cb41c2e72e6098fb6239f1e3d6fd1edefd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.0` - linux; amd64

```console
$ docker pull docker@sha256:48c45a5da08acef9293e5fa4d6527d1ba39689a498df135e8f5e0d90fa4b7f33
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74295694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aefe523efa57aaf5952272f1f3b1d4ccecd638bdfe3719304a9f7b5e464ec1cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:29:34 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 05:29:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:29:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:29:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:42 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e060f4bd70b333ccaa7ae441b42f1068621b39bbe8eb9c71b5a4e06d10b4ff3`  
		Last Modified: Fri, 11 Dec 2020 05:31:46 GMT  
		Size: 69.5 MB (69457871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e8d568a22304aafab5a456040525abd0b705efad0b6e60e64847ebe1c6e4e6`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc6ef1a942a0f6b2ab0993eecb7ce30d31f06af50a2ae40893e1a160c9a0892`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2312dd95470aa8eaccef80bbca7892390ca777559b50fab574e65147a35107fc`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.0` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f65a8021b3332e2cfe3498c23cf10ccd0010db66f6f0bc1fb65dff8d280b9ab8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68327992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeaf43b927733dcfd7b87c5a733c444df7c3d364e065dbebfdc2271d9caaa502`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:42:09 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 03:42:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:42:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:42:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:42:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:42:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:42:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:42:32 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330b718f631fe67ed5c2ddee0ac1f74cb77a1211022efb33aa66f6f5d6d2f05f`  
		Last Modified: Fri, 11 Dec 2020 03:45:09 GMT  
		Size: 63.6 MB (63558264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a938160415222146a455ed7ddae6e01d0c41f91a764f77ac05ed9794d08adf6a`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb6da89ff942a1c917a6a29653eb45dfc3826f334b16e17bc82207ce1193cc4`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a70c0c122f402fb4ee26f6661b037f3e6ee30e639f710e4f318dbf908e60a65`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.0-dind`

```console
$ docker pull docker@sha256:a995cba4a6982d53b0e9ab77561e90524de2bdc5d9ded02c0c25bb8d2ab75191
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.0-dind` - linux; amd64

```console
$ docker pull docker@sha256:49905ff8893d5ad789528ba8001cc1e4e3027d6a5c10275c9a118ff7fc911740
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.3 MB (80259119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f4d9e5111282b20a0adc2d28d7a4f6d5853311870eb262773594d07620fa043`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:29:34 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 05:29:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:29:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:29:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:42 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:29:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Dec 2020 05:29:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:29:50 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 11 Dec 2020 05:29:51 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Dec 2020 05:29:51 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:52 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Dec 2020 05:29:52 GMT
EXPOSE 2375 2376
# Fri, 11 Dec 2020 05:29:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:52 GMT
CMD []
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e060f4bd70b333ccaa7ae441b42f1068621b39bbe8eb9c71b5a4e06d10b4ff3`  
		Last Modified: Fri, 11 Dec 2020 05:31:46 GMT  
		Size: 69.5 MB (69457871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e8d568a22304aafab5a456040525abd0b705efad0b6e60e64847ebe1c6e4e6`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc6ef1a942a0f6b2ab0993eecb7ce30d31f06af50a2ae40893e1a160c9a0892`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2312dd95470aa8eaccef80bbca7892390ca777559b50fab574e65147a35107fc`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705044911461d972356a560402ae7212ac5b9e0cf5650c9e90e82c0168e363f4`  
		Last Modified: Fri, 11 Dec 2020 05:31:55 GMT  
		Size: 6.0 MB (5958710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca03bf2650888a6dd094e66dc51a4c7e9cf6e2d540eb0e6ee60447b670644cb`  
		Last Modified: Fri, 11 Dec 2020 05:31:54 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f30abe54315eba4800bca902658bb857afd12015cb658e13874c43042c93400`  
		Last Modified: Fri, 11 Dec 2020 05:31:53 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc682ce81f04b09d573611856b1c36f71a3da08529300ee33214d7d31432df2b`  
		Last Modified: Fri, 11 Dec 2020 05:31:53 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.0-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:31548ab869bd6fcf73471c44c5332bfef15a90b3bbdabfc8e744f38e3d6d10b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74319177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68cf207b112d9f66e003ee80b4be8fc38d493b4a6d3cb2b6097cd3a20273cf98`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:42:09 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 03:42:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:42:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:42:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:42:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:42:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:42:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:42:32 GMT
CMD ["sh"]
# Sat, 12 Dec 2020 14:05:54 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 12 Dec 2020 14:05:56 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 12 Dec 2020 14:05:57 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Sat, 12 Dec 2020 14:06:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 12 Dec 2020 14:06:03 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Sat, 12 Dec 2020 14:06:04 GMT
VOLUME [/var/lib/docker]
# Sat, 12 Dec 2020 14:06:05 GMT
EXPOSE 2375 2376
# Sat, 12 Dec 2020 14:06:06 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 12 Dec 2020 14:06:07 GMT
CMD []
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330b718f631fe67ed5c2ddee0ac1f74cb77a1211022efb33aa66f6f5d6d2f05f`  
		Last Modified: Fri, 11 Dec 2020 03:45:09 GMT  
		Size: 63.6 MB (63558264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a938160415222146a455ed7ddae6e01d0c41f91a764f77ac05ed9794d08adf6a`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb6da89ff942a1c917a6a29653eb45dfc3826f334b16e17bc82207ce1193cc4`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a70c0c122f402fb4ee26f6661b037f3e6ee30e639f710e4f318dbf908e60a65`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8afd8df3b7cdec4857f13fd9220eedddfec97a9b472d534b64c3061aa30cf6e`  
		Last Modified: Sat, 12 Dec 2020 14:06:56 GMT  
		Size: 6.0 MB (5986441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eff5b3d64e850cc6162e025f1861c218b1a6db4195963699adf17792510be4b`  
		Last Modified: Sat, 12 Dec 2020 14:06:54 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1864e7f84e2dee54ed6b17a27027327bef427f36ab47cc9a02a3fce44e887103`  
		Last Modified: Sat, 12 Dec 2020 14:06:53 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b60a743d62dd15c7c619c9a7c6940cd70e8efc3edf8fda03009c9be8301e1`  
		Last Modified: Sat, 12 Dec 2020 14:06:54 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.0-dind-rootless`

```console
$ docker pull docker@sha256:53e4c1ec262c4a6e14ce863b72b23aa21c33c1c2a5b9d9417989096c80260f8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:20.10.0-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:6921c855c141f3c87dd9736b3783aaead17b83c564a1afae678afe546c555f82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.5 MB (101524776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecd272bd50bff353249e99ef1c016e4465c8cd75b28f749659b6ca4af12b81d5`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:29:34 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 05:29:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:29:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:29:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:42 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:29:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Dec 2020 05:29:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:29:50 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 11 Dec 2020 05:29:51 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Dec 2020 05:29:51 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:52 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Dec 2020 05:29:52 GMT
EXPOSE 2375 2376
# Fri, 11 Dec 2020 05:29:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:52 GMT
CMD []
# Fri, 11 Dec 2020 05:30:00 GMT
RUN apk add --no-cache iproute2
# Fri, 11 Dec 2020 05:30:02 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 11 Dec 2020 05:30:03 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:30:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 11 Dec 2020 05:30:09 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 11 Dec 2020 05:30:10 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 11 Dec 2020 05:30:10 GMT
USER rootless
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e060f4bd70b333ccaa7ae441b42f1068621b39bbe8eb9c71b5a4e06d10b4ff3`  
		Last Modified: Fri, 11 Dec 2020 05:31:46 GMT  
		Size: 69.5 MB (69457871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e8d568a22304aafab5a456040525abd0b705efad0b6e60e64847ebe1c6e4e6`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc6ef1a942a0f6b2ab0993eecb7ce30d31f06af50a2ae40893e1a160c9a0892`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2312dd95470aa8eaccef80bbca7892390ca777559b50fab574e65147a35107fc`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705044911461d972356a560402ae7212ac5b9e0cf5650c9e90e82c0168e363f4`  
		Last Modified: Fri, 11 Dec 2020 05:31:55 GMT  
		Size: 6.0 MB (5958710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca03bf2650888a6dd094e66dc51a4c7e9cf6e2d540eb0e6ee60447b670644cb`  
		Last Modified: Fri, 11 Dec 2020 05:31:54 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f30abe54315eba4800bca902658bb857afd12015cb658e13874c43042c93400`  
		Last Modified: Fri, 11 Dec 2020 05:31:53 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc682ce81f04b09d573611856b1c36f71a3da08529300ee33214d7d31432df2b`  
		Last Modified: Fri, 11 Dec 2020 05:31:53 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3bb12715694c8d4d06340e7dee1e3254c8e3b7b70a93186d608231e3d078e2`  
		Last Modified: Fri, 11 Dec 2020 05:32:04 GMT  
		Size: 1.1 MB (1092673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a839f28eb57bd36d3aacb29facc913d8ab0f88f7dc151a1c4ed01678b588b880`  
		Last Modified: Fri, 11 Dec 2020 05:32:04 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0a6ba5f373ec6316a1554ce6f2b7006f8a1b8125ecd9d2b5a10737eccc0f39`  
		Last Modified: Fri, 11 Dec 2020 05:32:03 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa1dd6e35f0eddbcae4e4ce8274d76308a2b6c591c73a5265567a52e237f12e`  
		Last Modified: Fri, 11 Dec 2020 05:32:07 GMT  
		Size: 20.2 MB (20171373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348a90887c16fa0075d15a6c8c9a7c23ba9733360f2e894b4274351566a1e557`  
		Last Modified: Fri, 11 Dec 2020 05:32:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.0-git`

```console
$ docker pull docker@sha256:27544b0737bf1692fac937e63c4fbb7a6ee788be2fe02afe0d35b703ab9e6f24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.0-git` - linux; amd64

```console
$ docker pull docker@sha256:ee0863d21f5b6a72eddaa92b281ba08fefff01233b6ff7f21a3b4161e67b0701
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.6 MB (82607809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da02afe1f0a55690236398189fed8820ae95fa6810fbcb729de153940273c556`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:29:34 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 05:29:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:29:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:29:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:42 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:30:16 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e060f4bd70b333ccaa7ae441b42f1068621b39bbe8eb9c71b5a4e06d10b4ff3`  
		Last Modified: Fri, 11 Dec 2020 05:31:46 GMT  
		Size: 69.5 MB (69457871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e8d568a22304aafab5a456040525abd0b705efad0b6e60e64847ebe1c6e4e6`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc6ef1a942a0f6b2ab0993eecb7ce30d31f06af50a2ae40893e1a160c9a0892`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2312dd95470aa8eaccef80bbca7892390ca777559b50fab574e65147a35107fc`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3eb13f7c24ccd98855472084e1c92136894253750fb88152cf488dd3b87da`  
		Last Modified: Fri, 11 Dec 2020 05:32:20 GMT  
		Size: 8.3 MB (8312115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.0-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:836a38373d532ac55e66096590e2d8c7b4833cf0cfabd80c0f004d050080a74c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76831460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d961e0b3d34ce5f4ae39dcadff0006d5afcddf128492dfb2da665a0fb5c0d3ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:42:09 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 03:42:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:42:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:42:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:42:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:42:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:42:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:42:32 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 03:43:08 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330b718f631fe67ed5c2ddee0ac1f74cb77a1211022efb33aa66f6f5d6d2f05f`  
		Last Modified: Fri, 11 Dec 2020 03:45:09 GMT  
		Size: 63.6 MB (63558264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a938160415222146a455ed7ddae6e01d0c41f91a764f77ac05ed9794d08adf6a`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb6da89ff942a1c917a6a29653eb45dfc3826f334b16e17bc82207ce1193cc4`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a70c0c122f402fb4ee26f6661b037f3e6ee30e639f710e4f318dbf908e60a65`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99c483ed624af2276f16b538d32a3eec95bb4309d636878022d76d74bae9def`  
		Last Modified: Fri, 11 Dec 2020 03:45:39 GMT  
		Size: 8.5 MB (8503468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind`

```console
$ docker pull docker@sha256:a995cba4a6982d53b0e9ab77561e90524de2bdc5d9ded02c0c25bb8d2ab75191
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind` - linux; amd64

```console
$ docker pull docker@sha256:49905ff8893d5ad789528ba8001cc1e4e3027d6a5c10275c9a118ff7fc911740
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.3 MB (80259119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f4d9e5111282b20a0adc2d28d7a4f6d5853311870eb262773594d07620fa043`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:29:34 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 05:29:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:29:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:29:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:42 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:29:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Dec 2020 05:29:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:29:50 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 11 Dec 2020 05:29:51 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Dec 2020 05:29:51 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:52 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Dec 2020 05:29:52 GMT
EXPOSE 2375 2376
# Fri, 11 Dec 2020 05:29:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:52 GMT
CMD []
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e060f4bd70b333ccaa7ae441b42f1068621b39bbe8eb9c71b5a4e06d10b4ff3`  
		Last Modified: Fri, 11 Dec 2020 05:31:46 GMT  
		Size: 69.5 MB (69457871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e8d568a22304aafab5a456040525abd0b705efad0b6e60e64847ebe1c6e4e6`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc6ef1a942a0f6b2ab0993eecb7ce30d31f06af50a2ae40893e1a160c9a0892`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2312dd95470aa8eaccef80bbca7892390ca777559b50fab574e65147a35107fc`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705044911461d972356a560402ae7212ac5b9e0cf5650c9e90e82c0168e363f4`  
		Last Modified: Fri, 11 Dec 2020 05:31:55 GMT  
		Size: 6.0 MB (5958710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca03bf2650888a6dd094e66dc51a4c7e9cf6e2d540eb0e6ee60447b670644cb`  
		Last Modified: Fri, 11 Dec 2020 05:31:54 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f30abe54315eba4800bca902658bb857afd12015cb658e13874c43042c93400`  
		Last Modified: Fri, 11 Dec 2020 05:31:53 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc682ce81f04b09d573611856b1c36f71a3da08529300ee33214d7d31432df2b`  
		Last Modified: Fri, 11 Dec 2020 05:31:53 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:31548ab869bd6fcf73471c44c5332bfef15a90b3bbdabfc8e744f38e3d6d10b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74319177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68cf207b112d9f66e003ee80b4be8fc38d493b4a6d3cb2b6097cd3a20273cf98`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:42:09 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 03:42:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:42:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:42:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:42:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:42:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:42:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:42:32 GMT
CMD ["sh"]
# Sat, 12 Dec 2020 14:05:54 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 12 Dec 2020 14:05:56 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 12 Dec 2020 14:05:57 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Sat, 12 Dec 2020 14:06:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 12 Dec 2020 14:06:03 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Sat, 12 Dec 2020 14:06:04 GMT
VOLUME [/var/lib/docker]
# Sat, 12 Dec 2020 14:06:05 GMT
EXPOSE 2375 2376
# Sat, 12 Dec 2020 14:06:06 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 12 Dec 2020 14:06:07 GMT
CMD []
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330b718f631fe67ed5c2ddee0ac1f74cb77a1211022efb33aa66f6f5d6d2f05f`  
		Last Modified: Fri, 11 Dec 2020 03:45:09 GMT  
		Size: 63.6 MB (63558264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a938160415222146a455ed7ddae6e01d0c41f91a764f77ac05ed9794d08adf6a`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb6da89ff942a1c917a6a29653eb45dfc3826f334b16e17bc82207ce1193cc4`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a70c0c122f402fb4ee26f6661b037f3e6ee30e639f710e4f318dbf908e60a65`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8afd8df3b7cdec4857f13fd9220eedddfec97a9b472d534b64c3061aa30cf6e`  
		Last Modified: Sat, 12 Dec 2020 14:06:56 GMT  
		Size: 6.0 MB (5986441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eff5b3d64e850cc6162e025f1861c218b1a6db4195963699adf17792510be4b`  
		Last Modified: Sat, 12 Dec 2020 14:06:54 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1864e7f84e2dee54ed6b17a27027327bef427f36ab47cc9a02a3fce44e887103`  
		Last Modified: Sat, 12 Dec 2020 14:06:53 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b60a743d62dd15c7c619c9a7c6940cd70e8efc3edf8fda03009c9be8301e1`  
		Last Modified: Sat, 12 Dec 2020 14:06:54 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind-rootless`

```console
$ docker pull docker@sha256:53e4c1ec262c4a6e14ce863b72b23aa21c33c1c2a5b9d9417989096c80260f8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:20.10-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:6921c855c141f3c87dd9736b3783aaead17b83c564a1afae678afe546c555f82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.5 MB (101524776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecd272bd50bff353249e99ef1c016e4465c8cd75b28f749659b6ca4af12b81d5`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:29:34 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 05:29:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:29:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:29:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:42 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:29:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Dec 2020 05:29:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:29:50 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 11 Dec 2020 05:29:51 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Dec 2020 05:29:51 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:52 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Dec 2020 05:29:52 GMT
EXPOSE 2375 2376
# Fri, 11 Dec 2020 05:29:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:52 GMT
CMD []
# Fri, 11 Dec 2020 05:30:00 GMT
RUN apk add --no-cache iproute2
# Fri, 11 Dec 2020 05:30:02 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 11 Dec 2020 05:30:03 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:30:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 11 Dec 2020 05:30:09 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 11 Dec 2020 05:30:10 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 11 Dec 2020 05:30:10 GMT
USER rootless
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e060f4bd70b333ccaa7ae441b42f1068621b39bbe8eb9c71b5a4e06d10b4ff3`  
		Last Modified: Fri, 11 Dec 2020 05:31:46 GMT  
		Size: 69.5 MB (69457871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e8d568a22304aafab5a456040525abd0b705efad0b6e60e64847ebe1c6e4e6`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc6ef1a942a0f6b2ab0993eecb7ce30d31f06af50a2ae40893e1a160c9a0892`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2312dd95470aa8eaccef80bbca7892390ca777559b50fab574e65147a35107fc`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705044911461d972356a560402ae7212ac5b9e0cf5650c9e90e82c0168e363f4`  
		Last Modified: Fri, 11 Dec 2020 05:31:55 GMT  
		Size: 6.0 MB (5958710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca03bf2650888a6dd094e66dc51a4c7e9cf6e2d540eb0e6ee60447b670644cb`  
		Last Modified: Fri, 11 Dec 2020 05:31:54 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f30abe54315eba4800bca902658bb857afd12015cb658e13874c43042c93400`  
		Last Modified: Fri, 11 Dec 2020 05:31:53 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc682ce81f04b09d573611856b1c36f71a3da08529300ee33214d7d31432df2b`  
		Last Modified: Fri, 11 Dec 2020 05:31:53 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3bb12715694c8d4d06340e7dee1e3254c8e3b7b70a93186d608231e3d078e2`  
		Last Modified: Fri, 11 Dec 2020 05:32:04 GMT  
		Size: 1.1 MB (1092673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a839f28eb57bd36d3aacb29facc913d8ab0f88f7dc151a1c4ed01678b588b880`  
		Last Modified: Fri, 11 Dec 2020 05:32:04 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0a6ba5f373ec6316a1554ce6f2b7006f8a1b8125ecd9d2b5a10737eccc0f39`  
		Last Modified: Fri, 11 Dec 2020 05:32:03 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa1dd6e35f0eddbcae4e4ce8274d76308a2b6c591c73a5265567a52e237f12e`  
		Last Modified: Fri, 11 Dec 2020 05:32:07 GMT  
		Size: 20.2 MB (20171373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348a90887c16fa0075d15a6c8c9a7c23ba9733360f2e894b4274351566a1e557`  
		Last Modified: Fri, 11 Dec 2020 05:32:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-git`

```console
$ docker pull docker@sha256:27544b0737bf1692fac937e63c4fbb7a6ee788be2fe02afe0d35b703ab9e6f24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-git` - linux; amd64

```console
$ docker pull docker@sha256:ee0863d21f5b6a72eddaa92b281ba08fefff01233b6ff7f21a3b4161e67b0701
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.6 MB (82607809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da02afe1f0a55690236398189fed8820ae95fa6810fbcb729de153940273c556`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:29:34 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 05:29:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:29:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:29:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:42 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:30:16 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e060f4bd70b333ccaa7ae441b42f1068621b39bbe8eb9c71b5a4e06d10b4ff3`  
		Last Modified: Fri, 11 Dec 2020 05:31:46 GMT  
		Size: 69.5 MB (69457871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e8d568a22304aafab5a456040525abd0b705efad0b6e60e64847ebe1c6e4e6`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc6ef1a942a0f6b2ab0993eecb7ce30d31f06af50a2ae40893e1a160c9a0892`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2312dd95470aa8eaccef80bbca7892390ca777559b50fab574e65147a35107fc`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3eb13f7c24ccd98855472084e1c92136894253750fb88152cf488dd3b87da`  
		Last Modified: Fri, 11 Dec 2020 05:32:20 GMT  
		Size: 8.3 MB (8312115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:836a38373d532ac55e66096590e2d8c7b4833cf0cfabd80c0f004d050080a74c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76831460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d961e0b3d34ce5f4ae39dcadff0006d5afcddf128492dfb2da665a0fb5c0d3ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:42:09 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 03:42:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:42:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:42:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:42:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:42:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:42:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:42:32 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 03:43:08 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330b718f631fe67ed5c2ddee0ac1f74cb77a1211022efb33aa66f6f5d6d2f05f`  
		Last Modified: Fri, 11 Dec 2020 03:45:09 GMT  
		Size: 63.6 MB (63558264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a938160415222146a455ed7ddae6e01d0c41f91a764f77ac05ed9794d08adf6a`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb6da89ff942a1c917a6a29653eb45dfc3826f334b16e17bc82207ce1193cc4`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a70c0c122f402fb4ee26f6661b037f3e6ee30e639f710e4f318dbf908e60a65`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99c483ed624af2276f16b538d32a3eec95bb4309d636878022d76d74bae9def`  
		Last Modified: Fri, 11 Dec 2020 03:45:39 GMT  
		Size: 8.5 MB (8503468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind`

```console
$ docker pull docker@sha256:a995cba4a6982d53b0e9ab77561e90524de2bdc5d9ded02c0c25bb8d2ab75191
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind` - linux; amd64

```console
$ docker pull docker@sha256:49905ff8893d5ad789528ba8001cc1e4e3027d6a5c10275c9a118ff7fc911740
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.3 MB (80259119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f4d9e5111282b20a0adc2d28d7a4f6d5853311870eb262773594d07620fa043`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:29:34 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 05:29:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:29:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:29:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:42 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:29:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Dec 2020 05:29:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:29:50 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 11 Dec 2020 05:29:51 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Dec 2020 05:29:51 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:52 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Dec 2020 05:29:52 GMT
EXPOSE 2375 2376
# Fri, 11 Dec 2020 05:29:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:52 GMT
CMD []
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e060f4bd70b333ccaa7ae441b42f1068621b39bbe8eb9c71b5a4e06d10b4ff3`  
		Last Modified: Fri, 11 Dec 2020 05:31:46 GMT  
		Size: 69.5 MB (69457871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e8d568a22304aafab5a456040525abd0b705efad0b6e60e64847ebe1c6e4e6`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc6ef1a942a0f6b2ab0993eecb7ce30d31f06af50a2ae40893e1a160c9a0892`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2312dd95470aa8eaccef80bbca7892390ca777559b50fab574e65147a35107fc`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705044911461d972356a560402ae7212ac5b9e0cf5650c9e90e82c0168e363f4`  
		Last Modified: Fri, 11 Dec 2020 05:31:55 GMT  
		Size: 6.0 MB (5958710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca03bf2650888a6dd094e66dc51a4c7e9cf6e2d540eb0e6ee60447b670644cb`  
		Last Modified: Fri, 11 Dec 2020 05:31:54 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f30abe54315eba4800bca902658bb857afd12015cb658e13874c43042c93400`  
		Last Modified: Fri, 11 Dec 2020 05:31:53 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc682ce81f04b09d573611856b1c36f71a3da08529300ee33214d7d31432df2b`  
		Last Modified: Fri, 11 Dec 2020 05:31:53 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:31548ab869bd6fcf73471c44c5332bfef15a90b3bbdabfc8e744f38e3d6d10b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74319177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68cf207b112d9f66e003ee80b4be8fc38d493b4a6d3cb2b6097cd3a20273cf98`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:42:09 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 03:42:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:42:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:42:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:42:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:42:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:42:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:42:32 GMT
CMD ["sh"]
# Sat, 12 Dec 2020 14:05:54 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 12 Dec 2020 14:05:56 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 12 Dec 2020 14:05:57 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Sat, 12 Dec 2020 14:06:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 12 Dec 2020 14:06:03 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Sat, 12 Dec 2020 14:06:04 GMT
VOLUME [/var/lib/docker]
# Sat, 12 Dec 2020 14:06:05 GMT
EXPOSE 2375 2376
# Sat, 12 Dec 2020 14:06:06 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 12 Dec 2020 14:06:07 GMT
CMD []
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330b718f631fe67ed5c2ddee0ac1f74cb77a1211022efb33aa66f6f5d6d2f05f`  
		Last Modified: Fri, 11 Dec 2020 03:45:09 GMT  
		Size: 63.6 MB (63558264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a938160415222146a455ed7ddae6e01d0c41f91a764f77ac05ed9794d08adf6a`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb6da89ff942a1c917a6a29653eb45dfc3826f334b16e17bc82207ce1193cc4`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a70c0c122f402fb4ee26f6661b037f3e6ee30e639f710e4f318dbf908e60a65`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8afd8df3b7cdec4857f13fd9220eedddfec97a9b472d534b64c3061aa30cf6e`  
		Last Modified: Sat, 12 Dec 2020 14:06:56 GMT  
		Size: 6.0 MB (5986441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eff5b3d64e850cc6162e025f1861c218b1a6db4195963699adf17792510be4b`  
		Last Modified: Sat, 12 Dec 2020 14:06:54 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1864e7f84e2dee54ed6b17a27027327bef427f36ab47cc9a02a3fce44e887103`  
		Last Modified: Sat, 12 Dec 2020 14:06:53 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b60a743d62dd15c7c619c9a7c6940cd70e8efc3edf8fda03009c9be8301e1`  
		Last Modified: Sat, 12 Dec 2020 14:06:54 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:53e4c1ec262c4a6e14ce863b72b23aa21c33c1c2a5b9d9417989096c80260f8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:6921c855c141f3c87dd9736b3783aaead17b83c564a1afae678afe546c555f82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.5 MB (101524776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecd272bd50bff353249e99ef1c016e4465c8cd75b28f749659b6ca4af12b81d5`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:29:34 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 05:29:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:29:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:29:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:42 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:29:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Dec 2020 05:29:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:29:50 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 11 Dec 2020 05:29:51 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Dec 2020 05:29:51 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:52 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Dec 2020 05:29:52 GMT
EXPOSE 2375 2376
# Fri, 11 Dec 2020 05:29:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:52 GMT
CMD []
# Fri, 11 Dec 2020 05:30:00 GMT
RUN apk add --no-cache iproute2
# Fri, 11 Dec 2020 05:30:02 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 11 Dec 2020 05:30:03 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:30:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 11 Dec 2020 05:30:09 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 11 Dec 2020 05:30:10 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 11 Dec 2020 05:30:10 GMT
USER rootless
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e060f4bd70b333ccaa7ae441b42f1068621b39bbe8eb9c71b5a4e06d10b4ff3`  
		Last Modified: Fri, 11 Dec 2020 05:31:46 GMT  
		Size: 69.5 MB (69457871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e8d568a22304aafab5a456040525abd0b705efad0b6e60e64847ebe1c6e4e6`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc6ef1a942a0f6b2ab0993eecb7ce30d31f06af50a2ae40893e1a160c9a0892`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2312dd95470aa8eaccef80bbca7892390ca777559b50fab574e65147a35107fc`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705044911461d972356a560402ae7212ac5b9e0cf5650c9e90e82c0168e363f4`  
		Last Modified: Fri, 11 Dec 2020 05:31:55 GMT  
		Size: 6.0 MB (5958710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca03bf2650888a6dd094e66dc51a4c7e9cf6e2d540eb0e6ee60447b670644cb`  
		Last Modified: Fri, 11 Dec 2020 05:31:54 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f30abe54315eba4800bca902658bb857afd12015cb658e13874c43042c93400`  
		Last Modified: Fri, 11 Dec 2020 05:31:53 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc682ce81f04b09d573611856b1c36f71a3da08529300ee33214d7d31432df2b`  
		Last Modified: Fri, 11 Dec 2020 05:31:53 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3bb12715694c8d4d06340e7dee1e3254c8e3b7b70a93186d608231e3d078e2`  
		Last Modified: Fri, 11 Dec 2020 05:32:04 GMT  
		Size: 1.1 MB (1092673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a839f28eb57bd36d3aacb29facc913d8ab0f88f7dc151a1c4ed01678b588b880`  
		Last Modified: Fri, 11 Dec 2020 05:32:04 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0a6ba5f373ec6316a1554ce6f2b7006f8a1b8125ecd9d2b5a10737eccc0f39`  
		Last Modified: Fri, 11 Dec 2020 05:32:03 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa1dd6e35f0eddbcae4e4ce8274d76308a2b6c591c73a5265567a52e237f12e`  
		Last Modified: Fri, 11 Dec 2020 05:32:07 GMT  
		Size: 20.2 MB (20171373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348a90887c16fa0075d15a6c8c9a7c23ba9733360f2e894b4274351566a1e557`  
		Last Modified: Fri, 11 Dec 2020 05:32:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-git`

```console
$ docker pull docker@sha256:27544b0737bf1692fac937e63c4fbb7a6ee788be2fe02afe0d35b703ab9e6f24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-git` - linux; amd64

```console
$ docker pull docker@sha256:ee0863d21f5b6a72eddaa92b281ba08fefff01233b6ff7f21a3b4161e67b0701
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.6 MB (82607809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da02afe1f0a55690236398189fed8820ae95fa6810fbcb729de153940273c556`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:29:34 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 05:29:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:29:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:29:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:42 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:30:16 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e060f4bd70b333ccaa7ae441b42f1068621b39bbe8eb9c71b5a4e06d10b4ff3`  
		Last Modified: Fri, 11 Dec 2020 05:31:46 GMT  
		Size: 69.5 MB (69457871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e8d568a22304aafab5a456040525abd0b705efad0b6e60e64847ebe1c6e4e6`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc6ef1a942a0f6b2ab0993eecb7ce30d31f06af50a2ae40893e1a160c9a0892`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2312dd95470aa8eaccef80bbca7892390ca777559b50fab574e65147a35107fc`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3eb13f7c24ccd98855472084e1c92136894253750fb88152cf488dd3b87da`  
		Last Modified: Fri, 11 Dec 2020 05:32:20 GMT  
		Size: 8.3 MB (8312115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:836a38373d532ac55e66096590e2d8c7b4833cf0cfabd80c0f004d050080a74c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76831460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d961e0b3d34ce5f4ae39dcadff0006d5afcddf128492dfb2da665a0fb5c0d3ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:42:09 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 03:42:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:42:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:42:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:42:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:42:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:42:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:42:32 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 03:43:08 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330b718f631fe67ed5c2ddee0ac1f74cb77a1211022efb33aa66f6f5d6d2f05f`  
		Last Modified: Fri, 11 Dec 2020 03:45:09 GMT  
		Size: 63.6 MB (63558264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a938160415222146a455ed7ddae6e01d0c41f91a764f77ac05ed9794d08adf6a`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb6da89ff942a1c917a6a29653eb45dfc3826f334b16e17bc82207ce1193cc4`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a70c0c122f402fb4ee26f6661b037f3e6ee30e639f710e4f318dbf908e60a65`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99c483ed624af2276f16b538d32a3eec95bb4309d636878022d76d74bae9def`  
		Last Modified: Fri, 11 Dec 2020 03:45:39 GMT  
		Size: 8.5 MB (8503468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:78dd89ff0c9c7e6848501f1c58cf8c126b68e1d2174697004e6220ed84a84244
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:49905ff8893d5ad789528ba8001cc1e4e3027d6a5c10275c9a118ff7fc911740
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.3 MB (80259119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f4d9e5111282b20a0adc2d28d7a4f6d5853311870eb262773594d07620fa043`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:29:34 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 05:29:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:29:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:29:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:42 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:29:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Dec 2020 05:29:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:29:50 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 11 Dec 2020 05:29:51 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Dec 2020 05:29:51 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:52 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Dec 2020 05:29:52 GMT
EXPOSE 2375 2376
# Fri, 11 Dec 2020 05:29:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:52 GMT
CMD []
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e060f4bd70b333ccaa7ae441b42f1068621b39bbe8eb9c71b5a4e06d10b4ff3`  
		Last Modified: Fri, 11 Dec 2020 05:31:46 GMT  
		Size: 69.5 MB (69457871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e8d568a22304aafab5a456040525abd0b705efad0b6e60e64847ebe1c6e4e6`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc6ef1a942a0f6b2ab0993eecb7ce30d31f06af50a2ae40893e1a160c9a0892`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2312dd95470aa8eaccef80bbca7892390ca777559b50fab574e65147a35107fc`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705044911461d972356a560402ae7212ac5b9e0cf5650c9e90e82c0168e363f4`  
		Last Modified: Fri, 11 Dec 2020 05:31:55 GMT  
		Size: 6.0 MB (5958710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca03bf2650888a6dd094e66dc51a4c7e9cf6e2d540eb0e6ee60447b670644cb`  
		Last Modified: Fri, 11 Dec 2020 05:31:54 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f30abe54315eba4800bca902658bb857afd12015cb658e13874c43042c93400`  
		Last Modified: Fri, 11 Dec 2020 05:31:53 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc682ce81f04b09d573611856b1c36f71a3da08529300ee33214d7d31432df2b`  
		Last Modified: Fri, 11 Dec 2020 05:31:53 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:a6b0193cbf4d3c304f3bf6c6c253d88c25a22c6ffe6847fd57a6269e4324745f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67641153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50a37c38067d51b4185a04675f81f45209b82449ce8bbbec68b31d639ba45cd5`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:12:47 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 23 Apr 2020 17:12:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 17:12:50 GMT
ENV DOCKER_CHANNEL=stable
# Thu, 23 Apr 2020 17:12:51 GMT
ENV DOCKER_VERSION=19.03.8
# Thu, 23 Apr 2020 17:13:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 23 Apr 2020 17:13:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 23 Apr 2020 17:13:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:13:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 23 Apr 2020 17:13:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 23 Apr 2020 17:13:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 17:13:07 GMT
CMD ["sh"]
# Thu, 23 Apr 2020 17:13:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 23 Apr 2020 17:13:24 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 23 Apr 2020 17:13:25 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Thu, 23 Apr 2020 17:13:29 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 06 May 2020 00:49:37 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Wed, 06 May 2020 00:49:38 GMT
VOLUME [/var/lib/docker]
# Wed, 06 May 2020 00:49:38 GMT
EXPOSE 2375 2376
# Wed, 06 May 2020 00:49:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 06 May 2020 00:49:39 GMT
CMD []
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcb342235c0ef85c7b7836ba057f513df540f983f4dbe5587035824aec248ab`  
		Last Modified: Thu, 23 Apr 2020 17:14:04 GMT  
		Size: 1.9 MB (1926703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94018ec82f0af1c26efba50dc99b07f2db1d2fbfab94f814ca9e1b5147c73e56`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593e1c01de3a8ad095d83439f0112c9a534fe764682e7a0f99d0a5794f914591`  
		Last Modified: Thu, 23 Apr 2020 17:14:22 GMT  
		Size: 59.9 MB (59927152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3737124780efb66a0753c8acdb04e12dad9a04b3362b1496cfe1e1dcf2d60b`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a76f66eab7a2e5314dd5973bcbb4ab91a025072e77fd14a83ab87d5ed8cc39`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e1037ca5d5c489e9b1a5f1433e4d8be4b012c29ef660e05769c63bfbd63812`  
		Last Modified: Thu, 23 Apr 2020 17:14:02 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0227df4100f67814d05f04e139a5e9dca37299fd9d096c7574e16fe632211d4`  
		Last Modified: Thu, 23 Apr 2020 17:14:37 GMT  
		Size: 3.2 MB (3160940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a2483e804c9900710b0cfa9c5cad284336a14d95ec28dc1049dc1b3cc10de4`  
		Last Modified: Thu, 23 Apr 2020 17:14:36 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e906e300d3ad75b25c6513f466d68c5a2dc89ce9663dd6526821b9994ceef549`  
		Last Modified: Thu, 23 Apr 2020 17:14:36 GMT  
		Size: 753.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1dd819080e27b055eaa67e449dc1475fa02b89c7eb8406d4fd558c817df9ea`  
		Last Modified: Wed, 06 May 2020 00:50:04 GMT  
		Size: 2.5 KB (2501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:f998921d365053bf7e3f98794f6c23ca44e6809832d78105bc4d2da6bb8521ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67003102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e220c6648aa1a61c12d4f11dd3c99b4385828e8c4d9823a5656f4f40294c1d41`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:03:44 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 24 Apr 2020 02:03:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 02:03:47 GMT
ENV DOCKER_CHANNEL=stable
# Fri, 24 Apr 2020 02:03:48 GMT
ENV DOCKER_VERSION=19.03.8
# Fri, 24 Apr 2020 02:03:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 24 Apr 2020 02:04:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 24 Apr 2020 02:04:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 24 Apr 2020 02:04:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 24 Apr 2020 02:04:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 24 Apr 2020 02:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 02:04:05 GMT
CMD ["sh"]
# Fri, 24 Apr 2020 02:04:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 24 Apr 2020 02:04:18 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 24 Apr 2020 02:04:18 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 24 Apr 2020 02:04:21 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 06 May 2020 00:57:36 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Wed, 06 May 2020 00:57:37 GMT
VOLUME [/var/lib/docker]
# Wed, 06 May 2020 00:57:38 GMT
EXPOSE 2375 2376
# Wed, 06 May 2020 00:57:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 06 May 2020 00:57:39 GMT
CMD []
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c2ce1bf627500ac9aec72c466865536bbff375e04a4e409655bbdf2827c1a`  
		Last Modified: Fri, 24 Apr 2020 02:04:53 GMT  
		Size: 1.8 MB (1822716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14a8989d4305a13a6c1fbfab29671cacd99035dd4291710ba978fd29283481`  
		Last Modified: Fri, 24 Apr 2020 02:04:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0b1f8e9eedb57e967305efe997babe0185ba6f7fe9eb7f4cbed6ee3d3f4dbe`  
		Last Modified: Fri, 24 Apr 2020 02:05:12 GMT  
		Size: 59.9 MB (59927054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc59092f5c3af9ff086a7203470a39d43b9ba5593cdd2eb494796a245ce8ecd4`  
		Last Modified: Fri, 24 Apr 2020 02:04:52 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f54a6c116900f095c4bce429f827a4dcc0af52c0634e42b3f83a9f5ea321d39`  
		Last Modified: Fri, 24 Apr 2020 02:04:51 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb98a21ac35e0dd075007407e66183792d9dbc8c997513d6592918018b5312a`  
		Last Modified: Fri, 24 Apr 2020 02:04:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bec2c432e5c5b4a7f698ed4b9ae252a67bf63604d41a06f871228065ded28a0`  
		Last Modified: Fri, 24 Apr 2020 02:05:28 GMT  
		Size: 2.8 MB (2824842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75c0882dce0c322a151afe082f0005164734b3df8b685891a1796351c2c8155`  
		Last Modified: Fri, 24 Apr 2020 02:05:28 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53c8f90da7135b8a7bd1382287287fc0a77f5671a336d4e82b2d9bd7bfee975`  
		Last Modified: Fri, 24 Apr 2020 02:05:28 GMT  
		Size: 750.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd7687b9e4e3e2a29a9e10fda7c4e188a5f92507110c037afc83048a374ebb7`  
		Last Modified: Wed, 06 May 2020 00:58:02 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:31548ab869bd6fcf73471c44c5332bfef15a90b3bbdabfc8e744f38e3d6d10b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74319177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68cf207b112d9f66e003ee80b4be8fc38d493b4a6d3cb2b6097cd3a20273cf98`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:42:09 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 03:42:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:42:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:42:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:42:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:42:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:42:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:42:32 GMT
CMD ["sh"]
# Sat, 12 Dec 2020 14:05:54 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 12 Dec 2020 14:05:56 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 12 Dec 2020 14:05:57 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Sat, 12 Dec 2020 14:06:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 12 Dec 2020 14:06:03 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Sat, 12 Dec 2020 14:06:04 GMT
VOLUME [/var/lib/docker]
# Sat, 12 Dec 2020 14:06:05 GMT
EXPOSE 2375 2376
# Sat, 12 Dec 2020 14:06:06 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 12 Dec 2020 14:06:07 GMT
CMD []
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330b718f631fe67ed5c2ddee0ac1f74cb77a1211022efb33aa66f6f5d6d2f05f`  
		Last Modified: Fri, 11 Dec 2020 03:45:09 GMT  
		Size: 63.6 MB (63558264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a938160415222146a455ed7ddae6e01d0c41f91a764f77ac05ed9794d08adf6a`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb6da89ff942a1c917a6a29653eb45dfc3826f334b16e17bc82207ce1193cc4`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a70c0c122f402fb4ee26f6661b037f3e6ee30e639f710e4f318dbf908e60a65`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8afd8df3b7cdec4857f13fd9220eedddfec97a9b472d534b64c3061aa30cf6e`  
		Last Modified: Sat, 12 Dec 2020 14:06:56 GMT  
		Size: 6.0 MB (5986441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eff5b3d64e850cc6162e025f1861c218b1a6db4195963699adf17792510be4b`  
		Last Modified: Sat, 12 Dec 2020 14:06:54 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1864e7f84e2dee54ed6b17a27027327bef427f36ab47cc9a02a3fce44e887103`  
		Last Modified: Sat, 12 Dec 2020 14:06:53 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b60a743d62dd15c7c619c9a7c6940cd70e8efc3edf8fda03009c9be8301e1`  
		Last Modified: Sat, 12 Dec 2020 14:06:54 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:53e4c1ec262c4a6e14ce863b72b23aa21c33c1c2a5b9d9417989096c80260f8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:6921c855c141f3c87dd9736b3783aaead17b83c564a1afae678afe546c555f82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.5 MB (101524776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecd272bd50bff353249e99ef1c016e4465c8cd75b28f749659b6ca4af12b81d5`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:29:34 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 05:29:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:29:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:29:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:42 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:29:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Dec 2020 05:29:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:29:50 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 11 Dec 2020 05:29:51 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Dec 2020 05:29:51 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:52 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Dec 2020 05:29:52 GMT
EXPOSE 2375 2376
# Fri, 11 Dec 2020 05:29:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:52 GMT
CMD []
# Fri, 11 Dec 2020 05:30:00 GMT
RUN apk add --no-cache iproute2
# Fri, 11 Dec 2020 05:30:02 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 11 Dec 2020 05:30:03 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:30:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 11 Dec 2020 05:30:09 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 11 Dec 2020 05:30:10 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 11 Dec 2020 05:30:10 GMT
USER rootless
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e060f4bd70b333ccaa7ae441b42f1068621b39bbe8eb9c71b5a4e06d10b4ff3`  
		Last Modified: Fri, 11 Dec 2020 05:31:46 GMT  
		Size: 69.5 MB (69457871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e8d568a22304aafab5a456040525abd0b705efad0b6e60e64847ebe1c6e4e6`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc6ef1a942a0f6b2ab0993eecb7ce30d31f06af50a2ae40893e1a160c9a0892`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2312dd95470aa8eaccef80bbca7892390ca777559b50fab574e65147a35107fc`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705044911461d972356a560402ae7212ac5b9e0cf5650c9e90e82c0168e363f4`  
		Last Modified: Fri, 11 Dec 2020 05:31:55 GMT  
		Size: 6.0 MB (5958710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca03bf2650888a6dd094e66dc51a4c7e9cf6e2d540eb0e6ee60447b670644cb`  
		Last Modified: Fri, 11 Dec 2020 05:31:54 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f30abe54315eba4800bca902658bb857afd12015cb658e13874c43042c93400`  
		Last Modified: Fri, 11 Dec 2020 05:31:53 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc682ce81f04b09d573611856b1c36f71a3da08529300ee33214d7d31432df2b`  
		Last Modified: Fri, 11 Dec 2020 05:31:53 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3bb12715694c8d4d06340e7dee1e3254c8e3b7b70a93186d608231e3d078e2`  
		Last Modified: Fri, 11 Dec 2020 05:32:04 GMT  
		Size: 1.1 MB (1092673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a839f28eb57bd36d3aacb29facc913d8ab0f88f7dc151a1c4ed01678b588b880`  
		Last Modified: Fri, 11 Dec 2020 05:32:04 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0a6ba5f373ec6316a1554ce6f2b7006f8a1b8125ecd9d2b5a10737eccc0f39`  
		Last Modified: Fri, 11 Dec 2020 05:32:03 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa1dd6e35f0eddbcae4e4ce8274d76308a2b6c591c73a5265567a52e237f12e`  
		Last Modified: Fri, 11 Dec 2020 05:32:07 GMT  
		Size: 20.2 MB (20171373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348a90887c16fa0075d15a6c8c9a7c23ba9733360f2e894b4274351566a1e557`  
		Last Modified: Fri, 11 Dec 2020 05:32:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:fdd99cc50f397facb7692151450b1635ebc6b03591302c8a469364a8d5ccbcec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:ee0863d21f5b6a72eddaa92b281ba08fefff01233b6ff7f21a3b4161e67b0701
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.6 MB (82607809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da02afe1f0a55690236398189fed8820ae95fa6810fbcb729de153940273c556`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:29:34 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 05:29:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:29:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:29:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:42 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:30:16 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e060f4bd70b333ccaa7ae441b42f1068621b39bbe8eb9c71b5a4e06d10b4ff3`  
		Last Modified: Fri, 11 Dec 2020 05:31:46 GMT  
		Size: 69.5 MB (69457871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e8d568a22304aafab5a456040525abd0b705efad0b6e60e64847ebe1c6e4e6`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc6ef1a942a0f6b2ab0993eecb7ce30d31f06af50a2ae40893e1a160c9a0892`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2312dd95470aa8eaccef80bbca7892390ca777559b50fab574e65147a35107fc`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3eb13f7c24ccd98855472084e1c92136894253750fb88152cf488dd3b87da`  
		Last Modified: Fri, 11 Dec 2020 05:32:20 GMT  
		Size: 8.3 MB (8312115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm variant v6

```console
$ docker pull docker@sha256:bc0b0d405c1e2c6b365d09246756d2d4df5863ead71ff37cde0395e18832b525
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72273342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:124c69c34b8489345075587336e4f61de4c56072dd09e3f5d4a9ba6d2f9f4f5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:12:47 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 23 Apr 2020 17:12:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 17:12:50 GMT
ENV DOCKER_CHANNEL=stable
# Thu, 23 Apr 2020 17:12:51 GMT
ENV DOCKER_VERSION=19.03.8
# Thu, 23 Apr 2020 17:13:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 23 Apr 2020 17:13:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 23 Apr 2020 17:13:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:13:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 23 Apr 2020 17:13:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 23 Apr 2020 17:13:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 17:13:07 GMT
CMD ["sh"]
# Thu, 23 Apr 2020 17:13:45 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcb342235c0ef85c7b7836ba057f513df540f983f4dbe5587035824aec248ab`  
		Last Modified: Thu, 23 Apr 2020 17:14:04 GMT  
		Size: 1.9 MB (1926703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94018ec82f0af1c26efba50dc99b07f2db1d2fbfab94f814ca9e1b5147c73e56`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593e1c01de3a8ad095d83439f0112c9a534fe764682e7a0f99d0a5794f914591`  
		Last Modified: Thu, 23 Apr 2020 17:14:22 GMT  
		Size: 59.9 MB (59927152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3737124780efb66a0753c8acdb04e12dad9a04b3362b1496cfe1e1dcf2d60b`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a76f66eab7a2e5314dd5973bcbb4ab91a025072e77fd14a83ab87d5ed8cc39`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e1037ca5d5c489e9b1a5f1433e4d8be4b012c29ef660e05769c63bfbd63812`  
		Last Modified: Thu, 23 Apr 2020 17:14:02 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b7cb0ba4509eedc92c81006ddcf0e45d6676a0750dc0867dec331c7d6feb44`  
		Last Modified: Thu, 23 Apr 2020 17:14:54 GMT  
		Size: 7.8 MB (7797688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm variant v7

```console
$ docker pull docker@sha256:e89d2f422796bb472a3f6c301076f8f64fb9f6c3078ff96a8cc7918121a9130f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.2 MB (71205027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba101ef968406449d45b9bf5373293c6f08f400cea9e947b6158777032233591`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:03:44 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 24 Apr 2020 02:03:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 02:03:47 GMT
ENV DOCKER_CHANNEL=stable
# Fri, 24 Apr 2020 02:03:48 GMT
ENV DOCKER_VERSION=19.03.8
# Fri, 24 Apr 2020 02:03:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 24 Apr 2020 02:04:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 24 Apr 2020 02:04:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 24 Apr 2020 02:04:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 24 Apr 2020 02:04:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 24 Apr 2020 02:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 02:04:05 GMT
CMD ["sh"]
# Fri, 24 Apr 2020 02:04:35 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c2ce1bf627500ac9aec72c466865536bbff375e04a4e409655bbdf2827c1a`  
		Last Modified: Fri, 24 Apr 2020 02:04:53 GMT  
		Size: 1.8 MB (1822716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14a8989d4305a13a6c1fbfab29671cacd99035dd4291710ba978fd29283481`  
		Last Modified: Fri, 24 Apr 2020 02:04:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0b1f8e9eedb57e967305efe997babe0185ba6f7fe9eb7f4cbed6ee3d3f4dbe`  
		Last Modified: Fri, 24 Apr 2020 02:05:12 GMT  
		Size: 59.9 MB (59927054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc59092f5c3af9ff086a7203470a39d43b9ba5593cdd2eb494796a245ce8ecd4`  
		Last Modified: Fri, 24 Apr 2020 02:04:52 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f54a6c116900f095c4bce429f827a4dcc0af52c0634e42b3f83a9f5ea321d39`  
		Last Modified: Fri, 24 Apr 2020 02:04:51 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb98a21ac35e0dd075007407e66183792d9dbc8c997513d6592918018b5312a`  
		Last Modified: Fri, 24 Apr 2020 02:04:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2b175115645c91b877c5783ddd6faf72ccddb1584eabd8187f8f8def8c2e17`  
		Last Modified: Fri, 24 Apr 2020 02:05:44 GMT  
		Size: 7.0 MB (7031330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:836a38373d532ac55e66096590e2d8c7b4833cf0cfabd80c0f004d050080a74c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76831460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d961e0b3d34ce5f4ae39dcadff0006d5afcddf128492dfb2da665a0fb5c0d3ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:42:09 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 03:42:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:42:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:42:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:42:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:42:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:42:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:42:32 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 03:43:08 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330b718f631fe67ed5c2ddee0ac1f74cb77a1211022efb33aa66f6f5d6d2f05f`  
		Last Modified: Fri, 11 Dec 2020 03:45:09 GMT  
		Size: 63.6 MB (63558264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a938160415222146a455ed7ddae6e01d0c41f91a764f77ac05ed9794d08adf6a`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb6da89ff942a1c917a6a29653eb45dfc3826f334b16e17bc82207ce1193cc4`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a70c0c122f402fb4ee26f6661b037f3e6ee30e639f710e4f318dbf908e60a65`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99c483ed624af2276f16b538d32a3eec95bb4309d636878022d76d74bae9def`  
		Last Modified: Fri, 11 Dec 2020 03:45:39 GMT  
		Size: 8.5 MB (8503468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:11663df6a04f355f0d726c8ae20de03ee3b1ef1008bbb63027d0e13b137a8186
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:48c45a5da08acef9293e5fa4d6527d1ba39689a498df135e8f5e0d90fa4b7f33
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74295694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aefe523efa57aaf5952272f1f3b1d4ccecd638bdfe3719304a9f7b5e464ec1cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:29:34 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 05:29:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:29:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:29:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:42 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e060f4bd70b333ccaa7ae441b42f1068621b39bbe8eb9c71b5a4e06d10b4ff3`  
		Last Modified: Fri, 11 Dec 2020 05:31:46 GMT  
		Size: 69.5 MB (69457871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e8d568a22304aafab5a456040525abd0b705efad0b6e60e64847ebe1c6e4e6`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc6ef1a942a0f6b2ab0993eecb7ce30d31f06af50a2ae40893e1a160c9a0892`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2312dd95470aa8eaccef80bbca7892390ca777559b50fab574e65147a35107fc`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm variant v6

```console
$ docker pull docker@sha256:18d39b6848cecae067cc0d94c554029bfc88d3069c80bb5049d54da659249b94
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64475654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3106fcafb44a465ee4e0efadc103e5018d57587bd5d5ba6f465846bf7c3844`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:12:47 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 23 Apr 2020 17:12:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 17:12:50 GMT
ENV DOCKER_CHANNEL=stable
# Thu, 23 Apr 2020 17:12:51 GMT
ENV DOCKER_VERSION=19.03.8
# Thu, 23 Apr 2020 17:13:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 23 Apr 2020 17:13:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 23 Apr 2020 17:13:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:13:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 23 Apr 2020 17:13:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 23 Apr 2020 17:13:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 17:13:07 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcb342235c0ef85c7b7836ba057f513df540f983f4dbe5587035824aec248ab`  
		Last Modified: Thu, 23 Apr 2020 17:14:04 GMT  
		Size: 1.9 MB (1926703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94018ec82f0af1c26efba50dc99b07f2db1d2fbfab94f814ca9e1b5147c73e56`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593e1c01de3a8ad095d83439f0112c9a534fe764682e7a0f99d0a5794f914591`  
		Last Modified: Thu, 23 Apr 2020 17:14:22 GMT  
		Size: 59.9 MB (59927152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3737124780efb66a0753c8acdb04e12dad9a04b3362b1496cfe1e1dcf2d60b`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a76f66eab7a2e5314dd5973bcbb4ab91a025072e77fd14a83ab87d5ed8cc39`  
		Last Modified: Thu, 23 Apr 2020 17:14:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e1037ca5d5c489e9b1a5f1433e4d8be4b012c29ef660e05769c63bfbd63812`  
		Last Modified: Thu, 23 Apr 2020 17:14:02 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm variant v7

```console
$ docker pull docker@sha256:ce46ea18798c578f8923e0ced4c9996c30363fc35edd1b1c40e5e542407818ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64173697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81a685736103d7a1e988f52fb20b130a353e545dff4ccd52c9b075d5ead6f11d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:03:44 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 24 Apr 2020 02:03:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 02:03:47 GMT
ENV DOCKER_CHANNEL=stable
# Fri, 24 Apr 2020 02:03:48 GMT
ENV DOCKER_VERSION=19.03.8
# Fri, 24 Apr 2020 02:03:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 24 Apr 2020 02:04:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 24 Apr 2020 02:04:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 24 Apr 2020 02:04:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 24 Apr 2020 02:04:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 24 Apr 2020 02:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 02:04:05 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c2ce1bf627500ac9aec72c466865536bbff375e04a4e409655bbdf2827c1a`  
		Last Modified: Fri, 24 Apr 2020 02:04:53 GMT  
		Size: 1.8 MB (1822716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14a8989d4305a13a6c1fbfab29671cacd99035dd4291710ba978fd29283481`  
		Last Modified: Fri, 24 Apr 2020 02:04:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0b1f8e9eedb57e967305efe997babe0185ba6f7fe9eb7f4cbed6ee3d3f4dbe`  
		Last Modified: Fri, 24 Apr 2020 02:05:12 GMT  
		Size: 59.9 MB (59927054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc59092f5c3af9ff086a7203470a39d43b9ba5593cdd2eb494796a245ce8ecd4`  
		Last Modified: Fri, 24 Apr 2020 02:04:52 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f54a6c116900f095c4bce429f827a4dcc0af52c0634e42b3f83a9f5ea321d39`  
		Last Modified: Fri, 24 Apr 2020 02:04:51 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb98a21ac35e0dd075007407e66183792d9dbc8c997513d6592918018b5312a`  
		Last Modified: Fri, 24 Apr 2020 02:04:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f65a8021b3332e2cfe3498c23cf10ccd0010db66f6f0bc1fb65dff8d280b9ab8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68327992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeaf43b927733dcfd7b87c5a733c444df7c3d364e065dbebfdc2271d9caaa502`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:42:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 03:42:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:42:09 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 03:42:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 03:42:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 03:42:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:42:28 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 03:42:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 03:42:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:42:32 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a3295e0d61f852e263682a8285a62d0f4f5832be86af681abc9950847b3bf5`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 2.1 MB (2061244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f2e6d810069d5f3f3f5d961a35cf03d93a9046b8c37f0c5ad37b6c975f42b`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330b718f631fe67ed5c2ddee0ac1f74cb77a1211022efb33aa66f6f5d6d2f05f`  
		Last Modified: Fri, 11 Dec 2020 03:45:09 GMT  
		Size: 63.6 MB (63558264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a938160415222146a455ed7ddae6e01d0c41f91a764f77ac05ed9794d08adf6a`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb6da89ff942a1c917a6a29653eb45dfc3826f334b16e17bc82207ce1193cc4`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a70c0c122f402fb4ee26f6661b037f3e6ee30e639f710e4f318dbf908e60a65`  
		Last Modified: Fri, 11 Dec 2020 03:44:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
