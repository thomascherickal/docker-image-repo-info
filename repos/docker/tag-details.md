<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `docker`

-	[`docker:19`](#docker19)
-	[`docker:19.03`](#docker1903)
-	[`docker:19.03.15`](#docker190315)
-	[`docker:19.03.15-dind`](#docker190315-dind)
-	[`docker:19.03.15-dind-rootless`](#docker190315-dind-rootless)
-	[`docker:19.03.15-git`](#docker190315-git)
-	[`docker:19.03-dind`](#docker1903-dind)
-	[`docker:19.03-dind-rootless`](#docker1903-dind-rootless)
-	[`docker:19.03-git`](#docker1903-git)
-	[`docker:19-dind`](#docker19-dind)
-	[`docker:19-dind-rootless`](#docker19-dind-rootless)
-	[`docker:19-git`](#docker19-git)
-	[`docker:20`](#docker20)
-	[`docker:20.10`](#docker2010)
-	[`docker:20.10.3`](#docker20103)
-	[`docker:20.10.3-dind`](#docker20103-dind)
-	[`docker:20.10.3-dind-rootless`](#docker20103-dind-rootless)
-	[`docker:20.10.3-git`](#docker20103-git)
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
$ docker pull docker@sha256:4ee4236786271c53a36f9d85dcfd22376aa30afaa2a5e60b7929443ad69eb4cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19` - linux; amd64

```console
$ docker pull docker@sha256:4d89175b377bf65ade07c1f6e2967dd00fcdd5b3595d834cd135d3d045ad8d0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67747492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:934a8cac43d24b718300e155709c2cf6e2741ed3df5cb315e554dcaf84aa5746`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:13:09 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 02:13:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:13:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:13:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:13:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:13:19 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4db05ddd5899af30ee0c5795aec2b49ac9d71df0cc4cb94f6e0dd1a9d444b02`  
		Last Modified: Tue, 02 Feb 2021 02:15:09 GMT  
		Size: 62.9 MB (62882884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b5eba8b232ce16e5ee1c005b5474ce8c4ace39ebb54702cc2bd6494566636b`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bece180336fa27595ce33fedc51ec456725fa8da0fc5501ad698ab630352f15`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ed15b4f9e6397f01e3e062ac8fd3c0963368a642364660b3ce1de4fa7da789`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 117.0 B  
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
$ docker pull docker@sha256:6d28aa7e401298c015164e2b80ec4a3fc8b0af4bb9be4fe262b93f1e2e02c904
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60775500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c11ce0c45f83bb238b427793a9e70322ade153b18da5e7c2a76d0f398f8adfb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:08:16 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 01:08:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:08:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:08:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:08:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:08:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:08:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:08:29 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfacbe7a8297873d53ccd2934031ffd983d26a38c0d64c06ba89adc9a46e63f`  
		Last Modified: Tue, 02 Feb 2021 01:10:27 GMT  
		Size: 56.0 MB (55994350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59108e83ffd61d3abc101dadee24a3ff5510599266412671a77d06ebaab7351`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a749801b4affc00866ba4d39c4b287abe71dc3cca1e21fe88dbc432c72f9afe4`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e89e1ae2f76fef0ae611ca185f8e843df107f37f0f4128f6db6f0482c817c67`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03`

```console
$ docker pull docker@sha256:4ee4236786271c53a36f9d85dcfd22376aa30afaa2a5e60b7929443ad69eb4cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03` - linux; amd64

```console
$ docker pull docker@sha256:4d89175b377bf65ade07c1f6e2967dd00fcdd5b3595d834cd135d3d045ad8d0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67747492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:934a8cac43d24b718300e155709c2cf6e2741ed3df5cb315e554dcaf84aa5746`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:13:09 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 02:13:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:13:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:13:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:13:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:13:19 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4db05ddd5899af30ee0c5795aec2b49ac9d71df0cc4cb94f6e0dd1a9d444b02`  
		Last Modified: Tue, 02 Feb 2021 02:15:09 GMT  
		Size: 62.9 MB (62882884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b5eba8b232ce16e5ee1c005b5474ce8c4ace39ebb54702cc2bd6494566636b`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bece180336fa27595ce33fedc51ec456725fa8da0fc5501ad698ab630352f15`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ed15b4f9e6397f01e3e062ac8fd3c0963368a642364660b3ce1de4fa7da789`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 117.0 B  
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
$ docker pull docker@sha256:6d28aa7e401298c015164e2b80ec4a3fc8b0af4bb9be4fe262b93f1e2e02c904
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60775500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c11ce0c45f83bb238b427793a9e70322ade153b18da5e7c2a76d0f398f8adfb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:08:16 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 01:08:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:08:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:08:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:08:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:08:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:08:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:08:29 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfacbe7a8297873d53ccd2934031ffd983d26a38c0d64c06ba89adc9a46e63f`  
		Last Modified: Tue, 02 Feb 2021 01:10:27 GMT  
		Size: 56.0 MB (55994350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59108e83ffd61d3abc101dadee24a3ff5510599266412671a77d06ebaab7351`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a749801b4affc00866ba4d39c4b287abe71dc3cca1e21fe88dbc432c72f9afe4`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e89e1ae2f76fef0ae611ca185f8e843df107f37f0f4128f6db6f0482c817c67`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.15`

```console
$ docker pull docker@sha256:3b7414686e1bdb833f8ee24400b94e7c591a4e8605721b13db6791cacc5b0dd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:19.03.15` - linux; amd64

```console
$ docker pull docker@sha256:4d89175b377bf65ade07c1f6e2967dd00fcdd5b3595d834cd135d3d045ad8d0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67747492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:934a8cac43d24b718300e155709c2cf6e2741ed3df5cb315e554dcaf84aa5746`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:13:09 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 02:13:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:13:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:13:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:13:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:13:19 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4db05ddd5899af30ee0c5795aec2b49ac9d71df0cc4cb94f6e0dd1a9d444b02`  
		Last Modified: Tue, 02 Feb 2021 02:15:09 GMT  
		Size: 62.9 MB (62882884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b5eba8b232ce16e5ee1c005b5474ce8c4ace39ebb54702cc2bd6494566636b`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bece180336fa27595ce33fedc51ec456725fa8da0fc5501ad698ab630352f15`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ed15b4f9e6397f01e3e062ac8fd3c0963368a642364660b3ce1de4fa7da789`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.15` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:6d28aa7e401298c015164e2b80ec4a3fc8b0af4bb9be4fe262b93f1e2e02c904
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60775500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c11ce0c45f83bb238b427793a9e70322ade153b18da5e7c2a76d0f398f8adfb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:08:16 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 01:08:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:08:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:08:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:08:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:08:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:08:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:08:29 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfacbe7a8297873d53ccd2934031ffd983d26a38c0d64c06ba89adc9a46e63f`  
		Last Modified: Tue, 02 Feb 2021 01:10:27 GMT  
		Size: 56.0 MB (55994350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59108e83ffd61d3abc101dadee24a3ff5510599266412671a77d06ebaab7351`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a749801b4affc00866ba4d39c4b287abe71dc3cca1e21fe88dbc432c72f9afe4`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e89e1ae2f76fef0ae611ca185f8e843df107f37f0f4128f6db6f0482c817c67`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.15-dind`

```console
$ docker pull docker@sha256:12f8a523856d362e02432383135814828a1053e4f81a790bb3cf0b1b3a25f4d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:19.03.15-dind` - linux; amd64

```console
$ docker pull docker@sha256:1c0f0b3eed91743c6d2187dfc8656e8304d2d608f49c55b1210abbf5d47ce5d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74321798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0b6edc4e726ecab75cdb33715cb9e54dbd4430c953204bc33d941ce77154c76`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:13:09 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 02:13:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:13:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:13:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:13:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:13:19 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:13:25 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 02:13:26 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:13:26 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 02:13:28 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 02:13:28 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:13:28 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 02:13:28 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 02:13:28 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 02:13:29 GMT
CMD []
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4db05ddd5899af30ee0c5795aec2b49ac9d71df0cc4cb94f6e0dd1a9d444b02`  
		Last Modified: Tue, 02 Feb 2021 02:15:09 GMT  
		Size: 62.9 MB (62882884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b5eba8b232ce16e5ee1c005b5474ce8c4ace39ebb54702cc2bd6494566636b`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bece180336fa27595ce33fedc51ec456725fa8da0fc5501ad698ab630352f15`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ed15b4f9e6397f01e3e062ac8fd3c0963368a642364660b3ce1de4fa7da789`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a63ba1d9089b3bebe2f96e7531317a35bc1b9ee116a34230036cfb0c9dfce17`  
		Last Modified: Tue, 02 Feb 2021 02:15:16 GMT  
		Size: 6.6 MB (6569583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbbb8fe7a5d45862302213cc2177f69dd10b125332de13a02d16dbfca7eddbf`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b267352ad78ddb70e7fdf7d8904ee6ccdfddce228541c8fbbff0d1fde2785be6`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8000174dfbac9b913dd3a6f82102a020e542eb48afe878dccf5a75f237dba345`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 2.5 KB (2511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.15-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f6d9a8220cc07b17f39b1a3c94b794b220f2f5f95ec64f187b55a332e73ac9c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67253355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf086d7ce26eda0cdb992fafd1d435aca2c3971e72be1aec2a87a5c536b7915`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:08:16 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 01:08:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:08:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:08:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:08:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:08:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:08:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:08:29 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 01:08:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 01:08:41 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 01:08:41 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 01:08:43 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 01:08:44 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:08:45 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 01:08:45 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 01:08:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 01:08:47 GMT
CMD []
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfacbe7a8297873d53ccd2934031ffd983d26a38c0d64c06ba89adc9a46e63f`  
		Last Modified: Tue, 02 Feb 2021 01:10:27 GMT  
		Size: 56.0 MB (55994350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59108e83ffd61d3abc101dadee24a3ff5510599266412671a77d06ebaab7351`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a749801b4affc00866ba4d39c4b287abe71dc3cca1e21fe88dbc432c72f9afe4`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e89e1ae2f76fef0ae611ca185f8e843df107f37f0f4128f6db6f0482c817c67`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c0709505cc9bc0bc89250f09e36fec093b8ae5789ccf75958524ce4564b73c`  
		Last Modified: Tue, 02 Feb 2021 01:10:37 GMT  
		Size: 6.5 MB (6473103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1706fe37b0b88d619d5c9f5a2356bfa3c0872e72142fcd31fea3ad9a5165bd6`  
		Last Modified: Tue, 02 Feb 2021 01:10:35 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64b9ac91b40e871e83f892869b01590132bddeb2b981842bbc124a01a866ff4`  
		Last Modified: Tue, 02 Feb 2021 01:10:35 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c319efdbbbb5fc9252e24938e21173504d7af8f5675f0a0c2c92f9a51caa94cf`  
		Last Modified: Tue, 02 Feb 2021 01:10:35 GMT  
		Size: 2.5 KB (2510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.15-dind-rootless`

```console
$ docker pull docker@sha256:259dbf2fe0cc6d23c2a42caf0da1f0778fc850c26301657800fcc7d70086cd7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19.03.15-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:711ea28bf1f83af6b95c7122285a72af394304666c1b0bb74cc204cf0dd945ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94877543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32b072e6af370115fea331dd17919372cce51fa1e8c342b1a4c5d1eb4fc06e90`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:13:09 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 02:13:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:13:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:13:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:13:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:13:19 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:13:25 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 02:13:26 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:13:26 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 02:13:28 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 02:13:28 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:13:28 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 02:13:28 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 02:13:28 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 02:13:29 GMT
CMD []
# Tue, 02 Feb 2021 02:13:34 GMT
RUN apk add --no-cache iproute2
# Tue, 02 Feb 2021 02:13:35 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 02 Feb 2021 02:13:36 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:13:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 02 Feb 2021 02:13:40 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 02 Feb 2021 02:13:40 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 02 Feb 2021 02:13:40 GMT
USER rootless
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4db05ddd5899af30ee0c5795aec2b49ac9d71df0cc4cb94f6e0dd1a9d444b02`  
		Last Modified: Tue, 02 Feb 2021 02:15:09 GMT  
		Size: 62.9 MB (62882884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b5eba8b232ce16e5ee1c005b5474ce8c4ace39ebb54702cc2bd6494566636b`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bece180336fa27595ce33fedc51ec456725fa8da0fc5501ad698ab630352f15`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ed15b4f9e6397f01e3e062ac8fd3c0963368a642364660b3ce1de4fa7da789`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a63ba1d9089b3bebe2f96e7531317a35bc1b9ee116a34230036cfb0c9dfce17`  
		Last Modified: Tue, 02 Feb 2021 02:15:16 GMT  
		Size: 6.6 MB (6569583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbbb8fe7a5d45862302213cc2177f69dd10b125332de13a02d16dbfca7eddbf`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b267352ad78ddb70e7fdf7d8904ee6ccdfddce228541c8fbbff0d1fde2785be6`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8000174dfbac9b913dd3a6f82102a020e542eb48afe878dccf5a75f237dba345`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 2.5 KB (2511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a4e48614a44dbccd302d9c92fc5a86a79e863407c4430ee408de62defc66e3`  
		Last Modified: Tue, 02 Feb 2021 02:15:21 GMT  
		Size: 1.1 MB (1131433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff619e5e99aaf0556af66c31f305e3b054d8919f548d75b6abc09569bad530fe`  
		Last Modified: Tue, 02 Feb 2021 02:15:21 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17a0e7edbf7c145009ebf83b802edaae0acd03cbf04c6364ea3dfa4b85b22c9`  
		Last Modified: Tue, 02 Feb 2021 02:15:21 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a87220e4b94b4e720025144dae539d9e7a18dea719110830f32e76eeab0ea`  
		Last Modified: Tue, 02 Feb 2021 02:15:25 GMT  
		Size: 19.4 MB (19422701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e608ad6fa13da7ec47bdb2d866d9b83da78fb3de0e3f38dc4d099523608c63`  
		Last Modified: Tue, 02 Feb 2021 02:15:21 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.15-git`

```console
$ docker pull docker@sha256:bcd906510c51f636a4010d083fb9d1036e292e7d7e8aa10e53097b53d56cb2ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:19.03.15-git` - linux; amd64

```console
$ docker pull docker@sha256:cbb17781340bb4b808afc1fcdcc80f20b7479d143fcedb84238bd14aef165e8d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74136981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03d59e379976cf7f5a08850560d0249dfdde7452dffd83ecf2be927929f0439a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:13:09 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 02:13:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:13:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:13:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:13:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:13:19 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:13:47 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4db05ddd5899af30ee0c5795aec2b49ac9d71df0cc4cb94f6e0dd1a9d444b02`  
		Last Modified: Tue, 02 Feb 2021 02:15:09 GMT  
		Size: 62.9 MB (62882884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b5eba8b232ce16e5ee1c005b5474ce8c4ace39ebb54702cc2bd6494566636b`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bece180336fa27595ce33fedc51ec456725fa8da0fc5501ad698ab630352f15`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ed15b4f9e6397f01e3e062ac8fd3c0963368a642364660b3ce1de4fa7da789`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5965746c9a6b15b0f892e7835f368468857e61e769db8a89040e83b1d6f044c`  
		Last Modified: Tue, 02 Feb 2021 02:15:32 GMT  
		Size: 6.4 MB (6389489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.15-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:d9d3a928f0dc16c35f575c3b5cf05ddd4455430138242c8913c95dba6dfa09f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67250256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bebe02fc5bdc194a1a8524a0c5761b75d1112cc1bc12c21748e47244e645566`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:08:16 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 01:08:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:08:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:08:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:08:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:08:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:08:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:08:29 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 01:08:56 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfacbe7a8297873d53ccd2934031ffd983d26a38c0d64c06ba89adc9a46e63f`  
		Last Modified: Tue, 02 Feb 2021 01:10:27 GMT  
		Size: 56.0 MB (55994350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59108e83ffd61d3abc101dadee24a3ff5510599266412671a77d06ebaab7351`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a749801b4affc00866ba4d39c4b287abe71dc3cca1e21fe88dbc432c72f9afe4`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e89e1ae2f76fef0ae611ca185f8e843df107f37f0f4128f6db6f0482c817c67`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61605ccdd4993c4feac68657359616285bcbe0f273a264802a598b0e8fcddbc`  
		Last Modified: Tue, 02 Feb 2021 01:10:51 GMT  
		Size: 6.5 MB (6474756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-dind`

```console
$ docker pull docker@sha256:3f102649d944f417085acce09362927f8a6371c919c044ff1176d5c4c007f351
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03-dind` - linux; amd64

```console
$ docker pull docker@sha256:1c0f0b3eed91743c6d2187dfc8656e8304d2d608f49c55b1210abbf5d47ce5d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74321798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0b6edc4e726ecab75cdb33715cb9e54dbd4430c953204bc33d941ce77154c76`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:13:09 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 02:13:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:13:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:13:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:13:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:13:19 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:13:25 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 02:13:26 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:13:26 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 02:13:28 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 02:13:28 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:13:28 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 02:13:28 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 02:13:28 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 02:13:29 GMT
CMD []
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4db05ddd5899af30ee0c5795aec2b49ac9d71df0cc4cb94f6e0dd1a9d444b02`  
		Last Modified: Tue, 02 Feb 2021 02:15:09 GMT  
		Size: 62.9 MB (62882884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b5eba8b232ce16e5ee1c005b5474ce8c4ace39ebb54702cc2bd6494566636b`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bece180336fa27595ce33fedc51ec456725fa8da0fc5501ad698ab630352f15`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ed15b4f9e6397f01e3e062ac8fd3c0963368a642364660b3ce1de4fa7da789`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a63ba1d9089b3bebe2f96e7531317a35bc1b9ee116a34230036cfb0c9dfce17`  
		Last Modified: Tue, 02 Feb 2021 02:15:16 GMT  
		Size: 6.6 MB (6569583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbbb8fe7a5d45862302213cc2177f69dd10b125332de13a02d16dbfca7eddbf`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b267352ad78ddb70e7fdf7d8904ee6ccdfddce228541c8fbbff0d1fde2785be6`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8000174dfbac9b913dd3a6f82102a020e542eb48afe878dccf5a75f237dba345`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 2.5 KB (2511 bytes)  
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
$ docker pull docker@sha256:f6d9a8220cc07b17f39b1a3c94b794b220f2f5f95ec64f187b55a332e73ac9c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67253355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf086d7ce26eda0cdb992fafd1d435aca2c3971e72be1aec2a87a5c536b7915`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:08:16 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 01:08:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:08:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:08:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:08:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:08:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:08:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:08:29 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 01:08:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 01:08:41 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 01:08:41 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 01:08:43 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 01:08:44 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:08:45 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 01:08:45 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 01:08:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 01:08:47 GMT
CMD []
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfacbe7a8297873d53ccd2934031ffd983d26a38c0d64c06ba89adc9a46e63f`  
		Last Modified: Tue, 02 Feb 2021 01:10:27 GMT  
		Size: 56.0 MB (55994350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59108e83ffd61d3abc101dadee24a3ff5510599266412671a77d06ebaab7351`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a749801b4affc00866ba4d39c4b287abe71dc3cca1e21fe88dbc432c72f9afe4`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e89e1ae2f76fef0ae611ca185f8e843df107f37f0f4128f6db6f0482c817c67`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c0709505cc9bc0bc89250f09e36fec093b8ae5789ccf75958524ce4564b73c`  
		Last Modified: Tue, 02 Feb 2021 01:10:37 GMT  
		Size: 6.5 MB (6473103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1706fe37b0b88d619d5c9f5a2356bfa3c0872e72142fcd31fea3ad9a5165bd6`  
		Last Modified: Tue, 02 Feb 2021 01:10:35 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64b9ac91b40e871e83f892869b01590132bddeb2b981842bbc124a01a866ff4`  
		Last Modified: Tue, 02 Feb 2021 01:10:35 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c319efdbbbb5fc9252e24938e21173504d7af8f5675f0a0c2c92f9a51caa94cf`  
		Last Modified: Tue, 02 Feb 2021 01:10:35 GMT  
		Size: 2.5 KB (2510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-dind-rootless`

```console
$ docker pull docker@sha256:259dbf2fe0cc6d23c2a42caf0da1f0778fc850c26301657800fcc7d70086cd7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19.03-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:711ea28bf1f83af6b95c7122285a72af394304666c1b0bb74cc204cf0dd945ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94877543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32b072e6af370115fea331dd17919372cce51fa1e8c342b1a4c5d1eb4fc06e90`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:13:09 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 02:13:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:13:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:13:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:13:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:13:19 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:13:25 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 02:13:26 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:13:26 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 02:13:28 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 02:13:28 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:13:28 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 02:13:28 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 02:13:28 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 02:13:29 GMT
CMD []
# Tue, 02 Feb 2021 02:13:34 GMT
RUN apk add --no-cache iproute2
# Tue, 02 Feb 2021 02:13:35 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 02 Feb 2021 02:13:36 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:13:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 02 Feb 2021 02:13:40 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 02 Feb 2021 02:13:40 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 02 Feb 2021 02:13:40 GMT
USER rootless
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4db05ddd5899af30ee0c5795aec2b49ac9d71df0cc4cb94f6e0dd1a9d444b02`  
		Last Modified: Tue, 02 Feb 2021 02:15:09 GMT  
		Size: 62.9 MB (62882884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b5eba8b232ce16e5ee1c005b5474ce8c4ace39ebb54702cc2bd6494566636b`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bece180336fa27595ce33fedc51ec456725fa8da0fc5501ad698ab630352f15`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ed15b4f9e6397f01e3e062ac8fd3c0963368a642364660b3ce1de4fa7da789`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a63ba1d9089b3bebe2f96e7531317a35bc1b9ee116a34230036cfb0c9dfce17`  
		Last Modified: Tue, 02 Feb 2021 02:15:16 GMT  
		Size: 6.6 MB (6569583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbbb8fe7a5d45862302213cc2177f69dd10b125332de13a02d16dbfca7eddbf`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b267352ad78ddb70e7fdf7d8904ee6ccdfddce228541c8fbbff0d1fde2785be6`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8000174dfbac9b913dd3a6f82102a020e542eb48afe878dccf5a75f237dba345`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 2.5 KB (2511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a4e48614a44dbccd302d9c92fc5a86a79e863407c4430ee408de62defc66e3`  
		Last Modified: Tue, 02 Feb 2021 02:15:21 GMT  
		Size: 1.1 MB (1131433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff619e5e99aaf0556af66c31f305e3b054d8919f548d75b6abc09569bad530fe`  
		Last Modified: Tue, 02 Feb 2021 02:15:21 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17a0e7edbf7c145009ebf83b802edaae0acd03cbf04c6364ea3dfa4b85b22c9`  
		Last Modified: Tue, 02 Feb 2021 02:15:21 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a87220e4b94b4e720025144dae539d9e7a18dea719110830f32e76eeab0ea`  
		Last Modified: Tue, 02 Feb 2021 02:15:25 GMT  
		Size: 19.4 MB (19422701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e608ad6fa13da7ec47bdb2d866d9b83da78fb3de0e3f38dc4d099523608c63`  
		Last Modified: Tue, 02 Feb 2021 02:15:21 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-git`

```console
$ docker pull docker@sha256:6b62f3414d76aae8d8bfcd7b271eadf5db30a38b290bfcaebea2d8273aeaf7ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03-git` - linux; amd64

```console
$ docker pull docker@sha256:cbb17781340bb4b808afc1fcdcc80f20b7479d143fcedb84238bd14aef165e8d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74136981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03d59e379976cf7f5a08850560d0249dfdde7452dffd83ecf2be927929f0439a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:13:09 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 02:13:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:13:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:13:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:13:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:13:19 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:13:47 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4db05ddd5899af30ee0c5795aec2b49ac9d71df0cc4cb94f6e0dd1a9d444b02`  
		Last Modified: Tue, 02 Feb 2021 02:15:09 GMT  
		Size: 62.9 MB (62882884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b5eba8b232ce16e5ee1c005b5474ce8c4ace39ebb54702cc2bd6494566636b`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bece180336fa27595ce33fedc51ec456725fa8da0fc5501ad698ab630352f15`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ed15b4f9e6397f01e3e062ac8fd3c0963368a642364660b3ce1de4fa7da789`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5965746c9a6b15b0f892e7835f368468857e61e769db8a89040e83b1d6f044c`  
		Last Modified: Tue, 02 Feb 2021 02:15:32 GMT  
		Size: 6.4 MB (6389489 bytes)  
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
$ docker pull docker@sha256:d9d3a928f0dc16c35f575c3b5cf05ddd4455430138242c8913c95dba6dfa09f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67250256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bebe02fc5bdc194a1a8524a0c5761b75d1112cc1bc12c21748e47244e645566`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:08:16 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 01:08:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:08:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:08:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:08:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:08:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:08:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:08:29 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 01:08:56 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfacbe7a8297873d53ccd2934031ffd983d26a38c0d64c06ba89adc9a46e63f`  
		Last Modified: Tue, 02 Feb 2021 01:10:27 GMT  
		Size: 56.0 MB (55994350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59108e83ffd61d3abc101dadee24a3ff5510599266412671a77d06ebaab7351`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a749801b4affc00866ba4d39c4b287abe71dc3cca1e21fe88dbc432c72f9afe4`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e89e1ae2f76fef0ae611ca185f8e843df107f37f0f4128f6db6f0482c817c67`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61605ccdd4993c4feac68657359616285bcbe0f273a264802a598b0e8fcddbc`  
		Last Modified: Tue, 02 Feb 2021 01:10:51 GMT  
		Size: 6.5 MB (6474756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19-dind`

```console
$ docker pull docker@sha256:3f102649d944f417085acce09362927f8a6371c919c044ff1176d5c4c007f351
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19-dind` - linux; amd64

```console
$ docker pull docker@sha256:1c0f0b3eed91743c6d2187dfc8656e8304d2d608f49c55b1210abbf5d47ce5d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74321798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0b6edc4e726ecab75cdb33715cb9e54dbd4430c953204bc33d941ce77154c76`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:13:09 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 02:13:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:13:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:13:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:13:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:13:19 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:13:25 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 02:13:26 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:13:26 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 02:13:28 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 02:13:28 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:13:28 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 02:13:28 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 02:13:28 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 02:13:29 GMT
CMD []
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4db05ddd5899af30ee0c5795aec2b49ac9d71df0cc4cb94f6e0dd1a9d444b02`  
		Last Modified: Tue, 02 Feb 2021 02:15:09 GMT  
		Size: 62.9 MB (62882884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b5eba8b232ce16e5ee1c005b5474ce8c4ace39ebb54702cc2bd6494566636b`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bece180336fa27595ce33fedc51ec456725fa8da0fc5501ad698ab630352f15`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ed15b4f9e6397f01e3e062ac8fd3c0963368a642364660b3ce1de4fa7da789`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a63ba1d9089b3bebe2f96e7531317a35bc1b9ee116a34230036cfb0c9dfce17`  
		Last Modified: Tue, 02 Feb 2021 02:15:16 GMT  
		Size: 6.6 MB (6569583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbbb8fe7a5d45862302213cc2177f69dd10b125332de13a02d16dbfca7eddbf`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b267352ad78ddb70e7fdf7d8904ee6ccdfddce228541c8fbbff0d1fde2785be6`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8000174dfbac9b913dd3a6f82102a020e542eb48afe878dccf5a75f237dba345`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 2.5 KB (2511 bytes)  
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
$ docker pull docker@sha256:f6d9a8220cc07b17f39b1a3c94b794b220f2f5f95ec64f187b55a332e73ac9c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67253355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf086d7ce26eda0cdb992fafd1d435aca2c3971e72be1aec2a87a5c536b7915`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:08:16 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 01:08:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:08:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:08:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:08:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:08:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:08:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:08:29 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 01:08:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 01:08:41 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 01:08:41 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 01:08:43 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 01:08:44 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:08:45 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 01:08:45 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 01:08:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 01:08:47 GMT
CMD []
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfacbe7a8297873d53ccd2934031ffd983d26a38c0d64c06ba89adc9a46e63f`  
		Last Modified: Tue, 02 Feb 2021 01:10:27 GMT  
		Size: 56.0 MB (55994350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59108e83ffd61d3abc101dadee24a3ff5510599266412671a77d06ebaab7351`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a749801b4affc00866ba4d39c4b287abe71dc3cca1e21fe88dbc432c72f9afe4`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e89e1ae2f76fef0ae611ca185f8e843df107f37f0f4128f6db6f0482c817c67`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c0709505cc9bc0bc89250f09e36fec093b8ae5789ccf75958524ce4564b73c`  
		Last Modified: Tue, 02 Feb 2021 01:10:37 GMT  
		Size: 6.5 MB (6473103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1706fe37b0b88d619d5c9f5a2356bfa3c0872e72142fcd31fea3ad9a5165bd6`  
		Last Modified: Tue, 02 Feb 2021 01:10:35 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64b9ac91b40e871e83f892869b01590132bddeb2b981842bbc124a01a866ff4`  
		Last Modified: Tue, 02 Feb 2021 01:10:35 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c319efdbbbb5fc9252e24938e21173504d7af8f5675f0a0c2c92f9a51caa94cf`  
		Last Modified: Tue, 02 Feb 2021 01:10:35 GMT  
		Size: 2.5 KB (2510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19-dind-rootless`

```console
$ docker pull docker@sha256:259dbf2fe0cc6d23c2a42caf0da1f0778fc850c26301657800fcc7d70086cd7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:711ea28bf1f83af6b95c7122285a72af394304666c1b0bb74cc204cf0dd945ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94877543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32b072e6af370115fea331dd17919372cce51fa1e8c342b1a4c5d1eb4fc06e90`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:13:09 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 02:13:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:13:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:13:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:13:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:13:19 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:13:25 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 02:13:26 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:13:26 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 02:13:28 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 02:13:28 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:13:28 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 02:13:28 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 02:13:28 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 02:13:29 GMT
CMD []
# Tue, 02 Feb 2021 02:13:34 GMT
RUN apk add --no-cache iproute2
# Tue, 02 Feb 2021 02:13:35 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 02 Feb 2021 02:13:36 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:13:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 02 Feb 2021 02:13:40 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 02 Feb 2021 02:13:40 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 02 Feb 2021 02:13:40 GMT
USER rootless
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4db05ddd5899af30ee0c5795aec2b49ac9d71df0cc4cb94f6e0dd1a9d444b02`  
		Last Modified: Tue, 02 Feb 2021 02:15:09 GMT  
		Size: 62.9 MB (62882884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b5eba8b232ce16e5ee1c005b5474ce8c4ace39ebb54702cc2bd6494566636b`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bece180336fa27595ce33fedc51ec456725fa8da0fc5501ad698ab630352f15`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ed15b4f9e6397f01e3e062ac8fd3c0963368a642364660b3ce1de4fa7da789`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a63ba1d9089b3bebe2f96e7531317a35bc1b9ee116a34230036cfb0c9dfce17`  
		Last Modified: Tue, 02 Feb 2021 02:15:16 GMT  
		Size: 6.6 MB (6569583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbbb8fe7a5d45862302213cc2177f69dd10b125332de13a02d16dbfca7eddbf`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b267352ad78ddb70e7fdf7d8904ee6ccdfddce228541c8fbbff0d1fde2785be6`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8000174dfbac9b913dd3a6f82102a020e542eb48afe878dccf5a75f237dba345`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 2.5 KB (2511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a4e48614a44dbccd302d9c92fc5a86a79e863407c4430ee408de62defc66e3`  
		Last Modified: Tue, 02 Feb 2021 02:15:21 GMT  
		Size: 1.1 MB (1131433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff619e5e99aaf0556af66c31f305e3b054d8919f548d75b6abc09569bad530fe`  
		Last Modified: Tue, 02 Feb 2021 02:15:21 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17a0e7edbf7c145009ebf83b802edaae0acd03cbf04c6364ea3dfa4b85b22c9`  
		Last Modified: Tue, 02 Feb 2021 02:15:21 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a87220e4b94b4e720025144dae539d9e7a18dea719110830f32e76eeab0ea`  
		Last Modified: Tue, 02 Feb 2021 02:15:25 GMT  
		Size: 19.4 MB (19422701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e608ad6fa13da7ec47bdb2d866d9b83da78fb3de0e3f38dc4d099523608c63`  
		Last Modified: Tue, 02 Feb 2021 02:15:21 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19-git`

```console
$ docker pull docker@sha256:6b62f3414d76aae8d8bfcd7b271eadf5db30a38b290bfcaebea2d8273aeaf7ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19-git` - linux; amd64

```console
$ docker pull docker@sha256:cbb17781340bb4b808afc1fcdcc80f20b7479d143fcedb84238bd14aef165e8d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74136981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03d59e379976cf7f5a08850560d0249dfdde7452dffd83ecf2be927929f0439a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:13:09 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 02:13:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:13:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:13:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:13:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:13:19 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:13:47 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4db05ddd5899af30ee0c5795aec2b49ac9d71df0cc4cb94f6e0dd1a9d444b02`  
		Last Modified: Tue, 02 Feb 2021 02:15:09 GMT  
		Size: 62.9 MB (62882884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b5eba8b232ce16e5ee1c005b5474ce8c4ace39ebb54702cc2bd6494566636b`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bece180336fa27595ce33fedc51ec456725fa8da0fc5501ad698ab630352f15`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ed15b4f9e6397f01e3e062ac8fd3c0963368a642364660b3ce1de4fa7da789`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5965746c9a6b15b0f892e7835f368468857e61e769db8a89040e83b1d6f044c`  
		Last Modified: Tue, 02 Feb 2021 02:15:32 GMT  
		Size: 6.4 MB (6389489 bytes)  
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
$ docker pull docker@sha256:d9d3a928f0dc16c35f575c3b5cf05ddd4455430138242c8913c95dba6dfa09f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67250256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bebe02fc5bdc194a1a8524a0c5761b75d1112cc1bc12c21748e47244e645566`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:08:16 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 01:08:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:08:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:08:25 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:08:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:08:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:08:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:08:29 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 01:08:56 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfacbe7a8297873d53ccd2934031ffd983d26a38c0d64c06ba89adc9a46e63f`  
		Last Modified: Tue, 02 Feb 2021 01:10:27 GMT  
		Size: 56.0 MB (55994350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59108e83ffd61d3abc101dadee24a3ff5510599266412671a77d06ebaab7351`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a749801b4affc00866ba4d39c4b287abe71dc3cca1e21fe88dbc432c72f9afe4`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e89e1ae2f76fef0ae611ca185f8e843df107f37f0f4128f6db6f0482c817c67`  
		Last Modified: Tue, 02 Feb 2021 01:10:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61605ccdd4993c4feac68657359616285bcbe0f273a264802a598b0e8fcddbc`  
		Last Modified: Tue, 02 Feb 2021 01:10:51 GMT  
		Size: 6.5 MB (6474756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20`

```console
$ docker pull docker@sha256:950c22d6a7264d55ecaddc18be5f31da3a006d195cbe493a6dd1a55b89093854
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20` - linux; amd64

```console
$ docker pull docker@sha256:92d21018568e2ce434e492257c8333b5364566ab4fb47b9d9a069961ff81cb89
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74328888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e081696197d3ee50cccb7dc2c402da573d3a388eb7e2bc21c7ace31638a0f5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:12:24 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 02:12:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:12:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:12:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:35 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b102489fa5766c88e23ee2669f5da5315dc52527ecc33f4b1002a075d4464512`  
		Last Modified: Tue, 02 Feb 2021 02:14:28 GMT  
		Size: 69.5 MB (69464280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0085121e3c317ff3294353f5fc57d00fdd1281d8a974e777aefb7fad747f68`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b35ed1592a30ed19ce07f1c48826efb976b0e85a56fc4c7f45907e98e7344f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fabd30979878ac4c239f4eb3c17beb75bf1e76f77bb670c193db8709d896b9`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f7c2232e59d98f52fcd32679c9db88a62caa3d40a827ac793f6f028ce71535b7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68353383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ce399bb54c39a88a4b02d7e9c88f43afbcffb1a1da5e3905fef969364e9c63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:07:31 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 01:07:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:07:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:07:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:07:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:07:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:07:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:07:43 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ea4215e87a19277d3ad5191bd33bbc874d53668f5bab1d078e9be7be8fb12`  
		Last Modified: Tue, 02 Feb 2021 01:09:39 GMT  
		Size: 63.6 MB (63572234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afbccbf4e53fe57125e562dbb66792d01e4166e117597e31e419cab29894e3d`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b11151c2bc89ee34a665c25ced3ff48ae5a22718436d3ece90d6312884a09aa`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6a033d54e332e1f5c93adab630e5bd10f71a41174a5969dd6e3cac4ca58f5`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10`

```console
$ docker pull docker@sha256:950c22d6a7264d55ecaddc18be5f31da3a006d195cbe493a6dd1a55b89093854
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10` - linux; amd64

```console
$ docker pull docker@sha256:92d21018568e2ce434e492257c8333b5364566ab4fb47b9d9a069961ff81cb89
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74328888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e081696197d3ee50cccb7dc2c402da573d3a388eb7e2bc21c7ace31638a0f5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:12:24 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 02:12:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:12:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:12:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:35 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b102489fa5766c88e23ee2669f5da5315dc52527ecc33f4b1002a075d4464512`  
		Last Modified: Tue, 02 Feb 2021 02:14:28 GMT  
		Size: 69.5 MB (69464280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0085121e3c317ff3294353f5fc57d00fdd1281d8a974e777aefb7fad747f68`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b35ed1592a30ed19ce07f1c48826efb976b0e85a56fc4c7f45907e98e7344f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fabd30979878ac4c239f4eb3c17beb75bf1e76f77bb670c193db8709d896b9`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f7c2232e59d98f52fcd32679c9db88a62caa3d40a827ac793f6f028ce71535b7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68353383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ce399bb54c39a88a4b02d7e9c88f43afbcffb1a1da5e3905fef969364e9c63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:07:31 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 01:07:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:07:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:07:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:07:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:07:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:07:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:07:43 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ea4215e87a19277d3ad5191bd33bbc874d53668f5bab1d078e9be7be8fb12`  
		Last Modified: Tue, 02 Feb 2021 01:09:39 GMT  
		Size: 63.6 MB (63572234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afbccbf4e53fe57125e562dbb66792d01e4166e117597e31e419cab29894e3d`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b11151c2bc89ee34a665c25ced3ff48ae5a22718436d3ece90d6312884a09aa`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6a033d54e332e1f5c93adab630e5bd10f71a41174a5969dd6e3cac4ca58f5`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.3`

```console
$ docker pull docker@sha256:950c22d6a7264d55ecaddc18be5f31da3a006d195cbe493a6dd1a55b89093854
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.3` - linux; amd64

```console
$ docker pull docker@sha256:92d21018568e2ce434e492257c8333b5364566ab4fb47b9d9a069961ff81cb89
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74328888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e081696197d3ee50cccb7dc2c402da573d3a388eb7e2bc21c7ace31638a0f5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:12:24 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 02:12:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:12:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:12:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:35 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b102489fa5766c88e23ee2669f5da5315dc52527ecc33f4b1002a075d4464512`  
		Last Modified: Tue, 02 Feb 2021 02:14:28 GMT  
		Size: 69.5 MB (69464280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0085121e3c317ff3294353f5fc57d00fdd1281d8a974e777aefb7fad747f68`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b35ed1592a30ed19ce07f1c48826efb976b0e85a56fc4c7f45907e98e7344f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fabd30979878ac4c239f4eb3c17beb75bf1e76f77bb670c193db8709d896b9`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.3` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f7c2232e59d98f52fcd32679c9db88a62caa3d40a827ac793f6f028ce71535b7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68353383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ce399bb54c39a88a4b02d7e9c88f43afbcffb1a1da5e3905fef969364e9c63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:07:31 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 01:07:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:07:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:07:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:07:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:07:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:07:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:07:43 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ea4215e87a19277d3ad5191bd33bbc874d53668f5bab1d078e9be7be8fb12`  
		Last Modified: Tue, 02 Feb 2021 01:09:39 GMT  
		Size: 63.6 MB (63572234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afbccbf4e53fe57125e562dbb66792d01e4166e117597e31e419cab29894e3d`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b11151c2bc89ee34a665c25ced3ff48ae5a22718436d3ece90d6312884a09aa`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6a033d54e332e1f5c93adab630e5bd10f71a41174a5969dd6e3cac4ca58f5`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.3-dind`

```console
$ docker pull docker@sha256:7e1f7ea149d1d23e739dd763e918aa8adab341cef04e0ede6b9487c1859e445e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.3-dind` - linux; amd64

```console
$ docker pull docker@sha256:15ba912799db0ddb94115c841e701927b33a2f0bc2d3816eabb9493325e96cfe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.9 MB (80944119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1a6345c23f3afc5116579b8bf255373b8846e43b239937d90da550f16a5d362`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:12:24 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 02:12:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:12:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:12:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:35 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:12:43 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 02:12:44 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:12:44 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 02:12:45 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 02:12:45 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:46 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 02:12:46 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 02:12:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:46 GMT
CMD []
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b102489fa5766c88e23ee2669f5da5315dc52527ecc33f4b1002a075d4464512`  
		Last Modified: Tue, 02 Feb 2021 02:14:28 GMT  
		Size: 69.5 MB (69464280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0085121e3c317ff3294353f5fc57d00fdd1281d8a974e777aefb7fad747f68`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b35ed1592a30ed19ce07f1c48826efb976b0e85a56fc4c7f45907e98e7344f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fabd30979878ac4c239f4eb3c17beb75bf1e76f77bb670c193db8709d896b9`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d77114131928dd4600f932cdb60ffd93ec8228b74c782f61be79d5b0384f7a3`  
		Last Modified: Tue, 02 Feb 2021 02:14:35 GMT  
		Size: 6.6 MB (6610510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd79eae9e0ad88526c3d6c376d84138b44b914c4fdded0eadbe27ea994b5e0f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7601fb9e80f5256ebd27937de8e7dc0452ff522d90744fc7b634e4d2e43670b4`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be55c3a4b08c09f513e1e19ac44e48f25d65c12a47b432d2c988437887a772e`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 2.5 KB (2509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.3-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:618842321012016d9f1fc9467f76254e3ab902cbd02df4bc6558771dc86c3678
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74870808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f29e39472c1cca735738cf850b0fec5c81ca4b4e9cf3fa0825a7ff1b68a4a77`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:07:31 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 01:07:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:07:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:07:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:07:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:07:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:07:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:07:43 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 01:07:53 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 01:07:55 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 01:07:56 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 01:07:58 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 01:07:58 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:07:59 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 01:08:00 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 01:08:00 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 01:08:01 GMT
CMD []
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ea4215e87a19277d3ad5191bd33bbc874d53668f5bab1d078e9be7be8fb12`  
		Last Modified: Tue, 02 Feb 2021 01:09:39 GMT  
		Size: 63.6 MB (63572234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afbccbf4e53fe57125e562dbb66792d01e4166e117597e31e419cab29894e3d`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b11151c2bc89ee34a665c25ced3ff48ae5a22718436d3ece90d6312884a09aa`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6a033d54e332e1f5c93adab630e5bd10f71a41174a5969dd6e3cac4ca58f5`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52513ff398cf36ad2cdfcba256424267938dafe78194b47326522519e788a5aa`  
		Last Modified: Tue, 02 Feb 2021 01:09:50 GMT  
		Size: 6.5 MB (6512671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fcf6eb9d49b51ab977bf3882e1b8f1ac27a952ae2a33c6ab80f70e2221f5a00`  
		Last Modified: Tue, 02 Feb 2021 01:09:49 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15068978766db2d6d43c93a4221a9456b3380e1c29e702ee152cf292b2b8e29`  
		Last Modified: Tue, 02 Feb 2021 01:09:48 GMT  
		Size: 933.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e4b62c8f0c729e0b9b0e672138f25be96738cb388fc78ecc9e36b34ada6251`  
		Last Modified: Tue, 02 Feb 2021 01:09:48 GMT  
		Size: 2.5 KB (2512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.3-dind-rootless`

```console
$ docker pull docker@sha256:5599f5e50227c3380607e4c0024889a18cdefbf21d8676f6239e9bd3d22f37d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:20.10.3-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:828a9fce6eef3f231f058328d4f30511e4e2f62c52bf3eabd3c03e2b4747dd1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102248802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66947aa7a63a295db42b816e30dda4880d268fff8ff84fb59294acc6322c42fd`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:12:24 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 02:12:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:12:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:12:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:35 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:12:43 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 02:12:44 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:12:44 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 02:12:45 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 02:12:45 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:46 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 02:12:46 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 02:12:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:46 GMT
CMD []
# Tue, 02 Feb 2021 02:12:52 GMT
RUN apk add --no-cache iproute2
# Tue, 02 Feb 2021 02:12:53 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 02 Feb 2021 02:12:54 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:12:57 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 02 Feb 2021 02:12:58 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 02 Feb 2021 02:12:58 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 02 Feb 2021 02:12:58 GMT
USER rootless
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b102489fa5766c88e23ee2669f5da5315dc52527ecc33f4b1002a075d4464512`  
		Last Modified: Tue, 02 Feb 2021 02:14:28 GMT  
		Size: 69.5 MB (69464280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0085121e3c317ff3294353f5fc57d00fdd1281d8a974e777aefb7fad747f68`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b35ed1592a30ed19ce07f1c48826efb976b0e85a56fc4c7f45907e98e7344f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fabd30979878ac4c239f4eb3c17beb75bf1e76f77bb670c193db8709d896b9`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d77114131928dd4600f932cdb60ffd93ec8228b74c782f61be79d5b0384f7a3`  
		Last Modified: Tue, 02 Feb 2021 02:14:35 GMT  
		Size: 6.6 MB (6610510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd79eae9e0ad88526c3d6c376d84138b44b914c4fdded0eadbe27ea994b5e0f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7601fb9e80f5256ebd27937de8e7dc0452ff522d90744fc7b634e4d2e43670b4`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be55c3a4b08c09f513e1e19ac44e48f25d65c12a47b432d2c988437887a772e`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 2.5 KB (2509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c1c4727c96911df279f9517efc661a0bcc45aeac51701a9c2e0548b7a9b8ba`  
		Last Modified: Tue, 02 Feb 2021 02:14:41 GMT  
		Size: 1.1 MB (1131699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df17a804b3b2a14f4790c63cb64b9b001b00598516e8c363d7ee0db7bea897fc`  
		Last Modified: Tue, 02 Feb 2021 02:14:40 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd143a2bdb0e10bf2b6ff8c31e744338e52ed20d5c7e2066713b9200b88dfd4`  
		Last Modified: Tue, 02 Feb 2021 02:14:40 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af59019a28035daee12ef6285e030050f02193f3ae7be261dcec09ec1476c7f1`  
		Last Modified: Tue, 02 Feb 2021 02:14:44 GMT  
		Size: 20.2 MB (20171372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04805209f88c249ea3f9e9719d3ed26bcc03727713ba29dd83da3addd622831f`  
		Last Modified: Tue, 02 Feb 2021 02:14:40 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.3-git`

```console
$ docker pull docker@sha256:736e7b39093b20f4710f83d526a1869900c87b58bb60c5918dd37101e22a312b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.3-git` - linux; amd64

```console
$ docker pull docker@sha256:56cd9984e07c13d73acc6cf0aaeb18e2075f210616476f124d362d5229b106de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.7 MB (80718391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5675ce6408db5c04632749d40a4d38af1edcc8b089ce8efe41f62d0b2bb05dd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:12:24 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 02:12:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:12:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:12:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:35 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:13:04 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b102489fa5766c88e23ee2669f5da5315dc52527ecc33f4b1002a075d4464512`  
		Last Modified: Tue, 02 Feb 2021 02:14:28 GMT  
		Size: 69.5 MB (69464280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0085121e3c317ff3294353f5fc57d00fdd1281d8a974e777aefb7fad747f68`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b35ed1592a30ed19ce07f1c48826efb976b0e85a56fc4c7f45907e98e7344f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fabd30979878ac4c239f4eb3c17beb75bf1e76f77bb670c193db8709d896b9`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f51d5f71cf511ac9e105ec40bdb6301d6fd3c97da1ccc952951b3a382d5373`  
		Last Modified: Tue, 02 Feb 2021 02:14:51 GMT  
		Size: 6.4 MB (6389503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.3-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f50e160aec2b3c2084868d88c8fd12405b7c821b4d1eb3f6d0f212f7ab229ca4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74828139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f1bd1f86381bfb83fdd88698657ba8dfb6e246bf7c53e4d037d743306d3e1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:07:31 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 01:07:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:07:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:07:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:07:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:07:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:07:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:07:43 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 01:08:10 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ea4215e87a19277d3ad5191bd33bbc874d53668f5bab1d078e9be7be8fb12`  
		Last Modified: Tue, 02 Feb 2021 01:09:39 GMT  
		Size: 63.6 MB (63572234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afbccbf4e53fe57125e562dbb66792d01e4166e117597e31e419cab29894e3d`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b11151c2bc89ee34a665c25ced3ff48ae5a22718436d3ece90d6312884a09aa`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6a033d54e332e1f5c93adab630e5bd10f71a41174a5969dd6e3cac4ca58f5`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a55270903e654573ef5353863992734f533829903b93363b870b2e95ae7ed8`  
		Last Modified: Tue, 02 Feb 2021 01:10:02 GMT  
		Size: 6.5 MB (6474756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind`

```console
$ docker pull docker@sha256:7e1f7ea149d1d23e739dd763e918aa8adab341cef04e0ede6b9487c1859e445e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind` - linux; amd64

```console
$ docker pull docker@sha256:15ba912799db0ddb94115c841e701927b33a2f0bc2d3816eabb9493325e96cfe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.9 MB (80944119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1a6345c23f3afc5116579b8bf255373b8846e43b239937d90da550f16a5d362`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:12:24 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 02:12:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:12:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:12:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:35 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:12:43 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 02:12:44 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:12:44 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 02:12:45 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 02:12:45 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:46 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 02:12:46 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 02:12:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:46 GMT
CMD []
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b102489fa5766c88e23ee2669f5da5315dc52527ecc33f4b1002a075d4464512`  
		Last Modified: Tue, 02 Feb 2021 02:14:28 GMT  
		Size: 69.5 MB (69464280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0085121e3c317ff3294353f5fc57d00fdd1281d8a974e777aefb7fad747f68`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b35ed1592a30ed19ce07f1c48826efb976b0e85a56fc4c7f45907e98e7344f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fabd30979878ac4c239f4eb3c17beb75bf1e76f77bb670c193db8709d896b9`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d77114131928dd4600f932cdb60ffd93ec8228b74c782f61be79d5b0384f7a3`  
		Last Modified: Tue, 02 Feb 2021 02:14:35 GMT  
		Size: 6.6 MB (6610510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd79eae9e0ad88526c3d6c376d84138b44b914c4fdded0eadbe27ea994b5e0f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7601fb9e80f5256ebd27937de8e7dc0452ff522d90744fc7b634e4d2e43670b4`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be55c3a4b08c09f513e1e19ac44e48f25d65c12a47b432d2c988437887a772e`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 2.5 KB (2509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:618842321012016d9f1fc9467f76254e3ab902cbd02df4bc6558771dc86c3678
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74870808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f29e39472c1cca735738cf850b0fec5c81ca4b4e9cf3fa0825a7ff1b68a4a77`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:07:31 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 01:07:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:07:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:07:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:07:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:07:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:07:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:07:43 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 01:07:53 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 01:07:55 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 01:07:56 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 01:07:58 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 01:07:58 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:07:59 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 01:08:00 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 01:08:00 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 01:08:01 GMT
CMD []
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ea4215e87a19277d3ad5191bd33bbc874d53668f5bab1d078e9be7be8fb12`  
		Last Modified: Tue, 02 Feb 2021 01:09:39 GMT  
		Size: 63.6 MB (63572234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afbccbf4e53fe57125e562dbb66792d01e4166e117597e31e419cab29894e3d`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b11151c2bc89ee34a665c25ced3ff48ae5a22718436d3ece90d6312884a09aa`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6a033d54e332e1f5c93adab630e5bd10f71a41174a5969dd6e3cac4ca58f5`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52513ff398cf36ad2cdfcba256424267938dafe78194b47326522519e788a5aa`  
		Last Modified: Tue, 02 Feb 2021 01:09:50 GMT  
		Size: 6.5 MB (6512671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fcf6eb9d49b51ab977bf3882e1b8f1ac27a952ae2a33c6ab80f70e2221f5a00`  
		Last Modified: Tue, 02 Feb 2021 01:09:49 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15068978766db2d6d43c93a4221a9456b3380e1c29e702ee152cf292b2b8e29`  
		Last Modified: Tue, 02 Feb 2021 01:09:48 GMT  
		Size: 933.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e4b62c8f0c729e0b9b0e672138f25be96738cb388fc78ecc9e36b34ada6251`  
		Last Modified: Tue, 02 Feb 2021 01:09:48 GMT  
		Size: 2.5 KB (2512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind-rootless`

```console
$ docker pull docker@sha256:5599f5e50227c3380607e4c0024889a18cdefbf21d8676f6239e9bd3d22f37d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:20.10-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:828a9fce6eef3f231f058328d4f30511e4e2f62c52bf3eabd3c03e2b4747dd1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102248802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66947aa7a63a295db42b816e30dda4880d268fff8ff84fb59294acc6322c42fd`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:12:24 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 02:12:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:12:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:12:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:35 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:12:43 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 02:12:44 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:12:44 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 02:12:45 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 02:12:45 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:46 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 02:12:46 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 02:12:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:46 GMT
CMD []
# Tue, 02 Feb 2021 02:12:52 GMT
RUN apk add --no-cache iproute2
# Tue, 02 Feb 2021 02:12:53 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 02 Feb 2021 02:12:54 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:12:57 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 02 Feb 2021 02:12:58 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 02 Feb 2021 02:12:58 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 02 Feb 2021 02:12:58 GMT
USER rootless
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b102489fa5766c88e23ee2669f5da5315dc52527ecc33f4b1002a075d4464512`  
		Last Modified: Tue, 02 Feb 2021 02:14:28 GMT  
		Size: 69.5 MB (69464280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0085121e3c317ff3294353f5fc57d00fdd1281d8a974e777aefb7fad747f68`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b35ed1592a30ed19ce07f1c48826efb976b0e85a56fc4c7f45907e98e7344f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fabd30979878ac4c239f4eb3c17beb75bf1e76f77bb670c193db8709d896b9`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d77114131928dd4600f932cdb60ffd93ec8228b74c782f61be79d5b0384f7a3`  
		Last Modified: Tue, 02 Feb 2021 02:14:35 GMT  
		Size: 6.6 MB (6610510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd79eae9e0ad88526c3d6c376d84138b44b914c4fdded0eadbe27ea994b5e0f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7601fb9e80f5256ebd27937de8e7dc0452ff522d90744fc7b634e4d2e43670b4`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be55c3a4b08c09f513e1e19ac44e48f25d65c12a47b432d2c988437887a772e`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 2.5 KB (2509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c1c4727c96911df279f9517efc661a0bcc45aeac51701a9c2e0548b7a9b8ba`  
		Last Modified: Tue, 02 Feb 2021 02:14:41 GMT  
		Size: 1.1 MB (1131699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df17a804b3b2a14f4790c63cb64b9b001b00598516e8c363d7ee0db7bea897fc`  
		Last Modified: Tue, 02 Feb 2021 02:14:40 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd143a2bdb0e10bf2b6ff8c31e744338e52ed20d5c7e2066713b9200b88dfd4`  
		Last Modified: Tue, 02 Feb 2021 02:14:40 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af59019a28035daee12ef6285e030050f02193f3ae7be261dcec09ec1476c7f1`  
		Last Modified: Tue, 02 Feb 2021 02:14:44 GMT  
		Size: 20.2 MB (20171372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04805209f88c249ea3f9e9719d3ed26bcc03727713ba29dd83da3addd622831f`  
		Last Modified: Tue, 02 Feb 2021 02:14:40 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-git`

```console
$ docker pull docker@sha256:736e7b39093b20f4710f83d526a1869900c87b58bb60c5918dd37101e22a312b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-git` - linux; amd64

```console
$ docker pull docker@sha256:56cd9984e07c13d73acc6cf0aaeb18e2075f210616476f124d362d5229b106de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.7 MB (80718391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5675ce6408db5c04632749d40a4d38af1edcc8b089ce8efe41f62d0b2bb05dd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:12:24 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 02:12:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:12:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:12:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:35 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:13:04 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b102489fa5766c88e23ee2669f5da5315dc52527ecc33f4b1002a075d4464512`  
		Last Modified: Tue, 02 Feb 2021 02:14:28 GMT  
		Size: 69.5 MB (69464280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0085121e3c317ff3294353f5fc57d00fdd1281d8a974e777aefb7fad747f68`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b35ed1592a30ed19ce07f1c48826efb976b0e85a56fc4c7f45907e98e7344f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fabd30979878ac4c239f4eb3c17beb75bf1e76f77bb670c193db8709d896b9`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f51d5f71cf511ac9e105ec40bdb6301d6fd3c97da1ccc952951b3a382d5373`  
		Last Modified: Tue, 02 Feb 2021 02:14:51 GMT  
		Size: 6.4 MB (6389503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f50e160aec2b3c2084868d88c8fd12405b7c821b4d1eb3f6d0f212f7ab229ca4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74828139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f1bd1f86381bfb83fdd88698657ba8dfb6e246bf7c53e4d037d743306d3e1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:07:31 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 01:07:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:07:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:07:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:07:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:07:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:07:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:07:43 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 01:08:10 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ea4215e87a19277d3ad5191bd33bbc874d53668f5bab1d078e9be7be8fb12`  
		Last Modified: Tue, 02 Feb 2021 01:09:39 GMT  
		Size: 63.6 MB (63572234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afbccbf4e53fe57125e562dbb66792d01e4166e117597e31e419cab29894e3d`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b11151c2bc89ee34a665c25ced3ff48ae5a22718436d3ece90d6312884a09aa`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6a033d54e332e1f5c93adab630e5bd10f71a41174a5969dd6e3cac4ca58f5`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a55270903e654573ef5353863992734f533829903b93363b870b2e95ae7ed8`  
		Last Modified: Tue, 02 Feb 2021 01:10:02 GMT  
		Size: 6.5 MB (6474756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind`

```console
$ docker pull docker@sha256:7e1f7ea149d1d23e739dd763e918aa8adab341cef04e0ede6b9487c1859e445e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind` - linux; amd64

```console
$ docker pull docker@sha256:15ba912799db0ddb94115c841e701927b33a2f0bc2d3816eabb9493325e96cfe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.9 MB (80944119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1a6345c23f3afc5116579b8bf255373b8846e43b239937d90da550f16a5d362`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:12:24 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 02:12:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:12:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:12:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:35 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:12:43 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 02:12:44 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:12:44 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 02:12:45 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 02:12:45 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:46 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 02:12:46 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 02:12:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:46 GMT
CMD []
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b102489fa5766c88e23ee2669f5da5315dc52527ecc33f4b1002a075d4464512`  
		Last Modified: Tue, 02 Feb 2021 02:14:28 GMT  
		Size: 69.5 MB (69464280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0085121e3c317ff3294353f5fc57d00fdd1281d8a974e777aefb7fad747f68`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b35ed1592a30ed19ce07f1c48826efb976b0e85a56fc4c7f45907e98e7344f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fabd30979878ac4c239f4eb3c17beb75bf1e76f77bb670c193db8709d896b9`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d77114131928dd4600f932cdb60ffd93ec8228b74c782f61be79d5b0384f7a3`  
		Last Modified: Tue, 02 Feb 2021 02:14:35 GMT  
		Size: 6.6 MB (6610510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd79eae9e0ad88526c3d6c376d84138b44b914c4fdded0eadbe27ea994b5e0f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7601fb9e80f5256ebd27937de8e7dc0452ff522d90744fc7b634e4d2e43670b4`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be55c3a4b08c09f513e1e19ac44e48f25d65c12a47b432d2c988437887a772e`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 2.5 KB (2509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:618842321012016d9f1fc9467f76254e3ab902cbd02df4bc6558771dc86c3678
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74870808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f29e39472c1cca735738cf850b0fec5c81ca4b4e9cf3fa0825a7ff1b68a4a77`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:07:31 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 01:07:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:07:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:07:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:07:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:07:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:07:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:07:43 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 01:07:53 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 01:07:55 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 01:07:56 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 01:07:58 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 01:07:58 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:07:59 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 01:08:00 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 01:08:00 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 01:08:01 GMT
CMD []
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ea4215e87a19277d3ad5191bd33bbc874d53668f5bab1d078e9be7be8fb12`  
		Last Modified: Tue, 02 Feb 2021 01:09:39 GMT  
		Size: 63.6 MB (63572234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afbccbf4e53fe57125e562dbb66792d01e4166e117597e31e419cab29894e3d`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b11151c2bc89ee34a665c25ced3ff48ae5a22718436d3ece90d6312884a09aa`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6a033d54e332e1f5c93adab630e5bd10f71a41174a5969dd6e3cac4ca58f5`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52513ff398cf36ad2cdfcba256424267938dafe78194b47326522519e788a5aa`  
		Last Modified: Tue, 02 Feb 2021 01:09:50 GMT  
		Size: 6.5 MB (6512671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fcf6eb9d49b51ab977bf3882e1b8f1ac27a952ae2a33c6ab80f70e2221f5a00`  
		Last Modified: Tue, 02 Feb 2021 01:09:49 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15068978766db2d6d43c93a4221a9456b3380e1c29e702ee152cf292b2b8e29`  
		Last Modified: Tue, 02 Feb 2021 01:09:48 GMT  
		Size: 933.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e4b62c8f0c729e0b9b0e672138f25be96738cb388fc78ecc9e36b34ada6251`  
		Last Modified: Tue, 02 Feb 2021 01:09:48 GMT  
		Size: 2.5 KB (2512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:5599f5e50227c3380607e4c0024889a18cdefbf21d8676f6239e9bd3d22f37d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:828a9fce6eef3f231f058328d4f30511e4e2f62c52bf3eabd3c03e2b4747dd1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102248802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66947aa7a63a295db42b816e30dda4880d268fff8ff84fb59294acc6322c42fd`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:12:24 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 02:12:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:12:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:12:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:35 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:12:43 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 02:12:44 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:12:44 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 02:12:45 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 02:12:45 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:46 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 02:12:46 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 02:12:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:46 GMT
CMD []
# Tue, 02 Feb 2021 02:12:52 GMT
RUN apk add --no-cache iproute2
# Tue, 02 Feb 2021 02:12:53 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 02 Feb 2021 02:12:54 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:12:57 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 02 Feb 2021 02:12:58 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 02 Feb 2021 02:12:58 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 02 Feb 2021 02:12:58 GMT
USER rootless
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b102489fa5766c88e23ee2669f5da5315dc52527ecc33f4b1002a075d4464512`  
		Last Modified: Tue, 02 Feb 2021 02:14:28 GMT  
		Size: 69.5 MB (69464280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0085121e3c317ff3294353f5fc57d00fdd1281d8a974e777aefb7fad747f68`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b35ed1592a30ed19ce07f1c48826efb976b0e85a56fc4c7f45907e98e7344f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fabd30979878ac4c239f4eb3c17beb75bf1e76f77bb670c193db8709d896b9`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d77114131928dd4600f932cdb60ffd93ec8228b74c782f61be79d5b0384f7a3`  
		Last Modified: Tue, 02 Feb 2021 02:14:35 GMT  
		Size: 6.6 MB (6610510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd79eae9e0ad88526c3d6c376d84138b44b914c4fdded0eadbe27ea994b5e0f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7601fb9e80f5256ebd27937de8e7dc0452ff522d90744fc7b634e4d2e43670b4`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be55c3a4b08c09f513e1e19ac44e48f25d65c12a47b432d2c988437887a772e`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 2.5 KB (2509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c1c4727c96911df279f9517efc661a0bcc45aeac51701a9c2e0548b7a9b8ba`  
		Last Modified: Tue, 02 Feb 2021 02:14:41 GMT  
		Size: 1.1 MB (1131699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df17a804b3b2a14f4790c63cb64b9b001b00598516e8c363d7ee0db7bea897fc`  
		Last Modified: Tue, 02 Feb 2021 02:14:40 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd143a2bdb0e10bf2b6ff8c31e744338e52ed20d5c7e2066713b9200b88dfd4`  
		Last Modified: Tue, 02 Feb 2021 02:14:40 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af59019a28035daee12ef6285e030050f02193f3ae7be261dcec09ec1476c7f1`  
		Last Modified: Tue, 02 Feb 2021 02:14:44 GMT  
		Size: 20.2 MB (20171372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04805209f88c249ea3f9e9719d3ed26bcc03727713ba29dd83da3addd622831f`  
		Last Modified: Tue, 02 Feb 2021 02:14:40 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-git`

```console
$ docker pull docker@sha256:736e7b39093b20f4710f83d526a1869900c87b58bb60c5918dd37101e22a312b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-git` - linux; amd64

```console
$ docker pull docker@sha256:56cd9984e07c13d73acc6cf0aaeb18e2075f210616476f124d362d5229b106de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.7 MB (80718391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5675ce6408db5c04632749d40a4d38af1edcc8b089ce8efe41f62d0b2bb05dd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:12:24 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 02:12:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:12:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:12:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:35 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:13:04 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b102489fa5766c88e23ee2669f5da5315dc52527ecc33f4b1002a075d4464512`  
		Last Modified: Tue, 02 Feb 2021 02:14:28 GMT  
		Size: 69.5 MB (69464280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0085121e3c317ff3294353f5fc57d00fdd1281d8a974e777aefb7fad747f68`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b35ed1592a30ed19ce07f1c48826efb976b0e85a56fc4c7f45907e98e7344f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fabd30979878ac4c239f4eb3c17beb75bf1e76f77bb670c193db8709d896b9`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f51d5f71cf511ac9e105ec40bdb6301d6fd3c97da1ccc952951b3a382d5373`  
		Last Modified: Tue, 02 Feb 2021 02:14:51 GMT  
		Size: 6.4 MB (6389503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f50e160aec2b3c2084868d88c8fd12405b7c821b4d1eb3f6d0f212f7ab229ca4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74828139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f1bd1f86381bfb83fdd88698657ba8dfb6e246bf7c53e4d037d743306d3e1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:07:31 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 01:07:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:07:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:07:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:07:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:07:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:07:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:07:43 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 01:08:10 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ea4215e87a19277d3ad5191bd33bbc874d53668f5bab1d078e9be7be8fb12`  
		Last Modified: Tue, 02 Feb 2021 01:09:39 GMT  
		Size: 63.6 MB (63572234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afbccbf4e53fe57125e562dbb66792d01e4166e117597e31e419cab29894e3d`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b11151c2bc89ee34a665c25ced3ff48ae5a22718436d3ece90d6312884a09aa`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6a033d54e332e1f5c93adab630e5bd10f71a41174a5969dd6e3cac4ca58f5`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a55270903e654573ef5353863992734f533829903b93363b870b2e95ae7ed8`  
		Last Modified: Tue, 02 Feb 2021 01:10:02 GMT  
		Size: 6.5 MB (6474756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:9398e00a10c16fb3b98c77d452708702e790fd41c725b9b89de26352bea7fdce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:15ba912799db0ddb94115c841e701927b33a2f0bc2d3816eabb9493325e96cfe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.9 MB (80944119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1a6345c23f3afc5116579b8bf255373b8846e43b239937d90da550f16a5d362`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:12:24 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 02:12:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:12:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:12:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:35 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:12:43 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 02:12:44 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:12:44 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 02:12:45 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 02:12:45 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:46 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 02:12:46 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 02:12:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:46 GMT
CMD []
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b102489fa5766c88e23ee2669f5da5315dc52527ecc33f4b1002a075d4464512`  
		Last Modified: Tue, 02 Feb 2021 02:14:28 GMT  
		Size: 69.5 MB (69464280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0085121e3c317ff3294353f5fc57d00fdd1281d8a974e777aefb7fad747f68`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b35ed1592a30ed19ce07f1c48826efb976b0e85a56fc4c7f45907e98e7344f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fabd30979878ac4c239f4eb3c17beb75bf1e76f77bb670c193db8709d896b9`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d77114131928dd4600f932cdb60ffd93ec8228b74c782f61be79d5b0384f7a3`  
		Last Modified: Tue, 02 Feb 2021 02:14:35 GMT  
		Size: 6.6 MB (6610510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd79eae9e0ad88526c3d6c376d84138b44b914c4fdded0eadbe27ea994b5e0f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7601fb9e80f5256ebd27937de8e7dc0452ff522d90744fc7b634e4d2e43670b4`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be55c3a4b08c09f513e1e19ac44e48f25d65c12a47b432d2c988437887a772e`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 2.5 KB (2509 bytes)  
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
$ docker pull docker@sha256:618842321012016d9f1fc9467f76254e3ab902cbd02df4bc6558771dc86c3678
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74870808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f29e39472c1cca735738cf850b0fec5c81ca4b4e9cf3fa0825a7ff1b68a4a77`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:07:31 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 01:07:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:07:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:07:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:07:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:07:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:07:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:07:43 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 01:07:53 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 01:07:55 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 01:07:56 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 01:07:58 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 01:07:58 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:07:59 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 01:08:00 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 01:08:00 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 01:08:01 GMT
CMD []
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ea4215e87a19277d3ad5191bd33bbc874d53668f5bab1d078e9be7be8fb12`  
		Last Modified: Tue, 02 Feb 2021 01:09:39 GMT  
		Size: 63.6 MB (63572234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afbccbf4e53fe57125e562dbb66792d01e4166e117597e31e419cab29894e3d`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b11151c2bc89ee34a665c25ced3ff48ae5a22718436d3ece90d6312884a09aa`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6a033d54e332e1f5c93adab630e5bd10f71a41174a5969dd6e3cac4ca58f5`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52513ff398cf36ad2cdfcba256424267938dafe78194b47326522519e788a5aa`  
		Last Modified: Tue, 02 Feb 2021 01:09:50 GMT  
		Size: 6.5 MB (6512671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fcf6eb9d49b51ab977bf3882e1b8f1ac27a952ae2a33c6ab80f70e2221f5a00`  
		Last Modified: Tue, 02 Feb 2021 01:09:49 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15068978766db2d6d43c93a4221a9456b3380e1c29e702ee152cf292b2b8e29`  
		Last Modified: Tue, 02 Feb 2021 01:09:48 GMT  
		Size: 933.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e4b62c8f0c729e0b9b0e672138f25be96738cb388fc78ecc9e36b34ada6251`  
		Last Modified: Tue, 02 Feb 2021 01:09:48 GMT  
		Size: 2.5 KB (2512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:5599f5e50227c3380607e4c0024889a18cdefbf21d8676f6239e9bd3d22f37d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:828a9fce6eef3f231f058328d4f30511e4e2f62c52bf3eabd3c03e2b4747dd1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102248802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66947aa7a63a295db42b816e30dda4880d268fff8ff84fb59294acc6322c42fd`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:12:24 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 02:12:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:12:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:12:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:35 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:12:43 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 02:12:44 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:12:44 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 02:12:45 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 02:12:45 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:46 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 02:12:46 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 02:12:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:46 GMT
CMD []
# Tue, 02 Feb 2021 02:12:52 GMT
RUN apk add --no-cache iproute2
# Tue, 02 Feb 2021 02:12:53 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 02 Feb 2021 02:12:54 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:12:57 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 02 Feb 2021 02:12:58 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 02 Feb 2021 02:12:58 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 02 Feb 2021 02:12:58 GMT
USER rootless
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b102489fa5766c88e23ee2669f5da5315dc52527ecc33f4b1002a075d4464512`  
		Last Modified: Tue, 02 Feb 2021 02:14:28 GMT  
		Size: 69.5 MB (69464280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0085121e3c317ff3294353f5fc57d00fdd1281d8a974e777aefb7fad747f68`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b35ed1592a30ed19ce07f1c48826efb976b0e85a56fc4c7f45907e98e7344f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fabd30979878ac4c239f4eb3c17beb75bf1e76f77bb670c193db8709d896b9`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d77114131928dd4600f932cdb60ffd93ec8228b74c782f61be79d5b0384f7a3`  
		Last Modified: Tue, 02 Feb 2021 02:14:35 GMT  
		Size: 6.6 MB (6610510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd79eae9e0ad88526c3d6c376d84138b44b914c4fdded0eadbe27ea994b5e0f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7601fb9e80f5256ebd27937de8e7dc0452ff522d90744fc7b634e4d2e43670b4`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be55c3a4b08c09f513e1e19ac44e48f25d65c12a47b432d2c988437887a772e`  
		Last Modified: Tue, 02 Feb 2021 02:14:34 GMT  
		Size: 2.5 KB (2509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c1c4727c96911df279f9517efc661a0bcc45aeac51701a9c2e0548b7a9b8ba`  
		Last Modified: Tue, 02 Feb 2021 02:14:41 GMT  
		Size: 1.1 MB (1131699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df17a804b3b2a14f4790c63cb64b9b001b00598516e8c363d7ee0db7bea897fc`  
		Last Modified: Tue, 02 Feb 2021 02:14:40 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd143a2bdb0e10bf2b6ff8c31e744338e52ed20d5c7e2066713b9200b88dfd4`  
		Last Modified: Tue, 02 Feb 2021 02:14:40 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af59019a28035daee12ef6285e030050f02193f3ae7be261dcec09ec1476c7f1`  
		Last Modified: Tue, 02 Feb 2021 02:14:44 GMT  
		Size: 20.2 MB (20171372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04805209f88c249ea3f9e9719d3ed26bcc03727713ba29dd83da3addd622831f`  
		Last Modified: Tue, 02 Feb 2021 02:14:40 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:dd4f299c9b16c4d45e0425d3f763cb1ecc8123112f512dff1c527aa8a9d5d4b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:56cd9984e07c13d73acc6cf0aaeb18e2075f210616476f124d362d5229b106de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.7 MB (80718391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5675ce6408db5c04632749d40a4d38af1edcc8b089ce8efe41f62d0b2bb05dd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:12:24 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 02:12:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:12:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:12:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:35 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:13:04 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b102489fa5766c88e23ee2669f5da5315dc52527ecc33f4b1002a075d4464512`  
		Last Modified: Tue, 02 Feb 2021 02:14:28 GMT  
		Size: 69.5 MB (69464280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0085121e3c317ff3294353f5fc57d00fdd1281d8a974e777aefb7fad747f68`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b35ed1592a30ed19ce07f1c48826efb976b0e85a56fc4c7f45907e98e7344f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fabd30979878ac4c239f4eb3c17beb75bf1e76f77bb670c193db8709d896b9`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f51d5f71cf511ac9e105ec40bdb6301d6fd3c97da1ccc952951b3a382d5373`  
		Last Modified: Tue, 02 Feb 2021 02:14:51 GMT  
		Size: 6.4 MB (6389503 bytes)  
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
$ docker pull docker@sha256:f50e160aec2b3c2084868d88c8fd12405b7c821b4d1eb3f6d0f212f7ab229ca4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74828139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f1bd1f86381bfb83fdd88698657ba8dfb6e246bf7c53e4d037d743306d3e1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:07:31 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 01:07:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:07:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:07:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:07:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:07:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:07:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:07:43 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 01:08:10 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ea4215e87a19277d3ad5191bd33bbc874d53668f5bab1d078e9be7be8fb12`  
		Last Modified: Tue, 02 Feb 2021 01:09:39 GMT  
		Size: 63.6 MB (63572234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afbccbf4e53fe57125e562dbb66792d01e4166e117597e31e419cab29894e3d`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b11151c2bc89ee34a665c25ced3ff48ae5a22718436d3ece90d6312884a09aa`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6a033d54e332e1f5c93adab630e5bd10f71a41174a5969dd6e3cac4ca58f5`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a55270903e654573ef5353863992734f533829903b93363b870b2e95ae7ed8`  
		Last Modified: Tue, 02 Feb 2021 01:10:02 GMT  
		Size: 6.5 MB (6474756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:74df197ad4646763e1954829231c54b5e4c362a7bdc5c5198d2b59ab5ace06ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:92d21018568e2ce434e492257c8333b5364566ab4fb47b9d9a069961ff81cb89
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74328888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e081696197d3ee50cccb7dc2c402da573d3a388eb7e2bc21c7ace31638a0f5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:12:24 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 02:12:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:12:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:12:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:12:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:12:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:12:35 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b102489fa5766c88e23ee2669f5da5315dc52527ecc33f4b1002a075d4464512`  
		Last Modified: Tue, 02 Feb 2021 02:14:28 GMT  
		Size: 69.5 MB (69464280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0085121e3c317ff3294353f5fc57d00fdd1281d8a974e777aefb7fad747f68`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b35ed1592a30ed19ce07f1c48826efb976b0e85a56fc4c7f45907e98e7344f7`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fabd30979878ac4c239f4eb3c17beb75bf1e76f77bb670c193db8709d896b9`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 117.0 B  
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
$ docker pull docker@sha256:f7c2232e59d98f52fcd32679c9db88a62caa3d40a827ac793f6f028ce71535b7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68353383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ce399bb54c39a88a4b02d7e9c88f43afbcffb1a1da5e3905fef969364e9c63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 01:07:28 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 01:07:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 01:07:31 GMT
ENV DOCKER_VERSION=20.10.3
# Tue, 02 Feb 2021 01:07:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.3.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 01:07:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 01:07:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 01:07:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 01:07:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 01:07:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:07:43 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c677dae0e125b184b702e022e81dc6b58d852d919ce87d18f784a02a7a061`  
		Last Modified: Tue, 02 Feb 2021 01:09:23 GMT  
		Size: 2.1 MB (2068024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318712088e33177a73cbc991c387c8cab1c194c7c0ab69e07303a3121a2298dc`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ea4215e87a19277d3ad5191bd33bbc874d53668f5bab1d078e9be7be8fb12`  
		Last Modified: Tue, 02 Feb 2021 01:09:39 GMT  
		Size: 63.6 MB (63572234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afbccbf4e53fe57125e562dbb66792d01e4166e117597e31e419cab29894e3d`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b11151c2bc89ee34a665c25ced3ff48ae5a22718436d3ece90d6312884a09aa`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6a033d54e332e1f5c93adab630e5bd10f71a41174a5969dd6e3cac4ca58f5`  
		Last Modified: Tue, 02 Feb 2021 01:09:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
