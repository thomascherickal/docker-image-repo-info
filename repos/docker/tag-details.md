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
-	[`docker:20.10.14`](#docker201014)
-	[`docker:20.10.14-alpine3.15`](#docker201014-alpine315)
-	[`docker:20.10.14-dind`](#docker201014-dind)
-	[`docker:20.10.14-dind-alpine3.15`](#docker201014-dind-alpine315)
-	[`docker:20.10.14-dind-rootless`](#docker201014-dind-rootless)
-	[`docker:20.10.14-git`](#docker201014-git)
-	[`docker:20.10.14-windowsservercore`](#docker201014-windowsservercore)
-	[`docker:20.10.14-windowsservercore-1809`](#docker201014-windowsservercore-1809)
-	[`docker:20.10.14-windowsservercore-ltsc2022`](#docker201014-windowsservercore-ltsc2022)
-	[`docker:dind`](#dockerdind)
-	[`docker:dind-rootless`](#dockerdind-rootless)
-	[`docker:git`](#dockergit)
-	[`docker:latest`](#dockerlatest)
-	[`docker:windowsservercore`](#dockerwindowsservercore)
-	[`docker:windowsservercore-1809`](#dockerwindowsservercore-1809)
-	[`docker:windowsservercore-ltsc2022`](#dockerwindowsservercore-ltsc2022)

## `docker:20`

```console
$ docker pull docker@sha256:6d51c80ff60c5af6672cd56b99a19bee907503fbb5602e2d89d82c529029afef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20` - linux; amd64

```console
$ docker pull docker@sha256:6f9f8a915e5a4a8308fcb3e2ba14cd6c7a2dbc11acd03b5a604d97781e84f4e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69395718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68061fb4db0fb111497ee4144c9b3f2cf421a0d450f1d1bc294d0fee31bf5670`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:14:46 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 23 Mar 2022 16:14:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:19:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:19:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:19:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:19:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:19:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:38 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236b952b9466b604bbc4e060a2667d7a7a335bee006fd5104c151dbdb4bf787`  
		Last Modified: Wed, 23 Mar 2022 16:15:39 GMT  
		Size: 2.0 MB (1969538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580f7437ec44a9dd3670ee6fd964ecb068808106d1bd8b961e7a568ef3ceb4f`  
		Last Modified: Wed, 23 Mar 2022 16:15:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0577d395ae504f47fad1c4d36855a3577354d4f0eca32daf7e0b13cf768c17`  
		Last Modified: Thu, 24 Mar 2022 05:20:29 GMT  
		Size: 64.6 MB (64611627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a33444f604b483769f304acdb1c976a4ea78d16943f3be3f9814e1a1e495f`  
		Last Modified: Thu, 24 Mar 2022 05:20:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8453fa1b01e46b0305c4d091304622803430cc8d0b3edb47c7be3a951e62e3`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e8e864d7d32b260f5ca60b2065242e7c51ccaa371f2cc9807d0c32b2ec06f`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:92392048de09154bffb7835256dc671934d598a3093d353494c89502784c8758
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63221233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5544e5647dd04b7224537d744d5e6fee9ade047a9fdfc200ccff6fe4749c30b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:05:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 24 Mar 2022 05:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:05:37 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:05:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:05:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:05:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:05:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:05:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:05:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:05:48 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f777e60e93e1e25280d855dd6b0c8e7e7d1508b2cbd43b9678cd18b2bab72084`  
		Last Modified: Thu, 24 Mar 2022 05:07:13 GMT  
		Size: 1.9 MB (1938915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1b0eef4b739aafe07d37f6f0fc1850ff0b6f61ab14400a1b6348cd2c8b7186`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4e629eede4a3f517e93a1764b365c41b7b2d2554b27f9d6fa6c2e37473901`  
		Last Modified: Thu, 24 Mar 2022 05:07:20 GMT  
		Size: 58.6 MB (58565771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7213dc5eb38c445dc0cffd227536ad4e5265f45307b743d11d8eb43fbdd43c26`  
		Last Modified: Thu, 24 Mar 2022 05:07:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57979a88be1287b9ce5ca410359f13c10dea1b5859e7e42d1bed86fb996f2d6e`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44bdde740192774f34636311a0dbd2b1081ec88c6a24c81b246635938b65c1`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind`

```console
$ docker pull docker@sha256:1452760def210c3cc517fb4d4cb7c7b978badc5568b150914e0b5956950c67b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind` - linux; amd64

```console
$ docker pull docker@sha256:47396a9df5ce04bcd749c54fafbfc4f5139e72044fff120e79727c9a21f755b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76135513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce144dca3a1244e5eae70e9ab5929cc77871e8ea153e89be56c1aed80f2249d3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:14:46 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 23 Mar 2022 16:14:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:19:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:19:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:19:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:19:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:19:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:38 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:19:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 24 Mar 2022 05:19:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:19:45 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 24 Mar 2022 05:19:46 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 24 Mar 2022 05:19:46 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:46 GMT
VOLUME [/var/lib/docker]
# Thu, 24 Mar 2022 05:19:46 GMT
EXPOSE 2375 2376
# Thu, 24 Mar 2022 05:19:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:46 GMT
CMD []
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236b952b9466b604bbc4e060a2667d7a7a335bee006fd5104c151dbdb4bf787`  
		Last Modified: Wed, 23 Mar 2022 16:15:39 GMT  
		Size: 2.0 MB (1969538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580f7437ec44a9dd3670ee6fd964ecb068808106d1bd8b961e7a568ef3ceb4f`  
		Last Modified: Wed, 23 Mar 2022 16:15:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0577d395ae504f47fad1c4d36855a3577354d4f0eca32daf7e0b13cf768c17`  
		Last Modified: Thu, 24 Mar 2022 05:20:29 GMT  
		Size: 64.6 MB (64611627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a33444f604b483769f304acdb1c976a4ea78d16943f3be3f9814e1a1e495f`  
		Last Modified: Thu, 24 Mar 2022 05:20:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8453fa1b01e46b0305c4d091304622803430cc8d0b3edb47c7be3a951e62e3`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e8e864d7d32b260f5ca60b2065242e7c51ccaa371f2cc9807d0c32b2ec06f`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a66f354bc1c7dbe0f8a4b91950340d2866bdbc96f2242a3bfa44d783c053f9c`  
		Last Modified: Thu, 24 Mar 2022 05:20:47 GMT  
		Size: 6.7 MB (6734776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6c10722ade4d16c23d283767216f390533cfb55769e6033eea8c7f4a8a4dc2`  
		Last Modified: Thu, 24 Mar 2022 05:20:47 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78397fa147a16e3ed2f3d8231cf9588472123760e352ca95983aeb96d333a43e`  
		Last Modified: Thu, 24 Mar 2022 05:20:46 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa763b179fa70cb6a2ad1b6bf60c036a10f3b92e0372b67ed05efdf265e1fea`  
		Last Modified: Thu, 24 Mar 2022 05:20:46 GMT  
		Size: 2.7 KB (2745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:75505cc1bcd04f36672b8029910f09c4cc4a71f9d593707926df979f338a6d63
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69841807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a57d0f0cedd6ab4481d9e1ac90434454fe44b1ca846efc6dba36106458d732`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:05:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 24 Mar 2022 05:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:05:37 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:05:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:05:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:05:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:05:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:05:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:05:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:05:48 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:05:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 24 Mar 2022 05:05:58 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:05:59 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 24 Mar 2022 05:06:00 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 24 Mar 2022 05:06:02 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:06:02 GMT
VOLUME [/var/lib/docker]
# Thu, 24 Mar 2022 05:06:03 GMT
EXPOSE 2375 2376
# Thu, 24 Mar 2022 05:06:04 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 24 Mar 2022 05:06:05 GMT
CMD []
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f777e60e93e1e25280d855dd6b0c8e7e7d1508b2cbd43b9678cd18b2bab72084`  
		Last Modified: Thu, 24 Mar 2022 05:07:13 GMT  
		Size: 1.9 MB (1938915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1b0eef4b739aafe07d37f6f0fc1850ff0b6f61ab14400a1b6348cd2c8b7186`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4e629eede4a3f517e93a1764b365c41b7b2d2554b27f9d6fa6c2e37473901`  
		Last Modified: Thu, 24 Mar 2022 05:07:20 GMT  
		Size: 58.6 MB (58565771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7213dc5eb38c445dc0cffd227536ad4e5265f45307b743d11d8eb43fbdd43c26`  
		Last Modified: Thu, 24 Mar 2022 05:07:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57979a88be1287b9ce5ca410359f13c10dea1b5859e7e42d1bed86fb996f2d6e`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44bdde740192774f34636311a0dbd2b1081ec88c6a24c81b246635938b65c1`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc6a23bd8ea7facb45f466a82b87c2136b7f86ec714dab0f1466e6ee53fb65d`  
		Last Modified: Thu, 24 Mar 2022 05:07:42 GMT  
		Size: 6.6 MB (6615580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef7b6dc8191b8b5cc2c67b7b4228b517f4d6341cd3f3c8d3de3565c9f9c8b38`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0986d23cef445052b13281b734555dd4fba26dde5400b38a211f8ba542aa0eb4`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7fb89298925d38bdc861bda494f566d964eab170cf307814a1925a59123965`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:d836fb75037a409e5c7eaa2d86235b12c03f79cafca8acb2680f2f07397d7271
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:4e4e5426e9189d088d01d49d5f12495257c1b6f833966205cd34375f9c83fe76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 MB (96431045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:901a49bfc43b7f98ffcdd1aa26811571d1eb434164d9c35ba0dd3ec8e1fd7113`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:14:46 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 23 Mar 2022 16:14:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:19:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:19:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:19:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:19:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:19:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:38 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:19:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 24 Mar 2022 05:19:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:19:45 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 24 Mar 2022 05:19:46 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 24 Mar 2022 05:19:46 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:46 GMT
VOLUME [/var/lib/docker]
# Thu, 24 Mar 2022 05:19:46 GMT
EXPOSE 2375 2376
# Thu, 24 Mar 2022 05:19:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:46 GMT
CMD []
# Thu, 24 Mar 2022 05:19:50 GMT
RUN apk add --no-cache iproute2
# Thu, 24 Mar 2022 05:19:50 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 24 Mar 2022 05:19:51 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:19:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 24 Mar 2022 05:19:54 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 24 Mar 2022 05:19:54 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 24 Mar 2022 05:19:54 GMT
USER rootless
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236b952b9466b604bbc4e060a2667d7a7a335bee006fd5104c151dbdb4bf787`  
		Last Modified: Wed, 23 Mar 2022 16:15:39 GMT  
		Size: 2.0 MB (1969538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580f7437ec44a9dd3670ee6fd964ecb068808106d1bd8b961e7a568ef3ceb4f`  
		Last Modified: Wed, 23 Mar 2022 16:15:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0577d395ae504f47fad1c4d36855a3577354d4f0eca32daf7e0b13cf768c17`  
		Last Modified: Thu, 24 Mar 2022 05:20:29 GMT  
		Size: 64.6 MB (64611627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a33444f604b483769f304acdb1c976a4ea78d16943f3be3f9814e1a1e495f`  
		Last Modified: Thu, 24 Mar 2022 05:20:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8453fa1b01e46b0305c4d091304622803430cc8d0b3edb47c7be3a951e62e3`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e8e864d7d32b260f5ca60b2065242e7c51ccaa371f2cc9807d0c32b2ec06f`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a66f354bc1c7dbe0f8a4b91950340d2866bdbc96f2242a3bfa44d783c053f9c`  
		Last Modified: Thu, 24 Mar 2022 05:20:47 GMT  
		Size: 6.7 MB (6734776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6c10722ade4d16c23d283767216f390533cfb55769e6033eea8c7f4a8a4dc2`  
		Last Modified: Thu, 24 Mar 2022 05:20:47 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78397fa147a16e3ed2f3d8231cf9588472123760e352ca95983aeb96d333a43e`  
		Last Modified: Thu, 24 Mar 2022 05:20:46 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa763b179fa70cb6a2ad1b6bf60c036a10f3b92e0372b67ed05efdf265e1fea`  
		Last Modified: Thu, 24 Mar 2022 05:20:46 GMT  
		Size: 2.7 KB (2745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6085587cb5f72c79568b29cd55f4c3913866e9ed6397eaa76661ce55d266be`  
		Last Modified: Thu, 24 Mar 2022 05:21:06 GMT  
		Size: 1.2 MB (1161988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a25e47e24f1be9958fc51661a544e64751645608e5cedff2dda9dbc3f4e39c`  
		Last Modified: Thu, 24 Mar 2022 05:21:06 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05797a2b73a664a83ba4a1baf3ec188f150e43ced3f5c9b0d9b695f614e82e31`  
		Last Modified: Thu, 24 Mar 2022 05:21:06 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a221d919a583960b7e36174c14532d2a479dbff4a227c548323d06c4b423ab`  
		Last Modified: Thu, 24 Mar 2022 05:21:09 GMT  
		Size: 19.1 MB (19131826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daedd33adc3be410c282f07f922a10bbbfa3f6b0564eb37b71b60de416300b2a`  
		Last Modified: Thu, 24 Mar 2022 05:21:06 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:df7d7108fde667390444bf3b4fe7cb30ffc8158d555bc05aa7a5f43bd52fcf08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92132624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed85851cb7cd69079f6a55018697c1ac3a6d1c598a7e6c422bfed707a3608503`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:05:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 24 Mar 2022 05:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:05:37 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:05:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:05:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:05:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:05:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:05:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:05:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:05:48 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:05:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 24 Mar 2022 05:05:58 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:05:59 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 24 Mar 2022 05:06:00 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 24 Mar 2022 05:06:02 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:06:02 GMT
VOLUME [/var/lib/docker]
# Thu, 24 Mar 2022 05:06:03 GMT
EXPOSE 2375 2376
# Thu, 24 Mar 2022 05:06:04 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 24 Mar 2022 05:06:05 GMT
CMD []
# Thu, 24 Mar 2022 05:06:13 GMT
RUN apk add --no-cache iproute2
# Thu, 24 Mar 2022 05:06:14 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 24 Mar 2022 05:06:15 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:06:18 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 24 Mar 2022 05:06:19 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 24 Mar 2022 05:06:20 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 24 Mar 2022 05:06:21 GMT
USER rootless
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f777e60e93e1e25280d855dd6b0c8e7e7d1508b2cbd43b9678cd18b2bab72084`  
		Last Modified: Thu, 24 Mar 2022 05:07:13 GMT  
		Size: 1.9 MB (1938915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1b0eef4b739aafe07d37f6f0fc1850ff0b6f61ab14400a1b6348cd2c8b7186`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4e629eede4a3f517e93a1764b365c41b7b2d2554b27f9d6fa6c2e37473901`  
		Last Modified: Thu, 24 Mar 2022 05:07:20 GMT  
		Size: 58.6 MB (58565771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7213dc5eb38c445dc0cffd227536ad4e5265f45307b743d11d8eb43fbdd43c26`  
		Last Modified: Thu, 24 Mar 2022 05:07:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57979a88be1287b9ce5ca410359f13c10dea1b5859e7e42d1bed86fb996f2d6e`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44bdde740192774f34636311a0dbd2b1081ec88c6a24c81b246635938b65c1`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc6a23bd8ea7facb45f466a82b87c2136b7f86ec714dab0f1466e6ee53fb65d`  
		Last Modified: Thu, 24 Mar 2022 05:07:42 GMT  
		Size: 6.6 MB (6615580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef7b6dc8191b8b5cc2c67b7b4228b517f4d6341cd3f3c8d3de3565c9f9c8b38`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0986d23cef445052b13281b734555dd4fba26dde5400b38a211f8ba542aa0eb4`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7fb89298925d38bdc861bda494f566d964eab170cf307814a1925a59123965`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2a88bdadcae21855d08188cd8b67037b35b213029f2cffdd90dd25ba0c6386`  
		Last Modified: Thu, 24 Mar 2022 05:08:03 GMT  
		Size: 1.2 MB (1177944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0815bff1c961ac2d8113264775046dba30417f109f54ba09f493192934fd0940`  
		Last Modified: Thu, 24 Mar 2022 05:08:03 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399d118cae203620b47422a9705be6c340af1e0db7fef87338deff30269fb404`  
		Last Modified: Thu, 24 Mar 2022 05:08:03 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d745b7e9d65f0a9afee27aa8bacf9577cbcec66494bc9f115621f4f85366491`  
		Last Modified: Thu, 24 Mar 2022 05:08:06 GMT  
		Size: 21.1 MB (21111250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23af1a6c11dc14339ad8b7c79cf3ce581990a6e4193573afde6892824a7d045c`  
		Last Modified: Thu, 24 Mar 2022 05:08:03 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-git`

```console
$ docker pull docker@sha256:5b8f51320fb14ff3fbc45001d6477a8edc4155128fcd5dd4b7139294336e91fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-git` - linux; amd64

```console
$ docker pull docker@sha256:3728219f8cc46f4f397b330577000ca639d8324aa5a1556d0e6a5cf738ebe0ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76219858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b79097ab0874839ce4ef81b16354be702b88d942e0232d86af2acdc33e22b9bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:14:46 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 23 Mar 2022 16:14:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:19:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:19:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:19:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:19:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:19:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:38 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:19:57 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236b952b9466b604bbc4e060a2667d7a7a335bee006fd5104c151dbdb4bf787`  
		Last Modified: Wed, 23 Mar 2022 16:15:39 GMT  
		Size: 2.0 MB (1969538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580f7437ec44a9dd3670ee6fd964ecb068808106d1bd8b961e7a568ef3ceb4f`  
		Last Modified: Wed, 23 Mar 2022 16:15:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0577d395ae504f47fad1c4d36855a3577354d4f0eca32daf7e0b13cf768c17`  
		Last Modified: Thu, 24 Mar 2022 05:20:29 GMT  
		Size: 64.6 MB (64611627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a33444f604b483769f304acdb1c976a4ea78d16943f3be3f9814e1a1e495f`  
		Last Modified: Thu, 24 Mar 2022 05:20:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8453fa1b01e46b0305c4d091304622803430cc8d0b3edb47c7be3a951e62e3`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e8e864d7d32b260f5ca60b2065242e7c51ccaa371f2cc9807d0c32b2ec06f`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8260489be308ed8266d2c832c405abe7c01809d417bf17b473ec0f0f37339134`  
		Last Modified: Thu, 24 Mar 2022 05:21:32 GMT  
		Size: 6.8 MB (6824140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:7a2baddd024a7811ef67203d77de9ab3829ddca714ca6fe11f2ed2b3572fb5f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70154288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb42c0db861bb97af997256dc9ff427b43b0668bc7689aada6aa99ba4937b84e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:05:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 24 Mar 2022 05:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:05:37 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:05:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:05:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:05:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:05:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:05:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:05:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:05:48 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:06:28 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f777e60e93e1e25280d855dd6b0c8e7e7d1508b2cbd43b9678cd18b2bab72084`  
		Last Modified: Thu, 24 Mar 2022 05:07:13 GMT  
		Size: 1.9 MB (1938915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1b0eef4b739aafe07d37f6f0fc1850ff0b6f61ab14400a1b6348cd2c8b7186`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4e629eede4a3f517e93a1764b365c41b7b2d2554b27f9d6fa6c2e37473901`  
		Last Modified: Thu, 24 Mar 2022 05:07:20 GMT  
		Size: 58.6 MB (58565771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7213dc5eb38c445dc0cffd227536ad4e5265f45307b743d11d8eb43fbdd43c26`  
		Last Modified: Thu, 24 Mar 2022 05:07:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57979a88be1287b9ce5ca410359f13c10dea1b5859e7e42d1bed86fb996f2d6e`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44bdde740192774f34636311a0dbd2b1081ec88c6a24c81b246635938b65c1`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a06e853d235302bea036f40c1af6580b1f35dccf8df3f8610cab630655e58ca`  
		Last Modified: Thu, 24 Mar 2022 05:08:26 GMT  
		Size: 6.9 MB (6933055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore`

```console
$ docker pull docker@sha256:e975b7c270f2a35f16d48b91e2ab5f0eff84a690da1fcedab97e7157d0b3a5ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.587; amd64
	-	windows version 10.0.17763.2686; amd64

### `docker:20-windowsservercore` - windows version 10.0.20348.587; amd64

```console
$ docker pull docker@sha256:aefae8d2bf575204b17f88589c7741c350281048d96844f9fd3316a80ec2940e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2275653601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:723b6471c336c441aa997a1c5d0672ef1de87fe45687edb769c52bd0edce4e81`
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
# Thu, 24 Mar 2022 05:15:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:15:30 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.14.zip
# Thu, 24 Mar 2022 05:16:11 GMT
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
	-	`sha256:0181d328453c16ef4bf5dfa86a118c96a8325d7a3e58637e504f5425c5ea7ae2`  
		Last Modified: Thu, 24 Mar 2022 05:18:23 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e48a2566f0d50346970f29a77bd1cbfde2d33a34fc25d9227a8900f494b136a`  
		Last Modified: Thu, 24 Mar 2022 05:18:24 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cd9d001a2232e2f5406882e91758565fec1809573168d4e31cafa909ea5d4f`  
		Last Modified: Thu, 24 Mar 2022 05:18:35 GMT  
		Size: 53.8 MB (53804106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull docker@sha256:034598e549b6c0f2bb1ff47cbb638cb9785ab1456144eb4c0da198e075e70a9d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2769426444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2374652d04922dbe838fbdac11dc741534c504b1213d1110bcf7ab3ce0075be`
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
# Thu, 24 Mar 2022 05:16:22 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:16:23 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.14.zip
# Thu, 24 Mar 2022 05:17:56 GMT
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
	-	`sha256:3a37839ee100e0b4b77379ec17ab118f0b377c9d7f73de9b4fdfce26e5910d07`  
		Last Modified: Thu, 24 Mar 2022 05:18:49 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a35b5cdb293ca7295865a746b962b396382293a16a843862f866ad76d49b7d`  
		Last Modified: Thu, 24 Mar 2022 05:18:49 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791bcb5d614f3fbb4d6ff0b29ce1877c53e05d3b8536fe0fa4b549f20c0b6730`  
		Last Modified: Thu, 24 Mar 2022 05:19:47 GMT  
		Size: 53.6 MB (53615927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-1809`

```console
$ docker pull docker@sha256:6e21edf269ee8beed4808bae91f5cc840ad2a042a19a6eb6de13c97e3053906b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `docker:20-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull docker@sha256:034598e549b6c0f2bb1ff47cbb638cb9785ab1456144eb4c0da198e075e70a9d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2769426444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2374652d04922dbe838fbdac11dc741534c504b1213d1110bcf7ab3ce0075be`
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
# Thu, 24 Mar 2022 05:16:22 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:16:23 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.14.zip
# Thu, 24 Mar 2022 05:17:56 GMT
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
	-	`sha256:3a37839ee100e0b4b77379ec17ab118f0b377c9d7f73de9b4fdfce26e5910d07`  
		Last Modified: Thu, 24 Mar 2022 05:18:49 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a35b5cdb293ca7295865a746b962b396382293a16a843862f866ad76d49b7d`  
		Last Modified: Thu, 24 Mar 2022 05:18:49 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791bcb5d614f3fbb4d6ff0b29ce1877c53e05d3b8536fe0fa4b549f20c0b6730`  
		Last Modified: Thu, 24 Mar 2022 05:19:47 GMT  
		Size: 53.6 MB (53615927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:8520b3fc85f5fe47604cbba4353f8b2feda30bcf041e26848bd6d812173f4444
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.587; amd64

### `docker:20-windowsservercore-ltsc2022` - windows version 10.0.20348.587; amd64

```console
$ docker pull docker@sha256:aefae8d2bf575204b17f88589c7741c350281048d96844f9fd3316a80ec2940e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2275653601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:723b6471c336c441aa997a1c5d0672ef1de87fe45687edb769c52bd0edce4e81`
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
# Thu, 24 Mar 2022 05:15:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:15:30 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.14.zip
# Thu, 24 Mar 2022 05:16:11 GMT
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
	-	`sha256:0181d328453c16ef4bf5dfa86a118c96a8325d7a3e58637e504f5425c5ea7ae2`  
		Last Modified: Thu, 24 Mar 2022 05:18:23 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e48a2566f0d50346970f29a77bd1cbfde2d33a34fc25d9227a8900f494b136a`  
		Last Modified: Thu, 24 Mar 2022 05:18:24 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cd9d001a2232e2f5406882e91758565fec1809573168d4e31cafa909ea5d4f`  
		Last Modified: Thu, 24 Mar 2022 05:18:35 GMT  
		Size: 53.8 MB (53804106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10`

```console
$ docker pull docker@sha256:6d51c80ff60c5af6672cd56b99a19bee907503fbb5602e2d89d82c529029afef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10` - linux; amd64

```console
$ docker pull docker@sha256:6f9f8a915e5a4a8308fcb3e2ba14cd6c7a2dbc11acd03b5a604d97781e84f4e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69395718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68061fb4db0fb111497ee4144c9b3f2cf421a0d450f1d1bc294d0fee31bf5670`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:14:46 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 23 Mar 2022 16:14:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:19:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:19:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:19:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:19:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:19:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:38 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236b952b9466b604bbc4e060a2667d7a7a335bee006fd5104c151dbdb4bf787`  
		Last Modified: Wed, 23 Mar 2022 16:15:39 GMT  
		Size: 2.0 MB (1969538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580f7437ec44a9dd3670ee6fd964ecb068808106d1bd8b961e7a568ef3ceb4f`  
		Last Modified: Wed, 23 Mar 2022 16:15:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0577d395ae504f47fad1c4d36855a3577354d4f0eca32daf7e0b13cf768c17`  
		Last Modified: Thu, 24 Mar 2022 05:20:29 GMT  
		Size: 64.6 MB (64611627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a33444f604b483769f304acdb1c976a4ea78d16943f3be3f9814e1a1e495f`  
		Last Modified: Thu, 24 Mar 2022 05:20:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8453fa1b01e46b0305c4d091304622803430cc8d0b3edb47c7be3a951e62e3`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e8e864d7d32b260f5ca60b2065242e7c51ccaa371f2cc9807d0c32b2ec06f`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:92392048de09154bffb7835256dc671934d598a3093d353494c89502784c8758
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63221233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5544e5647dd04b7224537d744d5e6fee9ade047a9fdfc200ccff6fe4749c30b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:05:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 24 Mar 2022 05:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:05:37 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:05:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:05:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:05:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:05:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:05:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:05:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:05:48 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f777e60e93e1e25280d855dd6b0c8e7e7d1508b2cbd43b9678cd18b2bab72084`  
		Last Modified: Thu, 24 Mar 2022 05:07:13 GMT  
		Size: 1.9 MB (1938915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1b0eef4b739aafe07d37f6f0fc1850ff0b6f61ab14400a1b6348cd2c8b7186`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4e629eede4a3f517e93a1764b365c41b7b2d2554b27f9d6fa6c2e37473901`  
		Last Modified: Thu, 24 Mar 2022 05:07:20 GMT  
		Size: 58.6 MB (58565771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7213dc5eb38c445dc0cffd227536ad4e5265f45307b743d11d8eb43fbdd43c26`  
		Last Modified: Thu, 24 Mar 2022 05:07:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57979a88be1287b9ce5ca410359f13c10dea1b5859e7e42d1bed86fb996f2d6e`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44bdde740192774f34636311a0dbd2b1081ec88c6a24c81b246635938b65c1`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind`

```console
$ docker pull docker@sha256:1452760def210c3cc517fb4d4cb7c7b978badc5568b150914e0b5956950c67b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind` - linux; amd64

```console
$ docker pull docker@sha256:47396a9df5ce04bcd749c54fafbfc4f5139e72044fff120e79727c9a21f755b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76135513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce144dca3a1244e5eae70e9ab5929cc77871e8ea153e89be56c1aed80f2249d3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:14:46 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 23 Mar 2022 16:14:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:19:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:19:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:19:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:19:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:19:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:38 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:19:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 24 Mar 2022 05:19:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:19:45 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 24 Mar 2022 05:19:46 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 24 Mar 2022 05:19:46 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:46 GMT
VOLUME [/var/lib/docker]
# Thu, 24 Mar 2022 05:19:46 GMT
EXPOSE 2375 2376
# Thu, 24 Mar 2022 05:19:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:46 GMT
CMD []
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236b952b9466b604bbc4e060a2667d7a7a335bee006fd5104c151dbdb4bf787`  
		Last Modified: Wed, 23 Mar 2022 16:15:39 GMT  
		Size: 2.0 MB (1969538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580f7437ec44a9dd3670ee6fd964ecb068808106d1bd8b961e7a568ef3ceb4f`  
		Last Modified: Wed, 23 Mar 2022 16:15:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0577d395ae504f47fad1c4d36855a3577354d4f0eca32daf7e0b13cf768c17`  
		Last Modified: Thu, 24 Mar 2022 05:20:29 GMT  
		Size: 64.6 MB (64611627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a33444f604b483769f304acdb1c976a4ea78d16943f3be3f9814e1a1e495f`  
		Last Modified: Thu, 24 Mar 2022 05:20:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8453fa1b01e46b0305c4d091304622803430cc8d0b3edb47c7be3a951e62e3`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e8e864d7d32b260f5ca60b2065242e7c51ccaa371f2cc9807d0c32b2ec06f`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a66f354bc1c7dbe0f8a4b91950340d2866bdbc96f2242a3bfa44d783c053f9c`  
		Last Modified: Thu, 24 Mar 2022 05:20:47 GMT  
		Size: 6.7 MB (6734776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6c10722ade4d16c23d283767216f390533cfb55769e6033eea8c7f4a8a4dc2`  
		Last Modified: Thu, 24 Mar 2022 05:20:47 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78397fa147a16e3ed2f3d8231cf9588472123760e352ca95983aeb96d333a43e`  
		Last Modified: Thu, 24 Mar 2022 05:20:46 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa763b179fa70cb6a2ad1b6bf60c036a10f3b92e0372b67ed05efdf265e1fea`  
		Last Modified: Thu, 24 Mar 2022 05:20:46 GMT  
		Size: 2.7 KB (2745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:75505cc1bcd04f36672b8029910f09c4cc4a71f9d593707926df979f338a6d63
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69841807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a57d0f0cedd6ab4481d9e1ac90434454fe44b1ca846efc6dba36106458d732`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:05:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 24 Mar 2022 05:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:05:37 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:05:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:05:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:05:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:05:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:05:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:05:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:05:48 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:05:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 24 Mar 2022 05:05:58 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:05:59 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 24 Mar 2022 05:06:00 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 24 Mar 2022 05:06:02 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:06:02 GMT
VOLUME [/var/lib/docker]
# Thu, 24 Mar 2022 05:06:03 GMT
EXPOSE 2375 2376
# Thu, 24 Mar 2022 05:06:04 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 24 Mar 2022 05:06:05 GMT
CMD []
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f777e60e93e1e25280d855dd6b0c8e7e7d1508b2cbd43b9678cd18b2bab72084`  
		Last Modified: Thu, 24 Mar 2022 05:07:13 GMT  
		Size: 1.9 MB (1938915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1b0eef4b739aafe07d37f6f0fc1850ff0b6f61ab14400a1b6348cd2c8b7186`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4e629eede4a3f517e93a1764b365c41b7b2d2554b27f9d6fa6c2e37473901`  
		Last Modified: Thu, 24 Mar 2022 05:07:20 GMT  
		Size: 58.6 MB (58565771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7213dc5eb38c445dc0cffd227536ad4e5265f45307b743d11d8eb43fbdd43c26`  
		Last Modified: Thu, 24 Mar 2022 05:07:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57979a88be1287b9ce5ca410359f13c10dea1b5859e7e42d1bed86fb996f2d6e`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44bdde740192774f34636311a0dbd2b1081ec88c6a24c81b246635938b65c1`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc6a23bd8ea7facb45f466a82b87c2136b7f86ec714dab0f1466e6ee53fb65d`  
		Last Modified: Thu, 24 Mar 2022 05:07:42 GMT  
		Size: 6.6 MB (6615580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef7b6dc8191b8b5cc2c67b7b4228b517f4d6341cd3f3c8d3de3565c9f9c8b38`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0986d23cef445052b13281b734555dd4fba26dde5400b38a211f8ba542aa0eb4`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7fb89298925d38bdc861bda494f566d964eab170cf307814a1925a59123965`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind-rootless`

```console
$ docker pull docker@sha256:d836fb75037a409e5c7eaa2d86235b12c03f79cafca8acb2680f2f07397d7271
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:4e4e5426e9189d088d01d49d5f12495257c1b6f833966205cd34375f9c83fe76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 MB (96431045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:901a49bfc43b7f98ffcdd1aa26811571d1eb434164d9c35ba0dd3ec8e1fd7113`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:14:46 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 23 Mar 2022 16:14:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:19:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:19:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:19:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:19:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:19:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:38 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:19:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 24 Mar 2022 05:19:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:19:45 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 24 Mar 2022 05:19:46 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 24 Mar 2022 05:19:46 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:46 GMT
VOLUME [/var/lib/docker]
# Thu, 24 Mar 2022 05:19:46 GMT
EXPOSE 2375 2376
# Thu, 24 Mar 2022 05:19:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:46 GMT
CMD []
# Thu, 24 Mar 2022 05:19:50 GMT
RUN apk add --no-cache iproute2
# Thu, 24 Mar 2022 05:19:50 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 24 Mar 2022 05:19:51 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:19:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 24 Mar 2022 05:19:54 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 24 Mar 2022 05:19:54 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 24 Mar 2022 05:19:54 GMT
USER rootless
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236b952b9466b604bbc4e060a2667d7a7a335bee006fd5104c151dbdb4bf787`  
		Last Modified: Wed, 23 Mar 2022 16:15:39 GMT  
		Size: 2.0 MB (1969538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580f7437ec44a9dd3670ee6fd964ecb068808106d1bd8b961e7a568ef3ceb4f`  
		Last Modified: Wed, 23 Mar 2022 16:15:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0577d395ae504f47fad1c4d36855a3577354d4f0eca32daf7e0b13cf768c17`  
		Last Modified: Thu, 24 Mar 2022 05:20:29 GMT  
		Size: 64.6 MB (64611627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a33444f604b483769f304acdb1c976a4ea78d16943f3be3f9814e1a1e495f`  
		Last Modified: Thu, 24 Mar 2022 05:20:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8453fa1b01e46b0305c4d091304622803430cc8d0b3edb47c7be3a951e62e3`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e8e864d7d32b260f5ca60b2065242e7c51ccaa371f2cc9807d0c32b2ec06f`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a66f354bc1c7dbe0f8a4b91950340d2866bdbc96f2242a3bfa44d783c053f9c`  
		Last Modified: Thu, 24 Mar 2022 05:20:47 GMT  
		Size: 6.7 MB (6734776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6c10722ade4d16c23d283767216f390533cfb55769e6033eea8c7f4a8a4dc2`  
		Last Modified: Thu, 24 Mar 2022 05:20:47 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78397fa147a16e3ed2f3d8231cf9588472123760e352ca95983aeb96d333a43e`  
		Last Modified: Thu, 24 Mar 2022 05:20:46 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa763b179fa70cb6a2ad1b6bf60c036a10f3b92e0372b67ed05efdf265e1fea`  
		Last Modified: Thu, 24 Mar 2022 05:20:46 GMT  
		Size: 2.7 KB (2745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6085587cb5f72c79568b29cd55f4c3913866e9ed6397eaa76661ce55d266be`  
		Last Modified: Thu, 24 Mar 2022 05:21:06 GMT  
		Size: 1.2 MB (1161988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a25e47e24f1be9958fc51661a544e64751645608e5cedff2dda9dbc3f4e39c`  
		Last Modified: Thu, 24 Mar 2022 05:21:06 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05797a2b73a664a83ba4a1baf3ec188f150e43ced3f5c9b0d9b695f614e82e31`  
		Last Modified: Thu, 24 Mar 2022 05:21:06 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a221d919a583960b7e36174c14532d2a479dbff4a227c548323d06c4b423ab`  
		Last Modified: Thu, 24 Mar 2022 05:21:09 GMT  
		Size: 19.1 MB (19131826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daedd33adc3be410c282f07f922a10bbbfa3f6b0564eb37b71b60de416300b2a`  
		Last Modified: Thu, 24 Mar 2022 05:21:06 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:df7d7108fde667390444bf3b4fe7cb30ffc8158d555bc05aa7a5f43bd52fcf08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92132624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed85851cb7cd69079f6a55018697c1ac3a6d1c598a7e6c422bfed707a3608503`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:05:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 24 Mar 2022 05:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:05:37 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:05:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:05:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:05:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:05:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:05:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:05:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:05:48 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:05:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 24 Mar 2022 05:05:58 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:05:59 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 24 Mar 2022 05:06:00 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 24 Mar 2022 05:06:02 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:06:02 GMT
VOLUME [/var/lib/docker]
# Thu, 24 Mar 2022 05:06:03 GMT
EXPOSE 2375 2376
# Thu, 24 Mar 2022 05:06:04 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 24 Mar 2022 05:06:05 GMT
CMD []
# Thu, 24 Mar 2022 05:06:13 GMT
RUN apk add --no-cache iproute2
# Thu, 24 Mar 2022 05:06:14 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 24 Mar 2022 05:06:15 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:06:18 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 24 Mar 2022 05:06:19 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 24 Mar 2022 05:06:20 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 24 Mar 2022 05:06:21 GMT
USER rootless
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f777e60e93e1e25280d855dd6b0c8e7e7d1508b2cbd43b9678cd18b2bab72084`  
		Last Modified: Thu, 24 Mar 2022 05:07:13 GMT  
		Size: 1.9 MB (1938915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1b0eef4b739aafe07d37f6f0fc1850ff0b6f61ab14400a1b6348cd2c8b7186`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4e629eede4a3f517e93a1764b365c41b7b2d2554b27f9d6fa6c2e37473901`  
		Last Modified: Thu, 24 Mar 2022 05:07:20 GMT  
		Size: 58.6 MB (58565771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7213dc5eb38c445dc0cffd227536ad4e5265f45307b743d11d8eb43fbdd43c26`  
		Last Modified: Thu, 24 Mar 2022 05:07:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57979a88be1287b9ce5ca410359f13c10dea1b5859e7e42d1bed86fb996f2d6e`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44bdde740192774f34636311a0dbd2b1081ec88c6a24c81b246635938b65c1`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc6a23bd8ea7facb45f466a82b87c2136b7f86ec714dab0f1466e6ee53fb65d`  
		Last Modified: Thu, 24 Mar 2022 05:07:42 GMT  
		Size: 6.6 MB (6615580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef7b6dc8191b8b5cc2c67b7b4228b517f4d6341cd3f3c8d3de3565c9f9c8b38`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0986d23cef445052b13281b734555dd4fba26dde5400b38a211f8ba542aa0eb4`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7fb89298925d38bdc861bda494f566d964eab170cf307814a1925a59123965`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2a88bdadcae21855d08188cd8b67037b35b213029f2cffdd90dd25ba0c6386`  
		Last Modified: Thu, 24 Mar 2022 05:08:03 GMT  
		Size: 1.2 MB (1177944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0815bff1c961ac2d8113264775046dba30417f109f54ba09f493192934fd0940`  
		Last Modified: Thu, 24 Mar 2022 05:08:03 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399d118cae203620b47422a9705be6c340af1e0db7fef87338deff30269fb404`  
		Last Modified: Thu, 24 Mar 2022 05:08:03 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d745b7e9d65f0a9afee27aa8bacf9577cbcec66494bc9f115621f4f85366491`  
		Last Modified: Thu, 24 Mar 2022 05:08:06 GMT  
		Size: 21.1 MB (21111250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23af1a6c11dc14339ad8b7c79cf3ce581990a6e4193573afde6892824a7d045c`  
		Last Modified: Thu, 24 Mar 2022 05:08:03 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-git`

```console
$ docker pull docker@sha256:5b8f51320fb14ff3fbc45001d6477a8edc4155128fcd5dd4b7139294336e91fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-git` - linux; amd64

```console
$ docker pull docker@sha256:3728219f8cc46f4f397b330577000ca639d8324aa5a1556d0e6a5cf738ebe0ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76219858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b79097ab0874839ce4ef81b16354be702b88d942e0232d86af2acdc33e22b9bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:14:46 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 23 Mar 2022 16:14:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:19:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:19:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:19:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:19:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:19:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:38 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:19:57 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236b952b9466b604bbc4e060a2667d7a7a335bee006fd5104c151dbdb4bf787`  
		Last Modified: Wed, 23 Mar 2022 16:15:39 GMT  
		Size: 2.0 MB (1969538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580f7437ec44a9dd3670ee6fd964ecb068808106d1bd8b961e7a568ef3ceb4f`  
		Last Modified: Wed, 23 Mar 2022 16:15:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0577d395ae504f47fad1c4d36855a3577354d4f0eca32daf7e0b13cf768c17`  
		Last Modified: Thu, 24 Mar 2022 05:20:29 GMT  
		Size: 64.6 MB (64611627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a33444f604b483769f304acdb1c976a4ea78d16943f3be3f9814e1a1e495f`  
		Last Modified: Thu, 24 Mar 2022 05:20:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8453fa1b01e46b0305c4d091304622803430cc8d0b3edb47c7be3a951e62e3`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e8e864d7d32b260f5ca60b2065242e7c51ccaa371f2cc9807d0c32b2ec06f`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8260489be308ed8266d2c832c405abe7c01809d417bf17b473ec0f0f37339134`  
		Last Modified: Thu, 24 Mar 2022 05:21:32 GMT  
		Size: 6.8 MB (6824140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:7a2baddd024a7811ef67203d77de9ab3829ddca714ca6fe11f2ed2b3572fb5f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70154288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb42c0db861bb97af997256dc9ff427b43b0668bc7689aada6aa99ba4937b84e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:05:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 24 Mar 2022 05:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:05:37 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:05:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:05:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:05:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:05:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:05:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:05:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:05:48 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:06:28 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f777e60e93e1e25280d855dd6b0c8e7e7d1508b2cbd43b9678cd18b2bab72084`  
		Last Modified: Thu, 24 Mar 2022 05:07:13 GMT  
		Size: 1.9 MB (1938915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1b0eef4b739aafe07d37f6f0fc1850ff0b6f61ab14400a1b6348cd2c8b7186`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4e629eede4a3f517e93a1764b365c41b7b2d2554b27f9d6fa6c2e37473901`  
		Last Modified: Thu, 24 Mar 2022 05:07:20 GMT  
		Size: 58.6 MB (58565771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7213dc5eb38c445dc0cffd227536ad4e5265f45307b743d11d8eb43fbdd43c26`  
		Last Modified: Thu, 24 Mar 2022 05:07:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57979a88be1287b9ce5ca410359f13c10dea1b5859e7e42d1bed86fb996f2d6e`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44bdde740192774f34636311a0dbd2b1081ec88c6a24c81b246635938b65c1`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a06e853d235302bea036f40c1af6580b1f35dccf8df3f8610cab630655e58ca`  
		Last Modified: Thu, 24 Mar 2022 05:08:26 GMT  
		Size: 6.9 MB (6933055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore`

```console
$ docker pull docker@sha256:e975b7c270f2a35f16d48b91e2ab5f0eff84a690da1fcedab97e7157d0b3a5ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.587; amd64
	-	windows version 10.0.17763.2686; amd64

### `docker:20.10-windowsservercore` - windows version 10.0.20348.587; amd64

```console
$ docker pull docker@sha256:aefae8d2bf575204b17f88589c7741c350281048d96844f9fd3316a80ec2940e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2275653601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:723b6471c336c441aa997a1c5d0672ef1de87fe45687edb769c52bd0edce4e81`
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
# Thu, 24 Mar 2022 05:15:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:15:30 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.14.zip
# Thu, 24 Mar 2022 05:16:11 GMT
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
	-	`sha256:0181d328453c16ef4bf5dfa86a118c96a8325d7a3e58637e504f5425c5ea7ae2`  
		Last Modified: Thu, 24 Mar 2022 05:18:23 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e48a2566f0d50346970f29a77bd1cbfde2d33a34fc25d9227a8900f494b136a`  
		Last Modified: Thu, 24 Mar 2022 05:18:24 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cd9d001a2232e2f5406882e91758565fec1809573168d4e31cafa909ea5d4f`  
		Last Modified: Thu, 24 Mar 2022 05:18:35 GMT  
		Size: 53.8 MB (53804106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull docker@sha256:034598e549b6c0f2bb1ff47cbb638cb9785ab1456144eb4c0da198e075e70a9d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2769426444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2374652d04922dbe838fbdac11dc741534c504b1213d1110bcf7ab3ce0075be`
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
# Thu, 24 Mar 2022 05:16:22 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:16:23 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.14.zip
# Thu, 24 Mar 2022 05:17:56 GMT
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
	-	`sha256:3a37839ee100e0b4b77379ec17ab118f0b377c9d7f73de9b4fdfce26e5910d07`  
		Last Modified: Thu, 24 Mar 2022 05:18:49 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a35b5cdb293ca7295865a746b962b396382293a16a843862f866ad76d49b7d`  
		Last Modified: Thu, 24 Mar 2022 05:18:49 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791bcb5d614f3fbb4d6ff0b29ce1877c53e05d3b8536fe0fa4b549f20c0b6730`  
		Last Modified: Thu, 24 Mar 2022 05:19:47 GMT  
		Size: 53.6 MB (53615927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-1809`

```console
$ docker pull docker@sha256:6e21edf269ee8beed4808bae91f5cc840ad2a042a19a6eb6de13c97e3053906b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `docker:20.10-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull docker@sha256:034598e549b6c0f2bb1ff47cbb638cb9785ab1456144eb4c0da198e075e70a9d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2769426444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2374652d04922dbe838fbdac11dc741534c504b1213d1110bcf7ab3ce0075be`
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
# Thu, 24 Mar 2022 05:16:22 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:16:23 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.14.zip
# Thu, 24 Mar 2022 05:17:56 GMT
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
	-	`sha256:3a37839ee100e0b4b77379ec17ab118f0b377c9d7f73de9b4fdfce26e5910d07`  
		Last Modified: Thu, 24 Mar 2022 05:18:49 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a35b5cdb293ca7295865a746b962b396382293a16a843862f866ad76d49b7d`  
		Last Modified: Thu, 24 Mar 2022 05:18:49 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791bcb5d614f3fbb4d6ff0b29ce1877c53e05d3b8536fe0fa4b549f20c0b6730`  
		Last Modified: Thu, 24 Mar 2022 05:19:47 GMT  
		Size: 53.6 MB (53615927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:8520b3fc85f5fe47604cbba4353f8b2feda30bcf041e26848bd6d812173f4444
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.587; amd64

### `docker:20.10-windowsservercore-ltsc2022` - windows version 10.0.20348.587; amd64

```console
$ docker pull docker@sha256:aefae8d2bf575204b17f88589c7741c350281048d96844f9fd3316a80ec2940e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2275653601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:723b6471c336c441aa997a1c5d0672ef1de87fe45687edb769c52bd0edce4e81`
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
# Thu, 24 Mar 2022 05:15:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:15:30 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.14.zip
# Thu, 24 Mar 2022 05:16:11 GMT
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
	-	`sha256:0181d328453c16ef4bf5dfa86a118c96a8325d7a3e58637e504f5425c5ea7ae2`  
		Last Modified: Thu, 24 Mar 2022 05:18:23 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e48a2566f0d50346970f29a77bd1cbfde2d33a34fc25d9227a8900f494b136a`  
		Last Modified: Thu, 24 Mar 2022 05:18:24 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cd9d001a2232e2f5406882e91758565fec1809573168d4e31cafa909ea5d4f`  
		Last Modified: Thu, 24 Mar 2022 05:18:35 GMT  
		Size: 53.8 MB (53804106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.14`

```console
$ docker pull docker@sha256:6d51c80ff60c5af6672cd56b99a19bee907503fbb5602e2d89d82c529029afef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.14` - linux; amd64

```console
$ docker pull docker@sha256:6f9f8a915e5a4a8308fcb3e2ba14cd6c7a2dbc11acd03b5a604d97781e84f4e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69395718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68061fb4db0fb111497ee4144c9b3f2cf421a0d450f1d1bc294d0fee31bf5670`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:14:46 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 23 Mar 2022 16:14:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:19:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:19:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:19:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:19:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:19:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:38 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236b952b9466b604bbc4e060a2667d7a7a335bee006fd5104c151dbdb4bf787`  
		Last Modified: Wed, 23 Mar 2022 16:15:39 GMT  
		Size: 2.0 MB (1969538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580f7437ec44a9dd3670ee6fd964ecb068808106d1bd8b961e7a568ef3ceb4f`  
		Last Modified: Wed, 23 Mar 2022 16:15:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0577d395ae504f47fad1c4d36855a3577354d4f0eca32daf7e0b13cf768c17`  
		Last Modified: Thu, 24 Mar 2022 05:20:29 GMT  
		Size: 64.6 MB (64611627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a33444f604b483769f304acdb1c976a4ea78d16943f3be3f9814e1a1e495f`  
		Last Modified: Thu, 24 Mar 2022 05:20:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8453fa1b01e46b0305c4d091304622803430cc8d0b3edb47c7be3a951e62e3`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e8e864d7d32b260f5ca60b2065242e7c51ccaa371f2cc9807d0c32b2ec06f`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.14` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:92392048de09154bffb7835256dc671934d598a3093d353494c89502784c8758
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63221233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5544e5647dd04b7224537d744d5e6fee9ade047a9fdfc200ccff6fe4749c30b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:05:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 24 Mar 2022 05:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:05:37 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:05:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:05:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:05:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:05:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:05:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:05:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:05:48 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f777e60e93e1e25280d855dd6b0c8e7e7d1508b2cbd43b9678cd18b2bab72084`  
		Last Modified: Thu, 24 Mar 2022 05:07:13 GMT  
		Size: 1.9 MB (1938915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1b0eef4b739aafe07d37f6f0fc1850ff0b6f61ab14400a1b6348cd2c8b7186`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4e629eede4a3f517e93a1764b365c41b7b2d2554b27f9d6fa6c2e37473901`  
		Last Modified: Thu, 24 Mar 2022 05:07:20 GMT  
		Size: 58.6 MB (58565771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7213dc5eb38c445dc0cffd227536ad4e5265f45307b743d11d8eb43fbdd43c26`  
		Last Modified: Thu, 24 Mar 2022 05:07:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57979a88be1287b9ce5ca410359f13c10dea1b5859e7e42d1bed86fb996f2d6e`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44bdde740192774f34636311a0dbd2b1081ec88c6a24c81b246635938b65c1`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.14-alpine3.15`

```console
$ docker pull docker@sha256:6d51c80ff60c5af6672cd56b99a19bee907503fbb5602e2d89d82c529029afef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.14-alpine3.15` - linux; amd64

```console
$ docker pull docker@sha256:6f9f8a915e5a4a8308fcb3e2ba14cd6c7a2dbc11acd03b5a604d97781e84f4e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69395718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68061fb4db0fb111497ee4144c9b3f2cf421a0d450f1d1bc294d0fee31bf5670`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:14:46 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 23 Mar 2022 16:14:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:19:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:19:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:19:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:19:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:19:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:38 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236b952b9466b604bbc4e060a2667d7a7a335bee006fd5104c151dbdb4bf787`  
		Last Modified: Wed, 23 Mar 2022 16:15:39 GMT  
		Size: 2.0 MB (1969538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580f7437ec44a9dd3670ee6fd964ecb068808106d1bd8b961e7a568ef3ceb4f`  
		Last Modified: Wed, 23 Mar 2022 16:15:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0577d395ae504f47fad1c4d36855a3577354d4f0eca32daf7e0b13cf768c17`  
		Last Modified: Thu, 24 Mar 2022 05:20:29 GMT  
		Size: 64.6 MB (64611627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a33444f604b483769f304acdb1c976a4ea78d16943f3be3f9814e1a1e495f`  
		Last Modified: Thu, 24 Mar 2022 05:20:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8453fa1b01e46b0305c4d091304622803430cc8d0b3edb47c7be3a951e62e3`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e8e864d7d32b260f5ca60b2065242e7c51ccaa371f2cc9807d0c32b2ec06f`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.14-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:92392048de09154bffb7835256dc671934d598a3093d353494c89502784c8758
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63221233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5544e5647dd04b7224537d744d5e6fee9ade047a9fdfc200ccff6fe4749c30b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:05:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 24 Mar 2022 05:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:05:37 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:05:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:05:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:05:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:05:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:05:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:05:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:05:48 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f777e60e93e1e25280d855dd6b0c8e7e7d1508b2cbd43b9678cd18b2bab72084`  
		Last Modified: Thu, 24 Mar 2022 05:07:13 GMT  
		Size: 1.9 MB (1938915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1b0eef4b739aafe07d37f6f0fc1850ff0b6f61ab14400a1b6348cd2c8b7186`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4e629eede4a3f517e93a1764b365c41b7b2d2554b27f9d6fa6c2e37473901`  
		Last Modified: Thu, 24 Mar 2022 05:07:20 GMT  
		Size: 58.6 MB (58565771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7213dc5eb38c445dc0cffd227536ad4e5265f45307b743d11d8eb43fbdd43c26`  
		Last Modified: Thu, 24 Mar 2022 05:07:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57979a88be1287b9ce5ca410359f13c10dea1b5859e7e42d1bed86fb996f2d6e`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44bdde740192774f34636311a0dbd2b1081ec88c6a24c81b246635938b65c1`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.14-dind`

```console
$ docker pull docker@sha256:1452760def210c3cc517fb4d4cb7c7b978badc5568b150914e0b5956950c67b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.14-dind` - linux; amd64

```console
$ docker pull docker@sha256:47396a9df5ce04bcd749c54fafbfc4f5139e72044fff120e79727c9a21f755b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76135513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce144dca3a1244e5eae70e9ab5929cc77871e8ea153e89be56c1aed80f2249d3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:14:46 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 23 Mar 2022 16:14:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:19:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:19:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:19:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:19:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:19:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:38 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:19:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 24 Mar 2022 05:19:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:19:45 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 24 Mar 2022 05:19:46 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 24 Mar 2022 05:19:46 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:46 GMT
VOLUME [/var/lib/docker]
# Thu, 24 Mar 2022 05:19:46 GMT
EXPOSE 2375 2376
# Thu, 24 Mar 2022 05:19:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:46 GMT
CMD []
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236b952b9466b604bbc4e060a2667d7a7a335bee006fd5104c151dbdb4bf787`  
		Last Modified: Wed, 23 Mar 2022 16:15:39 GMT  
		Size: 2.0 MB (1969538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580f7437ec44a9dd3670ee6fd964ecb068808106d1bd8b961e7a568ef3ceb4f`  
		Last Modified: Wed, 23 Mar 2022 16:15:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0577d395ae504f47fad1c4d36855a3577354d4f0eca32daf7e0b13cf768c17`  
		Last Modified: Thu, 24 Mar 2022 05:20:29 GMT  
		Size: 64.6 MB (64611627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a33444f604b483769f304acdb1c976a4ea78d16943f3be3f9814e1a1e495f`  
		Last Modified: Thu, 24 Mar 2022 05:20:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8453fa1b01e46b0305c4d091304622803430cc8d0b3edb47c7be3a951e62e3`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e8e864d7d32b260f5ca60b2065242e7c51ccaa371f2cc9807d0c32b2ec06f`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a66f354bc1c7dbe0f8a4b91950340d2866bdbc96f2242a3bfa44d783c053f9c`  
		Last Modified: Thu, 24 Mar 2022 05:20:47 GMT  
		Size: 6.7 MB (6734776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6c10722ade4d16c23d283767216f390533cfb55769e6033eea8c7f4a8a4dc2`  
		Last Modified: Thu, 24 Mar 2022 05:20:47 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78397fa147a16e3ed2f3d8231cf9588472123760e352ca95983aeb96d333a43e`  
		Last Modified: Thu, 24 Mar 2022 05:20:46 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa763b179fa70cb6a2ad1b6bf60c036a10f3b92e0372b67ed05efdf265e1fea`  
		Last Modified: Thu, 24 Mar 2022 05:20:46 GMT  
		Size: 2.7 KB (2745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.14-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:75505cc1bcd04f36672b8029910f09c4cc4a71f9d593707926df979f338a6d63
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69841807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a57d0f0cedd6ab4481d9e1ac90434454fe44b1ca846efc6dba36106458d732`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:05:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 24 Mar 2022 05:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:05:37 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:05:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:05:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:05:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:05:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:05:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:05:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:05:48 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:05:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 24 Mar 2022 05:05:58 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:05:59 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 24 Mar 2022 05:06:00 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 24 Mar 2022 05:06:02 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:06:02 GMT
VOLUME [/var/lib/docker]
# Thu, 24 Mar 2022 05:06:03 GMT
EXPOSE 2375 2376
# Thu, 24 Mar 2022 05:06:04 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 24 Mar 2022 05:06:05 GMT
CMD []
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f777e60e93e1e25280d855dd6b0c8e7e7d1508b2cbd43b9678cd18b2bab72084`  
		Last Modified: Thu, 24 Mar 2022 05:07:13 GMT  
		Size: 1.9 MB (1938915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1b0eef4b739aafe07d37f6f0fc1850ff0b6f61ab14400a1b6348cd2c8b7186`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4e629eede4a3f517e93a1764b365c41b7b2d2554b27f9d6fa6c2e37473901`  
		Last Modified: Thu, 24 Mar 2022 05:07:20 GMT  
		Size: 58.6 MB (58565771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7213dc5eb38c445dc0cffd227536ad4e5265f45307b743d11d8eb43fbdd43c26`  
		Last Modified: Thu, 24 Mar 2022 05:07:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57979a88be1287b9ce5ca410359f13c10dea1b5859e7e42d1bed86fb996f2d6e`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44bdde740192774f34636311a0dbd2b1081ec88c6a24c81b246635938b65c1`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc6a23bd8ea7facb45f466a82b87c2136b7f86ec714dab0f1466e6ee53fb65d`  
		Last Modified: Thu, 24 Mar 2022 05:07:42 GMT  
		Size: 6.6 MB (6615580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef7b6dc8191b8b5cc2c67b7b4228b517f4d6341cd3f3c8d3de3565c9f9c8b38`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0986d23cef445052b13281b734555dd4fba26dde5400b38a211f8ba542aa0eb4`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7fb89298925d38bdc861bda494f566d964eab170cf307814a1925a59123965`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.14-dind-alpine3.15`

```console
$ docker pull docker@sha256:1452760def210c3cc517fb4d4cb7c7b978badc5568b150914e0b5956950c67b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.14-dind-alpine3.15` - linux; amd64

```console
$ docker pull docker@sha256:47396a9df5ce04bcd749c54fafbfc4f5139e72044fff120e79727c9a21f755b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76135513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce144dca3a1244e5eae70e9ab5929cc77871e8ea153e89be56c1aed80f2249d3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:14:46 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 23 Mar 2022 16:14:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:19:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:19:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:19:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:19:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:19:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:38 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:19:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 24 Mar 2022 05:19:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:19:45 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 24 Mar 2022 05:19:46 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 24 Mar 2022 05:19:46 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:46 GMT
VOLUME [/var/lib/docker]
# Thu, 24 Mar 2022 05:19:46 GMT
EXPOSE 2375 2376
# Thu, 24 Mar 2022 05:19:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:46 GMT
CMD []
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236b952b9466b604bbc4e060a2667d7a7a335bee006fd5104c151dbdb4bf787`  
		Last Modified: Wed, 23 Mar 2022 16:15:39 GMT  
		Size: 2.0 MB (1969538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580f7437ec44a9dd3670ee6fd964ecb068808106d1bd8b961e7a568ef3ceb4f`  
		Last Modified: Wed, 23 Mar 2022 16:15:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0577d395ae504f47fad1c4d36855a3577354d4f0eca32daf7e0b13cf768c17`  
		Last Modified: Thu, 24 Mar 2022 05:20:29 GMT  
		Size: 64.6 MB (64611627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a33444f604b483769f304acdb1c976a4ea78d16943f3be3f9814e1a1e495f`  
		Last Modified: Thu, 24 Mar 2022 05:20:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8453fa1b01e46b0305c4d091304622803430cc8d0b3edb47c7be3a951e62e3`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e8e864d7d32b260f5ca60b2065242e7c51ccaa371f2cc9807d0c32b2ec06f`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a66f354bc1c7dbe0f8a4b91950340d2866bdbc96f2242a3bfa44d783c053f9c`  
		Last Modified: Thu, 24 Mar 2022 05:20:47 GMT  
		Size: 6.7 MB (6734776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6c10722ade4d16c23d283767216f390533cfb55769e6033eea8c7f4a8a4dc2`  
		Last Modified: Thu, 24 Mar 2022 05:20:47 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78397fa147a16e3ed2f3d8231cf9588472123760e352ca95983aeb96d333a43e`  
		Last Modified: Thu, 24 Mar 2022 05:20:46 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa763b179fa70cb6a2ad1b6bf60c036a10f3b92e0372b67ed05efdf265e1fea`  
		Last Modified: Thu, 24 Mar 2022 05:20:46 GMT  
		Size: 2.7 KB (2745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.14-dind-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:75505cc1bcd04f36672b8029910f09c4cc4a71f9d593707926df979f338a6d63
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69841807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a57d0f0cedd6ab4481d9e1ac90434454fe44b1ca846efc6dba36106458d732`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:05:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 24 Mar 2022 05:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:05:37 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:05:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:05:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:05:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:05:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:05:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:05:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:05:48 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:05:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 24 Mar 2022 05:05:58 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:05:59 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 24 Mar 2022 05:06:00 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 24 Mar 2022 05:06:02 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:06:02 GMT
VOLUME [/var/lib/docker]
# Thu, 24 Mar 2022 05:06:03 GMT
EXPOSE 2375 2376
# Thu, 24 Mar 2022 05:06:04 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 24 Mar 2022 05:06:05 GMT
CMD []
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f777e60e93e1e25280d855dd6b0c8e7e7d1508b2cbd43b9678cd18b2bab72084`  
		Last Modified: Thu, 24 Mar 2022 05:07:13 GMT  
		Size: 1.9 MB (1938915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1b0eef4b739aafe07d37f6f0fc1850ff0b6f61ab14400a1b6348cd2c8b7186`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4e629eede4a3f517e93a1764b365c41b7b2d2554b27f9d6fa6c2e37473901`  
		Last Modified: Thu, 24 Mar 2022 05:07:20 GMT  
		Size: 58.6 MB (58565771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7213dc5eb38c445dc0cffd227536ad4e5265f45307b743d11d8eb43fbdd43c26`  
		Last Modified: Thu, 24 Mar 2022 05:07:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57979a88be1287b9ce5ca410359f13c10dea1b5859e7e42d1bed86fb996f2d6e`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44bdde740192774f34636311a0dbd2b1081ec88c6a24c81b246635938b65c1`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc6a23bd8ea7facb45f466a82b87c2136b7f86ec714dab0f1466e6ee53fb65d`  
		Last Modified: Thu, 24 Mar 2022 05:07:42 GMT  
		Size: 6.6 MB (6615580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef7b6dc8191b8b5cc2c67b7b4228b517f4d6341cd3f3c8d3de3565c9f9c8b38`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0986d23cef445052b13281b734555dd4fba26dde5400b38a211f8ba542aa0eb4`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7fb89298925d38bdc861bda494f566d964eab170cf307814a1925a59123965`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.14-dind-rootless`

```console
$ docker pull docker@sha256:d836fb75037a409e5c7eaa2d86235b12c03f79cafca8acb2680f2f07397d7271
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.14-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:4e4e5426e9189d088d01d49d5f12495257c1b6f833966205cd34375f9c83fe76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 MB (96431045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:901a49bfc43b7f98ffcdd1aa26811571d1eb434164d9c35ba0dd3ec8e1fd7113`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:14:46 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 23 Mar 2022 16:14:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:19:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:19:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:19:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:19:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:19:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:38 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:19:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 24 Mar 2022 05:19:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:19:45 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 24 Mar 2022 05:19:46 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 24 Mar 2022 05:19:46 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:46 GMT
VOLUME [/var/lib/docker]
# Thu, 24 Mar 2022 05:19:46 GMT
EXPOSE 2375 2376
# Thu, 24 Mar 2022 05:19:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:46 GMT
CMD []
# Thu, 24 Mar 2022 05:19:50 GMT
RUN apk add --no-cache iproute2
# Thu, 24 Mar 2022 05:19:50 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 24 Mar 2022 05:19:51 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:19:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 24 Mar 2022 05:19:54 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 24 Mar 2022 05:19:54 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 24 Mar 2022 05:19:54 GMT
USER rootless
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236b952b9466b604bbc4e060a2667d7a7a335bee006fd5104c151dbdb4bf787`  
		Last Modified: Wed, 23 Mar 2022 16:15:39 GMT  
		Size: 2.0 MB (1969538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580f7437ec44a9dd3670ee6fd964ecb068808106d1bd8b961e7a568ef3ceb4f`  
		Last Modified: Wed, 23 Mar 2022 16:15:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0577d395ae504f47fad1c4d36855a3577354d4f0eca32daf7e0b13cf768c17`  
		Last Modified: Thu, 24 Mar 2022 05:20:29 GMT  
		Size: 64.6 MB (64611627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a33444f604b483769f304acdb1c976a4ea78d16943f3be3f9814e1a1e495f`  
		Last Modified: Thu, 24 Mar 2022 05:20:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8453fa1b01e46b0305c4d091304622803430cc8d0b3edb47c7be3a951e62e3`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e8e864d7d32b260f5ca60b2065242e7c51ccaa371f2cc9807d0c32b2ec06f`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a66f354bc1c7dbe0f8a4b91950340d2866bdbc96f2242a3bfa44d783c053f9c`  
		Last Modified: Thu, 24 Mar 2022 05:20:47 GMT  
		Size: 6.7 MB (6734776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6c10722ade4d16c23d283767216f390533cfb55769e6033eea8c7f4a8a4dc2`  
		Last Modified: Thu, 24 Mar 2022 05:20:47 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78397fa147a16e3ed2f3d8231cf9588472123760e352ca95983aeb96d333a43e`  
		Last Modified: Thu, 24 Mar 2022 05:20:46 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa763b179fa70cb6a2ad1b6bf60c036a10f3b92e0372b67ed05efdf265e1fea`  
		Last Modified: Thu, 24 Mar 2022 05:20:46 GMT  
		Size: 2.7 KB (2745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6085587cb5f72c79568b29cd55f4c3913866e9ed6397eaa76661ce55d266be`  
		Last Modified: Thu, 24 Mar 2022 05:21:06 GMT  
		Size: 1.2 MB (1161988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a25e47e24f1be9958fc51661a544e64751645608e5cedff2dda9dbc3f4e39c`  
		Last Modified: Thu, 24 Mar 2022 05:21:06 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05797a2b73a664a83ba4a1baf3ec188f150e43ced3f5c9b0d9b695f614e82e31`  
		Last Modified: Thu, 24 Mar 2022 05:21:06 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a221d919a583960b7e36174c14532d2a479dbff4a227c548323d06c4b423ab`  
		Last Modified: Thu, 24 Mar 2022 05:21:09 GMT  
		Size: 19.1 MB (19131826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daedd33adc3be410c282f07f922a10bbbfa3f6b0564eb37b71b60de416300b2a`  
		Last Modified: Thu, 24 Mar 2022 05:21:06 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.14-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:df7d7108fde667390444bf3b4fe7cb30ffc8158d555bc05aa7a5f43bd52fcf08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92132624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed85851cb7cd69079f6a55018697c1ac3a6d1c598a7e6c422bfed707a3608503`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:05:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 24 Mar 2022 05:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:05:37 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:05:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:05:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:05:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:05:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:05:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:05:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:05:48 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:05:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 24 Mar 2022 05:05:58 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:05:59 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 24 Mar 2022 05:06:00 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 24 Mar 2022 05:06:02 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:06:02 GMT
VOLUME [/var/lib/docker]
# Thu, 24 Mar 2022 05:06:03 GMT
EXPOSE 2375 2376
# Thu, 24 Mar 2022 05:06:04 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 24 Mar 2022 05:06:05 GMT
CMD []
# Thu, 24 Mar 2022 05:06:13 GMT
RUN apk add --no-cache iproute2
# Thu, 24 Mar 2022 05:06:14 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 24 Mar 2022 05:06:15 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:06:18 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 24 Mar 2022 05:06:19 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 24 Mar 2022 05:06:20 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 24 Mar 2022 05:06:21 GMT
USER rootless
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f777e60e93e1e25280d855dd6b0c8e7e7d1508b2cbd43b9678cd18b2bab72084`  
		Last Modified: Thu, 24 Mar 2022 05:07:13 GMT  
		Size: 1.9 MB (1938915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1b0eef4b739aafe07d37f6f0fc1850ff0b6f61ab14400a1b6348cd2c8b7186`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4e629eede4a3f517e93a1764b365c41b7b2d2554b27f9d6fa6c2e37473901`  
		Last Modified: Thu, 24 Mar 2022 05:07:20 GMT  
		Size: 58.6 MB (58565771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7213dc5eb38c445dc0cffd227536ad4e5265f45307b743d11d8eb43fbdd43c26`  
		Last Modified: Thu, 24 Mar 2022 05:07:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57979a88be1287b9ce5ca410359f13c10dea1b5859e7e42d1bed86fb996f2d6e`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44bdde740192774f34636311a0dbd2b1081ec88c6a24c81b246635938b65c1`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc6a23bd8ea7facb45f466a82b87c2136b7f86ec714dab0f1466e6ee53fb65d`  
		Last Modified: Thu, 24 Mar 2022 05:07:42 GMT  
		Size: 6.6 MB (6615580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef7b6dc8191b8b5cc2c67b7b4228b517f4d6341cd3f3c8d3de3565c9f9c8b38`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0986d23cef445052b13281b734555dd4fba26dde5400b38a211f8ba542aa0eb4`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7fb89298925d38bdc861bda494f566d964eab170cf307814a1925a59123965`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2a88bdadcae21855d08188cd8b67037b35b213029f2cffdd90dd25ba0c6386`  
		Last Modified: Thu, 24 Mar 2022 05:08:03 GMT  
		Size: 1.2 MB (1177944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0815bff1c961ac2d8113264775046dba30417f109f54ba09f493192934fd0940`  
		Last Modified: Thu, 24 Mar 2022 05:08:03 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399d118cae203620b47422a9705be6c340af1e0db7fef87338deff30269fb404`  
		Last Modified: Thu, 24 Mar 2022 05:08:03 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d745b7e9d65f0a9afee27aa8bacf9577cbcec66494bc9f115621f4f85366491`  
		Last Modified: Thu, 24 Mar 2022 05:08:06 GMT  
		Size: 21.1 MB (21111250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23af1a6c11dc14339ad8b7c79cf3ce581990a6e4193573afde6892824a7d045c`  
		Last Modified: Thu, 24 Mar 2022 05:08:03 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.14-git`

```console
$ docker pull docker@sha256:5b8f51320fb14ff3fbc45001d6477a8edc4155128fcd5dd4b7139294336e91fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.14-git` - linux; amd64

```console
$ docker pull docker@sha256:3728219f8cc46f4f397b330577000ca639d8324aa5a1556d0e6a5cf738ebe0ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76219858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b79097ab0874839ce4ef81b16354be702b88d942e0232d86af2acdc33e22b9bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:14:46 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 23 Mar 2022 16:14:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:19:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:19:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:19:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:19:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:19:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:38 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:19:57 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236b952b9466b604bbc4e060a2667d7a7a335bee006fd5104c151dbdb4bf787`  
		Last Modified: Wed, 23 Mar 2022 16:15:39 GMT  
		Size: 2.0 MB (1969538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580f7437ec44a9dd3670ee6fd964ecb068808106d1bd8b961e7a568ef3ceb4f`  
		Last Modified: Wed, 23 Mar 2022 16:15:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0577d395ae504f47fad1c4d36855a3577354d4f0eca32daf7e0b13cf768c17`  
		Last Modified: Thu, 24 Mar 2022 05:20:29 GMT  
		Size: 64.6 MB (64611627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a33444f604b483769f304acdb1c976a4ea78d16943f3be3f9814e1a1e495f`  
		Last Modified: Thu, 24 Mar 2022 05:20:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8453fa1b01e46b0305c4d091304622803430cc8d0b3edb47c7be3a951e62e3`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e8e864d7d32b260f5ca60b2065242e7c51ccaa371f2cc9807d0c32b2ec06f`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8260489be308ed8266d2c832c405abe7c01809d417bf17b473ec0f0f37339134`  
		Last Modified: Thu, 24 Mar 2022 05:21:32 GMT  
		Size: 6.8 MB (6824140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.14-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:7a2baddd024a7811ef67203d77de9ab3829ddca714ca6fe11f2ed2b3572fb5f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70154288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb42c0db861bb97af997256dc9ff427b43b0668bc7689aada6aa99ba4937b84e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:05:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 24 Mar 2022 05:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:05:37 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:05:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:05:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:05:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:05:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:05:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:05:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:05:48 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:06:28 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f777e60e93e1e25280d855dd6b0c8e7e7d1508b2cbd43b9678cd18b2bab72084`  
		Last Modified: Thu, 24 Mar 2022 05:07:13 GMT  
		Size: 1.9 MB (1938915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1b0eef4b739aafe07d37f6f0fc1850ff0b6f61ab14400a1b6348cd2c8b7186`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4e629eede4a3f517e93a1764b365c41b7b2d2554b27f9d6fa6c2e37473901`  
		Last Modified: Thu, 24 Mar 2022 05:07:20 GMT  
		Size: 58.6 MB (58565771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7213dc5eb38c445dc0cffd227536ad4e5265f45307b743d11d8eb43fbdd43c26`  
		Last Modified: Thu, 24 Mar 2022 05:07:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57979a88be1287b9ce5ca410359f13c10dea1b5859e7e42d1bed86fb996f2d6e`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44bdde740192774f34636311a0dbd2b1081ec88c6a24c81b246635938b65c1`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a06e853d235302bea036f40c1af6580b1f35dccf8df3f8610cab630655e58ca`  
		Last Modified: Thu, 24 Mar 2022 05:08:26 GMT  
		Size: 6.9 MB (6933055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.14-windowsservercore`

```console
$ docker pull docker@sha256:e975b7c270f2a35f16d48b91e2ab5f0eff84a690da1fcedab97e7157d0b3a5ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.587; amd64
	-	windows version 10.0.17763.2686; amd64

### `docker:20.10.14-windowsservercore` - windows version 10.0.20348.587; amd64

```console
$ docker pull docker@sha256:aefae8d2bf575204b17f88589c7741c350281048d96844f9fd3316a80ec2940e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2275653601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:723b6471c336c441aa997a1c5d0672ef1de87fe45687edb769c52bd0edce4e81`
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
# Thu, 24 Mar 2022 05:15:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:15:30 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.14.zip
# Thu, 24 Mar 2022 05:16:11 GMT
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
	-	`sha256:0181d328453c16ef4bf5dfa86a118c96a8325d7a3e58637e504f5425c5ea7ae2`  
		Last Modified: Thu, 24 Mar 2022 05:18:23 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e48a2566f0d50346970f29a77bd1cbfde2d33a34fc25d9227a8900f494b136a`  
		Last Modified: Thu, 24 Mar 2022 05:18:24 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cd9d001a2232e2f5406882e91758565fec1809573168d4e31cafa909ea5d4f`  
		Last Modified: Thu, 24 Mar 2022 05:18:35 GMT  
		Size: 53.8 MB (53804106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.14-windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull docker@sha256:034598e549b6c0f2bb1ff47cbb638cb9785ab1456144eb4c0da198e075e70a9d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2769426444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2374652d04922dbe838fbdac11dc741534c504b1213d1110bcf7ab3ce0075be`
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
# Thu, 24 Mar 2022 05:16:22 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:16:23 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.14.zip
# Thu, 24 Mar 2022 05:17:56 GMT
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
	-	`sha256:3a37839ee100e0b4b77379ec17ab118f0b377c9d7f73de9b4fdfce26e5910d07`  
		Last Modified: Thu, 24 Mar 2022 05:18:49 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a35b5cdb293ca7295865a746b962b396382293a16a843862f866ad76d49b7d`  
		Last Modified: Thu, 24 Mar 2022 05:18:49 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791bcb5d614f3fbb4d6ff0b29ce1877c53e05d3b8536fe0fa4b549f20c0b6730`  
		Last Modified: Thu, 24 Mar 2022 05:19:47 GMT  
		Size: 53.6 MB (53615927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.14-windowsservercore-1809`

```console
$ docker pull docker@sha256:6e21edf269ee8beed4808bae91f5cc840ad2a042a19a6eb6de13c97e3053906b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `docker:20.10.14-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull docker@sha256:034598e549b6c0f2bb1ff47cbb638cb9785ab1456144eb4c0da198e075e70a9d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2769426444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2374652d04922dbe838fbdac11dc741534c504b1213d1110bcf7ab3ce0075be`
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
# Thu, 24 Mar 2022 05:16:22 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:16:23 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.14.zip
# Thu, 24 Mar 2022 05:17:56 GMT
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
	-	`sha256:3a37839ee100e0b4b77379ec17ab118f0b377c9d7f73de9b4fdfce26e5910d07`  
		Last Modified: Thu, 24 Mar 2022 05:18:49 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a35b5cdb293ca7295865a746b962b396382293a16a843862f866ad76d49b7d`  
		Last Modified: Thu, 24 Mar 2022 05:18:49 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791bcb5d614f3fbb4d6ff0b29ce1877c53e05d3b8536fe0fa4b549f20c0b6730`  
		Last Modified: Thu, 24 Mar 2022 05:19:47 GMT  
		Size: 53.6 MB (53615927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.14-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:8520b3fc85f5fe47604cbba4353f8b2feda30bcf041e26848bd6d812173f4444
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.587; amd64

### `docker:20.10.14-windowsservercore-ltsc2022` - windows version 10.0.20348.587; amd64

```console
$ docker pull docker@sha256:aefae8d2bf575204b17f88589c7741c350281048d96844f9fd3316a80ec2940e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2275653601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:723b6471c336c441aa997a1c5d0672ef1de87fe45687edb769c52bd0edce4e81`
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
# Thu, 24 Mar 2022 05:15:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:15:30 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.14.zip
# Thu, 24 Mar 2022 05:16:11 GMT
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
	-	`sha256:0181d328453c16ef4bf5dfa86a118c96a8325d7a3e58637e504f5425c5ea7ae2`  
		Last Modified: Thu, 24 Mar 2022 05:18:23 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e48a2566f0d50346970f29a77bd1cbfde2d33a34fc25d9227a8900f494b136a`  
		Last Modified: Thu, 24 Mar 2022 05:18:24 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cd9d001a2232e2f5406882e91758565fec1809573168d4e31cafa909ea5d4f`  
		Last Modified: Thu, 24 Mar 2022 05:18:35 GMT  
		Size: 53.8 MB (53804106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:1452760def210c3cc517fb4d4cb7c7b978badc5568b150914e0b5956950c67b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:47396a9df5ce04bcd749c54fafbfc4f5139e72044fff120e79727c9a21f755b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76135513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce144dca3a1244e5eae70e9ab5929cc77871e8ea153e89be56c1aed80f2249d3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:14:46 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 23 Mar 2022 16:14:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:19:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:19:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:19:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:19:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:19:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:38 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:19:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 24 Mar 2022 05:19:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:19:45 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 24 Mar 2022 05:19:46 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 24 Mar 2022 05:19:46 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:46 GMT
VOLUME [/var/lib/docker]
# Thu, 24 Mar 2022 05:19:46 GMT
EXPOSE 2375 2376
# Thu, 24 Mar 2022 05:19:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:46 GMT
CMD []
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236b952b9466b604bbc4e060a2667d7a7a335bee006fd5104c151dbdb4bf787`  
		Last Modified: Wed, 23 Mar 2022 16:15:39 GMT  
		Size: 2.0 MB (1969538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580f7437ec44a9dd3670ee6fd964ecb068808106d1bd8b961e7a568ef3ceb4f`  
		Last Modified: Wed, 23 Mar 2022 16:15:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0577d395ae504f47fad1c4d36855a3577354d4f0eca32daf7e0b13cf768c17`  
		Last Modified: Thu, 24 Mar 2022 05:20:29 GMT  
		Size: 64.6 MB (64611627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a33444f604b483769f304acdb1c976a4ea78d16943f3be3f9814e1a1e495f`  
		Last Modified: Thu, 24 Mar 2022 05:20:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8453fa1b01e46b0305c4d091304622803430cc8d0b3edb47c7be3a951e62e3`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e8e864d7d32b260f5ca60b2065242e7c51ccaa371f2cc9807d0c32b2ec06f`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a66f354bc1c7dbe0f8a4b91950340d2866bdbc96f2242a3bfa44d783c053f9c`  
		Last Modified: Thu, 24 Mar 2022 05:20:47 GMT  
		Size: 6.7 MB (6734776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6c10722ade4d16c23d283767216f390533cfb55769e6033eea8c7f4a8a4dc2`  
		Last Modified: Thu, 24 Mar 2022 05:20:47 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78397fa147a16e3ed2f3d8231cf9588472123760e352ca95983aeb96d333a43e`  
		Last Modified: Thu, 24 Mar 2022 05:20:46 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa763b179fa70cb6a2ad1b6bf60c036a10f3b92e0372b67ed05efdf265e1fea`  
		Last Modified: Thu, 24 Mar 2022 05:20:46 GMT  
		Size: 2.7 KB (2745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:75505cc1bcd04f36672b8029910f09c4cc4a71f9d593707926df979f338a6d63
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69841807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a57d0f0cedd6ab4481d9e1ac90434454fe44b1ca846efc6dba36106458d732`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:05:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 24 Mar 2022 05:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:05:37 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:05:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:05:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:05:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:05:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:05:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:05:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:05:48 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:05:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 24 Mar 2022 05:05:58 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:05:59 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 24 Mar 2022 05:06:00 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 24 Mar 2022 05:06:02 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:06:02 GMT
VOLUME [/var/lib/docker]
# Thu, 24 Mar 2022 05:06:03 GMT
EXPOSE 2375 2376
# Thu, 24 Mar 2022 05:06:04 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 24 Mar 2022 05:06:05 GMT
CMD []
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f777e60e93e1e25280d855dd6b0c8e7e7d1508b2cbd43b9678cd18b2bab72084`  
		Last Modified: Thu, 24 Mar 2022 05:07:13 GMT  
		Size: 1.9 MB (1938915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1b0eef4b739aafe07d37f6f0fc1850ff0b6f61ab14400a1b6348cd2c8b7186`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4e629eede4a3f517e93a1764b365c41b7b2d2554b27f9d6fa6c2e37473901`  
		Last Modified: Thu, 24 Mar 2022 05:07:20 GMT  
		Size: 58.6 MB (58565771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7213dc5eb38c445dc0cffd227536ad4e5265f45307b743d11d8eb43fbdd43c26`  
		Last Modified: Thu, 24 Mar 2022 05:07:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57979a88be1287b9ce5ca410359f13c10dea1b5859e7e42d1bed86fb996f2d6e`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44bdde740192774f34636311a0dbd2b1081ec88c6a24c81b246635938b65c1`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc6a23bd8ea7facb45f466a82b87c2136b7f86ec714dab0f1466e6ee53fb65d`  
		Last Modified: Thu, 24 Mar 2022 05:07:42 GMT  
		Size: 6.6 MB (6615580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef7b6dc8191b8b5cc2c67b7b4228b517f4d6341cd3f3c8d3de3565c9f9c8b38`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0986d23cef445052b13281b734555dd4fba26dde5400b38a211f8ba542aa0eb4`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7fb89298925d38bdc861bda494f566d964eab170cf307814a1925a59123965`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:d836fb75037a409e5c7eaa2d86235b12c03f79cafca8acb2680f2f07397d7271
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:4e4e5426e9189d088d01d49d5f12495257c1b6f833966205cd34375f9c83fe76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 MB (96431045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:901a49bfc43b7f98ffcdd1aa26811571d1eb434164d9c35ba0dd3ec8e1fd7113`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:14:46 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 23 Mar 2022 16:14:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:19:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:19:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:19:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:19:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:19:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:38 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:19:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 24 Mar 2022 05:19:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:19:45 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 24 Mar 2022 05:19:46 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 24 Mar 2022 05:19:46 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:46 GMT
VOLUME [/var/lib/docker]
# Thu, 24 Mar 2022 05:19:46 GMT
EXPOSE 2375 2376
# Thu, 24 Mar 2022 05:19:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:46 GMT
CMD []
# Thu, 24 Mar 2022 05:19:50 GMT
RUN apk add --no-cache iproute2
# Thu, 24 Mar 2022 05:19:50 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 24 Mar 2022 05:19:51 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:19:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 24 Mar 2022 05:19:54 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 24 Mar 2022 05:19:54 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 24 Mar 2022 05:19:54 GMT
USER rootless
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236b952b9466b604bbc4e060a2667d7a7a335bee006fd5104c151dbdb4bf787`  
		Last Modified: Wed, 23 Mar 2022 16:15:39 GMT  
		Size: 2.0 MB (1969538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580f7437ec44a9dd3670ee6fd964ecb068808106d1bd8b961e7a568ef3ceb4f`  
		Last Modified: Wed, 23 Mar 2022 16:15:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0577d395ae504f47fad1c4d36855a3577354d4f0eca32daf7e0b13cf768c17`  
		Last Modified: Thu, 24 Mar 2022 05:20:29 GMT  
		Size: 64.6 MB (64611627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a33444f604b483769f304acdb1c976a4ea78d16943f3be3f9814e1a1e495f`  
		Last Modified: Thu, 24 Mar 2022 05:20:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8453fa1b01e46b0305c4d091304622803430cc8d0b3edb47c7be3a951e62e3`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e8e864d7d32b260f5ca60b2065242e7c51ccaa371f2cc9807d0c32b2ec06f`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a66f354bc1c7dbe0f8a4b91950340d2866bdbc96f2242a3bfa44d783c053f9c`  
		Last Modified: Thu, 24 Mar 2022 05:20:47 GMT  
		Size: 6.7 MB (6734776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6c10722ade4d16c23d283767216f390533cfb55769e6033eea8c7f4a8a4dc2`  
		Last Modified: Thu, 24 Mar 2022 05:20:47 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78397fa147a16e3ed2f3d8231cf9588472123760e352ca95983aeb96d333a43e`  
		Last Modified: Thu, 24 Mar 2022 05:20:46 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa763b179fa70cb6a2ad1b6bf60c036a10f3b92e0372b67ed05efdf265e1fea`  
		Last Modified: Thu, 24 Mar 2022 05:20:46 GMT  
		Size: 2.7 KB (2745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6085587cb5f72c79568b29cd55f4c3913866e9ed6397eaa76661ce55d266be`  
		Last Modified: Thu, 24 Mar 2022 05:21:06 GMT  
		Size: 1.2 MB (1161988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a25e47e24f1be9958fc51661a544e64751645608e5cedff2dda9dbc3f4e39c`  
		Last Modified: Thu, 24 Mar 2022 05:21:06 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05797a2b73a664a83ba4a1baf3ec188f150e43ced3f5c9b0d9b695f614e82e31`  
		Last Modified: Thu, 24 Mar 2022 05:21:06 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a221d919a583960b7e36174c14532d2a479dbff4a227c548323d06c4b423ab`  
		Last Modified: Thu, 24 Mar 2022 05:21:09 GMT  
		Size: 19.1 MB (19131826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daedd33adc3be410c282f07f922a10bbbfa3f6b0564eb37b71b60de416300b2a`  
		Last Modified: Thu, 24 Mar 2022 05:21:06 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:df7d7108fde667390444bf3b4fe7cb30ffc8158d555bc05aa7a5f43bd52fcf08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92132624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed85851cb7cd69079f6a55018697c1ac3a6d1c598a7e6c422bfed707a3608503`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:05:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 24 Mar 2022 05:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:05:37 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:05:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:05:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:05:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:05:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:05:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:05:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:05:48 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:05:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 24 Mar 2022 05:05:58 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:05:59 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 24 Mar 2022 05:06:00 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 24 Mar 2022 05:06:02 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:06:02 GMT
VOLUME [/var/lib/docker]
# Thu, 24 Mar 2022 05:06:03 GMT
EXPOSE 2375 2376
# Thu, 24 Mar 2022 05:06:04 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 24 Mar 2022 05:06:05 GMT
CMD []
# Thu, 24 Mar 2022 05:06:13 GMT
RUN apk add --no-cache iproute2
# Thu, 24 Mar 2022 05:06:14 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 24 Mar 2022 05:06:15 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:06:18 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 24 Mar 2022 05:06:19 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 24 Mar 2022 05:06:20 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 24 Mar 2022 05:06:21 GMT
USER rootless
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f777e60e93e1e25280d855dd6b0c8e7e7d1508b2cbd43b9678cd18b2bab72084`  
		Last Modified: Thu, 24 Mar 2022 05:07:13 GMT  
		Size: 1.9 MB (1938915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1b0eef4b739aafe07d37f6f0fc1850ff0b6f61ab14400a1b6348cd2c8b7186`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4e629eede4a3f517e93a1764b365c41b7b2d2554b27f9d6fa6c2e37473901`  
		Last Modified: Thu, 24 Mar 2022 05:07:20 GMT  
		Size: 58.6 MB (58565771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7213dc5eb38c445dc0cffd227536ad4e5265f45307b743d11d8eb43fbdd43c26`  
		Last Modified: Thu, 24 Mar 2022 05:07:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57979a88be1287b9ce5ca410359f13c10dea1b5859e7e42d1bed86fb996f2d6e`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44bdde740192774f34636311a0dbd2b1081ec88c6a24c81b246635938b65c1`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc6a23bd8ea7facb45f466a82b87c2136b7f86ec714dab0f1466e6ee53fb65d`  
		Last Modified: Thu, 24 Mar 2022 05:07:42 GMT  
		Size: 6.6 MB (6615580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef7b6dc8191b8b5cc2c67b7b4228b517f4d6341cd3f3c8d3de3565c9f9c8b38`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0986d23cef445052b13281b734555dd4fba26dde5400b38a211f8ba542aa0eb4`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7fb89298925d38bdc861bda494f566d964eab170cf307814a1925a59123965`  
		Last Modified: Thu, 24 Mar 2022 05:07:41 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2a88bdadcae21855d08188cd8b67037b35b213029f2cffdd90dd25ba0c6386`  
		Last Modified: Thu, 24 Mar 2022 05:08:03 GMT  
		Size: 1.2 MB (1177944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0815bff1c961ac2d8113264775046dba30417f109f54ba09f493192934fd0940`  
		Last Modified: Thu, 24 Mar 2022 05:08:03 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399d118cae203620b47422a9705be6c340af1e0db7fef87338deff30269fb404`  
		Last Modified: Thu, 24 Mar 2022 05:08:03 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d745b7e9d65f0a9afee27aa8bacf9577cbcec66494bc9f115621f4f85366491`  
		Last Modified: Thu, 24 Mar 2022 05:08:06 GMT  
		Size: 21.1 MB (21111250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23af1a6c11dc14339ad8b7c79cf3ce581990a6e4193573afde6892824a7d045c`  
		Last Modified: Thu, 24 Mar 2022 05:08:03 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:5b8f51320fb14ff3fbc45001d6477a8edc4155128fcd5dd4b7139294336e91fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:3728219f8cc46f4f397b330577000ca639d8324aa5a1556d0e6a5cf738ebe0ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76219858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b79097ab0874839ce4ef81b16354be702b88d942e0232d86af2acdc33e22b9bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:14:46 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 23 Mar 2022 16:14:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:19:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:19:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:19:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:19:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:19:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:38 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:19:57 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236b952b9466b604bbc4e060a2667d7a7a335bee006fd5104c151dbdb4bf787`  
		Last Modified: Wed, 23 Mar 2022 16:15:39 GMT  
		Size: 2.0 MB (1969538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580f7437ec44a9dd3670ee6fd964ecb068808106d1bd8b961e7a568ef3ceb4f`  
		Last Modified: Wed, 23 Mar 2022 16:15:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0577d395ae504f47fad1c4d36855a3577354d4f0eca32daf7e0b13cf768c17`  
		Last Modified: Thu, 24 Mar 2022 05:20:29 GMT  
		Size: 64.6 MB (64611627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a33444f604b483769f304acdb1c976a4ea78d16943f3be3f9814e1a1e495f`  
		Last Modified: Thu, 24 Mar 2022 05:20:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8453fa1b01e46b0305c4d091304622803430cc8d0b3edb47c7be3a951e62e3`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e8e864d7d32b260f5ca60b2065242e7c51ccaa371f2cc9807d0c32b2ec06f`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8260489be308ed8266d2c832c405abe7c01809d417bf17b473ec0f0f37339134`  
		Last Modified: Thu, 24 Mar 2022 05:21:32 GMT  
		Size: 6.8 MB (6824140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:7a2baddd024a7811ef67203d77de9ab3829ddca714ca6fe11f2ed2b3572fb5f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70154288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb42c0db861bb97af997256dc9ff427b43b0668bc7689aada6aa99ba4937b84e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:05:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 24 Mar 2022 05:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:05:37 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:05:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:05:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:05:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:05:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:05:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:05:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:05:48 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:06:28 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f777e60e93e1e25280d855dd6b0c8e7e7d1508b2cbd43b9678cd18b2bab72084`  
		Last Modified: Thu, 24 Mar 2022 05:07:13 GMT  
		Size: 1.9 MB (1938915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1b0eef4b739aafe07d37f6f0fc1850ff0b6f61ab14400a1b6348cd2c8b7186`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4e629eede4a3f517e93a1764b365c41b7b2d2554b27f9d6fa6c2e37473901`  
		Last Modified: Thu, 24 Mar 2022 05:07:20 GMT  
		Size: 58.6 MB (58565771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7213dc5eb38c445dc0cffd227536ad4e5265f45307b743d11d8eb43fbdd43c26`  
		Last Modified: Thu, 24 Mar 2022 05:07:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57979a88be1287b9ce5ca410359f13c10dea1b5859e7e42d1bed86fb996f2d6e`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44bdde740192774f34636311a0dbd2b1081ec88c6a24c81b246635938b65c1`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a06e853d235302bea036f40c1af6580b1f35dccf8df3f8610cab630655e58ca`  
		Last Modified: Thu, 24 Mar 2022 05:08:26 GMT  
		Size: 6.9 MB (6933055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:6d51c80ff60c5af6672cd56b99a19bee907503fbb5602e2d89d82c529029afef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:6f9f8a915e5a4a8308fcb3e2ba14cd6c7a2dbc11acd03b5a604d97781e84f4e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69395718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68061fb4db0fb111497ee4144c9b3f2cf421a0d450f1d1bc294d0fee31bf5670`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:14:46 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 23 Mar 2022 16:14:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:19:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:19:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:19:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:19:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:19:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:38 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236b952b9466b604bbc4e060a2667d7a7a335bee006fd5104c151dbdb4bf787`  
		Last Modified: Wed, 23 Mar 2022 16:15:39 GMT  
		Size: 2.0 MB (1969538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580f7437ec44a9dd3670ee6fd964ecb068808106d1bd8b961e7a568ef3ceb4f`  
		Last Modified: Wed, 23 Mar 2022 16:15:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0577d395ae504f47fad1c4d36855a3577354d4f0eca32daf7e0b13cf768c17`  
		Last Modified: Thu, 24 Mar 2022 05:20:29 GMT  
		Size: 64.6 MB (64611627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a33444f604b483769f304acdb1c976a4ea78d16943f3be3f9814e1a1e495f`  
		Last Modified: Thu, 24 Mar 2022 05:20:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8453fa1b01e46b0305c4d091304622803430cc8d0b3edb47c7be3a951e62e3`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e8e864d7d32b260f5ca60b2065242e7c51ccaa371f2cc9807d0c32b2ec06f`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:92392048de09154bffb7835256dc671934d598a3093d353494c89502784c8758
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63221233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5544e5647dd04b7224537d744d5e6fee9ade047a9fdfc200ccff6fe4749c30b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:05:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 24 Mar 2022 05:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:05:37 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:05:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:05:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:05:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:05:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:05:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:05:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:05:48 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f777e60e93e1e25280d855dd6b0c8e7e7d1508b2cbd43b9678cd18b2bab72084`  
		Last Modified: Thu, 24 Mar 2022 05:07:13 GMT  
		Size: 1.9 MB (1938915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1b0eef4b739aafe07d37f6f0fc1850ff0b6f61ab14400a1b6348cd2c8b7186`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4e629eede4a3f517e93a1764b365c41b7b2d2554b27f9d6fa6c2e37473901`  
		Last Modified: Thu, 24 Mar 2022 05:07:20 GMT  
		Size: 58.6 MB (58565771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7213dc5eb38c445dc0cffd227536ad4e5265f45307b743d11d8eb43fbdd43c26`  
		Last Modified: Thu, 24 Mar 2022 05:07:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57979a88be1287b9ce5ca410359f13c10dea1b5859e7e42d1bed86fb996f2d6e`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44bdde740192774f34636311a0dbd2b1081ec88c6a24c81b246635938b65c1`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore`

```console
$ docker pull docker@sha256:e975b7c270f2a35f16d48b91e2ab5f0eff84a690da1fcedab97e7157d0b3a5ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.587; amd64
	-	windows version 10.0.17763.2686; amd64

### `docker:windowsservercore` - windows version 10.0.20348.587; amd64

```console
$ docker pull docker@sha256:aefae8d2bf575204b17f88589c7741c350281048d96844f9fd3316a80ec2940e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2275653601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:723b6471c336c441aa997a1c5d0672ef1de87fe45687edb769c52bd0edce4e81`
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
# Thu, 24 Mar 2022 05:15:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:15:30 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.14.zip
# Thu, 24 Mar 2022 05:16:11 GMT
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
	-	`sha256:0181d328453c16ef4bf5dfa86a118c96a8325d7a3e58637e504f5425c5ea7ae2`  
		Last Modified: Thu, 24 Mar 2022 05:18:23 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e48a2566f0d50346970f29a77bd1cbfde2d33a34fc25d9227a8900f494b136a`  
		Last Modified: Thu, 24 Mar 2022 05:18:24 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cd9d001a2232e2f5406882e91758565fec1809573168d4e31cafa909ea5d4f`  
		Last Modified: Thu, 24 Mar 2022 05:18:35 GMT  
		Size: 53.8 MB (53804106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull docker@sha256:034598e549b6c0f2bb1ff47cbb638cb9785ab1456144eb4c0da198e075e70a9d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2769426444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2374652d04922dbe838fbdac11dc741534c504b1213d1110bcf7ab3ce0075be`
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
# Thu, 24 Mar 2022 05:16:22 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:16:23 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.14.zip
# Thu, 24 Mar 2022 05:17:56 GMT
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
	-	`sha256:3a37839ee100e0b4b77379ec17ab118f0b377c9d7f73de9b4fdfce26e5910d07`  
		Last Modified: Thu, 24 Mar 2022 05:18:49 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a35b5cdb293ca7295865a746b962b396382293a16a843862f866ad76d49b7d`  
		Last Modified: Thu, 24 Mar 2022 05:18:49 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791bcb5d614f3fbb4d6ff0b29ce1877c53e05d3b8536fe0fa4b549f20c0b6730`  
		Last Modified: Thu, 24 Mar 2022 05:19:47 GMT  
		Size: 53.6 MB (53615927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:6e21edf269ee8beed4808bae91f5cc840ad2a042a19a6eb6de13c97e3053906b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull docker@sha256:034598e549b6c0f2bb1ff47cbb638cb9785ab1456144eb4c0da198e075e70a9d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2769426444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2374652d04922dbe838fbdac11dc741534c504b1213d1110bcf7ab3ce0075be`
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
# Thu, 24 Mar 2022 05:16:22 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:16:23 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.14.zip
# Thu, 24 Mar 2022 05:17:56 GMT
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
	-	`sha256:3a37839ee100e0b4b77379ec17ab118f0b377c9d7f73de9b4fdfce26e5910d07`  
		Last Modified: Thu, 24 Mar 2022 05:18:49 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a35b5cdb293ca7295865a746b962b396382293a16a843862f866ad76d49b7d`  
		Last Modified: Thu, 24 Mar 2022 05:18:49 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791bcb5d614f3fbb4d6ff0b29ce1877c53e05d3b8536fe0fa4b549f20c0b6730`  
		Last Modified: Thu, 24 Mar 2022 05:19:47 GMT  
		Size: 53.6 MB (53615927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:8520b3fc85f5fe47604cbba4353f8b2feda30bcf041e26848bd6d812173f4444
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.587; amd64

### `docker:windowsservercore-ltsc2022` - windows version 10.0.20348.587; amd64

```console
$ docker pull docker@sha256:aefae8d2bf575204b17f88589c7741c350281048d96844f9fd3316a80ec2940e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2275653601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:723b6471c336c441aa997a1c5d0672ef1de87fe45687edb769c52bd0edce4e81`
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
# Thu, 24 Mar 2022 05:15:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:15:30 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.14.zip
# Thu, 24 Mar 2022 05:16:11 GMT
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
	-	`sha256:0181d328453c16ef4bf5dfa86a118c96a8325d7a3e58637e504f5425c5ea7ae2`  
		Last Modified: Thu, 24 Mar 2022 05:18:23 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e48a2566f0d50346970f29a77bd1cbfde2d33a34fc25d9227a8900f494b136a`  
		Last Modified: Thu, 24 Mar 2022 05:18:24 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cd9d001a2232e2f5406882e91758565fec1809573168d4e31cafa909ea5d4f`  
		Last Modified: Thu, 24 Mar 2022 05:18:35 GMT  
		Size: 53.8 MB (53804106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
