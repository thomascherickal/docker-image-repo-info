<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `docker`

-	[`docker:19`](#docker19)
-	[`docker:19-dind`](#docker19-dind)
-	[`docker:19-dind-rootless`](#docker19-dind-rootless)
-	[`docker:19-git`](#docker19-git)
-	[`docker:19.03`](#docker1903)
-	[`docker:19.03-dind`](#docker1903-dind)
-	[`docker:19.03-dind-rootless`](#docker1903-dind-rootless)
-	[`docker:19.03-git`](#docker1903-git)
-	[`docker:19.03.15`](#docker190315)
-	[`docker:19.03.15-dind`](#docker190315-dind)
-	[`docker:19.03.15-dind-rootless`](#docker190315-dind-rootless)
-	[`docker:19.03.15-git`](#docker190315-git)
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
-	[`docker:20.10.7`](#docker20107)
-	[`docker:20.10.7-dind`](#docker20107-dind)
-	[`docker:20.10.7-dind-rootless`](#docker20107-dind-rootless)
-	[`docker:20.10.7-git`](#docker20107-git)
-	[`docker:20.10.7-windowsservercore`](#docker20107-windowsservercore)
-	[`docker:20.10.7-windowsservercore-1809`](#docker20107-windowsservercore-1809)
-	[`docker:dind`](#dockerdind)
-	[`docker:dind-rootless`](#dockerdind-rootless)
-	[`docker:git`](#dockergit)
-	[`docker:latest`](#dockerlatest)
-	[`docker:windowsservercore`](#dockerwindowsservercore)
-	[`docker:windowsservercore-1809`](#dockerwindowsservercore-1809)

## `docker:19`

```console
$ docker pull docker@sha256:8209ca87a5bd61f58b988d239bfeeea1e55ba0b0e7e3256c1bc1e5abe68a178b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19` - linux; amd64

```console
$ docker pull docker@sha256:51b4ccfcc03639a1bf1755de6789aaf506697aa416136e3874499296c179241d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67746929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33d3743ceb6ae9c655769327f4d723433841510d5d9602307e79189807dac391`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:17:37 GMT
ENV DOCKER_VERSION=19.03.15
# Wed, 14 Apr 2021 20:17:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 14 Apr 2021 20:17:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 14 Apr 2021 20:17:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:17:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 14 Apr 2021 20:17:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 14 Apr 2021 20:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:17:46 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09182082685c0a1147c9f22948720af9bb3544411a1b50562d18071cf31b8e21`  
		Last Modified: Wed, 14 Apr 2021 20:20:33 GMT  
		Size: 62.9 MB (62882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4562e3055ed2549b93e450d764e41b62a485d16bafb1f1ed6b67fd610444aa44`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4de57a4336a3a0ab0e109ff4c769bce1d354c121fe62fd5f6063c53fd009d61`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542e5df0dc5eda03440d4a00ca01ceefa7cb8282a9d7b406fd54dabcdf4197c0`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 149.0 B  
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
$ docker pull docker@sha256:b949cbbb354d40d2ec4d168cbb0f24f84d2b6b68e32f6f9dbda004992877194b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60766112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59291a2ff3232902f748ccdb0bfa9d9be4e3d9394a58a8f70ac80001eaa80c03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:33 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 15 Jun 2021 22:34:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:39 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31451232b129e45d3b41a480e8f13df618906b6c2d3f6808dd70af1c71c0c154`  
		Last Modified: Tue, 15 Jun 2021 22:37:13 GMT  
		Size: 56.0 MB (55994351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bf8ca3358da3ae665e1c0c6e8a117f99178132f6a06593366c7ddce01cbd06`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916486c0da5ab2c0c64755b93c82d4ac57ad744c716cf205359b065b6096fcc1`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6e4d5edf6083ebb0300314dd90b0e4f40774a97e9394beaef654f635ec9bc2`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19-dind`

```console
$ docker pull docker@sha256:3843cb86a094abeeb427c9e6365a0b2de6dfcba389d0870aebba9e4746d52014
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19-dind` - linux; amd64

```console
$ docker pull docker@sha256:1875a3437d87a2fa8ec5e6fcd3233a98d571fa9692516b1e7d8eb18b7dca87a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74321571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3b7a5678ece1ea157bb3f4fb6372911ad054e9d271f09d6401fb53e6a8c97d`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:17:37 GMT
ENV DOCKER_VERSION=19.03.15
# Wed, 14 Apr 2021 20:17:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 14 Apr 2021 20:17:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 14 Apr 2021 20:17:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:17:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 14 Apr 2021 20:17:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 14 Apr 2021 20:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:17:46 GMT
CMD ["sh"]
# Wed, 14 Apr 2021 20:17:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 14 Apr 2021 20:17:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 30 Apr 2021 21:20:01 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 30 Apr 2021 21:20:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:20:02 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:20:02 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:20:02 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:20:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:20:02 GMT
CMD []
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09182082685c0a1147c9f22948720af9bb3544411a1b50562d18071cf31b8e21`  
		Last Modified: Wed, 14 Apr 2021 20:20:33 GMT  
		Size: 62.9 MB (62882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4562e3055ed2549b93e450d764e41b62a485d16bafb1f1ed6b67fd610444aa44`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4de57a4336a3a0ab0e109ff4c769bce1d354c121fe62fd5f6063c53fd009d61`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542e5df0dc5eda03440d4a00ca01ceefa7cb8282a9d7b406fd54dabcdf4197c0`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8586280a334732de42259c879b0c7d8a9a16bfcb8764f797a9cdd720aac766bf`  
		Last Modified: Wed, 14 Apr 2021 20:20:50 GMT  
		Size: 6.6 MB (6569726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8926df9acf368d91f3a21b4465c45354ea1b091727a6297d78629f0e963576ca`  
		Last Modified: Wed, 14 Apr 2021 20:20:49 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8378b8f62b916e8b443090f2421b0c73ddef9f0fe93544516b22837b95fa9a29`  
		Last Modified: Fri, 30 Apr 2021 21:21:34 GMT  
		Size: 984.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84616459de5ba2ec2dbc43651c8f2b3200a8f0b820a3faedbd4aea29ace856b9`  
		Last Modified: Wed, 21 Jul 2021 18:21:33 GMT  
		Size: 2.6 KB (2623 bytes)  
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
$ docker pull docker@sha256:81f35202223dcd33991fcb0e12d287f854dfb63b0b47e0c805ed87c0dfc4c9b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67244127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf089d844e8ebe17e6ac30dfff7c0bbc32aa01d77a7304b47d2daa74d2f06892`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:33 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 15 Jun 2021 22:34:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:39 GMT
CMD ["sh"]
# Tue, 15 Jun 2021 22:34:47 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 15 Jun 2021 22:34:47 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 15 Jun 2021 22:34:48 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 15 Jun 2021 22:34:49 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:40:04 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:40:04 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:40:04 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:40:04 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:40:04 GMT
CMD []
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31451232b129e45d3b41a480e8f13df618906b6c2d3f6808dd70af1c71c0c154`  
		Last Modified: Tue, 15 Jun 2021 22:37:13 GMT  
		Size: 56.0 MB (55994351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bf8ca3358da3ae665e1c0c6e8a117f99178132f6a06593366c7ddce01cbd06`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916486c0da5ab2c0c64755b93c82d4ac57ad744c716cf205359b065b6096fcc1`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6e4d5edf6083ebb0300314dd90b0e4f40774a97e9394beaef654f635ec9bc2`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b598f2ed6f9fffa88a0dd4af8122cbbb4d0383b323de4bbbb671c77d790f74e6`  
		Last Modified: Tue, 15 Jun 2021 22:37:35 GMT  
		Size: 6.5 MB (6473103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6a38cf5d478452ab564814ed415a03fd8e566b58acdf6ee1388def50e49288`  
		Last Modified: Tue, 15 Jun 2021 22:37:34 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f80a9f85d33aa617ebc418c71f03b18aab259e5b8c4211374bbaed978d539`  
		Last Modified: Tue, 15 Jun 2021 22:37:34 GMT  
		Size: 980.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c333460c45808f2731f666614c70d9abb31a212c6e1c078b984bd50adee65ea`  
		Last Modified: Wed, 21 Jul 2021 18:42:24 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19-dind-rootless`

```console
$ docker pull docker@sha256:cc0898441121342ab4067df7fb2403bd79a0024364063ea3affd6b7f44f6e71c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `docker:19-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:c95faa54ab9657a6c605fdbd02ef783483489ee3e50726c26e3a4483cdf7fe4b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94877570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a734f636681143612b8d30799f1eb31e9739a7f75d531af0677ef2db336bb5d`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:17:37 GMT
ENV DOCKER_VERSION=19.03.15
# Wed, 14 Apr 2021 20:17:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 14 Apr 2021 20:17:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 14 Apr 2021 20:17:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:17:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 14 Apr 2021 20:17:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 14 Apr 2021 20:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:17:46 GMT
CMD ["sh"]
# Wed, 14 Apr 2021 20:17:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 14 Apr 2021 20:17:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 30 Apr 2021 21:20:01 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 30 Apr 2021 21:20:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:20:02 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:20:02 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:20:02 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:20:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:20:02 GMT
CMD []
# Wed, 21 Jul 2021 18:20:07 GMT
RUN apk add --no-cache iproute2
# Wed, 21 Jul 2021 18:20:08 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 21 Jul 2021 18:20:08 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 21 Jul 2021 18:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 21 Jul 2021 18:20:11 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 21 Jul 2021 18:20:11 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 21 Jul 2021 18:20:12 GMT
USER rootless
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09182082685c0a1147c9f22948720af9bb3544411a1b50562d18071cf31b8e21`  
		Last Modified: Wed, 14 Apr 2021 20:20:33 GMT  
		Size: 62.9 MB (62882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4562e3055ed2549b93e450d764e41b62a485d16bafb1f1ed6b67fd610444aa44`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4de57a4336a3a0ab0e109ff4c769bce1d354c121fe62fd5f6063c53fd009d61`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542e5df0dc5eda03440d4a00ca01ceefa7cb8282a9d7b406fd54dabcdf4197c0`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8586280a334732de42259c879b0c7d8a9a16bfcb8764f797a9cdd720aac766bf`  
		Last Modified: Wed, 14 Apr 2021 20:20:50 GMT  
		Size: 6.6 MB (6569726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8926df9acf368d91f3a21b4465c45354ea1b091727a6297d78629f0e963576ca`  
		Last Modified: Wed, 14 Apr 2021 20:20:49 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8378b8f62b916e8b443090f2421b0c73ddef9f0fe93544516b22837b95fa9a29`  
		Last Modified: Fri, 30 Apr 2021 21:21:34 GMT  
		Size: 984.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84616459de5ba2ec2dbc43651c8f2b3200a8f0b820a3faedbd4aea29ace856b9`  
		Last Modified: Wed, 21 Jul 2021 18:21:33 GMT  
		Size: 2.6 KB (2623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4020f645e5bd6b55e6045a0ce7fbc784eba3de98f8c238428833f7e9046f020`  
		Last Modified: Wed, 21 Jul 2021 18:21:47 GMT  
		Size: 1.1 MB (1131572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0064f2f0f4e800f3ebcf2c026b7c986333b3faa730b424dfb582f262b090d8`  
		Last Modified: Wed, 21 Jul 2021 18:21:47 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ebe403ae1de3318a64b3f231563a13a9da2f59d9abeaed6273811eefee3911e`  
		Last Modified: Wed, 21 Jul 2021 18:21:47 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88b1362e9ec1dea3e17da6db78ad5a40644da1a3827dcddde58917d8f61da3b`  
		Last Modified: Wed, 21 Jul 2021 18:21:51 GMT  
		Size: 19.4 MB (19422716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7afa2f10e3a7ba0c2847992c06e03c9ddede8ea3665e580db003a1c7ff40d7a`  
		Last Modified: Wed, 21 Jul 2021 18:21:47 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19-git`

```console
$ docker pull docker@sha256:09050c00a10184c03fa318e674133bf65e901b560e4ba07f52286bceee729d5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19-git` - linux; amd64

```console
$ docker pull docker@sha256:e241d82a7883bc40f80a72dd5f22ea7f7dc5b21ac76bd1dab271cb3b4d0ce3f2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74143302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c326f672251d3c2920e528b964728d9b20d5db3c421aec0cc05dce3915538b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:17:37 GMT
ENV DOCKER_VERSION=19.03.15
# Wed, 14 Apr 2021 20:17:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 14 Apr 2021 20:17:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 14 Apr 2021 20:17:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:17:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 14 Apr 2021 20:17:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 14 Apr 2021 20:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:17:46 GMT
CMD ["sh"]
# Wed, 14 Apr 2021 20:18:11 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09182082685c0a1147c9f22948720af9bb3544411a1b50562d18071cf31b8e21`  
		Last Modified: Wed, 14 Apr 2021 20:20:33 GMT  
		Size: 62.9 MB (62882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4562e3055ed2549b93e450d764e41b62a485d16bafb1f1ed6b67fd610444aa44`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4de57a4336a3a0ab0e109ff4c769bce1d354c121fe62fd5f6063c53fd009d61`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542e5df0dc5eda03440d4a00ca01ceefa7cb8282a9d7b406fd54dabcdf4197c0`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9f7f9542e413c7a06085d37d91b4eb7333df65cd7187a7c3507af2726649d1`  
		Last Modified: Wed, 14 Apr 2021 20:21:27 GMT  
		Size: 6.4 MB (6396373 bytes)  
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
$ docker pull docker@sha256:a554b216f7c86c0270f044575198d90b54229cce2784ec227c4aaae956f49914
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67250943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dcda5b8bb97d16ea565ebabfa6a00deda290b0422c4a59e4f8c289e5a1361a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:33 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 15 Jun 2021 22:34:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:39 GMT
CMD ["sh"]
# Tue, 15 Jun 2021 22:34:57 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31451232b129e45d3b41a480e8f13df618906b6c2d3f6808dd70af1c71c0c154`  
		Last Modified: Tue, 15 Jun 2021 22:37:13 GMT  
		Size: 56.0 MB (55994351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bf8ca3358da3ae665e1c0c6e8a117f99178132f6a06593366c7ddce01cbd06`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916486c0da5ab2c0c64755b93c82d4ac57ad744c716cf205359b065b6096fcc1`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6e4d5edf6083ebb0300314dd90b0e4f40774a97e9394beaef654f635ec9bc2`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a85a60edad049c09e2e5cf7baa7ac8adb3bad6062580f2d31fde8abef5a9020`  
		Last Modified: Tue, 15 Jun 2021 22:37:52 GMT  
		Size: 6.5 MB (6484831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03`

```console
$ docker pull docker@sha256:8209ca87a5bd61f58b988d239bfeeea1e55ba0b0e7e3256c1bc1e5abe68a178b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03` - linux; amd64

```console
$ docker pull docker@sha256:51b4ccfcc03639a1bf1755de6789aaf506697aa416136e3874499296c179241d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67746929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33d3743ceb6ae9c655769327f4d723433841510d5d9602307e79189807dac391`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:17:37 GMT
ENV DOCKER_VERSION=19.03.15
# Wed, 14 Apr 2021 20:17:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 14 Apr 2021 20:17:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 14 Apr 2021 20:17:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:17:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 14 Apr 2021 20:17:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 14 Apr 2021 20:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:17:46 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09182082685c0a1147c9f22948720af9bb3544411a1b50562d18071cf31b8e21`  
		Last Modified: Wed, 14 Apr 2021 20:20:33 GMT  
		Size: 62.9 MB (62882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4562e3055ed2549b93e450d764e41b62a485d16bafb1f1ed6b67fd610444aa44`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4de57a4336a3a0ab0e109ff4c769bce1d354c121fe62fd5f6063c53fd009d61`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542e5df0dc5eda03440d4a00ca01ceefa7cb8282a9d7b406fd54dabcdf4197c0`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 149.0 B  
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
$ docker pull docker@sha256:b949cbbb354d40d2ec4d168cbb0f24f84d2b6b68e32f6f9dbda004992877194b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60766112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59291a2ff3232902f748ccdb0bfa9d9be4e3d9394a58a8f70ac80001eaa80c03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:33 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 15 Jun 2021 22:34:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:39 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31451232b129e45d3b41a480e8f13df618906b6c2d3f6808dd70af1c71c0c154`  
		Last Modified: Tue, 15 Jun 2021 22:37:13 GMT  
		Size: 56.0 MB (55994351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bf8ca3358da3ae665e1c0c6e8a117f99178132f6a06593366c7ddce01cbd06`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916486c0da5ab2c0c64755b93c82d4ac57ad744c716cf205359b065b6096fcc1`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6e4d5edf6083ebb0300314dd90b0e4f40774a97e9394beaef654f635ec9bc2`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-dind`

```console
$ docker pull docker@sha256:3843cb86a094abeeb427c9e6365a0b2de6dfcba389d0870aebba9e4746d52014
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03-dind` - linux; amd64

```console
$ docker pull docker@sha256:1875a3437d87a2fa8ec5e6fcd3233a98d571fa9692516b1e7d8eb18b7dca87a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74321571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3b7a5678ece1ea157bb3f4fb6372911ad054e9d271f09d6401fb53e6a8c97d`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:17:37 GMT
ENV DOCKER_VERSION=19.03.15
# Wed, 14 Apr 2021 20:17:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 14 Apr 2021 20:17:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 14 Apr 2021 20:17:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:17:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 14 Apr 2021 20:17:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 14 Apr 2021 20:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:17:46 GMT
CMD ["sh"]
# Wed, 14 Apr 2021 20:17:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 14 Apr 2021 20:17:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 30 Apr 2021 21:20:01 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 30 Apr 2021 21:20:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:20:02 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:20:02 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:20:02 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:20:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:20:02 GMT
CMD []
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09182082685c0a1147c9f22948720af9bb3544411a1b50562d18071cf31b8e21`  
		Last Modified: Wed, 14 Apr 2021 20:20:33 GMT  
		Size: 62.9 MB (62882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4562e3055ed2549b93e450d764e41b62a485d16bafb1f1ed6b67fd610444aa44`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4de57a4336a3a0ab0e109ff4c769bce1d354c121fe62fd5f6063c53fd009d61`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542e5df0dc5eda03440d4a00ca01ceefa7cb8282a9d7b406fd54dabcdf4197c0`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8586280a334732de42259c879b0c7d8a9a16bfcb8764f797a9cdd720aac766bf`  
		Last Modified: Wed, 14 Apr 2021 20:20:50 GMT  
		Size: 6.6 MB (6569726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8926df9acf368d91f3a21b4465c45354ea1b091727a6297d78629f0e963576ca`  
		Last Modified: Wed, 14 Apr 2021 20:20:49 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8378b8f62b916e8b443090f2421b0c73ddef9f0fe93544516b22837b95fa9a29`  
		Last Modified: Fri, 30 Apr 2021 21:21:34 GMT  
		Size: 984.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84616459de5ba2ec2dbc43651c8f2b3200a8f0b820a3faedbd4aea29ace856b9`  
		Last Modified: Wed, 21 Jul 2021 18:21:33 GMT  
		Size: 2.6 KB (2623 bytes)  
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
$ docker pull docker@sha256:81f35202223dcd33991fcb0e12d287f854dfb63b0b47e0c805ed87c0dfc4c9b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67244127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf089d844e8ebe17e6ac30dfff7c0bbc32aa01d77a7304b47d2daa74d2f06892`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:33 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 15 Jun 2021 22:34:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:39 GMT
CMD ["sh"]
# Tue, 15 Jun 2021 22:34:47 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 15 Jun 2021 22:34:47 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 15 Jun 2021 22:34:48 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 15 Jun 2021 22:34:49 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:40:04 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:40:04 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:40:04 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:40:04 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:40:04 GMT
CMD []
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31451232b129e45d3b41a480e8f13df618906b6c2d3f6808dd70af1c71c0c154`  
		Last Modified: Tue, 15 Jun 2021 22:37:13 GMT  
		Size: 56.0 MB (55994351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bf8ca3358da3ae665e1c0c6e8a117f99178132f6a06593366c7ddce01cbd06`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916486c0da5ab2c0c64755b93c82d4ac57ad744c716cf205359b065b6096fcc1`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6e4d5edf6083ebb0300314dd90b0e4f40774a97e9394beaef654f635ec9bc2`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b598f2ed6f9fffa88a0dd4af8122cbbb4d0383b323de4bbbb671c77d790f74e6`  
		Last Modified: Tue, 15 Jun 2021 22:37:35 GMT  
		Size: 6.5 MB (6473103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6a38cf5d478452ab564814ed415a03fd8e566b58acdf6ee1388def50e49288`  
		Last Modified: Tue, 15 Jun 2021 22:37:34 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f80a9f85d33aa617ebc418c71f03b18aab259e5b8c4211374bbaed978d539`  
		Last Modified: Tue, 15 Jun 2021 22:37:34 GMT  
		Size: 980.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c333460c45808f2731f666614c70d9abb31a212c6e1c078b984bd50adee65ea`  
		Last Modified: Wed, 21 Jul 2021 18:42:24 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-dind-rootless`

```console
$ docker pull docker@sha256:cc0898441121342ab4067df7fb2403bd79a0024364063ea3affd6b7f44f6e71c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `docker:19.03-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:c95faa54ab9657a6c605fdbd02ef783483489ee3e50726c26e3a4483cdf7fe4b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94877570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a734f636681143612b8d30799f1eb31e9739a7f75d531af0677ef2db336bb5d`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:17:37 GMT
ENV DOCKER_VERSION=19.03.15
# Wed, 14 Apr 2021 20:17:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 14 Apr 2021 20:17:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 14 Apr 2021 20:17:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:17:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 14 Apr 2021 20:17:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 14 Apr 2021 20:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:17:46 GMT
CMD ["sh"]
# Wed, 14 Apr 2021 20:17:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 14 Apr 2021 20:17:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 30 Apr 2021 21:20:01 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 30 Apr 2021 21:20:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:20:02 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:20:02 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:20:02 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:20:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:20:02 GMT
CMD []
# Wed, 21 Jul 2021 18:20:07 GMT
RUN apk add --no-cache iproute2
# Wed, 21 Jul 2021 18:20:08 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 21 Jul 2021 18:20:08 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 21 Jul 2021 18:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 21 Jul 2021 18:20:11 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 21 Jul 2021 18:20:11 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 21 Jul 2021 18:20:12 GMT
USER rootless
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09182082685c0a1147c9f22948720af9bb3544411a1b50562d18071cf31b8e21`  
		Last Modified: Wed, 14 Apr 2021 20:20:33 GMT  
		Size: 62.9 MB (62882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4562e3055ed2549b93e450d764e41b62a485d16bafb1f1ed6b67fd610444aa44`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4de57a4336a3a0ab0e109ff4c769bce1d354c121fe62fd5f6063c53fd009d61`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542e5df0dc5eda03440d4a00ca01ceefa7cb8282a9d7b406fd54dabcdf4197c0`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8586280a334732de42259c879b0c7d8a9a16bfcb8764f797a9cdd720aac766bf`  
		Last Modified: Wed, 14 Apr 2021 20:20:50 GMT  
		Size: 6.6 MB (6569726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8926df9acf368d91f3a21b4465c45354ea1b091727a6297d78629f0e963576ca`  
		Last Modified: Wed, 14 Apr 2021 20:20:49 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8378b8f62b916e8b443090f2421b0c73ddef9f0fe93544516b22837b95fa9a29`  
		Last Modified: Fri, 30 Apr 2021 21:21:34 GMT  
		Size: 984.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84616459de5ba2ec2dbc43651c8f2b3200a8f0b820a3faedbd4aea29ace856b9`  
		Last Modified: Wed, 21 Jul 2021 18:21:33 GMT  
		Size: 2.6 KB (2623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4020f645e5bd6b55e6045a0ce7fbc784eba3de98f8c238428833f7e9046f020`  
		Last Modified: Wed, 21 Jul 2021 18:21:47 GMT  
		Size: 1.1 MB (1131572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0064f2f0f4e800f3ebcf2c026b7c986333b3faa730b424dfb582f262b090d8`  
		Last Modified: Wed, 21 Jul 2021 18:21:47 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ebe403ae1de3318a64b3f231563a13a9da2f59d9abeaed6273811eefee3911e`  
		Last Modified: Wed, 21 Jul 2021 18:21:47 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88b1362e9ec1dea3e17da6db78ad5a40644da1a3827dcddde58917d8f61da3b`  
		Last Modified: Wed, 21 Jul 2021 18:21:51 GMT  
		Size: 19.4 MB (19422716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7afa2f10e3a7ba0c2847992c06e03c9ddede8ea3665e580db003a1c7ff40d7a`  
		Last Modified: Wed, 21 Jul 2021 18:21:47 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-git`

```console
$ docker pull docker@sha256:09050c00a10184c03fa318e674133bf65e901b560e4ba07f52286bceee729d5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03-git` - linux; amd64

```console
$ docker pull docker@sha256:e241d82a7883bc40f80a72dd5f22ea7f7dc5b21ac76bd1dab271cb3b4d0ce3f2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74143302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c326f672251d3c2920e528b964728d9b20d5db3c421aec0cc05dce3915538b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:17:37 GMT
ENV DOCKER_VERSION=19.03.15
# Wed, 14 Apr 2021 20:17:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 14 Apr 2021 20:17:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 14 Apr 2021 20:17:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:17:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 14 Apr 2021 20:17:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 14 Apr 2021 20:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:17:46 GMT
CMD ["sh"]
# Wed, 14 Apr 2021 20:18:11 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09182082685c0a1147c9f22948720af9bb3544411a1b50562d18071cf31b8e21`  
		Last Modified: Wed, 14 Apr 2021 20:20:33 GMT  
		Size: 62.9 MB (62882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4562e3055ed2549b93e450d764e41b62a485d16bafb1f1ed6b67fd610444aa44`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4de57a4336a3a0ab0e109ff4c769bce1d354c121fe62fd5f6063c53fd009d61`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542e5df0dc5eda03440d4a00ca01ceefa7cb8282a9d7b406fd54dabcdf4197c0`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9f7f9542e413c7a06085d37d91b4eb7333df65cd7187a7c3507af2726649d1`  
		Last Modified: Wed, 14 Apr 2021 20:21:27 GMT  
		Size: 6.4 MB (6396373 bytes)  
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
$ docker pull docker@sha256:a554b216f7c86c0270f044575198d90b54229cce2784ec227c4aaae956f49914
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67250943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dcda5b8bb97d16ea565ebabfa6a00deda290b0422c4a59e4f8c289e5a1361a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:33 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 15 Jun 2021 22:34:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:39 GMT
CMD ["sh"]
# Tue, 15 Jun 2021 22:34:57 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31451232b129e45d3b41a480e8f13df618906b6c2d3f6808dd70af1c71c0c154`  
		Last Modified: Tue, 15 Jun 2021 22:37:13 GMT  
		Size: 56.0 MB (55994351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bf8ca3358da3ae665e1c0c6e8a117f99178132f6a06593366c7ddce01cbd06`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916486c0da5ab2c0c64755b93c82d4ac57ad744c716cf205359b065b6096fcc1`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6e4d5edf6083ebb0300314dd90b0e4f40774a97e9394beaef654f635ec9bc2`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a85a60edad049c09e2e5cf7baa7ac8adb3bad6062580f2d31fde8abef5a9020`  
		Last Modified: Tue, 15 Jun 2021 22:37:52 GMT  
		Size: 6.5 MB (6484831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.15`

```console
$ docker pull docker@sha256:ea1f0761c92b600417ad14bc9b2b3a30abf8e96e94895fee6cbb5353316f30b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:19.03.15` - linux; amd64

```console
$ docker pull docker@sha256:51b4ccfcc03639a1bf1755de6789aaf506697aa416136e3874499296c179241d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67746929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33d3743ceb6ae9c655769327f4d723433841510d5d9602307e79189807dac391`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:17:37 GMT
ENV DOCKER_VERSION=19.03.15
# Wed, 14 Apr 2021 20:17:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 14 Apr 2021 20:17:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 14 Apr 2021 20:17:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:17:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 14 Apr 2021 20:17:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 14 Apr 2021 20:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:17:46 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09182082685c0a1147c9f22948720af9bb3544411a1b50562d18071cf31b8e21`  
		Last Modified: Wed, 14 Apr 2021 20:20:33 GMT  
		Size: 62.9 MB (62882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4562e3055ed2549b93e450d764e41b62a485d16bafb1f1ed6b67fd610444aa44`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4de57a4336a3a0ab0e109ff4c769bce1d354c121fe62fd5f6063c53fd009d61`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542e5df0dc5eda03440d4a00ca01ceefa7cb8282a9d7b406fd54dabcdf4197c0`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.15` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:b949cbbb354d40d2ec4d168cbb0f24f84d2b6b68e32f6f9dbda004992877194b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60766112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59291a2ff3232902f748ccdb0bfa9d9be4e3d9394a58a8f70ac80001eaa80c03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:33 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 15 Jun 2021 22:34:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:39 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31451232b129e45d3b41a480e8f13df618906b6c2d3f6808dd70af1c71c0c154`  
		Last Modified: Tue, 15 Jun 2021 22:37:13 GMT  
		Size: 56.0 MB (55994351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bf8ca3358da3ae665e1c0c6e8a117f99178132f6a06593366c7ddce01cbd06`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916486c0da5ab2c0c64755b93c82d4ac57ad744c716cf205359b065b6096fcc1`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6e4d5edf6083ebb0300314dd90b0e4f40774a97e9394beaef654f635ec9bc2`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.15-dind`

```console
$ docker pull docker@sha256:c85365ad08c7f6e02ac962a8759c4a5b8512ea5c294d3bb9ed25fca52e9e22e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:19.03.15-dind` - linux; amd64

```console
$ docker pull docker@sha256:1875a3437d87a2fa8ec5e6fcd3233a98d571fa9692516b1e7d8eb18b7dca87a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74321571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3b7a5678ece1ea157bb3f4fb6372911ad054e9d271f09d6401fb53e6a8c97d`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:17:37 GMT
ENV DOCKER_VERSION=19.03.15
# Wed, 14 Apr 2021 20:17:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 14 Apr 2021 20:17:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 14 Apr 2021 20:17:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:17:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 14 Apr 2021 20:17:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 14 Apr 2021 20:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:17:46 GMT
CMD ["sh"]
# Wed, 14 Apr 2021 20:17:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 14 Apr 2021 20:17:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 30 Apr 2021 21:20:01 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 30 Apr 2021 21:20:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:20:02 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:20:02 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:20:02 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:20:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:20:02 GMT
CMD []
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09182082685c0a1147c9f22948720af9bb3544411a1b50562d18071cf31b8e21`  
		Last Modified: Wed, 14 Apr 2021 20:20:33 GMT  
		Size: 62.9 MB (62882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4562e3055ed2549b93e450d764e41b62a485d16bafb1f1ed6b67fd610444aa44`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4de57a4336a3a0ab0e109ff4c769bce1d354c121fe62fd5f6063c53fd009d61`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542e5df0dc5eda03440d4a00ca01ceefa7cb8282a9d7b406fd54dabcdf4197c0`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8586280a334732de42259c879b0c7d8a9a16bfcb8764f797a9cdd720aac766bf`  
		Last Modified: Wed, 14 Apr 2021 20:20:50 GMT  
		Size: 6.6 MB (6569726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8926df9acf368d91f3a21b4465c45354ea1b091727a6297d78629f0e963576ca`  
		Last Modified: Wed, 14 Apr 2021 20:20:49 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8378b8f62b916e8b443090f2421b0c73ddef9f0fe93544516b22837b95fa9a29`  
		Last Modified: Fri, 30 Apr 2021 21:21:34 GMT  
		Size: 984.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84616459de5ba2ec2dbc43651c8f2b3200a8f0b820a3faedbd4aea29ace856b9`  
		Last Modified: Wed, 21 Jul 2021 18:21:33 GMT  
		Size: 2.6 KB (2623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.15-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:81f35202223dcd33991fcb0e12d287f854dfb63b0b47e0c805ed87c0dfc4c9b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67244127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf089d844e8ebe17e6ac30dfff7c0bbc32aa01d77a7304b47d2daa74d2f06892`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:33 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 15 Jun 2021 22:34:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:39 GMT
CMD ["sh"]
# Tue, 15 Jun 2021 22:34:47 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 15 Jun 2021 22:34:47 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 15 Jun 2021 22:34:48 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 15 Jun 2021 22:34:49 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:40:04 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:40:04 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:40:04 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:40:04 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:40:04 GMT
CMD []
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31451232b129e45d3b41a480e8f13df618906b6c2d3f6808dd70af1c71c0c154`  
		Last Modified: Tue, 15 Jun 2021 22:37:13 GMT  
		Size: 56.0 MB (55994351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bf8ca3358da3ae665e1c0c6e8a117f99178132f6a06593366c7ddce01cbd06`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916486c0da5ab2c0c64755b93c82d4ac57ad744c716cf205359b065b6096fcc1`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6e4d5edf6083ebb0300314dd90b0e4f40774a97e9394beaef654f635ec9bc2`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b598f2ed6f9fffa88a0dd4af8122cbbb4d0383b323de4bbbb671c77d790f74e6`  
		Last Modified: Tue, 15 Jun 2021 22:37:35 GMT  
		Size: 6.5 MB (6473103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6a38cf5d478452ab564814ed415a03fd8e566b58acdf6ee1388def50e49288`  
		Last Modified: Tue, 15 Jun 2021 22:37:34 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f80a9f85d33aa617ebc418c71f03b18aab259e5b8c4211374bbaed978d539`  
		Last Modified: Tue, 15 Jun 2021 22:37:34 GMT  
		Size: 980.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c333460c45808f2731f666614c70d9abb31a212c6e1c078b984bd50adee65ea`  
		Last Modified: Wed, 21 Jul 2021 18:42:24 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.15-dind-rootless`

```console
$ docker pull docker@sha256:cc0898441121342ab4067df7fb2403bd79a0024364063ea3affd6b7f44f6e71c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `docker:19.03.15-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:c95faa54ab9657a6c605fdbd02ef783483489ee3e50726c26e3a4483cdf7fe4b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94877570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a734f636681143612b8d30799f1eb31e9739a7f75d531af0677ef2db336bb5d`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:17:37 GMT
ENV DOCKER_VERSION=19.03.15
# Wed, 14 Apr 2021 20:17:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 14 Apr 2021 20:17:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 14 Apr 2021 20:17:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:17:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 14 Apr 2021 20:17:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 14 Apr 2021 20:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:17:46 GMT
CMD ["sh"]
# Wed, 14 Apr 2021 20:17:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 14 Apr 2021 20:17:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 30 Apr 2021 21:20:01 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 30 Apr 2021 21:20:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:20:02 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:20:02 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:20:02 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:20:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:20:02 GMT
CMD []
# Wed, 21 Jul 2021 18:20:07 GMT
RUN apk add --no-cache iproute2
# Wed, 21 Jul 2021 18:20:08 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 21 Jul 2021 18:20:08 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 21 Jul 2021 18:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 21 Jul 2021 18:20:11 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 21 Jul 2021 18:20:11 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 21 Jul 2021 18:20:12 GMT
USER rootless
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09182082685c0a1147c9f22948720af9bb3544411a1b50562d18071cf31b8e21`  
		Last Modified: Wed, 14 Apr 2021 20:20:33 GMT  
		Size: 62.9 MB (62882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4562e3055ed2549b93e450d764e41b62a485d16bafb1f1ed6b67fd610444aa44`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4de57a4336a3a0ab0e109ff4c769bce1d354c121fe62fd5f6063c53fd009d61`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542e5df0dc5eda03440d4a00ca01ceefa7cb8282a9d7b406fd54dabcdf4197c0`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8586280a334732de42259c879b0c7d8a9a16bfcb8764f797a9cdd720aac766bf`  
		Last Modified: Wed, 14 Apr 2021 20:20:50 GMT  
		Size: 6.6 MB (6569726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8926df9acf368d91f3a21b4465c45354ea1b091727a6297d78629f0e963576ca`  
		Last Modified: Wed, 14 Apr 2021 20:20:49 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8378b8f62b916e8b443090f2421b0c73ddef9f0fe93544516b22837b95fa9a29`  
		Last Modified: Fri, 30 Apr 2021 21:21:34 GMT  
		Size: 984.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84616459de5ba2ec2dbc43651c8f2b3200a8f0b820a3faedbd4aea29ace856b9`  
		Last Modified: Wed, 21 Jul 2021 18:21:33 GMT  
		Size: 2.6 KB (2623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4020f645e5bd6b55e6045a0ce7fbc784eba3de98f8c238428833f7e9046f020`  
		Last Modified: Wed, 21 Jul 2021 18:21:47 GMT  
		Size: 1.1 MB (1131572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0064f2f0f4e800f3ebcf2c026b7c986333b3faa730b424dfb582f262b090d8`  
		Last Modified: Wed, 21 Jul 2021 18:21:47 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ebe403ae1de3318a64b3f231563a13a9da2f59d9abeaed6273811eefee3911e`  
		Last Modified: Wed, 21 Jul 2021 18:21:47 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88b1362e9ec1dea3e17da6db78ad5a40644da1a3827dcddde58917d8f61da3b`  
		Last Modified: Wed, 21 Jul 2021 18:21:51 GMT  
		Size: 19.4 MB (19422716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7afa2f10e3a7ba0c2847992c06e03c9ddede8ea3665e580db003a1c7ff40d7a`  
		Last Modified: Wed, 21 Jul 2021 18:21:47 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.15-git`

```console
$ docker pull docker@sha256:5fbf776b8bb0e431ff612631fb058c5d8d82736d29fedf068d91f7487a2c3587
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:19.03.15-git` - linux; amd64

```console
$ docker pull docker@sha256:e241d82a7883bc40f80a72dd5f22ea7f7dc5b21ac76bd1dab271cb3b4d0ce3f2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74143302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c326f672251d3c2920e528b964728d9b20d5db3c421aec0cc05dce3915538b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:17:37 GMT
ENV DOCKER_VERSION=19.03.15
# Wed, 14 Apr 2021 20:17:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 14 Apr 2021 20:17:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 14 Apr 2021 20:17:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:17:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 14 Apr 2021 20:17:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 14 Apr 2021 20:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:17:46 GMT
CMD ["sh"]
# Wed, 14 Apr 2021 20:18:11 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09182082685c0a1147c9f22948720af9bb3544411a1b50562d18071cf31b8e21`  
		Last Modified: Wed, 14 Apr 2021 20:20:33 GMT  
		Size: 62.9 MB (62882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4562e3055ed2549b93e450d764e41b62a485d16bafb1f1ed6b67fd610444aa44`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4de57a4336a3a0ab0e109ff4c769bce1d354c121fe62fd5f6063c53fd009d61`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542e5df0dc5eda03440d4a00ca01ceefa7cb8282a9d7b406fd54dabcdf4197c0`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9f7f9542e413c7a06085d37d91b4eb7333df65cd7187a7c3507af2726649d1`  
		Last Modified: Wed, 14 Apr 2021 20:21:27 GMT  
		Size: 6.4 MB (6396373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.15-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:a554b216f7c86c0270f044575198d90b54229cce2784ec227c4aaae956f49914
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67250943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dcda5b8bb97d16ea565ebabfa6a00deda290b0422c4a59e4f8c289e5a1361a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:33 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 15 Jun 2021 22:34:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:39 GMT
CMD ["sh"]
# Tue, 15 Jun 2021 22:34:57 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31451232b129e45d3b41a480e8f13df618906b6c2d3f6808dd70af1c71c0c154`  
		Last Modified: Tue, 15 Jun 2021 22:37:13 GMT  
		Size: 56.0 MB (55994351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bf8ca3358da3ae665e1c0c6e8a117f99178132f6a06593366c7ddce01cbd06`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916486c0da5ab2c0c64755b93c82d4ac57ad744c716cf205359b065b6096fcc1`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6e4d5edf6083ebb0300314dd90b0e4f40774a97e9394beaef654f635ec9bc2`  
		Last Modified: Tue, 15 Jun 2021 22:37:02 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a85a60edad049c09e2e5cf7baa7ac8adb3bad6062580f2d31fde8abef5a9020`  
		Last Modified: Tue, 15 Jun 2021 22:37:52 GMT  
		Size: 6.5 MB (6484831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20`

```console
$ docker pull docker@sha256:bfc499cef26daa22da31b76be1752813a6921ee1fa1dd1f56d4fdf19c701d332
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20` - linux; amd64

```console
$ docker pull docker@sha256:63cb2df6dfe1fb041b952ddb9f75c69569331fa39577bc41a3e56cf8f79f7e2e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75111066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08bdaf2f88f90320cd3e92a469969efb1f066c6d318631f94e7864828abd7c75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Jun 2021 21:21:16 GMT
ENV DOCKER_VERSION=20.10.7
# Thu, 03 Jun 2021 21:21:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:21:24 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Jun 2021 21:21:25 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Jun 2021 21:21:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Jun 2021 21:21:25 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c521bbbd9945cde2415eae95c3a2a604ea5ca18eb86ab5cadeb589d3b8a13185`  
		Last Modified: Thu, 03 Jun 2021 21:22:44 GMT  
		Size: 70.2 MB (70247077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59707d521c45c42bbb7dbbef463d5d3800859f20122fb54894f0c79d9b435483`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26abe223b186967eef77715b2c6efd147f3a203a0c7b19e61a8947dab4236397`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d806bc203610fb061281b581a0b2522c9fcbd15e55c55ac0c496c9b1dbe63b0`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:85fa729480d21cd25e5b7f2ba40b53492068501da59e4c23639bd41c5a43040e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69194991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df445af6242a928d36d8a3b4259ba3db9de1d7be5c9806e49b2746cdab4df048`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:00 GMT
ENV DOCKER_VERSION=20.10.7
# Tue, 15 Jun 2021 22:34:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:06 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:07 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829992c79f06822894e73d9a962015a75a5d65ef5a60de627fbb32a973dc0462`  
		Last Modified: Tue, 15 Jun 2021 22:36:03 GMT  
		Size: 64.4 MB (64423231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6714f1b9096eb751a830a9dd13c67cd5e669c68403f1675efd7e78ff8905896d`  
		Last Modified: Tue, 15 Jun 2021 22:35:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997b259c822c244af1192eb31913d45df7f269da56a37fa1c7dc5b9fe273134`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b041c447a8f648b5910833f3c76e5a3231d34a6d76b56d0c22c64b232da92519`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind`

```console
$ docker pull docker@sha256:b36fdccb118bfaa8d5026da5183a077b87bc790051fcd2c5686bfb8f7fa2563c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind` - linux; amd64

```console
$ docker pull docker@sha256:4f0e01f764b10c633334cb44fe6926a27b06390b482cb24e1add823b2ca781fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.7 MB (81726552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca749f2062c41ad54191b9c242dd1b3f6132a11299b251fc2128e37c9800ebba`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Jun 2021 21:21:16 GMT
ENV DOCKER_VERSION=20.10.7
# Thu, 03 Jun 2021 21:21:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:21:24 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Jun 2021 21:21:25 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Jun 2021 21:21:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Jun 2021 21:21:25 GMT
CMD ["sh"]
# Thu, 03 Jun 2021 21:21:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 03 Jun 2021 21:21:33 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 03 Jun 2021 21:21:33 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 03 Jun 2021 21:21:34 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:19:42 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:19:42 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:19:42 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:19:43 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:19:43 GMT
CMD []
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c521bbbd9945cde2415eae95c3a2a604ea5ca18eb86ab5cadeb589d3b8a13185`  
		Last Modified: Thu, 03 Jun 2021 21:22:44 GMT  
		Size: 70.2 MB (70247077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59707d521c45c42bbb7dbbef463d5d3800859f20122fb54894f0c79d9b435483`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26abe223b186967eef77715b2c6efd147f3a203a0c7b19e61a8947dab4236397`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d806bc203610fb061281b581a0b2522c9fcbd15e55c55ac0c496c9b1dbe63b0`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918595a0e69b201bdd25b6da798216629c61256ba541408487536b3953169aa6`  
		Last Modified: Thu, 03 Jun 2021 21:23:02 GMT  
		Size: 6.6 MB (6610580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf6f33d26f8a966febfc6cfc6677aadddee7d77d37476f660cb4b3e9d4659bd`  
		Last Modified: Thu, 03 Jun 2021 21:23:00 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0522a0264f7030f681722a192902d53421d886507aac6dafeced99b9ed932a`  
		Last Modified: Thu, 03 Jun 2021 21:23:00 GMT  
		Size: 978.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8d570be2274d0bfa2a8df30021696ca2af3e7a44553d24aa5f58314e32590b`  
		Last Modified: Wed, 21 Jul 2021 18:20:48 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:778521a7c301de26994f7aca616ab10c1bc35b8f66b802345d0cad89af381dcb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75712568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a81be9fbf6452a40403d288e5b6a6c422b96bb07fc23d07ac2d46d5a92a63fa`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:00 GMT
ENV DOCKER_VERSION=20.10.7
# Tue, 15 Jun 2021 22:34:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:06 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:07 GMT
CMD ["sh"]
# Tue, 15 Jun 2021 22:34:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 15 Jun 2021 22:34:17 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 15 Jun 2021 22:34:17 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 15 Jun 2021 22:34:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:39:35 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:39:35 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:39:36 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:39:36 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:39:36 GMT
CMD []
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829992c79f06822894e73d9a962015a75a5d65ef5a60de627fbb32a973dc0462`  
		Last Modified: Tue, 15 Jun 2021 22:36:03 GMT  
		Size: 64.4 MB (64423231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6714f1b9096eb751a830a9dd13c67cd5e669c68403f1675efd7e78ff8905896d`  
		Last Modified: Tue, 15 Jun 2021 22:35:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997b259c822c244af1192eb31913d45df7f269da56a37fa1c7dc5b9fe273134`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b041c447a8f648b5910833f3c76e5a3231d34a6d76b56d0c22c64b232da92519`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f113d638e141615986b3c011ad91c657741ff84a21689c75c2159588d5fa89`  
		Last Modified: Tue, 15 Jun 2021 22:36:23 GMT  
		Size: 6.5 MB (6512663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b39bf84d6c6efaf352aeda8411d48487604fc126ff58dca169cff3ff189c31`  
		Last Modified: Tue, 15 Jun 2021 22:36:22 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0bd70db64874c3f0cd49b3492a9b270b52df5ed2834293a13cf84b0f2a2e54`  
		Last Modified: Tue, 15 Jun 2021 22:36:21 GMT  
		Size: 980.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79495f766691b68d3917bf6efd5a8faa1db74fe519664cf9546ac3cac184759`  
		Last Modified: Wed, 21 Jul 2021 18:41:23 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:edc07fe6ed074ed1cc7d1458a4c4b9ae7aa0055ffe8490747a7ffa4bcbb0a372
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:dfbd1f47be3ffee2e49da3e4676e95303730984ac4589f85ac9b741da6b757b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.2 MB (103209649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff81e7c521ef9185419614e07d935ee9d3fc84633b7779e7b78011d5c3118559`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Jun 2021 21:21:16 GMT
ENV DOCKER_VERSION=20.10.7
# Thu, 03 Jun 2021 21:21:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:21:24 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Jun 2021 21:21:25 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Jun 2021 21:21:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Jun 2021 21:21:25 GMT
CMD ["sh"]
# Thu, 03 Jun 2021 21:21:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 03 Jun 2021 21:21:33 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 03 Jun 2021 21:21:33 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 03 Jun 2021 21:21:34 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:19:42 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:19:42 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:19:42 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:19:43 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:19:43 GMT
CMD []
# Wed, 21 Jul 2021 18:19:48 GMT
RUN apk add --no-cache iproute2
# Wed, 21 Jul 2021 18:19:48 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 21 Jul 2021 18:19:49 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 21 Jul 2021 18:19:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 21 Jul 2021 18:19:52 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 21 Jul 2021 18:19:53 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 21 Jul 2021 18:19:53 GMT
USER rootless
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c521bbbd9945cde2415eae95c3a2a604ea5ca18eb86ab5cadeb589d3b8a13185`  
		Last Modified: Thu, 03 Jun 2021 21:22:44 GMT  
		Size: 70.2 MB (70247077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59707d521c45c42bbb7dbbef463d5d3800859f20122fb54894f0c79d9b435483`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26abe223b186967eef77715b2c6efd147f3a203a0c7b19e61a8947dab4236397`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d806bc203610fb061281b581a0b2522c9fcbd15e55c55ac0c496c9b1dbe63b0`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918595a0e69b201bdd25b6da798216629c61256ba541408487536b3953169aa6`  
		Last Modified: Thu, 03 Jun 2021 21:23:02 GMT  
		Size: 6.6 MB (6610580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf6f33d26f8a966febfc6cfc6677aadddee7d77d37476f660cb4b3e9d4659bd`  
		Last Modified: Thu, 03 Jun 2021 21:23:00 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0522a0264f7030f681722a192902d53421d886507aac6dafeced99b9ed932a`  
		Last Modified: Thu, 03 Jun 2021 21:23:00 GMT  
		Size: 978.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8d570be2274d0bfa2a8df30021696ca2af3e7a44553d24aa5f58314e32590b`  
		Last Modified: Wed, 21 Jul 2021 18:20:48 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c37506dcb7b254503a249acc77ad639791ccf1f50295d5c31788df27f3af7a`  
		Last Modified: Wed, 21 Jul 2021 18:21:05 GMT  
		Size: 1.1 MB (1131822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed0d82dd18063ee718b6d064e94ca32972e492eb12f03c8ee2a94c842c536fd`  
		Last Modified: Wed, 21 Jul 2021 18:21:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb9af9dfb3987a4cfb9807320de0c84c041a753e2472584eddd1d8278091314`  
		Last Modified: Wed, 21 Jul 2021 18:21:05 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e5aef124d58f59364dea12fad3563c4490f722b4bfc7f41451ba31e1963fb3`  
		Last Modified: Wed, 21 Jul 2021 18:21:08 GMT  
		Size: 20.3 MB (20349562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce68dd174b47186f06cde9a7d3eeda47cd379df950d750f80a358b2546669830`  
		Last Modified: Wed, 21 Jul 2021 18:21:05 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:a0ed9fee53f55f9f57d9261b466f40f641b2cfdf71e9836f66a8654248342294
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99111252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:700d0971fe8509aa4e4be25407976bc681c6261b26cf2bfb3ba905f3a67da188`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:00 GMT
ENV DOCKER_VERSION=20.10.7
# Tue, 15 Jun 2021 22:34:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:06 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:07 GMT
CMD ["sh"]
# Tue, 15 Jun 2021 22:34:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 15 Jun 2021 22:34:17 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 15 Jun 2021 22:34:17 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 15 Jun 2021 22:34:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:39:35 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:39:35 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:39:36 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:39:36 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:39:36 GMT
CMD []
# Wed, 21 Jul 2021 18:39:43 GMT
RUN apk add --no-cache iproute2
# Wed, 21 Jul 2021 18:39:44 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 21 Jul 2021 18:39:45 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 21 Jul 2021 18:39:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 21 Jul 2021 18:39:47 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 21 Jul 2021 18:39:47 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 21 Jul 2021 18:39:47 GMT
USER rootless
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829992c79f06822894e73d9a962015a75a5d65ef5a60de627fbb32a973dc0462`  
		Last Modified: Tue, 15 Jun 2021 22:36:03 GMT  
		Size: 64.4 MB (64423231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6714f1b9096eb751a830a9dd13c67cd5e669c68403f1675efd7e78ff8905896d`  
		Last Modified: Tue, 15 Jun 2021 22:35:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997b259c822c244af1192eb31913d45df7f269da56a37fa1c7dc5b9fe273134`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b041c447a8f648b5910833f3c76e5a3231d34a6d76b56d0c22c64b232da92519`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f113d638e141615986b3c011ad91c657741ff84a21689c75c2159588d5fa89`  
		Last Modified: Tue, 15 Jun 2021 22:36:23 GMT  
		Size: 6.5 MB (6512663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b39bf84d6c6efaf352aeda8411d48487604fc126ff58dca169cff3ff189c31`  
		Last Modified: Tue, 15 Jun 2021 22:36:22 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0bd70db64874c3f0cd49b3492a9b270b52df5ed2834293a13cf84b0f2a2e54`  
		Last Modified: Tue, 15 Jun 2021 22:36:21 GMT  
		Size: 980.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79495f766691b68d3917bf6efd5a8faa1db74fe519664cf9546ac3cac184759`  
		Last Modified: Wed, 21 Jul 2021 18:41:23 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d315f8014af109443f85b9f4d5f32c7b5fab2052af1a41b5dfb847eac9f160db`  
		Last Modified: Wed, 21 Jul 2021 18:41:52 GMT  
		Size: 1.2 MB (1153026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943d0afddc57ec5c68ce14e40454a1b87cbf480a597671581a2ca174e2cde571`  
		Last Modified: Wed, 21 Jul 2021 18:41:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d9287e79d4393132efb37c503d4160abe844d8f6292fec8bc64db2cd72007`  
		Last Modified: Wed, 21 Jul 2021 18:41:49 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9950840e88dd7c60f47e04de064c506bf702cc91e7b6b046885ffd9aa2d7cdf`  
		Last Modified: Wed, 21 Jul 2021 18:41:53 GMT  
		Size: 22.2 MB (22243949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b87281b8c123dcba3d6d1cf37aa4aae40b07a21eb5d20421196b59900321efe`  
		Last Modified: Wed, 21 Jul 2021 18:41:49 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-git`

```console
$ docker pull docker@sha256:622321c57531b57ee6a3d701c0c50debecc9411f9456dc3ed7b4b56d23940e99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-git` - linux; amd64

```console
$ docker pull docker@sha256:24c3d74e41f606a88ceb6b79c0d0c570590e13e46123c57ee17c4bd0a7d62e27
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.5 MB (81513063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7303fde5f20624623382d7b52fcd3c5f82d10035dbd93c9790385c2cc5e46ac7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Jun 2021 21:21:16 GMT
ENV DOCKER_VERSION=20.10.7
# Thu, 03 Jun 2021 21:21:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:21:24 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Jun 2021 21:21:25 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Jun 2021 21:21:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Jun 2021 21:21:25 GMT
CMD ["sh"]
# Thu, 03 Jun 2021 21:21:51 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c521bbbd9945cde2415eae95c3a2a604ea5ca18eb86ab5cadeb589d3b8a13185`  
		Last Modified: Thu, 03 Jun 2021 21:22:44 GMT  
		Size: 70.2 MB (70247077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59707d521c45c42bbb7dbbef463d5d3800859f20122fb54894f0c79d9b435483`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26abe223b186967eef77715b2c6efd147f3a203a0c7b19e61a8947dab4236397`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d806bc203610fb061281b581a0b2522c9fcbd15e55c55ac0c496c9b1dbe63b0`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee8b9b961bd083ca85d7c5a0f9e60a899f6a2185a581a890c03416b9b6e30df`  
		Last Modified: Thu, 03 Jun 2021 21:23:41 GMT  
		Size: 6.4 MB (6401997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:b86ac69b6c23bec2cd158a60d1cfbbe21e680b68123448507c509e3a50e73e2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75679816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6375cfb3695b26f65830e1831fc5fdf4ef758ec8e8adcb98f82b1074a5efa5b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:00 GMT
ENV DOCKER_VERSION=20.10.7
# Tue, 15 Jun 2021 22:34:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:06 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:07 GMT
CMD ["sh"]
# Tue, 15 Jun 2021 22:34:26 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829992c79f06822894e73d9a962015a75a5d65ef5a60de627fbb32a973dc0462`  
		Last Modified: Tue, 15 Jun 2021 22:36:03 GMT  
		Size: 64.4 MB (64423231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6714f1b9096eb751a830a9dd13c67cd5e669c68403f1675efd7e78ff8905896d`  
		Last Modified: Tue, 15 Jun 2021 22:35:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997b259c822c244af1192eb31913d45df7f269da56a37fa1c7dc5b9fe273134`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b041c447a8f648b5910833f3c76e5a3231d34a6d76b56d0c22c64b232da92519`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cbc3fd7a1a583e66318479683c0f605e6495f88cea87228beb20e8e811c3f1`  
		Last Modified: Tue, 15 Jun 2021 22:36:43 GMT  
		Size: 6.5 MB (6484825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore`

```console
$ docker pull docker@sha256:990b6fbd26ffa675431ea674ff416a850294146bb692e261fe93910d741913f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `docker:20-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull docker@sha256:a3b09a7c9d1cfeed83761a580c0fe5ab0d884c80537bbf2b2c9268faaf0964fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2734838564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452c96258d1fa3197a86ab2b95977bf99c84d244914b061957da1461fd17a66a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 18:19:31 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 18:19:35 GMT
ENV DOCKER_VERSION=20.10.7
# Wed, 14 Jul 2021 18:19:38 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.7.zip
# Wed, 14 Jul 2021 18:20:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca81d46af1fb75d88c51bffddab081ffb30e74d3771ee61adfcad7c1b2c6298e`  
		Last Modified: Wed, 14 Jul 2021 18:21:15 GMT  
		Size: 369.1 KB (369149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbc6b36bac5136f1a1dad152043de212420ac9833c3a31b54e9f3aaafa6c473`  
		Last Modified: Wed, 14 Jul 2021 18:21:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bec43c94884d1108711c15e1c29fd2dd7f22fb8092d7bda5d789efac2094f56`  
		Last Modified: Wed, 14 Jul 2021 18:21:14 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ff8b661ba3368d139c4ed45fb23ec33afb51968caee207cb0775444dbd634a`  
		Last Modified: Wed, 14 Jul 2021 18:22:12 GMT  
		Size: 49.0 MB (49018469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-1809`

```console
$ docker pull docker@sha256:990b6fbd26ffa675431ea674ff416a850294146bb692e261fe93910d741913f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `docker:20-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull docker@sha256:a3b09a7c9d1cfeed83761a580c0fe5ab0d884c80537bbf2b2c9268faaf0964fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2734838564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452c96258d1fa3197a86ab2b95977bf99c84d244914b061957da1461fd17a66a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 18:19:31 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 18:19:35 GMT
ENV DOCKER_VERSION=20.10.7
# Wed, 14 Jul 2021 18:19:38 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.7.zip
# Wed, 14 Jul 2021 18:20:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca81d46af1fb75d88c51bffddab081ffb30e74d3771ee61adfcad7c1b2c6298e`  
		Last Modified: Wed, 14 Jul 2021 18:21:15 GMT  
		Size: 369.1 KB (369149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbc6b36bac5136f1a1dad152043de212420ac9833c3a31b54e9f3aaafa6c473`  
		Last Modified: Wed, 14 Jul 2021 18:21:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bec43c94884d1108711c15e1c29fd2dd7f22fb8092d7bda5d789efac2094f56`  
		Last Modified: Wed, 14 Jul 2021 18:21:14 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ff8b661ba3368d139c4ed45fb23ec33afb51968caee207cb0775444dbd634a`  
		Last Modified: Wed, 14 Jul 2021 18:22:12 GMT  
		Size: 49.0 MB (49018469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10`

```console
$ docker pull docker@sha256:bfc499cef26daa22da31b76be1752813a6921ee1fa1dd1f56d4fdf19c701d332
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10` - linux; amd64

```console
$ docker pull docker@sha256:63cb2df6dfe1fb041b952ddb9f75c69569331fa39577bc41a3e56cf8f79f7e2e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75111066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08bdaf2f88f90320cd3e92a469969efb1f066c6d318631f94e7864828abd7c75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Jun 2021 21:21:16 GMT
ENV DOCKER_VERSION=20.10.7
# Thu, 03 Jun 2021 21:21:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:21:24 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Jun 2021 21:21:25 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Jun 2021 21:21:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Jun 2021 21:21:25 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c521bbbd9945cde2415eae95c3a2a604ea5ca18eb86ab5cadeb589d3b8a13185`  
		Last Modified: Thu, 03 Jun 2021 21:22:44 GMT  
		Size: 70.2 MB (70247077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59707d521c45c42bbb7dbbef463d5d3800859f20122fb54894f0c79d9b435483`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26abe223b186967eef77715b2c6efd147f3a203a0c7b19e61a8947dab4236397`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d806bc203610fb061281b581a0b2522c9fcbd15e55c55ac0c496c9b1dbe63b0`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:85fa729480d21cd25e5b7f2ba40b53492068501da59e4c23639bd41c5a43040e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69194991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df445af6242a928d36d8a3b4259ba3db9de1d7be5c9806e49b2746cdab4df048`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:00 GMT
ENV DOCKER_VERSION=20.10.7
# Tue, 15 Jun 2021 22:34:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:06 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:07 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829992c79f06822894e73d9a962015a75a5d65ef5a60de627fbb32a973dc0462`  
		Last Modified: Tue, 15 Jun 2021 22:36:03 GMT  
		Size: 64.4 MB (64423231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6714f1b9096eb751a830a9dd13c67cd5e669c68403f1675efd7e78ff8905896d`  
		Last Modified: Tue, 15 Jun 2021 22:35:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997b259c822c244af1192eb31913d45df7f269da56a37fa1c7dc5b9fe273134`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b041c447a8f648b5910833f3c76e5a3231d34a6d76b56d0c22c64b232da92519`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind`

```console
$ docker pull docker@sha256:b36fdccb118bfaa8d5026da5183a077b87bc790051fcd2c5686bfb8f7fa2563c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind` - linux; amd64

```console
$ docker pull docker@sha256:4f0e01f764b10c633334cb44fe6926a27b06390b482cb24e1add823b2ca781fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.7 MB (81726552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca749f2062c41ad54191b9c242dd1b3f6132a11299b251fc2128e37c9800ebba`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Jun 2021 21:21:16 GMT
ENV DOCKER_VERSION=20.10.7
# Thu, 03 Jun 2021 21:21:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:21:24 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Jun 2021 21:21:25 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Jun 2021 21:21:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Jun 2021 21:21:25 GMT
CMD ["sh"]
# Thu, 03 Jun 2021 21:21:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 03 Jun 2021 21:21:33 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 03 Jun 2021 21:21:33 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 03 Jun 2021 21:21:34 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:19:42 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:19:42 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:19:42 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:19:43 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:19:43 GMT
CMD []
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c521bbbd9945cde2415eae95c3a2a604ea5ca18eb86ab5cadeb589d3b8a13185`  
		Last Modified: Thu, 03 Jun 2021 21:22:44 GMT  
		Size: 70.2 MB (70247077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59707d521c45c42bbb7dbbef463d5d3800859f20122fb54894f0c79d9b435483`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26abe223b186967eef77715b2c6efd147f3a203a0c7b19e61a8947dab4236397`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d806bc203610fb061281b581a0b2522c9fcbd15e55c55ac0c496c9b1dbe63b0`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918595a0e69b201bdd25b6da798216629c61256ba541408487536b3953169aa6`  
		Last Modified: Thu, 03 Jun 2021 21:23:02 GMT  
		Size: 6.6 MB (6610580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf6f33d26f8a966febfc6cfc6677aadddee7d77d37476f660cb4b3e9d4659bd`  
		Last Modified: Thu, 03 Jun 2021 21:23:00 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0522a0264f7030f681722a192902d53421d886507aac6dafeced99b9ed932a`  
		Last Modified: Thu, 03 Jun 2021 21:23:00 GMT  
		Size: 978.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8d570be2274d0bfa2a8df30021696ca2af3e7a44553d24aa5f58314e32590b`  
		Last Modified: Wed, 21 Jul 2021 18:20:48 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:778521a7c301de26994f7aca616ab10c1bc35b8f66b802345d0cad89af381dcb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75712568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a81be9fbf6452a40403d288e5b6a6c422b96bb07fc23d07ac2d46d5a92a63fa`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:00 GMT
ENV DOCKER_VERSION=20.10.7
# Tue, 15 Jun 2021 22:34:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:06 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:07 GMT
CMD ["sh"]
# Tue, 15 Jun 2021 22:34:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 15 Jun 2021 22:34:17 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 15 Jun 2021 22:34:17 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 15 Jun 2021 22:34:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:39:35 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:39:35 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:39:36 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:39:36 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:39:36 GMT
CMD []
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829992c79f06822894e73d9a962015a75a5d65ef5a60de627fbb32a973dc0462`  
		Last Modified: Tue, 15 Jun 2021 22:36:03 GMT  
		Size: 64.4 MB (64423231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6714f1b9096eb751a830a9dd13c67cd5e669c68403f1675efd7e78ff8905896d`  
		Last Modified: Tue, 15 Jun 2021 22:35:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997b259c822c244af1192eb31913d45df7f269da56a37fa1c7dc5b9fe273134`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b041c447a8f648b5910833f3c76e5a3231d34a6d76b56d0c22c64b232da92519`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f113d638e141615986b3c011ad91c657741ff84a21689c75c2159588d5fa89`  
		Last Modified: Tue, 15 Jun 2021 22:36:23 GMT  
		Size: 6.5 MB (6512663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b39bf84d6c6efaf352aeda8411d48487604fc126ff58dca169cff3ff189c31`  
		Last Modified: Tue, 15 Jun 2021 22:36:22 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0bd70db64874c3f0cd49b3492a9b270b52df5ed2834293a13cf84b0f2a2e54`  
		Last Modified: Tue, 15 Jun 2021 22:36:21 GMT  
		Size: 980.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79495f766691b68d3917bf6efd5a8faa1db74fe519664cf9546ac3cac184759`  
		Last Modified: Wed, 21 Jul 2021 18:41:23 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind-rootless`

```console
$ docker pull docker@sha256:edc07fe6ed074ed1cc7d1458a4c4b9ae7aa0055ffe8490747a7ffa4bcbb0a372
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:dfbd1f47be3ffee2e49da3e4676e95303730984ac4589f85ac9b741da6b757b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.2 MB (103209649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff81e7c521ef9185419614e07d935ee9d3fc84633b7779e7b78011d5c3118559`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Jun 2021 21:21:16 GMT
ENV DOCKER_VERSION=20.10.7
# Thu, 03 Jun 2021 21:21:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:21:24 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Jun 2021 21:21:25 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Jun 2021 21:21:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Jun 2021 21:21:25 GMT
CMD ["sh"]
# Thu, 03 Jun 2021 21:21:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 03 Jun 2021 21:21:33 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 03 Jun 2021 21:21:33 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 03 Jun 2021 21:21:34 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:19:42 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:19:42 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:19:42 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:19:43 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:19:43 GMT
CMD []
# Wed, 21 Jul 2021 18:19:48 GMT
RUN apk add --no-cache iproute2
# Wed, 21 Jul 2021 18:19:48 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 21 Jul 2021 18:19:49 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 21 Jul 2021 18:19:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 21 Jul 2021 18:19:52 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 21 Jul 2021 18:19:53 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 21 Jul 2021 18:19:53 GMT
USER rootless
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c521bbbd9945cde2415eae95c3a2a604ea5ca18eb86ab5cadeb589d3b8a13185`  
		Last Modified: Thu, 03 Jun 2021 21:22:44 GMT  
		Size: 70.2 MB (70247077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59707d521c45c42bbb7dbbef463d5d3800859f20122fb54894f0c79d9b435483`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26abe223b186967eef77715b2c6efd147f3a203a0c7b19e61a8947dab4236397`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d806bc203610fb061281b581a0b2522c9fcbd15e55c55ac0c496c9b1dbe63b0`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918595a0e69b201bdd25b6da798216629c61256ba541408487536b3953169aa6`  
		Last Modified: Thu, 03 Jun 2021 21:23:02 GMT  
		Size: 6.6 MB (6610580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf6f33d26f8a966febfc6cfc6677aadddee7d77d37476f660cb4b3e9d4659bd`  
		Last Modified: Thu, 03 Jun 2021 21:23:00 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0522a0264f7030f681722a192902d53421d886507aac6dafeced99b9ed932a`  
		Last Modified: Thu, 03 Jun 2021 21:23:00 GMT  
		Size: 978.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8d570be2274d0bfa2a8df30021696ca2af3e7a44553d24aa5f58314e32590b`  
		Last Modified: Wed, 21 Jul 2021 18:20:48 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c37506dcb7b254503a249acc77ad639791ccf1f50295d5c31788df27f3af7a`  
		Last Modified: Wed, 21 Jul 2021 18:21:05 GMT  
		Size: 1.1 MB (1131822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed0d82dd18063ee718b6d064e94ca32972e492eb12f03c8ee2a94c842c536fd`  
		Last Modified: Wed, 21 Jul 2021 18:21:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb9af9dfb3987a4cfb9807320de0c84c041a753e2472584eddd1d8278091314`  
		Last Modified: Wed, 21 Jul 2021 18:21:05 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e5aef124d58f59364dea12fad3563c4490f722b4bfc7f41451ba31e1963fb3`  
		Last Modified: Wed, 21 Jul 2021 18:21:08 GMT  
		Size: 20.3 MB (20349562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce68dd174b47186f06cde9a7d3eeda47cd379df950d750f80a358b2546669830`  
		Last Modified: Wed, 21 Jul 2021 18:21:05 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:a0ed9fee53f55f9f57d9261b466f40f641b2cfdf71e9836f66a8654248342294
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99111252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:700d0971fe8509aa4e4be25407976bc681c6261b26cf2bfb3ba905f3a67da188`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:00 GMT
ENV DOCKER_VERSION=20.10.7
# Tue, 15 Jun 2021 22:34:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:06 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:07 GMT
CMD ["sh"]
# Tue, 15 Jun 2021 22:34:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 15 Jun 2021 22:34:17 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 15 Jun 2021 22:34:17 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 15 Jun 2021 22:34:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:39:35 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:39:35 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:39:36 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:39:36 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:39:36 GMT
CMD []
# Wed, 21 Jul 2021 18:39:43 GMT
RUN apk add --no-cache iproute2
# Wed, 21 Jul 2021 18:39:44 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 21 Jul 2021 18:39:45 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 21 Jul 2021 18:39:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 21 Jul 2021 18:39:47 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 21 Jul 2021 18:39:47 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 21 Jul 2021 18:39:47 GMT
USER rootless
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829992c79f06822894e73d9a962015a75a5d65ef5a60de627fbb32a973dc0462`  
		Last Modified: Tue, 15 Jun 2021 22:36:03 GMT  
		Size: 64.4 MB (64423231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6714f1b9096eb751a830a9dd13c67cd5e669c68403f1675efd7e78ff8905896d`  
		Last Modified: Tue, 15 Jun 2021 22:35:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997b259c822c244af1192eb31913d45df7f269da56a37fa1c7dc5b9fe273134`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b041c447a8f648b5910833f3c76e5a3231d34a6d76b56d0c22c64b232da92519`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f113d638e141615986b3c011ad91c657741ff84a21689c75c2159588d5fa89`  
		Last Modified: Tue, 15 Jun 2021 22:36:23 GMT  
		Size: 6.5 MB (6512663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b39bf84d6c6efaf352aeda8411d48487604fc126ff58dca169cff3ff189c31`  
		Last Modified: Tue, 15 Jun 2021 22:36:22 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0bd70db64874c3f0cd49b3492a9b270b52df5ed2834293a13cf84b0f2a2e54`  
		Last Modified: Tue, 15 Jun 2021 22:36:21 GMT  
		Size: 980.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79495f766691b68d3917bf6efd5a8faa1db74fe519664cf9546ac3cac184759`  
		Last Modified: Wed, 21 Jul 2021 18:41:23 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d315f8014af109443f85b9f4d5f32c7b5fab2052af1a41b5dfb847eac9f160db`  
		Last Modified: Wed, 21 Jul 2021 18:41:52 GMT  
		Size: 1.2 MB (1153026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943d0afddc57ec5c68ce14e40454a1b87cbf480a597671581a2ca174e2cde571`  
		Last Modified: Wed, 21 Jul 2021 18:41:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d9287e79d4393132efb37c503d4160abe844d8f6292fec8bc64db2cd72007`  
		Last Modified: Wed, 21 Jul 2021 18:41:49 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9950840e88dd7c60f47e04de064c506bf702cc91e7b6b046885ffd9aa2d7cdf`  
		Last Modified: Wed, 21 Jul 2021 18:41:53 GMT  
		Size: 22.2 MB (22243949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b87281b8c123dcba3d6d1cf37aa4aae40b07a21eb5d20421196b59900321efe`  
		Last Modified: Wed, 21 Jul 2021 18:41:49 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-git`

```console
$ docker pull docker@sha256:622321c57531b57ee6a3d701c0c50debecc9411f9456dc3ed7b4b56d23940e99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-git` - linux; amd64

```console
$ docker pull docker@sha256:24c3d74e41f606a88ceb6b79c0d0c570590e13e46123c57ee17c4bd0a7d62e27
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.5 MB (81513063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7303fde5f20624623382d7b52fcd3c5f82d10035dbd93c9790385c2cc5e46ac7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Jun 2021 21:21:16 GMT
ENV DOCKER_VERSION=20.10.7
# Thu, 03 Jun 2021 21:21:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:21:24 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Jun 2021 21:21:25 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Jun 2021 21:21:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Jun 2021 21:21:25 GMT
CMD ["sh"]
# Thu, 03 Jun 2021 21:21:51 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c521bbbd9945cde2415eae95c3a2a604ea5ca18eb86ab5cadeb589d3b8a13185`  
		Last Modified: Thu, 03 Jun 2021 21:22:44 GMT  
		Size: 70.2 MB (70247077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59707d521c45c42bbb7dbbef463d5d3800859f20122fb54894f0c79d9b435483`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26abe223b186967eef77715b2c6efd147f3a203a0c7b19e61a8947dab4236397`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d806bc203610fb061281b581a0b2522c9fcbd15e55c55ac0c496c9b1dbe63b0`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee8b9b961bd083ca85d7c5a0f9e60a899f6a2185a581a890c03416b9b6e30df`  
		Last Modified: Thu, 03 Jun 2021 21:23:41 GMT  
		Size: 6.4 MB (6401997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:b86ac69b6c23bec2cd158a60d1cfbbe21e680b68123448507c509e3a50e73e2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75679816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6375cfb3695b26f65830e1831fc5fdf4ef758ec8e8adcb98f82b1074a5efa5b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:00 GMT
ENV DOCKER_VERSION=20.10.7
# Tue, 15 Jun 2021 22:34:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:06 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:07 GMT
CMD ["sh"]
# Tue, 15 Jun 2021 22:34:26 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829992c79f06822894e73d9a962015a75a5d65ef5a60de627fbb32a973dc0462`  
		Last Modified: Tue, 15 Jun 2021 22:36:03 GMT  
		Size: 64.4 MB (64423231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6714f1b9096eb751a830a9dd13c67cd5e669c68403f1675efd7e78ff8905896d`  
		Last Modified: Tue, 15 Jun 2021 22:35:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997b259c822c244af1192eb31913d45df7f269da56a37fa1c7dc5b9fe273134`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b041c447a8f648b5910833f3c76e5a3231d34a6d76b56d0c22c64b232da92519`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cbc3fd7a1a583e66318479683c0f605e6495f88cea87228beb20e8e811c3f1`  
		Last Modified: Tue, 15 Jun 2021 22:36:43 GMT  
		Size: 6.5 MB (6484825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore`

```console
$ docker pull docker@sha256:990b6fbd26ffa675431ea674ff416a850294146bb692e261fe93910d741913f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `docker:20.10-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull docker@sha256:a3b09a7c9d1cfeed83761a580c0fe5ab0d884c80537bbf2b2c9268faaf0964fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2734838564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452c96258d1fa3197a86ab2b95977bf99c84d244914b061957da1461fd17a66a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 18:19:31 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 18:19:35 GMT
ENV DOCKER_VERSION=20.10.7
# Wed, 14 Jul 2021 18:19:38 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.7.zip
# Wed, 14 Jul 2021 18:20:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca81d46af1fb75d88c51bffddab081ffb30e74d3771ee61adfcad7c1b2c6298e`  
		Last Modified: Wed, 14 Jul 2021 18:21:15 GMT  
		Size: 369.1 KB (369149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbc6b36bac5136f1a1dad152043de212420ac9833c3a31b54e9f3aaafa6c473`  
		Last Modified: Wed, 14 Jul 2021 18:21:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bec43c94884d1108711c15e1c29fd2dd7f22fb8092d7bda5d789efac2094f56`  
		Last Modified: Wed, 14 Jul 2021 18:21:14 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ff8b661ba3368d139c4ed45fb23ec33afb51968caee207cb0775444dbd634a`  
		Last Modified: Wed, 14 Jul 2021 18:22:12 GMT  
		Size: 49.0 MB (49018469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-1809`

```console
$ docker pull docker@sha256:990b6fbd26ffa675431ea674ff416a850294146bb692e261fe93910d741913f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `docker:20.10-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull docker@sha256:a3b09a7c9d1cfeed83761a580c0fe5ab0d884c80537bbf2b2c9268faaf0964fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2734838564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452c96258d1fa3197a86ab2b95977bf99c84d244914b061957da1461fd17a66a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 18:19:31 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 18:19:35 GMT
ENV DOCKER_VERSION=20.10.7
# Wed, 14 Jul 2021 18:19:38 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.7.zip
# Wed, 14 Jul 2021 18:20:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca81d46af1fb75d88c51bffddab081ffb30e74d3771ee61adfcad7c1b2c6298e`  
		Last Modified: Wed, 14 Jul 2021 18:21:15 GMT  
		Size: 369.1 KB (369149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbc6b36bac5136f1a1dad152043de212420ac9833c3a31b54e9f3aaafa6c473`  
		Last Modified: Wed, 14 Jul 2021 18:21:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bec43c94884d1108711c15e1c29fd2dd7f22fb8092d7bda5d789efac2094f56`  
		Last Modified: Wed, 14 Jul 2021 18:21:14 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ff8b661ba3368d139c4ed45fb23ec33afb51968caee207cb0775444dbd634a`  
		Last Modified: Wed, 14 Jul 2021 18:22:12 GMT  
		Size: 49.0 MB (49018469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.7`

```console
$ docker pull docker@sha256:bfc499cef26daa22da31b76be1752813a6921ee1fa1dd1f56d4fdf19c701d332
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.7` - linux; amd64

```console
$ docker pull docker@sha256:63cb2df6dfe1fb041b952ddb9f75c69569331fa39577bc41a3e56cf8f79f7e2e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75111066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08bdaf2f88f90320cd3e92a469969efb1f066c6d318631f94e7864828abd7c75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Jun 2021 21:21:16 GMT
ENV DOCKER_VERSION=20.10.7
# Thu, 03 Jun 2021 21:21:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:21:24 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Jun 2021 21:21:25 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Jun 2021 21:21:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Jun 2021 21:21:25 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c521bbbd9945cde2415eae95c3a2a604ea5ca18eb86ab5cadeb589d3b8a13185`  
		Last Modified: Thu, 03 Jun 2021 21:22:44 GMT  
		Size: 70.2 MB (70247077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59707d521c45c42bbb7dbbef463d5d3800859f20122fb54894f0c79d9b435483`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26abe223b186967eef77715b2c6efd147f3a203a0c7b19e61a8947dab4236397`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d806bc203610fb061281b581a0b2522c9fcbd15e55c55ac0c496c9b1dbe63b0`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.7` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:85fa729480d21cd25e5b7f2ba40b53492068501da59e4c23639bd41c5a43040e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69194991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df445af6242a928d36d8a3b4259ba3db9de1d7be5c9806e49b2746cdab4df048`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:00 GMT
ENV DOCKER_VERSION=20.10.7
# Tue, 15 Jun 2021 22:34:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:06 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:07 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829992c79f06822894e73d9a962015a75a5d65ef5a60de627fbb32a973dc0462`  
		Last Modified: Tue, 15 Jun 2021 22:36:03 GMT  
		Size: 64.4 MB (64423231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6714f1b9096eb751a830a9dd13c67cd5e669c68403f1675efd7e78ff8905896d`  
		Last Modified: Tue, 15 Jun 2021 22:35:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997b259c822c244af1192eb31913d45df7f269da56a37fa1c7dc5b9fe273134`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b041c447a8f648b5910833f3c76e5a3231d34a6d76b56d0c22c64b232da92519`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.7-dind`

```console
$ docker pull docker@sha256:b36fdccb118bfaa8d5026da5183a077b87bc790051fcd2c5686bfb8f7fa2563c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.7-dind` - linux; amd64

```console
$ docker pull docker@sha256:4f0e01f764b10c633334cb44fe6926a27b06390b482cb24e1add823b2ca781fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.7 MB (81726552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca749f2062c41ad54191b9c242dd1b3f6132a11299b251fc2128e37c9800ebba`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Jun 2021 21:21:16 GMT
ENV DOCKER_VERSION=20.10.7
# Thu, 03 Jun 2021 21:21:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:21:24 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Jun 2021 21:21:25 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Jun 2021 21:21:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Jun 2021 21:21:25 GMT
CMD ["sh"]
# Thu, 03 Jun 2021 21:21:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 03 Jun 2021 21:21:33 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 03 Jun 2021 21:21:33 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 03 Jun 2021 21:21:34 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:19:42 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:19:42 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:19:42 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:19:43 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:19:43 GMT
CMD []
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c521bbbd9945cde2415eae95c3a2a604ea5ca18eb86ab5cadeb589d3b8a13185`  
		Last Modified: Thu, 03 Jun 2021 21:22:44 GMT  
		Size: 70.2 MB (70247077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59707d521c45c42bbb7dbbef463d5d3800859f20122fb54894f0c79d9b435483`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26abe223b186967eef77715b2c6efd147f3a203a0c7b19e61a8947dab4236397`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d806bc203610fb061281b581a0b2522c9fcbd15e55c55ac0c496c9b1dbe63b0`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918595a0e69b201bdd25b6da798216629c61256ba541408487536b3953169aa6`  
		Last Modified: Thu, 03 Jun 2021 21:23:02 GMT  
		Size: 6.6 MB (6610580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf6f33d26f8a966febfc6cfc6677aadddee7d77d37476f660cb4b3e9d4659bd`  
		Last Modified: Thu, 03 Jun 2021 21:23:00 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0522a0264f7030f681722a192902d53421d886507aac6dafeced99b9ed932a`  
		Last Modified: Thu, 03 Jun 2021 21:23:00 GMT  
		Size: 978.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8d570be2274d0bfa2a8df30021696ca2af3e7a44553d24aa5f58314e32590b`  
		Last Modified: Wed, 21 Jul 2021 18:20:48 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.7-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:778521a7c301de26994f7aca616ab10c1bc35b8f66b802345d0cad89af381dcb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75712568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a81be9fbf6452a40403d288e5b6a6c422b96bb07fc23d07ac2d46d5a92a63fa`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:00 GMT
ENV DOCKER_VERSION=20.10.7
# Tue, 15 Jun 2021 22:34:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:06 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:07 GMT
CMD ["sh"]
# Tue, 15 Jun 2021 22:34:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 15 Jun 2021 22:34:17 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 15 Jun 2021 22:34:17 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 15 Jun 2021 22:34:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:39:35 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:39:35 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:39:36 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:39:36 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:39:36 GMT
CMD []
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829992c79f06822894e73d9a962015a75a5d65ef5a60de627fbb32a973dc0462`  
		Last Modified: Tue, 15 Jun 2021 22:36:03 GMT  
		Size: 64.4 MB (64423231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6714f1b9096eb751a830a9dd13c67cd5e669c68403f1675efd7e78ff8905896d`  
		Last Modified: Tue, 15 Jun 2021 22:35:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997b259c822c244af1192eb31913d45df7f269da56a37fa1c7dc5b9fe273134`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b041c447a8f648b5910833f3c76e5a3231d34a6d76b56d0c22c64b232da92519`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f113d638e141615986b3c011ad91c657741ff84a21689c75c2159588d5fa89`  
		Last Modified: Tue, 15 Jun 2021 22:36:23 GMT  
		Size: 6.5 MB (6512663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b39bf84d6c6efaf352aeda8411d48487604fc126ff58dca169cff3ff189c31`  
		Last Modified: Tue, 15 Jun 2021 22:36:22 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0bd70db64874c3f0cd49b3492a9b270b52df5ed2834293a13cf84b0f2a2e54`  
		Last Modified: Tue, 15 Jun 2021 22:36:21 GMT  
		Size: 980.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79495f766691b68d3917bf6efd5a8faa1db74fe519664cf9546ac3cac184759`  
		Last Modified: Wed, 21 Jul 2021 18:41:23 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.7-dind-rootless`

```console
$ docker pull docker@sha256:edc07fe6ed074ed1cc7d1458a4c4b9ae7aa0055ffe8490747a7ffa4bcbb0a372
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.7-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:dfbd1f47be3ffee2e49da3e4676e95303730984ac4589f85ac9b741da6b757b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.2 MB (103209649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff81e7c521ef9185419614e07d935ee9d3fc84633b7779e7b78011d5c3118559`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Jun 2021 21:21:16 GMT
ENV DOCKER_VERSION=20.10.7
# Thu, 03 Jun 2021 21:21:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:21:24 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Jun 2021 21:21:25 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Jun 2021 21:21:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Jun 2021 21:21:25 GMT
CMD ["sh"]
# Thu, 03 Jun 2021 21:21:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 03 Jun 2021 21:21:33 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 03 Jun 2021 21:21:33 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 03 Jun 2021 21:21:34 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:19:42 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:19:42 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:19:42 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:19:43 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:19:43 GMT
CMD []
# Wed, 21 Jul 2021 18:19:48 GMT
RUN apk add --no-cache iproute2
# Wed, 21 Jul 2021 18:19:48 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 21 Jul 2021 18:19:49 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 21 Jul 2021 18:19:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 21 Jul 2021 18:19:52 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 21 Jul 2021 18:19:53 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 21 Jul 2021 18:19:53 GMT
USER rootless
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c521bbbd9945cde2415eae95c3a2a604ea5ca18eb86ab5cadeb589d3b8a13185`  
		Last Modified: Thu, 03 Jun 2021 21:22:44 GMT  
		Size: 70.2 MB (70247077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59707d521c45c42bbb7dbbef463d5d3800859f20122fb54894f0c79d9b435483`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26abe223b186967eef77715b2c6efd147f3a203a0c7b19e61a8947dab4236397`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d806bc203610fb061281b581a0b2522c9fcbd15e55c55ac0c496c9b1dbe63b0`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918595a0e69b201bdd25b6da798216629c61256ba541408487536b3953169aa6`  
		Last Modified: Thu, 03 Jun 2021 21:23:02 GMT  
		Size: 6.6 MB (6610580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf6f33d26f8a966febfc6cfc6677aadddee7d77d37476f660cb4b3e9d4659bd`  
		Last Modified: Thu, 03 Jun 2021 21:23:00 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0522a0264f7030f681722a192902d53421d886507aac6dafeced99b9ed932a`  
		Last Modified: Thu, 03 Jun 2021 21:23:00 GMT  
		Size: 978.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8d570be2274d0bfa2a8df30021696ca2af3e7a44553d24aa5f58314e32590b`  
		Last Modified: Wed, 21 Jul 2021 18:20:48 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c37506dcb7b254503a249acc77ad639791ccf1f50295d5c31788df27f3af7a`  
		Last Modified: Wed, 21 Jul 2021 18:21:05 GMT  
		Size: 1.1 MB (1131822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed0d82dd18063ee718b6d064e94ca32972e492eb12f03c8ee2a94c842c536fd`  
		Last Modified: Wed, 21 Jul 2021 18:21:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb9af9dfb3987a4cfb9807320de0c84c041a753e2472584eddd1d8278091314`  
		Last Modified: Wed, 21 Jul 2021 18:21:05 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e5aef124d58f59364dea12fad3563c4490f722b4bfc7f41451ba31e1963fb3`  
		Last Modified: Wed, 21 Jul 2021 18:21:08 GMT  
		Size: 20.3 MB (20349562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce68dd174b47186f06cde9a7d3eeda47cd379df950d750f80a358b2546669830`  
		Last Modified: Wed, 21 Jul 2021 18:21:05 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.7-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:a0ed9fee53f55f9f57d9261b466f40f641b2cfdf71e9836f66a8654248342294
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99111252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:700d0971fe8509aa4e4be25407976bc681c6261b26cf2bfb3ba905f3a67da188`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:00 GMT
ENV DOCKER_VERSION=20.10.7
# Tue, 15 Jun 2021 22:34:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:06 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:07 GMT
CMD ["sh"]
# Tue, 15 Jun 2021 22:34:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 15 Jun 2021 22:34:17 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 15 Jun 2021 22:34:17 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 15 Jun 2021 22:34:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:39:35 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:39:35 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:39:36 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:39:36 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:39:36 GMT
CMD []
# Wed, 21 Jul 2021 18:39:43 GMT
RUN apk add --no-cache iproute2
# Wed, 21 Jul 2021 18:39:44 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 21 Jul 2021 18:39:45 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 21 Jul 2021 18:39:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 21 Jul 2021 18:39:47 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 21 Jul 2021 18:39:47 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 21 Jul 2021 18:39:47 GMT
USER rootless
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829992c79f06822894e73d9a962015a75a5d65ef5a60de627fbb32a973dc0462`  
		Last Modified: Tue, 15 Jun 2021 22:36:03 GMT  
		Size: 64.4 MB (64423231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6714f1b9096eb751a830a9dd13c67cd5e669c68403f1675efd7e78ff8905896d`  
		Last Modified: Tue, 15 Jun 2021 22:35:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997b259c822c244af1192eb31913d45df7f269da56a37fa1c7dc5b9fe273134`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b041c447a8f648b5910833f3c76e5a3231d34a6d76b56d0c22c64b232da92519`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f113d638e141615986b3c011ad91c657741ff84a21689c75c2159588d5fa89`  
		Last Modified: Tue, 15 Jun 2021 22:36:23 GMT  
		Size: 6.5 MB (6512663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b39bf84d6c6efaf352aeda8411d48487604fc126ff58dca169cff3ff189c31`  
		Last Modified: Tue, 15 Jun 2021 22:36:22 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0bd70db64874c3f0cd49b3492a9b270b52df5ed2834293a13cf84b0f2a2e54`  
		Last Modified: Tue, 15 Jun 2021 22:36:21 GMT  
		Size: 980.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79495f766691b68d3917bf6efd5a8faa1db74fe519664cf9546ac3cac184759`  
		Last Modified: Wed, 21 Jul 2021 18:41:23 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d315f8014af109443f85b9f4d5f32c7b5fab2052af1a41b5dfb847eac9f160db`  
		Last Modified: Wed, 21 Jul 2021 18:41:52 GMT  
		Size: 1.2 MB (1153026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943d0afddc57ec5c68ce14e40454a1b87cbf480a597671581a2ca174e2cde571`  
		Last Modified: Wed, 21 Jul 2021 18:41:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d9287e79d4393132efb37c503d4160abe844d8f6292fec8bc64db2cd72007`  
		Last Modified: Wed, 21 Jul 2021 18:41:49 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9950840e88dd7c60f47e04de064c506bf702cc91e7b6b046885ffd9aa2d7cdf`  
		Last Modified: Wed, 21 Jul 2021 18:41:53 GMT  
		Size: 22.2 MB (22243949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b87281b8c123dcba3d6d1cf37aa4aae40b07a21eb5d20421196b59900321efe`  
		Last Modified: Wed, 21 Jul 2021 18:41:49 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.7-git`

```console
$ docker pull docker@sha256:622321c57531b57ee6a3d701c0c50debecc9411f9456dc3ed7b4b56d23940e99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.7-git` - linux; amd64

```console
$ docker pull docker@sha256:24c3d74e41f606a88ceb6b79c0d0c570590e13e46123c57ee17c4bd0a7d62e27
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.5 MB (81513063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7303fde5f20624623382d7b52fcd3c5f82d10035dbd93c9790385c2cc5e46ac7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Jun 2021 21:21:16 GMT
ENV DOCKER_VERSION=20.10.7
# Thu, 03 Jun 2021 21:21:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:21:24 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Jun 2021 21:21:25 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Jun 2021 21:21:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Jun 2021 21:21:25 GMT
CMD ["sh"]
# Thu, 03 Jun 2021 21:21:51 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c521bbbd9945cde2415eae95c3a2a604ea5ca18eb86ab5cadeb589d3b8a13185`  
		Last Modified: Thu, 03 Jun 2021 21:22:44 GMT  
		Size: 70.2 MB (70247077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59707d521c45c42bbb7dbbef463d5d3800859f20122fb54894f0c79d9b435483`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26abe223b186967eef77715b2c6efd147f3a203a0c7b19e61a8947dab4236397`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d806bc203610fb061281b581a0b2522c9fcbd15e55c55ac0c496c9b1dbe63b0`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee8b9b961bd083ca85d7c5a0f9e60a899f6a2185a581a890c03416b9b6e30df`  
		Last Modified: Thu, 03 Jun 2021 21:23:41 GMT  
		Size: 6.4 MB (6401997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.7-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:b86ac69b6c23bec2cd158a60d1cfbbe21e680b68123448507c509e3a50e73e2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75679816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6375cfb3695b26f65830e1831fc5fdf4ef758ec8e8adcb98f82b1074a5efa5b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:00 GMT
ENV DOCKER_VERSION=20.10.7
# Tue, 15 Jun 2021 22:34:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:06 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:07 GMT
CMD ["sh"]
# Tue, 15 Jun 2021 22:34:26 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829992c79f06822894e73d9a962015a75a5d65ef5a60de627fbb32a973dc0462`  
		Last Modified: Tue, 15 Jun 2021 22:36:03 GMT  
		Size: 64.4 MB (64423231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6714f1b9096eb751a830a9dd13c67cd5e669c68403f1675efd7e78ff8905896d`  
		Last Modified: Tue, 15 Jun 2021 22:35:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997b259c822c244af1192eb31913d45df7f269da56a37fa1c7dc5b9fe273134`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b041c447a8f648b5910833f3c76e5a3231d34a6d76b56d0c22c64b232da92519`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cbc3fd7a1a583e66318479683c0f605e6495f88cea87228beb20e8e811c3f1`  
		Last Modified: Tue, 15 Jun 2021 22:36:43 GMT  
		Size: 6.5 MB (6484825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.7-windowsservercore`

```console
$ docker pull docker@sha256:990b6fbd26ffa675431ea674ff416a850294146bb692e261fe93910d741913f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `docker:20.10.7-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull docker@sha256:a3b09a7c9d1cfeed83761a580c0fe5ab0d884c80537bbf2b2c9268faaf0964fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2734838564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452c96258d1fa3197a86ab2b95977bf99c84d244914b061957da1461fd17a66a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 18:19:31 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 18:19:35 GMT
ENV DOCKER_VERSION=20.10.7
# Wed, 14 Jul 2021 18:19:38 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.7.zip
# Wed, 14 Jul 2021 18:20:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca81d46af1fb75d88c51bffddab081ffb30e74d3771ee61adfcad7c1b2c6298e`  
		Last Modified: Wed, 14 Jul 2021 18:21:15 GMT  
		Size: 369.1 KB (369149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbc6b36bac5136f1a1dad152043de212420ac9833c3a31b54e9f3aaafa6c473`  
		Last Modified: Wed, 14 Jul 2021 18:21:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bec43c94884d1108711c15e1c29fd2dd7f22fb8092d7bda5d789efac2094f56`  
		Last Modified: Wed, 14 Jul 2021 18:21:14 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ff8b661ba3368d139c4ed45fb23ec33afb51968caee207cb0775444dbd634a`  
		Last Modified: Wed, 14 Jul 2021 18:22:12 GMT  
		Size: 49.0 MB (49018469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.7-windowsservercore-1809`

```console
$ docker pull docker@sha256:990b6fbd26ffa675431ea674ff416a850294146bb692e261fe93910d741913f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `docker:20.10.7-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull docker@sha256:a3b09a7c9d1cfeed83761a580c0fe5ab0d884c80537bbf2b2c9268faaf0964fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2734838564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452c96258d1fa3197a86ab2b95977bf99c84d244914b061957da1461fd17a66a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 18:19:31 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 18:19:35 GMT
ENV DOCKER_VERSION=20.10.7
# Wed, 14 Jul 2021 18:19:38 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.7.zip
# Wed, 14 Jul 2021 18:20:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca81d46af1fb75d88c51bffddab081ffb30e74d3771ee61adfcad7c1b2c6298e`  
		Last Modified: Wed, 14 Jul 2021 18:21:15 GMT  
		Size: 369.1 KB (369149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbc6b36bac5136f1a1dad152043de212420ac9833c3a31b54e9f3aaafa6c473`  
		Last Modified: Wed, 14 Jul 2021 18:21:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bec43c94884d1108711c15e1c29fd2dd7f22fb8092d7bda5d789efac2094f56`  
		Last Modified: Wed, 14 Jul 2021 18:21:14 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ff8b661ba3368d139c4ed45fb23ec33afb51968caee207cb0775444dbd634a`  
		Last Modified: Wed, 14 Jul 2021 18:22:12 GMT  
		Size: 49.0 MB (49018469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:07263bef8759a4d773431719856c3845b163c07034d200b00cd44b85b5e53d94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:4f0e01f764b10c633334cb44fe6926a27b06390b482cb24e1add823b2ca781fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.7 MB (81726552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca749f2062c41ad54191b9c242dd1b3f6132a11299b251fc2128e37c9800ebba`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Jun 2021 21:21:16 GMT
ENV DOCKER_VERSION=20.10.7
# Thu, 03 Jun 2021 21:21:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:21:24 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Jun 2021 21:21:25 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Jun 2021 21:21:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Jun 2021 21:21:25 GMT
CMD ["sh"]
# Thu, 03 Jun 2021 21:21:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 03 Jun 2021 21:21:33 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 03 Jun 2021 21:21:33 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 03 Jun 2021 21:21:34 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:19:42 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:19:42 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:19:42 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:19:43 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:19:43 GMT
CMD []
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c521bbbd9945cde2415eae95c3a2a604ea5ca18eb86ab5cadeb589d3b8a13185`  
		Last Modified: Thu, 03 Jun 2021 21:22:44 GMT  
		Size: 70.2 MB (70247077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59707d521c45c42bbb7dbbef463d5d3800859f20122fb54894f0c79d9b435483`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26abe223b186967eef77715b2c6efd147f3a203a0c7b19e61a8947dab4236397`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d806bc203610fb061281b581a0b2522c9fcbd15e55c55ac0c496c9b1dbe63b0`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918595a0e69b201bdd25b6da798216629c61256ba541408487536b3953169aa6`  
		Last Modified: Thu, 03 Jun 2021 21:23:02 GMT  
		Size: 6.6 MB (6610580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf6f33d26f8a966febfc6cfc6677aadddee7d77d37476f660cb4b3e9d4659bd`  
		Last Modified: Thu, 03 Jun 2021 21:23:00 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0522a0264f7030f681722a192902d53421d886507aac6dafeced99b9ed932a`  
		Last Modified: Thu, 03 Jun 2021 21:23:00 GMT  
		Size: 978.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8d570be2274d0bfa2a8df30021696ca2af3e7a44553d24aa5f58314e32590b`  
		Last Modified: Wed, 21 Jul 2021 18:20:48 GMT  
		Size: 2.6 KB (2617 bytes)  
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
$ docker pull docker@sha256:778521a7c301de26994f7aca616ab10c1bc35b8f66b802345d0cad89af381dcb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75712568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a81be9fbf6452a40403d288e5b6a6c422b96bb07fc23d07ac2d46d5a92a63fa`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:00 GMT
ENV DOCKER_VERSION=20.10.7
# Tue, 15 Jun 2021 22:34:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:06 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:07 GMT
CMD ["sh"]
# Tue, 15 Jun 2021 22:34:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 15 Jun 2021 22:34:17 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 15 Jun 2021 22:34:17 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 15 Jun 2021 22:34:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:39:35 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:39:35 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:39:36 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:39:36 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:39:36 GMT
CMD []
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829992c79f06822894e73d9a962015a75a5d65ef5a60de627fbb32a973dc0462`  
		Last Modified: Tue, 15 Jun 2021 22:36:03 GMT  
		Size: 64.4 MB (64423231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6714f1b9096eb751a830a9dd13c67cd5e669c68403f1675efd7e78ff8905896d`  
		Last Modified: Tue, 15 Jun 2021 22:35:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997b259c822c244af1192eb31913d45df7f269da56a37fa1c7dc5b9fe273134`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b041c447a8f648b5910833f3c76e5a3231d34a6d76b56d0c22c64b232da92519`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f113d638e141615986b3c011ad91c657741ff84a21689c75c2159588d5fa89`  
		Last Modified: Tue, 15 Jun 2021 22:36:23 GMT  
		Size: 6.5 MB (6512663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b39bf84d6c6efaf352aeda8411d48487604fc126ff58dca169cff3ff189c31`  
		Last Modified: Tue, 15 Jun 2021 22:36:22 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0bd70db64874c3f0cd49b3492a9b270b52df5ed2834293a13cf84b0f2a2e54`  
		Last Modified: Tue, 15 Jun 2021 22:36:21 GMT  
		Size: 980.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79495f766691b68d3917bf6efd5a8faa1db74fe519664cf9546ac3cac184759`  
		Last Modified: Wed, 21 Jul 2021 18:41:23 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:edc07fe6ed074ed1cc7d1458a4c4b9ae7aa0055ffe8490747a7ffa4bcbb0a372
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:dfbd1f47be3ffee2e49da3e4676e95303730984ac4589f85ac9b741da6b757b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.2 MB (103209649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff81e7c521ef9185419614e07d935ee9d3fc84633b7779e7b78011d5c3118559`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Jun 2021 21:21:16 GMT
ENV DOCKER_VERSION=20.10.7
# Thu, 03 Jun 2021 21:21:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:21:24 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Jun 2021 21:21:25 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Jun 2021 21:21:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Jun 2021 21:21:25 GMT
CMD ["sh"]
# Thu, 03 Jun 2021 21:21:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 03 Jun 2021 21:21:33 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 03 Jun 2021 21:21:33 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 03 Jun 2021 21:21:34 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:19:42 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:19:42 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:19:42 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:19:43 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:19:43 GMT
CMD []
# Wed, 21 Jul 2021 18:19:48 GMT
RUN apk add --no-cache iproute2
# Wed, 21 Jul 2021 18:19:48 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 21 Jul 2021 18:19:49 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 21 Jul 2021 18:19:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 21 Jul 2021 18:19:52 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 21 Jul 2021 18:19:53 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 21 Jul 2021 18:19:53 GMT
USER rootless
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c521bbbd9945cde2415eae95c3a2a604ea5ca18eb86ab5cadeb589d3b8a13185`  
		Last Modified: Thu, 03 Jun 2021 21:22:44 GMT  
		Size: 70.2 MB (70247077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59707d521c45c42bbb7dbbef463d5d3800859f20122fb54894f0c79d9b435483`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26abe223b186967eef77715b2c6efd147f3a203a0c7b19e61a8947dab4236397`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d806bc203610fb061281b581a0b2522c9fcbd15e55c55ac0c496c9b1dbe63b0`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918595a0e69b201bdd25b6da798216629c61256ba541408487536b3953169aa6`  
		Last Modified: Thu, 03 Jun 2021 21:23:02 GMT  
		Size: 6.6 MB (6610580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf6f33d26f8a966febfc6cfc6677aadddee7d77d37476f660cb4b3e9d4659bd`  
		Last Modified: Thu, 03 Jun 2021 21:23:00 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0522a0264f7030f681722a192902d53421d886507aac6dafeced99b9ed932a`  
		Last Modified: Thu, 03 Jun 2021 21:23:00 GMT  
		Size: 978.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8d570be2274d0bfa2a8df30021696ca2af3e7a44553d24aa5f58314e32590b`  
		Last Modified: Wed, 21 Jul 2021 18:20:48 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c37506dcb7b254503a249acc77ad639791ccf1f50295d5c31788df27f3af7a`  
		Last Modified: Wed, 21 Jul 2021 18:21:05 GMT  
		Size: 1.1 MB (1131822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed0d82dd18063ee718b6d064e94ca32972e492eb12f03c8ee2a94c842c536fd`  
		Last Modified: Wed, 21 Jul 2021 18:21:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb9af9dfb3987a4cfb9807320de0c84c041a753e2472584eddd1d8278091314`  
		Last Modified: Wed, 21 Jul 2021 18:21:05 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e5aef124d58f59364dea12fad3563c4490f722b4bfc7f41451ba31e1963fb3`  
		Last Modified: Wed, 21 Jul 2021 18:21:08 GMT  
		Size: 20.3 MB (20349562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce68dd174b47186f06cde9a7d3eeda47cd379df950d750f80a358b2546669830`  
		Last Modified: Wed, 21 Jul 2021 18:21:05 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:a0ed9fee53f55f9f57d9261b466f40f641b2cfdf71e9836f66a8654248342294
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99111252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:700d0971fe8509aa4e4be25407976bc681c6261b26cf2bfb3ba905f3a67da188`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:00 GMT
ENV DOCKER_VERSION=20.10.7
# Tue, 15 Jun 2021 22:34:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:06 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:07 GMT
CMD ["sh"]
# Tue, 15 Jun 2021 22:34:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 15 Jun 2021 22:34:17 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 15 Jun 2021 22:34:17 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 15 Jun 2021 22:34:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:39:35 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:39:35 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:39:36 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:39:36 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:39:36 GMT
CMD []
# Wed, 21 Jul 2021 18:39:43 GMT
RUN apk add --no-cache iproute2
# Wed, 21 Jul 2021 18:39:44 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 21 Jul 2021 18:39:45 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 21 Jul 2021 18:39:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 21 Jul 2021 18:39:47 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 21 Jul 2021 18:39:47 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 21 Jul 2021 18:39:47 GMT
USER rootless
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829992c79f06822894e73d9a962015a75a5d65ef5a60de627fbb32a973dc0462`  
		Last Modified: Tue, 15 Jun 2021 22:36:03 GMT  
		Size: 64.4 MB (64423231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6714f1b9096eb751a830a9dd13c67cd5e669c68403f1675efd7e78ff8905896d`  
		Last Modified: Tue, 15 Jun 2021 22:35:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997b259c822c244af1192eb31913d45df7f269da56a37fa1c7dc5b9fe273134`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b041c447a8f648b5910833f3c76e5a3231d34a6d76b56d0c22c64b232da92519`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f113d638e141615986b3c011ad91c657741ff84a21689c75c2159588d5fa89`  
		Last Modified: Tue, 15 Jun 2021 22:36:23 GMT  
		Size: 6.5 MB (6512663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b39bf84d6c6efaf352aeda8411d48487604fc126ff58dca169cff3ff189c31`  
		Last Modified: Tue, 15 Jun 2021 22:36:22 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0bd70db64874c3f0cd49b3492a9b270b52df5ed2834293a13cf84b0f2a2e54`  
		Last Modified: Tue, 15 Jun 2021 22:36:21 GMT  
		Size: 980.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79495f766691b68d3917bf6efd5a8faa1db74fe519664cf9546ac3cac184759`  
		Last Modified: Wed, 21 Jul 2021 18:41:23 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d315f8014af109443f85b9f4d5f32c7b5fab2052af1a41b5dfb847eac9f160db`  
		Last Modified: Wed, 21 Jul 2021 18:41:52 GMT  
		Size: 1.2 MB (1153026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943d0afddc57ec5c68ce14e40454a1b87cbf480a597671581a2ca174e2cde571`  
		Last Modified: Wed, 21 Jul 2021 18:41:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d9287e79d4393132efb37c503d4160abe844d8f6292fec8bc64db2cd72007`  
		Last Modified: Wed, 21 Jul 2021 18:41:49 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9950840e88dd7c60f47e04de064c506bf702cc91e7b6b046885ffd9aa2d7cdf`  
		Last Modified: Wed, 21 Jul 2021 18:41:53 GMT  
		Size: 22.2 MB (22243949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b87281b8c123dcba3d6d1cf37aa4aae40b07a21eb5d20421196b59900321efe`  
		Last Modified: Wed, 21 Jul 2021 18:41:49 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:0e57f1aa5a8dfd70a24f2922aad2ff16114f20567cff313aebea7341ebdf528d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:24c3d74e41f606a88ceb6b79c0d0c570590e13e46123c57ee17c4bd0a7d62e27
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.5 MB (81513063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7303fde5f20624623382d7b52fcd3c5f82d10035dbd93c9790385c2cc5e46ac7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Jun 2021 21:21:16 GMT
ENV DOCKER_VERSION=20.10.7
# Thu, 03 Jun 2021 21:21:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:21:24 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Jun 2021 21:21:25 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Jun 2021 21:21:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Jun 2021 21:21:25 GMT
CMD ["sh"]
# Thu, 03 Jun 2021 21:21:51 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c521bbbd9945cde2415eae95c3a2a604ea5ca18eb86ab5cadeb589d3b8a13185`  
		Last Modified: Thu, 03 Jun 2021 21:22:44 GMT  
		Size: 70.2 MB (70247077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59707d521c45c42bbb7dbbef463d5d3800859f20122fb54894f0c79d9b435483`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26abe223b186967eef77715b2c6efd147f3a203a0c7b19e61a8947dab4236397`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d806bc203610fb061281b581a0b2522c9fcbd15e55c55ac0c496c9b1dbe63b0`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee8b9b961bd083ca85d7c5a0f9e60a899f6a2185a581a890c03416b9b6e30df`  
		Last Modified: Thu, 03 Jun 2021 21:23:41 GMT  
		Size: 6.4 MB (6401997 bytes)  
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
$ docker pull docker@sha256:b86ac69b6c23bec2cd158a60d1cfbbe21e680b68123448507c509e3a50e73e2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75679816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6375cfb3695b26f65830e1831fc5fdf4ef758ec8e8adcb98f82b1074a5efa5b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:00 GMT
ENV DOCKER_VERSION=20.10.7
# Tue, 15 Jun 2021 22:34:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:06 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:07 GMT
CMD ["sh"]
# Tue, 15 Jun 2021 22:34:26 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829992c79f06822894e73d9a962015a75a5d65ef5a60de627fbb32a973dc0462`  
		Last Modified: Tue, 15 Jun 2021 22:36:03 GMT  
		Size: 64.4 MB (64423231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6714f1b9096eb751a830a9dd13c67cd5e669c68403f1675efd7e78ff8905896d`  
		Last Modified: Tue, 15 Jun 2021 22:35:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997b259c822c244af1192eb31913d45df7f269da56a37fa1c7dc5b9fe273134`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b041c447a8f648b5910833f3c76e5a3231d34a6d76b56d0c22c64b232da92519`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cbc3fd7a1a583e66318479683c0f605e6495f88cea87228beb20e8e811c3f1`  
		Last Modified: Tue, 15 Jun 2021 22:36:43 GMT  
		Size: 6.5 MB (6484825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:a61102937d2bda8319882998ef1ffa27387617f6eea6c298b18a05f7fba82c0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:63cb2df6dfe1fb041b952ddb9f75c69569331fa39577bc41a3e56cf8f79f7e2e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75111066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08bdaf2f88f90320cd3e92a469969efb1f066c6d318631f94e7864828abd7c75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Jun 2021 21:21:16 GMT
ENV DOCKER_VERSION=20.10.7
# Thu, 03 Jun 2021 21:21:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:21:24 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Jun 2021 21:21:25 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Jun 2021 21:21:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Jun 2021 21:21:25 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c521bbbd9945cde2415eae95c3a2a604ea5ca18eb86ab5cadeb589d3b8a13185`  
		Last Modified: Thu, 03 Jun 2021 21:22:44 GMT  
		Size: 70.2 MB (70247077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59707d521c45c42bbb7dbbef463d5d3800859f20122fb54894f0c79d9b435483`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26abe223b186967eef77715b2c6efd147f3a203a0c7b19e61a8947dab4236397`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d806bc203610fb061281b581a0b2522c9fcbd15e55c55ac0c496c9b1dbe63b0`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 150.0 B  
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
$ docker pull docker@sha256:85fa729480d21cd25e5b7f2ba40b53492068501da59e4c23639bd41c5a43040e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69194991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df445af6242a928d36d8a3b4259ba3db9de1d7be5c9806e49b2746cdab4df048`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:00 GMT
ENV DOCKER_VERSION=20.10.7
# Tue, 15 Jun 2021 22:34:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:06 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:07 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829992c79f06822894e73d9a962015a75a5d65ef5a60de627fbb32a973dc0462`  
		Last Modified: Tue, 15 Jun 2021 22:36:03 GMT  
		Size: 64.4 MB (64423231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6714f1b9096eb751a830a9dd13c67cd5e669c68403f1675efd7e78ff8905896d`  
		Last Modified: Tue, 15 Jun 2021 22:35:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997b259c822c244af1192eb31913d45df7f269da56a37fa1c7dc5b9fe273134`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b041c447a8f648b5910833f3c76e5a3231d34a6d76b56d0c22c64b232da92519`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore`

```console
$ docker pull docker@sha256:990b6fbd26ffa675431ea674ff416a850294146bb692e261fe93910d741913f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `docker:windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull docker@sha256:a3b09a7c9d1cfeed83761a580c0fe5ab0d884c80537bbf2b2c9268faaf0964fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2734838564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452c96258d1fa3197a86ab2b95977bf99c84d244914b061957da1461fd17a66a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 18:19:31 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 18:19:35 GMT
ENV DOCKER_VERSION=20.10.7
# Wed, 14 Jul 2021 18:19:38 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.7.zip
# Wed, 14 Jul 2021 18:20:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca81d46af1fb75d88c51bffddab081ffb30e74d3771ee61adfcad7c1b2c6298e`  
		Last Modified: Wed, 14 Jul 2021 18:21:15 GMT  
		Size: 369.1 KB (369149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbc6b36bac5136f1a1dad152043de212420ac9833c3a31b54e9f3aaafa6c473`  
		Last Modified: Wed, 14 Jul 2021 18:21:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bec43c94884d1108711c15e1c29fd2dd7f22fb8092d7bda5d789efac2094f56`  
		Last Modified: Wed, 14 Jul 2021 18:21:14 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ff8b661ba3368d139c4ed45fb23ec33afb51968caee207cb0775444dbd634a`  
		Last Modified: Wed, 14 Jul 2021 18:22:12 GMT  
		Size: 49.0 MB (49018469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:990b6fbd26ffa675431ea674ff416a850294146bb692e261fe93910d741913f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull docker@sha256:a3b09a7c9d1cfeed83761a580c0fe5ab0d884c80537bbf2b2c9268faaf0964fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2734838564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452c96258d1fa3197a86ab2b95977bf99c84d244914b061957da1461fd17a66a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 18:19:31 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 18:19:35 GMT
ENV DOCKER_VERSION=20.10.7
# Wed, 14 Jul 2021 18:19:38 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.7.zip
# Wed, 14 Jul 2021 18:20:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca81d46af1fb75d88c51bffddab081ffb30e74d3771ee61adfcad7c1b2c6298e`  
		Last Modified: Wed, 14 Jul 2021 18:21:15 GMT  
		Size: 369.1 KB (369149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbc6b36bac5136f1a1dad152043de212420ac9833c3a31b54e9f3aaafa6c473`  
		Last Modified: Wed, 14 Jul 2021 18:21:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bec43c94884d1108711c15e1c29fd2dd7f22fb8092d7bda5d789efac2094f56`  
		Last Modified: Wed, 14 Jul 2021 18:21:14 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ff8b661ba3368d139c4ed45fb23ec33afb51968caee207cb0775444dbd634a`  
		Last Modified: Wed, 14 Jul 2021 18:22:12 GMT  
		Size: 49.0 MB (49018469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
