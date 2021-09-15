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
-	[`docker:20.10.8-alpine3.14`](#docker20108-alpine314)
-	[`docker:20.10.8-dind`](#docker20108-dind)
-	[`docker:20.10.8-dind-alpine3.14`](#docker20108-dind-alpine314)
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
$ docker pull docker@sha256:63107bd6ce718f130bb2668704239467b74f034c446f9e9c4ae1ffa5ddf4e3dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20` - linux; amd64

```console
$ docker pull docker@sha256:6ac2f3862aa1353a5fe6bf12439f3e56e695e56d7c3098898c96ef33eae78bf9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (66035309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc6c0ffef6650bcfbb0afd5a07b813b5ccf1d00ecddccadb85123c6ee57a7995`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 22:19:34 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 22:19:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 22:19:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 22:19:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 22:19:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 22:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:42 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14df950e5a796f46eb6615169002a1c428bd908141de49fb35ec026c206e77aa`  
		Last Modified: Wed, 01 Sep 2021 22:20:33 GMT  
		Size: 1.9 MB (1935099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a31cc9e913427e8959328b7d290bdcc639a9f84c11956c33c0ce112788cf19`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a4137012260e097fc6b4bf6d75ba3b193acb399fb1276687303dea63ba519c`  
		Last Modified: Wed, 01 Sep 2021 22:20:40 GMT  
		Size: 61.3 MB (61283898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d92eaf14165f5a5883286b050c77b9c7022efbde954c3b7e96e92565515f0a`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e701314a31132c239baf0de9d4922559fc419c445e13c9ce7ffd8b4518b4f98e`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea1be2ff281d99199cd048ef3bf1464615aec1ca9abfc20e73838913432dc0`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:2fad5f90265a7c9c4ee73f0b0eaa7b5ed8203af4cd0464dda8f7e1f4b28a5ad7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (60042992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3734d5adc5ac9557175d6c0acb930e7ed6d75e1f2e52e8c170b4ade3f76806a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 21:39:27 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 21:39:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 21:39:28 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 21:39:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 21:39:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 21:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:34 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8b53fc582fabf462979a1e3b92dd264069a8c4db48d483900b12ffaf539203`  
		Last Modified: Wed, 01 Sep 2021 21:41:00 GMT  
		Size: 1.9 MB (1909030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6288aa69581811c8fced6884b0ce72c344df8f72b9317062be7b6672c538444`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a48a30fd82efeed488ce352f8151d74bb4484cd178fc5fd08e6a8ccfc69560`  
		Last Modified: Wed, 01 Sep 2021 21:41:06 GMT  
		Size: 55.4 MB (55420270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fb6b55a7508af4b07b8ca08ae9f62ea7c5aa6bf46bc94cca92c15f6f418faf`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8605ad73716feec4bef5573f92fe2b1472d4e43804d33bd45d3656b83af314c`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ddbc92192571b4db6ee00ea2473aa0cdb78b7628f95560f0571a4ac15e330a`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind`

```console
$ docker pull docker@sha256:1efacb06edbb1e2bd4a39dcc69883866c7dd98562a49fa97d7d29c2da1c3974f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind` - linux; amd64

```console
$ docker pull docker@sha256:903b889a009176428a2c11ad1b0e72135d07fd51f56db7042b8119eafb808112
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72561611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e5d106d317b2ddf45e60b5ba90a53082d306fac5c96e36ef3f2ad48e9719adb`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 22:19:34 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 22:19:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 22:19:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 22:19:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 22:19:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 22:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:42 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 22:19:48 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 22:19:48 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 22:19:49 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 22:19:49 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 22:19:50 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:50 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 22:19:50 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 22:19:50 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:50 GMT
CMD []
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14df950e5a796f46eb6615169002a1c428bd908141de49fb35ec026c206e77aa`  
		Last Modified: Wed, 01 Sep 2021 22:20:33 GMT  
		Size: 1.9 MB (1935099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a31cc9e913427e8959328b7d290bdcc639a9f84c11956c33c0ce112788cf19`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a4137012260e097fc6b4bf6d75ba3b193acb399fb1276687303dea63ba519c`  
		Last Modified: Wed, 01 Sep 2021 22:20:40 GMT  
		Size: 61.3 MB (61283898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d92eaf14165f5a5883286b050c77b9c7022efbde954c3b7e96e92565515f0a`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e701314a31132c239baf0de9d4922559fc419c445e13c9ce7ffd8b4518b4f98e`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea1be2ff281d99199cd048ef3bf1464615aec1ca9abfc20e73838913432dc0`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb11622685e894072cc7fb1688ea686f6b0c903c25fda9d6f41915b279ce29`  
		Last Modified: Wed, 01 Sep 2021 22:21:00 GMT  
		Size: 6.5 MB (6521412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3448405a219f5e629e26687cfb38c611068e556983153df486257e8cf73a99`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf064520bf422a76e00ad9efafcb13da5dbd3054b24b434db5b60bfb36f7ade6`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d24f2f3cafbe18c3b4670d84f15a678aa265a9b90de016ff565157a15c7acc3`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f21866d81ae3b92303af07fe477794e4e4bf43836de0d41b4c212d4469d41a1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66466448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de95d7c2e2d4cc59123fcfef69442499876a675bb59ab504b9ad78c5881fe85a`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 21:39:27 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 21:39:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 21:39:28 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 21:39:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 21:39:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 21:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:34 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 21:39:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 21:39:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 21:39:45 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 21:39:46 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 21:39:46 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:47 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 21:39:47 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 21:39:47 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:47 GMT
CMD []
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8b53fc582fabf462979a1e3b92dd264069a8c4db48d483900b12ffaf539203`  
		Last Modified: Wed, 01 Sep 2021 21:41:00 GMT  
		Size: 1.9 MB (1909030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6288aa69581811c8fced6884b0ce72c344df8f72b9317062be7b6672c538444`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a48a30fd82efeed488ce352f8151d74bb4484cd178fc5fd08e6a8ccfc69560`  
		Last Modified: Wed, 01 Sep 2021 21:41:06 GMT  
		Size: 55.4 MB (55420270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fb6b55a7508af4b07b8ca08ae9f62ea7c5aa6bf46bc94cca92c15f6f418faf`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8605ad73716feec4bef5573f92fe2b1472d4e43804d33bd45d3656b83af314c`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ddbc92192571b4db6ee00ea2473aa0cdb78b7628f95560f0571a4ac15e330a`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373ff707a384f2d3eeae1ec32f9044142bb5c896541416c18d1bf45142da30ae`  
		Last Modified: Wed, 01 Sep 2021 21:41:30 GMT  
		Size: 6.4 MB (6418561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436d94df880147a87f1fba1c3115c37eb4b50c95fc93694f4d5e1fc22f353fd3`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ada35578ff611689fc1c810d1603dd6b6c606175e97737d9f3073f4631235b0`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fcd3a1f2fec5765d757040410b3f777d30970931dd552544b55ada1dc9ebe8`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:d75833c3ed601b634c871302b025c4fd070816e8e81394f1bf7161658a49da3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:ec2140865f2bc0705f6d17a575b2036e5d60a768007321245faa9eebdc031488
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.8 MB (92828157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5ff4e7c8157ca219e02e8525c28f1a8350b01b405a72860e2c926a26a8e9d6b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 22:19:34 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 22:19:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 22:19:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 22:19:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 22:19:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 22:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:42 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 22:19:48 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 22:19:48 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 22:19:49 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 22:19:49 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 22:19:50 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:50 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 22:19:50 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 22:19:50 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:50 GMT
CMD []
# Wed, 01 Sep 2021 22:19:55 GMT
RUN apk add --no-cache iproute2
# Wed, 01 Sep 2021 22:19:56 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Sep 2021 22:19:57 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Sep 2021 22:19:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Sep 2021 22:19:59 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Sep 2021 22:20:00 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Sep 2021 22:20:00 GMT
USER rootless
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14df950e5a796f46eb6615169002a1c428bd908141de49fb35ec026c206e77aa`  
		Last Modified: Wed, 01 Sep 2021 22:20:33 GMT  
		Size: 1.9 MB (1935099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a31cc9e913427e8959328b7d290bdcc639a9f84c11956c33c0ce112788cf19`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a4137012260e097fc6b4bf6d75ba3b193acb399fb1276687303dea63ba519c`  
		Last Modified: Wed, 01 Sep 2021 22:20:40 GMT  
		Size: 61.3 MB (61283898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d92eaf14165f5a5883286b050c77b9c7022efbde954c3b7e96e92565515f0a`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e701314a31132c239baf0de9d4922559fc419c445e13c9ce7ffd8b4518b4f98e`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea1be2ff281d99199cd048ef3bf1464615aec1ca9abfc20e73838913432dc0`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb11622685e894072cc7fb1688ea686f6b0c903c25fda9d6f41915b279ce29`  
		Last Modified: Wed, 01 Sep 2021 22:21:00 GMT  
		Size: 6.5 MB (6521412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3448405a219f5e629e26687cfb38c611068e556983153df486257e8cf73a99`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf064520bf422a76e00ad9efafcb13da5dbd3054b24b434db5b60bfb36f7ade6`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d24f2f3cafbe18c3b4670d84f15a678aa265a9b90de016ff565157a15c7acc3`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ee8eb2774788b07752bfe9bada2565d0759149471b1e1184fe1b8b9b723291`  
		Last Modified: Wed, 01 Sep 2021 22:21:20 GMT  
		Size: 1.1 MB (1148735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4811cca51263afbb69cb08a00b9ced312530c69efdd89d18432a10d708b9793`  
		Last Modified: Wed, 01 Sep 2021 22:21:20 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1196b78c6ec13dfea9317ce19a5c0297ffa1b7bb71c9cbdcbd8898a7d1c488fe`  
		Last Modified: Wed, 01 Sep 2021 22:21:20 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951aa128211fa2e81475296d3178c72f82de1b9b0fca6577a41522b421d33333`  
		Last Modified: Wed, 01 Sep 2021 22:21:23 GMT  
		Size: 19.1 MB (19116094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b58b08848076b0b593d64fb903397d255b9467bb9f93f4492d852beb23532af`  
		Last Modified: Wed, 01 Sep 2021 22:21:20 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:01a3353757a17aa2125c2a6181c436134d7a0055df0ef3ba323826350e1d0ff1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88731007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bcfee17c3e4c3e92f1ae3c5a77520971a3633eebf269f8a4a895634a5ad06c2`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 21:39:27 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 21:39:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 21:39:28 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 21:39:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 21:39:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 21:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:34 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 21:39:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 21:39:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 21:39:45 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 21:39:46 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 21:39:46 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:47 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 21:39:47 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 21:39:47 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:47 GMT
CMD []
# Wed, 01 Sep 2021 21:39:55 GMT
RUN apk add --no-cache iproute2
# Wed, 01 Sep 2021 21:39:56 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Sep 2021 21:39:57 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Sep 2021 21:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Sep 2021 21:39:59 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Sep 2021 21:39:59 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Sep 2021 21:39:59 GMT
USER rootless
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8b53fc582fabf462979a1e3b92dd264069a8c4db48d483900b12ffaf539203`  
		Last Modified: Wed, 01 Sep 2021 21:41:00 GMT  
		Size: 1.9 MB (1909030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6288aa69581811c8fced6884b0ce72c344df8f72b9317062be7b6672c538444`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a48a30fd82efeed488ce352f8151d74bb4484cd178fc5fd08e6a8ccfc69560`  
		Last Modified: Wed, 01 Sep 2021 21:41:06 GMT  
		Size: 55.4 MB (55420270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fb6b55a7508af4b07b8ca08ae9f62ea7c5aa6bf46bc94cca92c15f6f418faf`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8605ad73716feec4bef5573f92fe2b1472d4e43804d33bd45d3656b83af314c`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ddbc92192571b4db6ee00ea2473aa0cdb78b7628f95560f0571a4ac15e330a`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373ff707a384f2d3eeae1ec32f9044142bb5c896541416c18d1bf45142da30ae`  
		Last Modified: Wed, 01 Sep 2021 21:41:30 GMT  
		Size: 6.4 MB (6418561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436d94df880147a87f1fba1c3115c37eb4b50c95fc93694f4d5e1fc22f353fd3`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ada35578ff611689fc1c810d1603dd6b6c606175e97737d9f3073f4631235b0`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fcd3a1f2fec5765d757040410b3f777d30970931dd552544b55ada1dc9ebe8`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0727607c4852e6356bf01e7ea1c0d090e6100e1045cd881eca01515749b53e6`  
		Last Modified: Wed, 01 Sep 2021 21:41:53 GMT  
		Size: 1.2 MB (1168111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee229379e57fe13e75a06a3453c3afa2ec3959e936165ad25b24fa00a2bec57`  
		Last Modified: Wed, 01 Sep 2021 21:41:53 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5c0508be8bb4e91bd2c3895baa8ee248bf3b1bb5bd9d605a8c5da8b4aeff1a`  
		Last Modified: Wed, 01 Sep 2021 21:41:53 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dc3c7f21a4603739eb746480b3aa01086f70941d2b2141504e7c7e796a1bab`  
		Last Modified: Wed, 01 Sep 2021 21:41:57 GMT  
		Size: 21.1 MB (21094732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da3b6b5f43f82f2e3e8c853aefbe98b52cbd1ff0fc99294851db16ee9eefa2f`  
		Last Modified: Wed, 01 Sep 2021 21:41:53 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-git`

```console
$ docker pull docker@sha256:d7f576652c05a6e86970cbdb477d4bb5d30932599806786e126067e406ef59cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-git` - linux; amd64

```console
$ docker pull docker@sha256:5ccbe97e61943749d3f7aa5f14caa1265de865ae65eba21798943588a7ed9796
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72665297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94f59df6fc6382ef41eefeb7025d1db3fc3f724644192060b565cc1c010df180`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 22:19:34 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 22:19:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 22:19:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 22:19:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 22:19:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 22:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:42 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 22:20:05 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14df950e5a796f46eb6615169002a1c428bd908141de49fb35ec026c206e77aa`  
		Last Modified: Wed, 01 Sep 2021 22:20:33 GMT  
		Size: 1.9 MB (1935099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a31cc9e913427e8959328b7d290bdcc639a9f84c11956c33c0ce112788cf19`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a4137012260e097fc6b4bf6d75ba3b193acb399fb1276687303dea63ba519c`  
		Last Modified: Wed, 01 Sep 2021 22:20:40 GMT  
		Size: 61.3 MB (61283898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d92eaf14165f5a5883286b050c77b9c7022efbde954c3b7e96e92565515f0a`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e701314a31132c239baf0de9d4922559fc419c445e13c9ce7ffd8b4518b4f98e`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea1be2ff281d99199cd048ef3bf1464615aec1ca9abfc20e73838913432dc0`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7649c299d9b594bf34994b3bda767e79eca59d49cbc5e59c93e350890fce080`  
		Last Modified: Wed, 01 Sep 2021 22:21:42 GMT  
		Size: 6.6 MB (6629988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4951d55d07df56eb3dc8823e5abb438f05ced009af250666aab6381f9ef2a99c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.8 MB (66784792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c1f1eae55906bc481ffd709ea71e35a3f9aa3dde59572a62cadf79d7442716`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 21:39:27 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 21:39:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 21:39:28 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 21:39:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 21:39:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 21:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:34 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 21:40:07 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8b53fc582fabf462979a1e3b92dd264069a8c4db48d483900b12ffaf539203`  
		Last Modified: Wed, 01 Sep 2021 21:41:00 GMT  
		Size: 1.9 MB (1909030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6288aa69581811c8fced6884b0ce72c344df8f72b9317062be7b6672c538444`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a48a30fd82efeed488ce352f8151d74bb4484cd178fc5fd08e6a8ccfc69560`  
		Last Modified: Wed, 01 Sep 2021 21:41:06 GMT  
		Size: 55.4 MB (55420270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fb6b55a7508af4b07b8ca08ae9f62ea7c5aa6bf46bc94cca92c15f6f418faf`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8605ad73716feec4bef5573f92fe2b1472d4e43804d33bd45d3656b83af314c`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ddbc92192571b4db6ee00ea2473aa0cdb78b7628f95560f0571a4ac15e330a`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac87a5e4495fa9d6f260ed353f2f2ed60461d2ccc2fcce309f3a0ab5cfe2a01`  
		Last Modified: Wed, 01 Sep 2021 21:42:18 GMT  
		Size: 6.7 MB (6741800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore`

```console
$ docker pull docker@sha256:f4af31b74a5253ec58671de6c2710e16a5f2ac2817548c6a7e2154049cbc3bf2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `docker:20-windowsservercore` - windows version 10.0.17763.2183; amd64

```console
$ docker pull docker@sha256:a9020b9c4925433869c0c958d9e53f8ad2176330779b65f82f4bf310ea4bc9ab
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737923247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1ab891d90a3bc1ec92ff32071fc677c238ee44a43d6eb073003da02862bd7d8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 19:24:35 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Sep 2021 19:24:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 15 Sep 2021 19:24:37 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Wed, 15 Sep 2021 19:25:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f6f3cf73df901f0ef53d2cf3a1187cb87ff309f8b28b24c1adcc34ea9ad1`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 353.9 KB (353857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451d02c3ec1421ec5056fe967d7be6a344cb53cfd77445f76f4b50483cfae635`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5f2c36a2ae93fffd565b76d88402e7eb238d7097f5ea1c17d64a5d85d745ac`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f40204892cf05231048b06e8d6fb355be34ff937c4cfe6ac6cecb768f816d1d`  
		Last Modified: Wed, 15 Sep 2021 19:26:08 GMT  
		Size: 50.9 MB (50867243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-1809`

```console
$ docker pull docker@sha256:f4af31b74a5253ec58671de6c2710e16a5f2ac2817548c6a7e2154049cbc3bf2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `docker:20-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull docker@sha256:a9020b9c4925433869c0c958d9e53f8ad2176330779b65f82f4bf310ea4bc9ab
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737923247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1ab891d90a3bc1ec92ff32071fc677c238ee44a43d6eb073003da02862bd7d8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 19:24:35 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Sep 2021 19:24:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 15 Sep 2021 19:24:37 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Wed, 15 Sep 2021 19:25:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f6f3cf73df901f0ef53d2cf3a1187cb87ff309f8b28b24c1adcc34ea9ad1`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 353.9 KB (353857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451d02c3ec1421ec5056fe967d7be6a344cb53cfd77445f76f4b50483cfae635`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5f2c36a2ae93fffd565b76d88402e7eb238d7097f5ea1c17d64a5d85d745ac`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f40204892cf05231048b06e8d6fb355be34ff937c4cfe6ac6cecb768f816d1d`  
		Last Modified: Wed, 15 Sep 2021 19:26:08 GMT  
		Size: 50.9 MB (50867243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10`

```console
$ docker pull docker@sha256:63107bd6ce718f130bb2668704239467b74f034c446f9e9c4ae1ffa5ddf4e3dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10` - linux; amd64

```console
$ docker pull docker@sha256:6ac2f3862aa1353a5fe6bf12439f3e56e695e56d7c3098898c96ef33eae78bf9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (66035309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc6c0ffef6650bcfbb0afd5a07b813b5ccf1d00ecddccadb85123c6ee57a7995`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 22:19:34 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 22:19:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 22:19:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 22:19:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 22:19:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 22:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:42 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14df950e5a796f46eb6615169002a1c428bd908141de49fb35ec026c206e77aa`  
		Last Modified: Wed, 01 Sep 2021 22:20:33 GMT  
		Size: 1.9 MB (1935099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a31cc9e913427e8959328b7d290bdcc639a9f84c11956c33c0ce112788cf19`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a4137012260e097fc6b4bf6d75ba3b193acb399fb1276687303dea63ba519c`  
		Last Modified: Wed, 01 Sep 2021 22:20:40 GMT  
		Size: 61.3 MB (61283898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d92eaf14165f5a5883286b050c77b9c7022efbde954c3b7e96e92565515f0a`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e701314a31132c239baf0de9d4922559fc419c445e13c9ce7ffd8b4518b4f98e`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea1be2ff281d99199cd048ef3bf1464615aec1ca9abfc20e73838913432dc0`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:2fad5f90265a7c9c4ee73f0b0eaa7b5ed8203af4cd0464dda8f7e1f4b28a5ad7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (60042992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3734d5adc5ac9557175d6c0acb930e7ed6d75e1f2e52e8c170b4ade3f76806a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 21:39:27 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 21:39:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 21:39:28 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 21:39:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 21:39:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 21:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:34 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8b53fc582fabf462979a1e3b92dd264069a8c4db48d483900b12ffaf539203`  
		Last Modified: Wed, 01 Sep 2021 21:41:00 GMT  
		Size: 1.9 MB (1909030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6288aa69581811c8fced6884b0ce72c344df8f72b9317062be7b6672c538444`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a48a30fd82efeed488ce352f8151d74bb4484cd178fc5fd08e6a8ccfc69560`  
		Last Modified: Wed, 01 Sep 2021 21:41:06 GMT  
		Size: 55.4 MB (55420270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fb6b55a7508af4b07b8ca08ae9f62ea7c5aa6bf46bc94cca92c15f6f418faf`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8605ad73716feec4bef5573f92fe2b1472d4e43804d33bd45d3656b83af314c`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ddbc92192571b4db6ee00ea2473aa0cdb78b7628f95560f0571a4ac15e330a`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind`

```console
$ docker pull docker@sha256:1efacb06edbb1e2bd4a39dcc69883866c7dd98562a49fa97d7d29c2da1c3974f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind` - linux; amd64

```console
$ docker pull docker@sha256:903b889a009176428a2c11ad1b0e72135d07fd51f56db7042b8119eafb808112
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72561611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e5d106d317b2ddf45e60b5ba90a53082d306fac5c96e36ef3f2ad48e9719adb`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 22:19:34 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 22:19:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 22:19:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 22:19:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 22:19:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 22:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:42 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 22:19:48 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 22:19:48 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 22:19:49 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 22:19:49 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 22:19:50 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:50 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 22:19:50 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 22:19:50 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:50 GMT
CMD []
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14df950e5a796f46eb6615169002a1c428bd908141de49fb35ec026c206e77aa`  
		Last Modified: Wed, 01 Sep 2021 22:20:33 GMT  
		Size: 1.9 MB (1935099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a31cc9e913427e8959328b7d290bdcc639a9f84c11956c33c0ce112788cf19`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a4137012260e097fc6b4bf6d75ba3b193acb399fb1276687303dea63ba519c`  
		Last Modified: Wed, 01 Sep 2021 22:20:40 GMT  
		Size: 61.3 MB (61283898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d92eaf14165f5a5883286b050c77b9c7022efbde954c3b7e96e92565515f0a`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e701314a31132c239baf0de9d4922559fc419c445e13c9ce7ffd8b4518b4f98e`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea1be2ff281d99199cd048ef3bf1464615aec1ca9abfc20e73838913432dc0`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb11622685e894072cc7fb1688ea686f6b0c903c25fda9d6f41915b279ce29`  
		Last Modified: Wed, 01 Sep 2021 22:21:00 GMT  
		Size: 6.5 MB (6521412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3448405a219f5e629e26687cfb38c611068e556983153df486257e8cf73a99`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf064520bf422a76e00ad9efafcb13da5dbd3054b24b434db5b60bfb36f7ade6`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d24f2f3cafbe18c3b4670d84f15a678aa265a9b90de016ff565157a15c7acc3`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f21866d81ae3b92303af07fe477794e4e4bf43836de0d41b4c212d4469d41a1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66466448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de95d7c2e2d4cc59123fcfef69442499876a675bb59ab504b9ad78c5881fe85a`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 21:39:27 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 21:39:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 21:39:28 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 21:39:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 21:39:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 21:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:34 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 21:39:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 21:39:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 21:39:45 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 21:39:46 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 21:39:46 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:47 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 21:39:47 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 21:39:47 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:47 GMT
CMD []
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8b53fc582fabf462979a1e3b92dd264069a8c4db48d483900b12ffaf539203`  
		Last Modified: Wed, 01 Sep 2021 21:41:00 GMT  
		Size: 1.9 MB (1909030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6288aa69581811c8fced6884b0ce72c344df8f72b9317062be7b6672c538444`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a48a30fd82efeed488ce352f8151d74bb4484cd178fc5fd08e6a8ccfc69560`  
		Last Modified: Wed, 01 Sep 2021 21:41:06 GMT  
		Size: 55.4 MB (55420270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fb6b55a7508af4b07b8ca08ae9f62ea7c5aa6bf46bc94cca92c15f6f418faf`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8605ad73716feec4bef5573f92fe2b1472d4e43804d33bd45d3656b83af314c`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ddbc92192571b4db6ee00ea2473aa0cdb78b7628f95560f0571a4ac15e330a`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373ff707a384f2d3eeae1ec32f9044142bb5c896541416c18d1bf45142da30ae`  
		Last Modified: Wed, 01 Sep 2021 21:41:30 GMT  
		Size: 6.4 MB (6418561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436d94df880147a87f1fba1c3115c37eb4b50c95fc93694f4d5e1fc22f353fd3`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ada35578ff611689fc1c810d1603dd6b6c606175e97737d9f3073f4631235b0`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fcd3a1f2fec5765d757040410b3f777d30970931dd552544b55ada1dc9ebe8`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind-rootless`

```console
$ docker pull docker@sha256:d75833c3ed601b634c871302b025c4fd070816e8e81394f1bf7161658a49da3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:ec2140865f2bc0705f6d17a575b2036e5d60a768007321245faa9eebdc031488
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.8 MB (92828157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5ff4e7c8157ca219e02e8525c28f1a8350b01b405a72860e2c926a26a8e9d6b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 22:19:34 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 22:19:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 22:19:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 22:19:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 22:19:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 22:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:42 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 22:19:48 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 22:19:48 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 22:19:49 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 22:19:49 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 22:19:50 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:50 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 22:19:50 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 22:19:50 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:50 GMT
CMD []
# Wed, 01 Sep 2021 22:19:55 GMT
RUN apk add --no-cache iproute2
# Wed, 01 Sep 2021 22:19:56 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Sep 2021 22:19:57 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Sep 2021 22:19:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Sep 2021 22:19:59 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Sep 2021 22:20:00 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Sep 2021 22:20:00 GMT
USER rootless
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14df950e5a796f46eb6615169002a1c428bd908141de49fb35ec026c206e77aa`  
		Last Modified: Wed, 01 Sep 2021 22:20:33 GMT  
		Size: 1.9 MB (1935099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a31cc9e913427e8959328b7d290bdcc639a9f84c11956c33c0ce112788cf19`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a4137012260e097fc6b4bf6d75ba3b193acb399fb1276687303dea63ba519c`  
		Last Modified: Wed, 01 Sep 2021 22:20:40 GMT  
		Size: 61.3 MB (61283898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d92eaf14165f5a5883286b050c77b9c7022efbde954c3b7e96e92565515f0a`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e701314a31132c239baf0de9d4922559fc419c445e13c9ce7ffd8b4518b4f98e`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea1be2ff281d99199cd048ef3bf1464615aec1ca9abfc20e73838913432dc0`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb11622685e894072cc7fb1688ea686f6b0c903c25fda9d6f41915b279ce29`  
		Last Modified: Wed, 01 Sep 2021 22:21:00 GMT  
		Size: 6.5 MB (6521412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3448405a219f5e629e26687cfb38c611068e556983153df486257e8cf73a99`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf064520bf422a76e00ad9efafcb13da5dbd3054b24b434db5b60bfb36f7ade6`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d24f2f3cafbe18c3b4670d84f15a678aa265a9b90de016ff565157a15c7acc3`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ee8eb2774788b07752bfe9bada2565d0759149471b1e1184fe1b8b9b723291`  
		Last Modified: Wed, 01 Sep 2021 22:21:20 GMT  
		Size: 1.1 MB (1148735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4811cca51263afbb69cb08a00b9ced312530c69efdd89d18432a10d708b9793`  
		Last Modified: Wed, 01 Sep 2021 22:21:20 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1196b78c6ec13dfea9317ce19a5c0297ffa1b7bb71c9cbdcbd8898a7d1c488fe`  
		Last Modified: Wed, 01 Sep 2021 22:21:20 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951aa128211fa2e81475296d3178c72f82de1b9b0fca6577a41522b421d33333`  
		Last Modified: Wed, 01 Sep 2021 22:21:23 GMT  
		Size: 19.1 MB (19116094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b58b08848076b0b593d64fb903397d255b9467bb9f93f4492d852beb23532af`  
		Last Modified: Wed, 01 Sep 2021 22:21:20 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:01a3353757a17aa2125c2a6181c436134d7a0055df0ef3ba323826350e1d0ff1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88731007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bcfee17c3e4c3e92f1ae3c5a77520971a3633eebf269f8a4a895634a5ad06c2`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 21:39:27 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 21:39:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 21:39:28 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 21:39:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 21:39:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 21:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:34 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 21:39:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 21:39:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 21:39:45 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 21:39:46 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 21:39:46 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:47 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 21:39:47 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 21:39:47 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:47 GMT
CMD []
# Wed, 01 Sep 2021 21:39:55 GMT
RUN apk add --no-cache iproute2
# Wed, 01 Sep 2021 21:39:56 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Sep 2021 21:39:57 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Sep 2021 21:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Sep 2021 21:39:59 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Sep 2021 21:39:59 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Sep 2021 21:39:59 GMT
USER rootless
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8b53fc582fabf462979a1e3b92dd264069a8c4db48d483900b12ffaf539203`  
		Last Modified: Wed, 01 Sep 2021 21:41:00 GMT  
		Size: 1.9 MB (1909030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6288aa69581811c8fced6884b0ce72c344df8f72b9317062be7b6672c538444`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a48a30fd82efeed488ce352f8151d74bb4484cd178fc5fd08e6a8ccfc69560`  
		Last Modified: Wed, 01 Sep 2021 21:41:06 GMT  
		Size: 55.4 MB (55420270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fb6b55a7508af4b07b8ca08ae9f62ea7c5aa6bf46bc94cca92c15f6f418faf`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8605ad73716feec4bef5573f92fe2b1472d4e43804d33bd45d3656b83af314c`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ddbc92192571b4db6ee00ea2473aa0cdb78b7628f95560f0571a4ac15e330a`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373ff707a384f2d3eeae1ec32f9044142bb5c896541416c18d1bf45142da30ae`  
		Last Modified: Wed, 01 Sep 2021 21:41:30 GMT  
		Size: 6.4 MB (6418561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436d94df880147a87f1fba1c3115c37eb4b50c95fc93694f4d5e1fc22f353fd3`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ada35578ff611689fc1c810d1603dd6b6c606175e97737d9f3073f4631235b0`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fcd3a1f2fec5765d757040410b3f777d30970931dd552544b55ada1dc9ebe8`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0727607c4852e6356bf01e7ea1c0d090e6100e1045cd881eca01515749b53e6`  
		Last Modified: Wed, 01 Sep 2021 21:41:53 GMT  
		Size: 1.2 MB (1168111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee229379e57fe13e75a06a3453c3afa2ec3959e936165ad25b24fa00a2bec57`  
		Last Modified: Wed, 01 Sep 2021 21:41:53 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5c0508be8bb4e91bd2c3895baa8ee248bf3b1bb5bd9d605a8c5da8b4aeff1a`  
		Last Modified: Wed, 01 Sep 2021 21:41:53 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dc3c7f21a4603739eb746480b3aa01086f70941d2b2141504e7c7e796a1bab`  
		Last Modified: Wed, 01 Sep 2021 21:41:57 GMT  
		Size: 21.1 MB (21094732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da3b6b5f43f82f2e3e8c853aefbe98b52cbd1ff0fc99294851db16ee9eefa2f`  
		Last Modified: Wed, 01 Sep 2021 21:41:53 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-git`

```console
$ docker pull docker@sha256:d7f576652c05a6e86970cbdb477d4bb5d30932599806786e126067e406ef59cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-git` - linux; amd64

```console
$ docker pull docker@sha256:5ccbe97e61943749d3f7aa5f14caa1265de865ae65eba21798943588a7ed9796
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72665297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94f59df6fc6382ef41eefeb7025d1db3fc3f724644192060b565cc1c010df180`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 22:19:34 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 22:19:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 22:19:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 22:19:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 22:19:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 22:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:42 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 22:20:05 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14df950e5a796f46eb6615169002a1c428bd908141de49fb35ec026c206e77aa`  
		Last Modified: Wed, 01 Sep 2021 22:20:33 GMT  
		Size: 1.9 MB (1935099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a31cc9e913427e8959328b7d290bdcc639a9f84c11956c33c0ce112788cf19`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a4137012260e097fc6b4bf6d75ba3b193acb399fb1276687303dea63ba519c`  
		Last Modified: Wed, 01 Sep 2021 22:20:40 GMT  
		Size: 61.3 MB (61283898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d92eaf14165f5a5883286b050c77b9c7022efbde954c3b7e96e92565515f0a`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e701314a31132c239baf0de9d4922559fc419c445e13c9ce7ffd8b4518b4f98e`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea1be2ff281d99199cd048ef3bf1464615aec1ca9abfc20e73838913432dc0`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7649c299d9b594bf34994b3bda767e79eca59d49cbc5e59c93e350890fce080`  
		Last Modified: Wed, 01 Sep 2021 22:21:42 GMT  
		Size: 6.6 MB (6629988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4951d55d07df56eb3dc8823e5abb438f05ced009af250666aab6381f9ef2a99c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.8 MB (66784792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c1f1eae55906bc481ffd709ea71e35a3f9aa3dde59572a62cadf79d7442716`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 21:39:27 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 21:39:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 21:39:28 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 21:39:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 21:39:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 21:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:34 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 21:40:07 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8b53fc582fabf462979a1e3b92dd264069a8c4db48d483900b12ffaf539203`  
		Last Modified: Wed, 01 Sep 2021 21:41:00 GMT  
		Size: 1.9 MB (1909030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6288aa69581811c8fced6884b0ce72c344df8f72b9317062be7b6672c538444`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a48a30fd82efeed488ce352f8151d74bb4484cd178fc5fd08e6a8ccfc69560`  
		Last Modified: Wed, 01 Sep 2021 21:41:06 GMT  
		Size: 55.4 MB (55420270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fb6b55a7508af4b07b8ca08ae9f62ea7c5aa6bf46bc94cca92c15f6f418faf`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8605ad73716feec4bef5573f92fe2b1472d4e43804d33bd45d3656b83af314c`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ddbc92192571b4db6ee00ea2473aa0cdb78b7628f95560f0571a4ac15e330a`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac87a5e4495fa9d6f260ed353f2f2ed60461d2ccc2fcce309f3a0ab5cfe2a01`  
		Last Modified: Wed, 01 Sep 2021 21:42:18 GMT  
		Size: 6.7 MB (6741800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore`

```console
$ docker pull docker@sha256:f4af31b74a5253ec58671de6c2710e16a5f2ac2817548c6a7e2154049cbc3bf2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `docker:20.10-windowsservercore` - windows version 10.0.17763.2183; amd64

```console
$ docker pull docker@sha256:a9020b9c4925433869c0c958d9e53f8ad2176330779b65f82f4bf310ea4bc9ab
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737923247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1ab891d90a3bc1ec92ff32071fc677c238ee44a43d6eb073003da02862bd7d8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 19:24:35 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Sep 2021 19:24:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 15 Sep 2021 19:24:37 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Wed, 15 Sep 2021 19:25:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f6f3cf73df901f0ef53d2cf3a1187cb87ff309f8b28b24c1adcc34ea9ad1`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 353.9 KB (353857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451d02c3ec1421ec5056fe967d7be6a344cb53cfd77445f76f4b50483cfae635`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5f2c36a2ae93fffd565b76d88402e7eb238d7097f5ea1c17d64a5d85d745ac`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f40204892cf05231048b06e8d6fb355be34ff937c4cfe6ac6cecb768f816d1d`  
		Last Modified: Wed, 15 Sep 2021 19:26:08 GMT  
		Size: 50.9 MB (50867243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-1809`

```console
$ docker pull docker@sha256:f4af31b74a5253ec58671de6c2710e16a5f2ac2817548c6a7e2154049cbc3bf2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `docker:20.10-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull docker@sha256:a9020b9c4925433869c0c958d9e53f8ad2176330779b65f82f4bf310ea4bc9ab
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737923247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1ab891d90a3bc1ec92ff32071fc677c238ee44a43d6eb073003da02862bd7d8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 19:24:35 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Sep 2021 19:24:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 15 Sep 2021 19:24:37 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Wed, 15 Sep 2021 19:25:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f6f3cf73df901f0ef53d2cf3a1187cb87ff309f8b28b24c1adcc34ea9ad1`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 353.9 KB (353857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451d02c3ec1421ec5056fe967d7be6a344cb53cfd77445f76f4b50483cfae635`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5f2c36a2ae93fffd565b76d88402e7eb238d7097f5ea1c17d64a5d85d745ac`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f40204892cf05231048b06e8d6fb355be34ff937c4cfe6ac6cecb768f816d1d`  
		Last Modified: Wed, 15 Sep 2021 19:26:08 GMT  
		Size: 50.9 MB (50867243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8`

```console
$ docker pull docker@sha256:63107bd6ce718f130bb2668704239467b74f034c446f9e9c4ae1ffa5ddf4e3dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.8` - linux; amd64

```console
$ docker pull docker@sha256:6ac2f3862aa1353a5fe6bf12439f3e56e695e56d7c3098898c96ef33eae78bf9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (66035309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc6c0ffef6650bcfbb0afd5a07b813b5ccf1d00ecddccadb85123c6ee57a7995`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 22:19:34 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 22:19:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 22:19:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 22:19:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 22:19:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 22:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:42 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14df950e5a796f46eb6615169002a1c428bd908141de49fb35ec026c206e77aa`  
		Last Modified: Wed, 01 Sep 2021 22:20:33 GMT  
		Size: 1.9 MB (1935099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a31cc9e913427e8959328b7d290bdcc639a9f84c11956c33c0ce112788cf19`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a4137012260e097fc6b4bf6d75ba3b193acb399fb1276687303dea63ba519c`  
		Last Modified: Wed, 01 Sep 2021 22:20:40 GMT  
		Size: 61.3 MB (61283898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d92eaf14165f5a5883286b050c77b9c7022efbde954c3b7e96e92565515f0a`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e701314a31132c239baf0de9d4922559fc419c445e13c9ce7ffd8b4518b4f98e`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea1be2ff281d99199cd048ef3bf1464615aec1ca9abfc20e73838913432dc0`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.8` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:2fad5f90265a7c9c4ee73f0b0eaa7b5ed8203af4cd0464dda8f7e1f4b28a5ad7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (60042992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3734d5adc5ac9557175d6c0acb930e7ed6d75e1f2e52e8c170b4ade3f76806a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 21:39:27 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 21:39:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 21:39:28 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 21:39:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 21:39:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 21:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:34 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8b53fc582fabf462979a1e3b92dd264069a8c4db48d483900b12ffaf539203`  
		Last Modified: Wed, 01 Sep 2021 21:41:00 GMT  
		Size: 1.9 MB (1909030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6288aa69581811c8fced6884b0ce72c344df8f72b9317062be7b6672c538444`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a48a30fd82efeed488ce352f8151d74bb4484cd178fc5fd08e6a8ccfc69560`  
		Last Modified: Wed, 01 Sep 2021 21:41:06 GMT  
		Size: 55.4 MB (55420270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fb6b55a7508af4b07b8ca08ae9f62ea7c5aa6bf46bc94cca92c15f6f418faf`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8605ad73716feec4bef5573f92fe2b1472d4e43804d33bd45d3656b83af314c`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ddbc92192571b4db6ee00ea2473aa0cdb78b7628f95560f0571a4ac15e330a`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8-alpine3.14`

```console
$ docker pull docker@sha256:63107bd6ce718f130bb2668704239467b74f034c446f9e9c4ae1ffa5ddf4e3dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.8-alpine3.14` - linux; amd64

```console
$ docker pull docker@sha256:6ac2f3862aa1353a5fe6bf12439f3e56e695e56d7c3098898c96ef33eae78bf9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (66035309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc6c0ffef6650bcfbb0afd5a07b813b5ccf1d00ecddccadb85123c6ee57a7995`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 22:19:34 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 22:19:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 22:19:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 22:19:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 22:19:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 22:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:42 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14df950e5a796f46eb6615169002a1c428bd908141de49fb35ec026c206e77aa`  
		Last Modified: Wed, 01 Sep 2021 22:20:33 GMT  
		Size: 1.9 MB (1935099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a31cc9e913427e8959328b7d290bdcc639a9f84c11956c33c0ce112788cf19`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a4137012260e097fc6b4bf6d75ba3b193acb399fb1276687303dea63ba519c`  
		Last Modified: Wed, 01 Sep 2021 22:20:40 GMT  
		Size: 61.3 MB (61283898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d92eaf14165f5a5883286b050c77b9c7022efbde954c3b7e96e92565515f0a`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e701314a31132c239baf0de9d4922559fc419c445e13c9ce7ffd8b4518b4f98e`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea1be2ff281d99199cd048ef3bf1464615aec1ca9abfc20e73838913432dc0`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.8-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:2fad5f90265a7c9c4ee73f0b0eaa7b5ed8203af4cd0464dda8f7e1f4b28a5ad7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (60042992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3734d5adc5ac9557175d6c0acb930e7ed6d75e1f2e52e8c170b4ade3f76806a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 21:39:27 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 21:39:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 21:39:28 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 21:39:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 21:39:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 21:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:34 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8b53fc582fabf462979a1e3b92dd264069a8c4db48d483900b12ffaf539203`  
		Last Modified: Wed, 01 Sep 2021 21:41:00 GMT  
		Size: 1.9 MB (1909030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6288aa69581811c8fced6884b0ce72c344df8f72b9317062be7b6672c538444`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a48a30fd82efeed488ce352f8151d74bb4484cd178fc5fd08e6a8ccfc69560`  
		Last Modified: Wed, 01 Sep 2021 21:41:06 GMT  
		Size: 55.4 MB (55420270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fb6b55a7508af4b07b8ca08ae9f62ea7c5aa6bf46bc94cca92c15f6f418faf`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8605ad73716feec4bef5573f92fe2b1472d4e43804d33bd45d3656b83af314c`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ddbc92192571b4db6ee00ea2473aa0cdb78b7628f95560f0571a4ac15e330a`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8-dind`

```console
$ docker pull docker@sha256:1efacb06edbb1e2bd4a39dcc69883866c7dd98562a49fa97d7d29c2da1c3974f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.8-dind` - linux; amd64

```console
$ docker pull docker@sha256:903b889a009176428a2c11ad1b0e72135d07fd51f56db7042b8119eafb808112
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72561611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e5d106d317b2ddf45e60b5ba90a53082d306fac5c96e36ef3f2ad48e9719adb`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 22:19:34 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 22:19:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 22:19:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 22:19:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 22:19:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 22:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:42 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 22:19:48 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 22:19:48 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 22:19:49 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 22:19:49 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 22:19:50 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:50 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 22:19:50 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 22:19:50 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:50 GMT
CMD []
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14df950e5a796f46eb6615169002a1c428bd908141de49fb35ec026c206e77aa`  
		Last Modified: Wed, 01 Sep 2021 22:20:33 GMT  
		Size: 1.9 MB (1935099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a31cc9e913427e8959328b7d290bdcc639a9f84c11956c33c0ce112788cf19`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a4137012260e097fc6b4bf6d75ba3b193acb399fb1276687303dea63ba519c`  
		Last Modified: Wed, 01 Sep 2021 22:20:40 GMT  
		Size: 61.3 MB (61283898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d92eaf14165f5a5883286b050c77b9c7022efbde954c3b7e96e92565515f0a`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e701314a31132c239baf0de9d4922559fc419c445e13c9ce7ffd8b4518b4f98e`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea1be2ff281d99199cd048ef3bf1464615aec1ca9abfc20e73838913432dc0`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb11622685e894072cc7fb1688ea686f6b0c903c25fda9d6f41915b279ce29`  
		Last Modified: Wed, 01 Sep 2021 22:21:00 GMT  
		Size: 6.5 MB (6521412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3448405a219f5e629e26687cfb38c611068e556983153df486257e8cf73a99`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf064520bf422a76e00ad9efafcb13da5dbd3054b24b434db5b60bfb36f7ade6`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d24f2f3cafbe18c3b4670d84f15a678aa265a9b90de016ff565157a15c7acc3`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.8-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f21866d81ae3b92303af07fe477794e4e4bf43836de0d41b4c212d4469d41a1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66466448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de95d7c2e2d4cc59123fcfef69442499876a675bb59ab504b9ad78c5881fe85a`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 21:39:27 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 21:39:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 21:39:28 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 21:39:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 21:39:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 21:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:34 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 21:39:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 21:39:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 21:39:45 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 21:39:46 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 21:39:46 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:47 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 21:39:47 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 21:39:47 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:47 GMT
CMD []
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8b53fc582fabf462979a1e3b92dd264069a8c4db48d483900b12ffaf539203`  
		Last Modified: Wed, 01 Sep 2021 21:41:00 GMT  
		Size: 1.9 MB (1909030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6288aa69581811c8fced6884b0ce72c344df8f72b9317062be7b6672c538444`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a48a30fd82efeed488ce352f8151d74bb4484cd178fc5fd08e6a8ccfc69560`  
		Last Modified: Wed, 01 Sep 2021 21:41:06 GMT  
		Size: 55.4 MB (55420270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fb6b55a7508af4b07b8ca08ae9f62ea7c5aa6bf46bc94cca92c15f6f418faf`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8605ad73716feec4bef5573f92fe2b1472d4e43804d33bd45d3656b83af314c`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ddbc92192571b4db6ee00ea2473aa0cdb78b7628f95560f0571a4ac15e330a`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373ff707a384f2d3eeae1ec32f9044142bb5c896541416c18d1bf45142da30ae`  
		Last Modified: Wed, 01 Sep 2021 21:41:30 GMT  
		Size: 6.4 MB (6418561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436d94df880147a87f1fba1c3115c37eb4b50c95fc93694f4d5e1fc22f353fd3`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ada35578ff611689fc1c810d1603dd6b6c606175e97737d9f3073f4631235b0`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fcd3a1f2fec5765d757040410b3f777d30970931dd552544b55ada1dc9ebe8`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8-dind-alpine3.14`

```console
$ docker pull docker@sha256:1efacb06edbb1e2bd4a39dcc69883866c7dd98562a49fa97d7d29c2da1c3974f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.8-dind-alpine3.14` - linux; amd64

```console
$ docker pull docker@sha256:903b889a009176428a2c11ad1b0e72135d07fd51f56db7042b8119eafb808112
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72561611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e5d106d317b2ddf45e60b5ba90a53082d306fac5c96e36ef3f2ad48e9719adb`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 22:19:34 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 22:19:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 22:19:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 22:19:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 22:19:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 22:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:42 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 22:19:48 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 22:19:48 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 22:19:49 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 22:19:49 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 22:19:50 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:50 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 22:19:50 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 22:19:50 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:50 GMT
CMD []
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14df950e5a796f46eb6615169002a1c428bd908141de49fb35ec026c206e77aa`  
		Last Modified: Wed, 01 Sep 2021 22:20:33 GMT  
		Size: 1.9 MB (1935099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a31cc9e913427e8959328b7d290bdcc639a9f84c11956c33c0ce112788cf19`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a4137012260e097fc6b4bf6d75ba3b193acb399fb1276687303dea63ba519c`  
		Last Modified: Wed, 01 Sep 2021 22:20:40 GMT  
		Size: 61.3 MB (61283898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d92eaf14165f5a5883286b050c77b9c7022efbde954c3b7e96e92565515f0a`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e701314a31132c239baf0de9d4922559fc419c445e13c9ce7ffd8b4518b4f98e`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea1be2ff281d99199cd048ef3bf1464615aec1ca9abfc20e73838913432dc0`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb11622685e894072cc7fb1688ea686f6b0c903c25fda9d6f41915b279ce29`  
		Last Modified: Wed, 01 Sep 2021 22:21:00 GMT  
		Size: 6.5 MB (6521412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3448405a219f5e629e26687cfb38c611068e556983153df486257e8cf73a99`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf064520bf422a76e00ad9efafcb13da5dbd3054b24b434db5b60bfb36f7ade6`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d24f2f3cafbe18c3b4670d84f15a678aa265a9b90de016ff565157a15c7acc3`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.8-dind-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f21866d81ae3b92303af07fe477794e4e4bf43836de0d41b4c212d4469d41a1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66466448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de95d7c2e2d4cc59123fcfef69442499876a675bb59ab504b9ad78c5881fe85a`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 21:39:27 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 21:39:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 21:39:28 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 21:39:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 21:39:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 21:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:34 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 21:39:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 21:39:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 21:39:45 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 21:39:46 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 21:39:46 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:47 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 21:39:47 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 21:39:47 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:47 GMT
CMD []
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8b53fc582fabf462979a1e3b92dd264069a8c4db48d483900b12ffaf539203`  
		Last Modified: Wed, 01 Sep 2021 21:41:00 GMT  
		Size: 1.9 MB (1909030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6288aa69581811c8fced6884b0ce72c344df8f72b9317062be7b6672c538444`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a48a30fd82efeed488ce352f8151d74bb4484cd178fc5fd08e6a8ccfc69560`  
		Last Modified: Wed, 01 Sep 2021 21:41:06 GMT  
		Size: 55.4 MB (55420270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fb6b55a7508af4b07b8ca08ae9f62ea7c5aa6bf46bc94cca92c15f6f418faf`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8605ad73716feec4bef5573f92fe2b1472d4e43804d33bd45d3656b83af314c`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ddbc92192571b4db6ee00ea2473aa0cdb78b7628f95560f0571a4ac15e330a`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373ff707a384f2d3eeae1ec32f9044142bb5c896541416c18d1bf45142da30ae`  
		Last Modified: Wed, 01 Sep 2021 21:41:30 GMT  
		Size: 6.4 MB (6418561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436d94df880147a87f1fba1c3115c37eb4b50c95fc93694f4d5e1fc22f353fd3`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ada35578ff611689fc1c810d1603dd6b6c606175e97737d9f3073f4631235b0`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fcd3a1f2fec5765d757040410b3f777d30970931dd552544b55ada1dc9ebe8`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8-dind-rootless`

```console
$ docker pull docker@sha256:d75833c3ed601b634c871302b025c4fd070816e8e81394f1bf7161658a49da3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.8-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:ec2140865f2bc0705f6d17a575b2036e5d60a768007321245faa9eebdc031488
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.8 MB (92828157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5ff4e7c8157ca219e02e8525c28f1a8350b01b405a72860e2c926a26a8e9d6b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 22:19:34 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 22:19:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 22:19:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 22:19:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 22:19:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 22:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:42 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 22:19:48 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 22:19:48 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 22:19:49 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 22:19:49 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 22:19:50 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:50 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 22:19:50 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 22:19:50 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:50 GMT
CMD []
# Wed, 01 Sep 2021 22:19:55 GMT
RUN apk add --no-cache iproute2
# Wed, 01 Sep 2021 22:19:56 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Sep 2021 22:19:57 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Sep 2021 22:19:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Sep 2021 22:19:59 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Sep 2021 22:20:00 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Sep 2021 22:20:00 GMT
USER rootless
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14df950e5a796f46eb6615169002a1c428bd908141de49fb35ec026c206e77aa`  
		Last Modified: Wed, 01 Sep 2021 22:20:33 GMT  
		Size: 1.9 MB (1935099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a31cc9e913427e8959328b7d290bdcc639a9f84c11956c33c0ce112788cf19`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a4137012260e097fc6b4bf6d75ba3b193acb399fb1276687303dea63ba519c`  
		Last Modified: Wed, 01 Sep 2021 22:20:40 GMT  
		Size: 61.3 MB (61283898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d92eaf14165f5a5883286b050c77b9c7022efbde954c3b7e96e92565515f0a`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e701314a31132c239baf0de9d4922559fc419c445e13c9ce7ffd8b4518b4f98e`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea1be2ff281d99199cd048ef3bf1464615aec1ca9abfc20e73838913432dc0`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb11622685e894072cc7fb1688ea686f6b0c903c25fda9d6f41915b279ce29`  
		Last Modified: Wed, 01 Sep 2021 22:21:00 GMT  
		Size: 6.5 MB (6521412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3448405a219f5e629e26687cfb38c611068e556983153df486257e8cf73a99`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf064520bf422a76e00ad9efafcb13da5dbd3054b24b434db5b60bfb36f7ade6`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d24f2f3cafbe18c3b4670d84f15a678aa265a9b90de016ff565157a15c7acc3`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ee8eb2774788b07752bfe9bada2565d0759149471b1e1184fe1b8b9b723291`  
		Last Modified: Wed, 01 Sep 2021 22:21:20 GMT  
		Size: 1.1 MB (1148735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4811cca51263afbb69cb08a00b9ced312530c69efdd89d18432a10d708b9793`  
		Last Modified: Wed, 01 Sep 2021 22:21:20 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1196b78c6ec13dfea9317ce19a5c0297ffa1b7bb71c9cbdcbd8898a7d1c488fe`  
		Last Modified: Wed, 01 Sep 2021 22:21:20 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951aa128211fa2e81475296d3178c72f82de1b9b0fca6577a41522b421d33333`  
		Last Modified: Wed, 01 Sep 2021 22:21:23 GMT  
		Size: 19.1 MB (19116094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b58b08848076b0b593d64fb903397d255b9467bb9f93f4492d852beb23532af`  
		Last Modified: Wed, 01 Sep 2021 22:21:20 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.8-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:01a3353757a17aa2125c2a6181c436134d7a0055df0ef3ba323826350e1d0ff1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88731007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bcfee17c3e4c3e92f1ae3c5a77520971a3633eebf269f8a4a895634a5ad06c2`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 21:39:27 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 21:39:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 21:39:28 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 21:39:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 21:39:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 21:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:34 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 21:39:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 21:39:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 21:39:45 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 21:39:46 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 21:39:46 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:47 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 21:39:47 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 21:39:47 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:47 GMT
CMD []
# Wed, 01 Sep 2021 21:39:55 GMT
RUN apk add --no-cache iproute2
# Wed, 01 Sep 2021 21:39:56 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Sep 2021 21:39:57 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Sep 2021 21:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Sep 2021 21:39:59 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Sep 2021 21:39:59 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Sep 2021 21:39:59 GMT
USER rootless
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8b53fc582fabf462979a1e3b92dd264069a8c4db48d483900b12ffaf539203`  
		Last Modified: Wed, 01 Sep 2021 21:41:00 GMT  
		Size: 1.9 MB (1909030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6288aa69581811c8fced6884b0ce72c344df8f72b9317062be7b6672c538444`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a48a30fd82efeed488ce352f8151d74bb4484cd178fc5fd08e6a8ccfc69560`  
		Last Modified: Wed, 01 Sep 2021 21:41:06 GMT  
		Size: 55.4 MB (55420270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fb6b55a7508af4b07b8ca08ae9f62ea7c5aa6bf46bc94cca92c15f6f418faf`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8605ad73716feec4bef5573f92fe2b1472d4e43804d33bd45d3656b83af314c`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ddbc92192571b4db6ee00ea2473aa0cdb78b7628f95560f0571a4ac15e330a`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373ff707a384f2d3eeae1ec32f9044142bb5c896541416c18d1bf45142da30ae`  
		Last Modified: Wed, 01 Sep 2021 21:41:30 GMT  
		Size: 6.4 MB (6418561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436d94df880147a87f1fba1c3115c37eb4b50c95fc93694f4d5e1fc22f353fd3`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ada35578ff611689fc1c810d1603dd6b6c606175e97737d9f3073f4631235b0`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fcd3a1f2fec5765d757040410b3f777d30970931dd552544b55ada1dc9ebe8`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0727607c4852e6356bf01e7ea1c0d090e6100e1045cd881eca01515749b53e6`  
		Last Modified: Wed, 01 Sep 2021 21:41:53 GMT  
		Size: 1.2 MB (1168111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee229379e57fe13e75a06a3453c3afa2ec3959e936165ad25b24fa00a2bec57`  
		Last Modified: Wed, 01 Sep 2021 21:41:53 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5c0508be8bb4e91bd2c3895baa8ee248bf3b1bb5bd9d605a8c5da8b4aeff1a`  
		Last Modified: Wed, 01 Sep 2021 21:41:53 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dc3c7f21a4603739eb746480b3aa01086f70941d2b2141504e7c7e796a1bab`  
		Last Modified: Wed, 01 Sep 2021 21:41:57 GMT  
		Size: 21.1 MB (21094732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da3b6b5f43f82f2e3e8c853aefbe98b52cbd1ff0fc99294851db16ee9eefa2f`  
		Last Modified: Wed, 01 Sep 2021 21:41:53 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8-git`

```console
$ docker pull docker@sha256:d7f576652c05a6e86970cbdb477d4bb5d30932599806786e126067e406ef59cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.8-git` - linux; amd64

```console
$ docker pull docker@sha256:5ccbe97e61943749d3f7aa5f14caa1265de865ae65eba21798943588a7ed9796
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72665297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94f59df6fc6382ef41eefeb7025d1db3fc3f724644192060b565cc1c010df180`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 22:19:34 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 22:19:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 22:19:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 22:19:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 22:19:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 22:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:42 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 22:20:05 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14df950e5a796f46eb6615169002a1c428bd908141de49fb35ec026c206e77aa`  
		Last Modified: Wed, 01 Sep 2021 22:20:33 GMT  
		Size: 1.9 MB (1935099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a31cc9e913427e8959328b7d290bdcc639a9f84c11956c33c0ce112788cf19`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a4137012260e097fc6b4bf6d75ba3b193acb399fb1276687303dea63ba519c`  
		Last Modified: Wed, 01 Sep 2021 22:20:40 GMT  
		Size: 61.3 MB (61283898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d92eaf14165f5a5883286b050c77b9c7022efbde954c3b7e96e92565515f0a`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e701314a31132c239baf0de9d4922559fc419c445e13c9ce7ffd8b4518b4f98e`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea1be2ff281d99199cd048ef3bf1464615aec1ca9abfc20e73838913432dc0`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7649c299d9b594bf34994b3bda767e79eca59d49cbc5e59c93e350890fce080`  
		Last Modified: Wed, 01 Sep 2021 22:21:42 GMT  
		Size: 6.6 MB (6629988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.8-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4951d55d07df56eb3dc8823e5abb438f05ced009af250666aab6381f9ef2a99c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.8 MB (66784792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c1f1eae55906bc481ffd709ea71e35a3f9aa3dde59572a62cadf79d7442716`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 21:39:27 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 21:39:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 21:39:28 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 21:39:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 21:39:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 21:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:34 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 21:40:07 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8b53fc582fabf462979a1e3b92dd264069a8c4db48d483900b12ffaf539203`  
		Last Modified: Wed, 01 Sep 2021 21:41:00 GMT  
		Size: 1.9 MB (1909030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6288aa69581811c8fced6884b0ce72c344df8f72b9317062be7b6672c538444`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a48a30fd82efeed488ce352f8151d74bb4484cd178fc5fd08e6a8ccfc69560`  
		Last Modified: Wed, 01 Sep 2021 21:41:06 GMT  
		Size: 55.4 MB (55420270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fb6b55a7508af4b07b8ca08ae9f62ea7c5aa6bf46bc94cca92c15f6f418faf`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8605ad73716feec4bef5573f92fe2b1472d4e43804d33bd45d3656b83af314c`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ddbc92192571b4db6ee00ea2473aa0cdb78b7628f95560f0571a4ac15e330a`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac87a5e4495fa9d6f260ed353f2f2ed60461d2ccc2fcce309f3a0ab5cfe2a01`  
		Last Modified: Wed, 01 Sep 2021 21:42:18 GMT  
		Size: 6.7 MB (6741800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8-windowsservercore`

```console
$ docker pull docker@sha256:f4af31b74a5253ec58671de6c2710e16a5f2ac2817548c6a7e2154049cbc3bf2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `docker:20.10.8-windowsservercore` - windows version 10.0.17763.2183; amd64

```console
$ docker pull docker@sha256:a9020b9c4925433869c0c958d9e53f8ad2176330779b65f82f4bf310ea4bc9ab
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737923247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1ab891d90a3bc1ec92ff32071fc677c238ee44a43d6eb073003da02862bd7d8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 19:24:35 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Sep 2021 19:24:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 15 Sep 2021 19:24:37 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Wed, 15 Sep 2021 19:25:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f6f3cf73df901f0ef53d2cf3a1187cb87ff309f8b28b24c1adcc34ea9ad1`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 353.9 KB (353857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451d02c3ec1421ec5056fe967d7be6a344cb53cfd77445f76f4b50483cfae635`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5f2c36a2ae93fffd565b76d88402e7eb238d7097f5ea1c17d64a5d85d745ac`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f40204892cf05231048b06e8d6fb355be34ff937c4cfe6ac6cecb768f816d1d`  
		Last Modified: Wed, 15 Sep 2021 19:26:08 GMT  
		Size: 50.9 MB (50867243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8-windowsservercore-1809`

```console
$ docker pull docker@sha256:f4af31b74a5253ec58671de6c2710e16a5f2ac2817548c6a7e2154049cbc3bf2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `docker:20.10.8-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull docker@sha256:a9020b9c4925433869c0c958d9e53f8ad2176330779b65f82f4bf310ea4bc9ab
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737923247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1ab891d90a3bc1ec92ff32071fc677c238ee44a43d6eb073003da02862bd7d8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 19:24:35 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Sep 2021 19:24:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 15 Sep 2021 19:24:37 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Wed, 15 Sep 2021 19:25:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f6f3cf73df901f0ef53d2cf3a1187cb87ff309f8b28b24c1adcc34ea9ad1`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 353.9 KB (353857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451d02c3ec1421ec5056fe967d7be6a344cb53cfd77445f76f4b50483cfae635`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5f2c36a2ae93fffd565b76d88402e7eb238d7097f5ea1c17d64a5d85d745ac`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f40204892cf05231048b06e8d6fb355be34ff937c4cfe6ac6cecb768f816d1d`  
		Last Modified: Wed, 15 Sep 2021 19:26:08 GMT  
		Size: 50.9 MB (50867243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:1efacb06edbb1e2bd4a39dcc69883866c7dd98562a49fa97d7d29c2da1c3974f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:903b889a009176428a2c11ad1b0e72135d07fd51f56db7042b8119eafb808112
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72561611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e5d106d317b2ddf45e60b5ba90a53082d306fac5c96e36ef3f2ad48e9719adb`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 22:19:34 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 22:19:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 22:19:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 22:19:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 22:19:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 22:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:42 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 22:19:48 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 22:19:48 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 22:19:49 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 22:19:49 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 22:19:50 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:50 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 22:19:50 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 22:19:50 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:50 GMT
CMD []
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14df950e5a796f46eb6615169002a1c428bd908141de49fb35ec026c206e77aa`  
		Last Modified: Wed, 01 Sep 2021 22:20:33 GMT  
		Size: 1.9 MB (1935099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a31cc9e913427e8959328b7d290bdcc639a9f84c11956c33c0ce112788cf19`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a4137012260e097fc6b4bf6d75ba3b193acb399fb1276687303dea63ba519c`  
		Last Modified: Wed, 01 Sep 2021 22:20:40 GMT  
		Size: 61.3 MB (61283898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d92eaf14165f5a5883286b050c77b9c7022efbde954c3b7e96e92565515f0a`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e701314a31132c239baf0de9d4922559fc419c445e13c9ce7ffd8b4518b4f98e`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea1be2ff281d99199cd048ef3bf1464615aec1ca9abfc20e73838913432dc0`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb11622685e894072cc7fb1688ea686f6b0c903c25fda9d6f41915b279ce29`  
		Last Modified: Wed, 01 Sep 2021 22:21:00 GMT  
		Size: 6.5 MB (6521412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3448405a219f5e629e26687cfb38c611068e556983153df486257e8cf73a99`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf064520bf422a76e00ad9efafcb13da5dbd3054b24b434db5b60bfb36f7ade6`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d24f2f3cafbe18c3b4670d84f15a678aa265a9b90de016ff565157a15c7acc3`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f21866d81ae3b92303af07fe477794e4e4bf43836de0d41b4c212d4469d41a1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66466448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de95d7c2e2d4cc59123fcfef69442499876a675bb59ab504b9ad78c5881fe85a`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 21:39:27 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 21:39:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 21:39:28 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 21:39:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 21:39:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 21:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:34 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 21:39:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 21:39:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 21:39:45 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 21:39:46 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 21:39:46 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:47 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 21:39:47 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 21:39:47 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:47 GMT
CMD []
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8b53fc582fabf462979a1e3b92dd264069a8c4db48d483900b12ffaf539203`  
		Last Modified: Wed, 01 Sep 2021 21:41:00 GMT  
		Size: 1.9 MB (1909030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6288aa69581811c8fced6884b0ce72c344df8f72b9317062be7b6672c538444`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a48a30fd82efeed488ce352f8151d74bb4484cd178fc5fd08e6a8ccfc69560`  
		Last Modified: Wed, 01 Sep 2021 21:41:06 GMT  
		Size: 55.4 MB (55420270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fb6b55a7508af4b07b8ca08ae9f62ea7c5aa6bf46bc94cca92c15f6f418faf`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8605ad73716feec4bef5573f92fe2b1472d4e43804d33bd45d3656b83af314c`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ddbc92192571b4db6ee00ea2473aa0cdb78b7628f95560f0571a4ac15e330a`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373ff707a384f2d3eeae1ec32f9044142bb5c896541416c18d1bf45142da30ae`  
		Last Modified: Wed, 01 Sep 2021 21:41:30 GMT  
		Size: 6.4 MB (6418561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436d94df880147a87f1fba1c3115c37eb4b50c95fc93694f4d5e1fc22f353fd3`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ada35578ff611689fc1c810d1603dd6b6c606175e97737d9f3073f4631235b0`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fcd3a1f2fec5765d757040410b3f777d30970931dd552544b55ada1dc9ebe8`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:d75833c3ed601b634c871302b025c4fd070816e8e81394f1bf7161658a49da3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:ec2140865f2bc0705f6d17a575b2036e5d60a768007321245faa9eebdc031488
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.8 MB (92828157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5ff4e7c8157ca219e02e8525c28f1a8350b01b405a72860e2c926a26a8e9d6b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 22:19:34 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 22:19:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 22:19:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 22:19:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 22:19:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 22:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:42 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 22:19:48 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 22:19:48 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 22:19:49 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 22:19:49 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 22:19:50 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:50 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 22:19:50 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 22:19:50 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:50 GMT
CMD []
# Wed, 01 Sep 2021 22:19:55 GMT
RUN apk add --no-cache iproute2
# Wed, 01 Sep 2021 22:19:56 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Sep 2021 22:19:57 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Sep 2021 22:19:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Sep 2021 22:19:59 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Sep 2021 22:20:00 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Sep 2021 22:20:00 GMT
USER rootless
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14df950e5a796f46eb6615169002a1c428bd908141de49fb35ec026c206e77aa`  
		Last Modified: Wed, 01 Sep 2021 22:20:33 GMT  
		Size: 1.9 MB (1935099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a31cc9e913427e8959328b7d290bdcc639a9f84c11956c33c0ce112788cf19`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a4137012260e097fc6b4bf6d75ba3b193acb399fb1276687303dea63ba519c`  
		Last Modified: Wed, 01 Sep 2021 22:20:40 GMT  
		Size: 61.3 MB (61283898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d92eaf14165f5a5883286b050c77b9c7022efbde954c3b7e96e92565515f0a`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e701314a31132c239baf0de9d4922559fc419c445e13c9ce7ffd8b4518b4f98e`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea1be2ff281d99199cd048ef3bf1464615aec1ca9abfc20e73838913432dc0`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb11622685e894072cc7fb1688ea686f6b0c903c25fda9d6f41915b279ce29`  
		Last Modified: Wed, 01 Sep 2021 22:21:00 GMT  
		Size: 6.5 MB (6521412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3448405a219f5e629e26687cfb38c611068e556983153df486257e8cf73a99`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf064520bf422a76e00ad9efafcb13da5dbd3054b24b434db5b60bfb36f7ade6`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d24f2f3cafbe18c3b4670d84f15a678aa265a9b90de016ff565157a15c7acc3`  
		Last Modified: Wed, 01 Sep 2021 22:20:59 GMT  
		Size: 2.6 KB (2614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ee8eb2774788b07752bfe9bada2565d0759149471b1e1184fe1b8b9b723291`  
		Last Modified: Wed, 01 Sep 2021 22:21:20 GMT  
		Size: 1.1 MB (1148735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4811cca51263afbb69cb08a00b9ced312530c69efdd89d18432a10d708b9793`  
		Last Modified: Wed, 01 Sep 2021 22:21:20 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1196b78c6ec13dfea9317ce19a5c0297ffa1b7bb71c9cbdcbd8898a7d1c488fe`  
		Last Modified: Wed, 01 Sep 2021 22:21:20 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951aa128211fa2e81475296d3178c72f82de1b9b0fca6577a41522b421d33333`  
		Last Modified: Wed, 01 Sep 2021 22:21:23 GMT  
		Size: 19.1 MB (19116094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b58b08848076b0b593d64fb903397d255b9467bb9f93f4492d852beb23532af`  
		Last Modified: Wed, 01 Sep 2021 22:21:20 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:01a3353757a17aa2125c2a6181c436134d7a0055df0ef3ba323826350e1d0ff1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88731007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bcfee17c3e4c3e92f1ae3c5a77520971a3633eebf269f8a4a895634a5ad06c2`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 21:39:27 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 21:39:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 21:39:28 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 21:39:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 21:39:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 21:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:34 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 21:39:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Sep 2021 21:39:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Sep 2021 21:39:45 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Sep 2021 21:39:46 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Sep 2021 21:39:46 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:47 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Sep 2021 21:39:47 GMT
EXPOSE 2375 2376
# Wed, 01 Sep 2021 21:39:47 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:47 GMT
CMD []
# Wed, 01 Sep 2021 21:39:55 GMT
RUN apk add --no-cache iproute2
# Wed, 01 Sep 2021 21:39:56 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Sep 2021 21:39:57 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Sep 2021 21:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Sep 2021 21:39:59 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Sep 2021 21:39:59 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Sep 2021 21:39:59 GMT
USER rootless
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8b53fc582fabf462979a1e3b92dd264069a8c4db48d483900b12ffaf539203`  
		Last Modified: Wed, 01 Sep 2021 21:41:00 GMT  
		Size: 1.9 MB (1909030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6288aa69581811c8fced6884b0ce72c344df8f72b9317062be7b6672c538444`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a48a30fd82efeed488ce352f8151d74bb4484cd178fc5fd08e6a8ccfc69560`  
		Last Modified: Wed, 01 Sep 2021 21:41:06 GMT  
		Size: 55.4 MB (55420270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fb6b55a7508af4b07b8ca08ae9f62ea7c5aa6bf46bc94cca92c15f6f418faf`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8605ad73716feec4bef5573f92fe2b1472d4e43804d33bd45d3656b83af314c`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ddbc92192571b4db6ee00ea2473aa0cdb78b7628f95560f0571a4ac15e330a`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373ff707a384f2d3eeae1ec32f9044142bb5c896541416c18d1bf45142da30ae`  
		Last Modified: Wed, 01 Sep 2021 21:41:30 GMT  
		Size: 6.4 MB (6418561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436d94df880147a87f1fba1c3115c37eb4b50c95fc93694f4d5e1fc22f353fd3`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ada35578ff611689fc1c810d1603dd6b6c606175e97737d9f3073f4631235b0`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fcd3a1f2fec5765d757040410b3f777d30970931dd552544b55ada1dc9ebe8`  
		Last Modified: Wed, 01 Sep 2021 21:41:29 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0727607c4852e6356bf01e7ea1c0d090e6100e1045cd881eca01515749b53e6`  
		Last Modified: Wed, 01 Sep 2021 21:41:53 GMT  
		Size: 1.2 MB (1168111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee229379e57fe13e75a06a3453c3afa2ec3959e936165ad25b24fa00a2bec57`  
		Last Modified: Wed, 01 Sep 2021 21:41:53 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5c0508be8bb4e91bd2c3895baa8ee248bf3b1bb5bd9d605a8c5da8b4aeff1a`  
		Last Modified: Wed, 01 Sep 2021 21:41:53 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dc3c7f21a4603739eb746480b3aa01086f70941d2b2141504e7c7e796a1bab`  
		Last Modified: Wed, 01 Sep 2021 21:41:57 GMT  
		Size: 21.1 MB (21094732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da3b6b5f43f82f2e3e8c853aefbe98b52cbd1ff0fc99294851db16ee9eefa2f`  
		Last Modified: Wed, 01 Sep 2021 21:41:53 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:d7f576652c05a6e86970cbdb477d4bb5d30932599806786e126067e406ef59cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:5ccbe97e61943749d3f7aa5f14caa1265de865ae65eba21798943588a7ed9796
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72665297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94f59df6fc6382ef41eefeb7025d1db3fc3f724644192060b565cc1c010df180`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 22:19:34 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 22:19:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 22:19:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 22:19:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 22:19:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 22:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:42 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 22:20:05 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14df950e5a796f46eb6615169002a1c428bd908141de49fb35ec026c206e77aa`  
		Last Modified: Wed, 01 Sep 2021 22:20:33 GMT  
		Size: 1.9 MB (1935099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a31cc9e913427e8959328b7d290bdcc639a9f84c11956c33c0ce112788cf19`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a4137012260e097fc6b4bf6d75ba3b193acb399fb1276687303dea63ba519c`  
		Last Modified: Wed, 01 Sep 2021 22:20:40 GMT  
		Size: 61.3 MB (61283898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d92eaf14165f5a5883286b050c77b9c7022efbde954c3b7e96e92565515f0a`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e701314a31132c239baf0de9d4922559fc419c445e13c9ce7ffd8b4518b4f98e`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea1be2ff281d99199cd048ef3bf1464615aec1ca9abfc20e73838913432dc0`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7649c299d9b594bf34994b3bda767e79eca59d49cbc5e59c93e350890fce080`  
		Last Modified: Wed, 01 Sep 2021 22:21:42 GMT  
		Size: 6.6 MB (6629988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4951d55d07df56eb3dc8823e5abb438f05ced009af250666aab6381f9ef2a99c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.8 MB (66784792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c1f1eae55906bc481ffd709ea71e35a3f9aa3dde59572a62cadf79d7442716`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 21:39:27 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 21:39:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 21:39:28 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 21:39:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 21:39:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 21:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:34 GMT
CMD ["sh"]
# Wed, 01 Sep 2021 21:40:07 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8b53fc582fabf462979a1e3b92dd264069a8c4db48d483900b12ffaf539203`  
		Last Modified: Wed, 01 Sep 2021 21:41:00 GMT  
		Size: 1.9 MB (1909030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6288aa69581811c8fced6884b0ce72c344df8f72b9317062be7b6672c538444`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a48a30fd82efeed488ce352f8151d74bb4484cd178fc5fd08e6a8ccfc69560`  
		Last Modified: Wed, 01 Sep 2021 21:41:06 GMT  
		Size: 55.4 MB (55420270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fb6b55a7508af4b07b8ca08ae9f62ea7c5aa6bf46bc94cca92c15f6f418faf`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8605ad73716feec4bef5573f92fe2b1472d4e43804d33bd45d3656b83af314c`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ddbc92192571b4db6ee00ea2473aa0cdb78b7628f95560f0571a4ac15e330a`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac87a5e4495fa9d6f260ed353f2f2ed60461d2ccc2fcce309f3a0ab5cfe2a01`  
		Last Modified: Wed, 01 Sep 2021 21:42:18 GMT  
		Size: 6.7 MB (6741800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:63107bd6ce718f130bb2668704239467b74f034c446f9e9c4ae1ffa5ddf4e3dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:6ac2f3862aa1353a5fe6bf12439f3e56e695e56d7c3098898c96ef33eae78bf9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (66035309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc6c0ffef6650bcfbb0afd5a07b813b5ccf1d00ecddccadb85123c6ee57a7995`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 22:19:34 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 22:19:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 22:19:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 22:19:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 22:19:40 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 22:19:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 22:19:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 22:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 22:19:42 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14df950e5a796f46eb6615169002a1c428bd908141de49fb35ec026c206e77aa`  
		Last Modified: Wed, 01 Sep 2021 22:20:33 GMT  
		Size: 1.9 MB (1935099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a31cc9e913427e8959328b7d290bdcc639a9f84c11956c33c0ce112788cf19`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a4137012260e097fc6b4bf6d75ba3b193acb399fb1276687303dea63ba519c`  
		Last Modified: Wed, 01 Sep 2021 22:20:40 GMT  
		Size: 61.3 MB (61283898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d92eaf14165f5a5883286b050c77b9c7022efbde954c3b7e96e92565515f0a`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e701314a31132c239baf0de9d4922559fc419c445e13c9ce7ffd8b4518b4f98e`  
		Last Modified: Wed, 01 Sep 2021 22:20:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea1be2ff281d99199cd048ef3bf1464615aec1ca9abfc20e73838913432dc0`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:2fad5f90265a7c9c4ee73f0b0eaa7b5ed8203af4cd0464dda8f7e1f4b28a5ad7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (60042992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3734d5adc5ac9557175d6c0acb930e7ed6d75e1f2e52e8c170b4ade3f76806a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 21:39:27 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 21:39:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 21:39:28 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 21:39:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 21:39:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 21:39:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 21:39:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 21:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 21:39:34 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8b53fc582fabf462979a1e3b92dd264069a8c4db48d483900b12ffaf539203`  
		Last Modified: Wed, 01 Sep 2021 21:41:00 GMT  
		Size: 1.9 MB (1909030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6288aa69581811c8fced6884b0ce72c344df8f72b9317062be7b6672c538444`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a48a30fd82efeed488ce352f8151d74bb4484cd178fc5fd08e6a8ccfc69560`  
		Last Modified: Wed, 01 Sep 2021 21:41:06 GMT  
		Size: 55.4 MB (55420270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fb6b55a7508af4b07b8ca08ae9f62ea7c5aa6bf46bc94cca92c15f6f418faf`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8605ad73716feec4bef5573f92fe2b1472d4e43804d33bd45d3656b83af314c`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ddbc92192571b4db6ee00ea2473aa0cdb78b7628f95560f0571a4ac15e330a`  
		Last Modified: Wed, 01 Sep 2021 21:40:56 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore`

```console
$ docker pull docker@sha256:f4af31b74a5253ec58671de6c2710e16a5f2ac2817548c6a7e2154049cbc3bf2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `docker:windowsservercore` - windows version 10.0.17763.2183; amd64

```console
$ docker pull docker@sha256:a9020b9c4925433869c0c958d9e53f8ad2176330779b65f82f4bf310ea4bc9ab
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737923247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1ab891d90a3bc1ec92ff32071fc677c238ee44a43d6eb073003da02862bd7d8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 19:24:35 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Sep 2021 19:24:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 15 Sep 2021 19:24:37 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Wed, 15 Sep 2021 19:25:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f6f3cf73df901f0ef53d2cf3a1187cb87ff309f8b28b24c1adcc34ea9ad1`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 353.9 KB (353857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451d02c3ec1421ec5056fe967d7be6a344cb53cfd77445f76f4b50483cfae635`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5f2c36a2ae93fffd565b76d88402e7eb238d7097f5ea1c17d64a5d85d745ac`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f40204892cf05231048b06e8d6fb355be34ff937c4cfe6ac6cecb768f816d1d`  
		Last Modified: Wed, 15 Sep 2021 19:26:08 GMT  
		Size: 50.9 MB (50867243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:f4af31b74a5253ec58671de6c2710e16a5f2ac2817548c6a7e2154049cbc3bf2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull docker@sha256:a9020b9c4925433869c0c958d9e53f8ad2176330779b65f82f4bf310ea4bc9ab
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737923247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1ab891d90a3bc1ec92ff32071fc677c238ee44a43d6eb073003da02862bd7d8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 19:24:35 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Sep 2021 19:24:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 15 Sep 2021 19:24:37 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Wed, 15 Sep 2021 19:25:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f6f3cf73df901f0ef53d2cf3a1187cb87ff309f8b28b24c1adcc34ea9ad1`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 353.9 KB (353857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451d02c3ec1421ec5056fe967d7be6a344cb53cfd77445f76f4b50483cfae635`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5f2c36a2ae93fffd565b76d88402e7eb238d7097f5ea1c17d64a5d85d745ac`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f40204892cf05231048b06e8d6fb355be34ff937c4cfe6ac6cecb768f816d1d`  
		Last Modified: Wed, 15 Sep 2021 19:26:08 GMT  
		Size: 50.9 MB (50867243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
