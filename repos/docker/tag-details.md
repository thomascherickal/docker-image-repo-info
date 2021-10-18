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
-	[`docker:20.10-rc`](#docker2010-rc)
-	[`docker:20.10-rc-dind`](#docker2010-rc-dind)
-	[`docker:20.10-rc-dind-rootless`](#docker2010-rc-dind-rootless)
-	[`docker:20.10-rc-git`](#docker2010-rc-git)
-	[`docker:20.10-rc-windowsservercore`](#docker2010-rc-windowsservercore)
-	[`docker:20.10-rc-windowsservercore-1809`](#docker2010-rc-windowsservercore-1809)
-	[`docker:20.10-windowsservercore`](#docker2010-windowsservercore)
-	[`docker:20.10-windowsservercore-1809`](#docker2010-windowsservercore-1809)
-	[`docker:20.10.10-rc1`](#docker201010-rc1)
-	[`docker:20.10.10-rc1-alpine3.14`](#docker201010-rc1-alpine314)
-	[`docker:20.10.10-rc1-dind`](#docker201010-rc1-dind)
-	[`docker:20.10.10-rc1-dind-alpine3.14`](#docker201010-rc1-dind-alpine314)
-	[`docker:20.10.10-rc1-dind-rootless`](#docker201010-rc1-dind-rootless)
-	[`docker:20.10.10-rc1-git`](#docker201010-rc1-git)
-	[`docker:20.10.10-rc1-windowsservercore`](#docker201010-rc1-windowsservercore)
-	[`docker:20.10.10-rc1-windowsservercore-1809`](#docker201010-rc1-windowsservercore-1809)
-	[`docker:20.10.9`](#docker20109)
-	[`docker:20.10.9-alpine3.14`](#docker20109-alpine314)
-	[`docker:20.10.9-dind`](#docker20109-dind)
-	[`docker:20.10.9-dind-alpine3.14`](#docker20109-dind-alpine314)
-	[`docker:20.10.9-dind-rootless`](#docker20109-dind-rootless)
-	[`docker:20.10.9-git`](#docker20109-git)
-	[`docker:20.10.9-windowsservercore`](#docker20109-windowsservercore)
-	[`docker:20.10.9-windowsservercore-1809`](#docker20109-windowsservercore-1809)
-	[`docker:dind`](#dockerdind)
-	[`docker:dind-rootless`](#dockerdind-rootless)
-	[`docker:git`](#dockergit)
-	[`docker:latest`](#dockerlatest)
-	[`docker:rc`](#dockerrc)
-	[`docker:rc-dind`](#dockerrc-dind)
-	[`docker:rc-dind-rootless`](#dockerrc-dind-rootless)
-	[`docker:rc-git`](#dockerrc-git)
-	[`docker:rc-windowsservercore`](#dockerrc-windowsservercore)
-	[`docker:rc-windowsservercore-1809`](#dockerrc-windowsservercore-1809)
-	[`docker:windowsservercore`](#dockerwindowsservercore)
-	[`docker:windowsservercore-1809`](#dockerwindowsservercore-1809)

## `docker:20`

```console
$ docker pull docker@sha256:938bcb85cf77db2b80d219abd5a1424ec15ce11a3adaea6423fa16cc9acfe926
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20` - linux; amd64

```console
$ docker pull docker@sha256:62302357e804b152e157d3603ce7a97c3f368a626ce027eee1d1e02b5ae924f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68441124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6448e722e510f9bb0bb5c2f65ef99295fc2321b656c00f088078ccf6564372b`
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
# Tue, 05 Oct 2021 17:32:23 GMT
ENV DOCKER_VERSION=20.10.9
# Tue, 05 Oct 2021 17:32:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Oct 2021 17:32:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 05 Oct 2021 17:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:31 GMT
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
	-	`sha256:c6e88c3a8ccafbb819665e363fc6947b47a896d85170e8b267c6c12176385b3c`  
		Last Modified: Tue, 05 Oct 2021 17:33:31 GMT  
		Size: 63.7 MB (63689714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e00801cfc09a8e327c9cced9fbc94f179e9f03caf50d0ac1c01ae1ca92c3b`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a43c1017099b38ffcabb7b27169d9ca7821bbfea77b15059c969020a0acfd`  
		Last Modified: Tue, 05 Oct 2021 17:33:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52f4e484f770e1039348c98519c8610f67ba16969fb9ab93afae3f4421f7d1`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1710b19ecaa7eba8537ea64a35ddec333ff128cda5f2f19b7c4cd6e3a4e0daf7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62356500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c324afd4ac0437589f8f6e825c2fed8ef663773f55ac7c8e85cd589f554239d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:40:48 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 18 Oct 2021 21:40:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:59 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bacb27c3d6ff01f6e8f051e37ec17341cc7fbc76073dea248afcf223aba5d`  
		Last Modified: Mon, 18 Oct 2021 21:44:10 GMT  
		Size: 57.7 MB (57733379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79bdbfa9a5540080db6017b27b917e7c21fbf947abefb068a974a0b55d481e`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a13bdd3b1cef3426a41cadec19b55904b133d95c31c10574f56b0419a93f72`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb034e6582742a188487a0bdde846bf28e29179005b5f423b7d465a2c4e368df`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind`

```console
$ docker pull docker@sha256:d842418d21545fde57c2512681d9bdc4ce0e54f2e0305a293ee20a9b6166932b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind` - linux; amd64

```console
$ docker pull docker@sha256:24628ded7711e48db56af875236ac30a8950305ac461332955b3375ac5a87e1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (74967424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1efbbff84703848e1c787073a954e8e3f0146836d94673f2d54f3672296bf82f`
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
# Tue, 05 Oct 2021 17:32:23 GMT
ENV DOCKER_VERSION=20.10.9
# Tue, 05 Oct 2021 17:32:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Oct 2021 17:32:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 05 Oct 2021 17:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:31 GMT
CMD ["sh"]
# Tue, 05 Oct 2021 17:32:37 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 05 Oct 2021 17:32:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 05 Oct 2021 17:32:38 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 05 Oct 2021 17:32:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 05 Oct 2021 17:32:39 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:39 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Oct 2021 17:32:39 GMT
EXPOSE 2375 2376
# Tue, 05 Oct 2021 17:32:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:40 GMT
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
	-	`sha256:c6e88c3a8ccafbb819665e363fc6947b47a896d85170e8b267c6c12176385b3c`  
		Last Modified: Tue, 05 Oct 2021 17:33:31 GMT  
		Size: 63.7 MB (63689714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e00801cfc09a8e327c9cced9fbc94f179e9f03caf50d0ac1c01ae1ca92c3b`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a43c1017099b38ffcabb7b27169d9ca7821bbfea77b15059c969020a0acfd`  
		Last Modified: Tue, 05 Oct 2021 17:33:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52f4e484f770e1039348c98519c8610f67ba16969fb9ab93afae3f4421f7d1`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec67a583a94bdc153dacab38a9b85a032e58cd332069a169388b45727d5a03c`  
		Last Modified: Tue, 05 Oct 2021 17:33:49 GMT  
		Size: 6.5 MB (6521405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a20c97b2389ddc8160afed72508ba7d5ae1464e5837dd19905c4e7130c4e5`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170df0071614602fcd5820d60cc7c9a73f8e10a616928d111e25041951c3507d`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfeb3c70a4f70f3868998e1000a4907ec50a8303595dbf0e96bdd03d59e086c`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:3ba0867a449ca78b731e3251ddeb677fa893dc500293ab0e303a8188b9e4d106
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68779801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6144797d483747bee375b8607893579ff8b6d6ff47e83b10ed4827e4123f549e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:40:48 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 18 Oct 2021 21:40:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:59 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:41:08 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 18 Oct 2021 21:41:08 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:41:09 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 18 Oct 2021 21:41:10 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 18 Oct 2021 21:41:12 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:41:12 GMT
VOLUME [/var/lib/docker]
# Mon, 18 Oct 2021 21:41:13 GMT
EXPOSE 2375 2376
# Mon, 18 Oct 2021 21:41:14 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 18 Oct 2021 21:41:15 GMT
CMD []
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bacb27c3d6ff01f6e8f051e37ec17341cc7fbc76073dea248afcf223aba5d`  
		Last Modified: Mon, 18 Oct 2021 21:44:10 GMT  
		Size: 57.7 MB (57733379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79bdbfa9a5540080db6017b27b917e7c21fbf947abefb068a974a0b55d481e`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a13bdd3b1cef3426a41cadec19b55904b133d95c31c10574f56b0419a93f72`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb034e6582742a188487a0bdde846bf28e29179005b5f423b7d465a2c4e368df`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e8bdd67624c83a9918b7d0bb7d24f84d32a306b3453ac55e213380ee17335d`  
		Last Modified: Mon, 18 Oct 2021 21:44:31 GMT  
		Size: 6.4 MB (6418437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9e9de043d240e7a3e0baf2f1a9bd6bd1da52fd1a1df9db1d97b50b294c98b8`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b746a27963c477864e414004aab19efff02e763e88444128d5bbf735410a4f`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c17f756b76c3b8328ed61cc3fef72a62229860b3a7fefcc6e94edda353b7d3a`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 2.6 KB (2615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:51cd937b2ad1a1d32179f2e9acc01ea46d4e127cdaf493a533172b1fb019af15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:75acfc77a83d9b4d557aab529432058b78ac6d629325c9d61c385cd2fc48fe7c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 MB (95235937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b4aec2427ffe9836431bca031ae4354053a010dae4736917b174d52da90dba`
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
# Tue, 05 Oct 2021 17:32:23 GMT
ENV DOCKER_VERSION=20.10.9
# Tue, 05 Oct 2021 17:32:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Oct 2021 17:32:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 05 Oct 2021 17:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:31 GMT
CMD ["sh"]
# Tue, 05 Oct 2021 17:32:37 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 05 Oct 2021 17:32:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 05 Oct 2021 17:32:38 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 05 Oct 2021 17:32:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 05 Oct 2021 17:32:39 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:39 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Oct 2021 17:32:39 GMT
EXPOSE 2375 2376
# Tue, 05 Oct 2021 17:32:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:40 GMT
CMD []
# Tue, 05 Oct 2021 17:32:44 GMT
RUN apk add --no-cache iproute2
# Tue, 05 Oct 2021 17:32:45 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 05 Oct 2021 17:32:46 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 05 Oct 2021 17:32:48 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 05 Oct 2021 17:32:49 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 05 Oct 2021 17:32:50 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 05 Oct 2021 17:32:50 GMT
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
	-	`sha256:c6e88c3a8ccafbb819665e363fc6947b47a896d85170e8b267c6c12176385b3c`  
		Last Modified: Tue, 05 Oct 2021 17:33:31 GMT  
		Size: 63.7 MB (63689714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e00801cfc09a8e327c9cced9fbc94f179e9f03caf50d0ac1c01ae1ca92c3b`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a43c1017099b38ffcabb7b27169d9ca7821bbfea77b15059c969020a0acfd`  
		Last Modified: Tue, 05 Oct 2021 17:33:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52f4e484f770e1039348c98519c8610f67ba16969fb9ab93afae3f4421f7d1`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec67a583a94bdc153dacab38a9b85a032e58cd332069a169388b45727d5a03c`  
		Last Modified: Tue, 05 Oct 2021 17:33:49 GMT  
		Size: 6.5 MB (6521405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a20c97b2389ddc8160afed72508ba7d5ae1464e5837dd19905c4e7130c4e5`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170df0071614602fcd5820d60cc7c9a73f8e10a616928d111e25041951c3507d`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfeb3c70a4f70f3868998e1000a4907ec50a8303595dbf0e96bdd03d59e086c`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418f850bf44d36d532f71a72ed317e54531b904953d99821dd316e73e777d23c`  
		Last Modified: Tue, 05 Oct 2021 17:34:08 GMT  
		Size: 1.1 MB (1148745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03facf1a1e41afef60e2e7bad46f0fbd44f5b2b3a3328337c3e0a6049120dd8`  
		Last Modified: Tue, 05 Oct 2021 17:34:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f919e685bb3723d38cd895248bb1c99de9588af3aba7f57ef5cb72eca54106a9`  
		Last Modified: Tue, 05 Oct 2021 17:34:08 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79573e4e685e01787d1e021ea1cecb99cdbf78577b160037c6ed2c7f8f2b304`  
		Last Modified: Tue, 05 Oct 2021 17:34:11 GMT  
		Size: 19.1 MB (19118054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7054ab8c007ff95ebed9750aae6c97b9f692ed317ea464234611c57db8601634`  
		Last Modified: Tue, 05 Oct 2021 17:34:08 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:eb9feb96a9c979384276b169446b5134c441625461108344fde1f18fdee9ce75
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.0 MB (91045261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a26cf3ffc31a4748452e2da3ca2a290c3354e441650e7617aaf4a9fbf6d1750`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:40:48 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 18 Oct 2021 21:40:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:59 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:41:08 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 18 Oct 2021 21:41:08 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:41:09 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 18 Oct 2021 21:41:10 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 18 Oct 2021 21:41:12 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:41:12 GMT
VOLUME [/var/lib/docker]
# Mon, 18 Oct 2021 21:41:13 GMT
EXPOSE 2375 2376
# Mon, 18 Oct 2021 21:41:14 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 18 Oct 2021 21:41:15 GMT
CMD []
# Mon, 18 Oct 2021 21:41:23 GMT
RUN apk add --no-cache iproute2
# Mon, 18 Oct 2021 21:41:24 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 18 Oct 2021 21:41:25 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:41:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 18 Oct 2021 21:41:29 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 18 Oct 2021 21:41:30 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 18 Oct 2021 21:41:31 GMT
USER rootless
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bacb27c3d6ff01f6e8f051e37ec17341cc7fbc76073dea248afcf223aba5d`  
		Last Modified: Mon, 18 Oct 2021 21:44:10 GMT  
		Size: 57.7 MB (57733379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79bdbfa9a5540080db6017b27b917e7c21fbf947abefb068a974a0b55d481e`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a13bdd3b1cef3426a41cadec19b55904b133d95c31c10574f56b0419a93f72`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb034e6582742a188487a0bdde846bf28e29179005b5f423b7d465a2c4e368df`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e8bdd67624c83a9918b7d0bb7d24f84d32a306b3453ac55e213380ee17335d`  
		Last Modified: Mon, 18 Oct 2021 21:44:31 GMT  
		Size: 6.4 MB (6418437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9e9de043d240e7a3e0baf2f1a9bd6bd1da52fd1a1df9db1d97b50b294c98b8`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b746a27963c477864e414004aab19efff02e763e88444128d5bbf735410a4f`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c17f756b76c3b8328ed61cc3fef72a62229860b3a7fefcc6e94edda353b7d3a`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 2.6 KB (2615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da73c72dcad0b534b2f4febbace9688a2f4a30bf46b188501e200b3be5977b03`  
		Last Modified: Mon, 18 Oct 2021 21:44:52 GMT  
		Size: 1.2 MB (1167836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff4316d7dcf66341a4e5a7a7519ed9d36f902bb95d2169ebc26549a0f95849`  
		Last Modified: Mon, 18 Oct 2021 21:44:52 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba611fb139d8c880c857badbc205cee357e35952ae811c52e90139e68f959d57`  
		Last Modified: Mon, 18 Oct 2021 21:44:52 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098b6fcc42aecdd56305fc4ceba9415e977d589f359ff58a7ee2c72612859ce9`  
		Last Modified: Mon, 18 Oct 2021 21:44:55 GMT  
		Size: 21.1 MB (21096004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeef11aee822059479265f63f55446205a437ef50e49fbfb586c607571b58574`  
		Last Modified: Mon, 18 Oct 2021 21:44:53 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-git`

```console
$ docker pull docker@sha256:370cbd65cbf44658bc2ce46c8b606213d9e3e3ea04a7d53a0243d67ca6db95aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-git` - linux; amd64

```console
$ docker pull docker@sha256:3bf13c54edb2a2b817bcad4ae459bf6d8b867930b5026d1f51d4593f598495fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75071530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed61dfae734a45e9440fbd932eeb2b244f0079a45398e33dd1478f62a4f3be3`
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
# Tue, 05 Oct 2021 17:32:23 GMT
ENV DOCKER_VERSION=20.10.9
# Tue, 05 Oct 2021 17:32:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Oct 2021 17:32:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 05 Oct 2021 17:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:31 GMT
CMD ["sh"]
# Tue, 05 Oct 2021 17:32:54 GMT
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
	-	`sha256:c6e88c3a8ccafbb819665e363fc6947b47a896d85170e8b267c6c12176385b3c`  
		Last Modified: Tue, 05 Oct 2021 17:33:31 GMT  
		Size: 63.7 MB (63689714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e00801cfc09a8e327c9cced9fbc94f179e9f03caf50d0ac1c01ae1ca92c3b`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a43c1017099b38ffcabb7b27169d9ca7821bbfea77b15059c969020a0acfd`  
		Last Modified: Tue, 05 Oct 2021 17:33:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52f4e484f770e1039348c98519c8610f67ba16969fb9ab93afae3f4421f7d1`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e22895e9057604af4145b328a599ef34ed98eee9085de276ad33fe1adf50f5f`  
		Last Modified: Tue, 05 Oct 2021 17:34:29 GMT  
		Size: 6.6 MB (6630406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:6f7fe91a5a952fb482822be280a9c17313785627cdf33330c1980bf4404d6787
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69095577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b1ae00454f4fd0beeab581baa00fe5961ae9b97bae5802e58bc1d0e49636a41`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:40:48 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 18 Oct 2021 21:40:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:59 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:41:38 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bacb27c3d6ff01f6e8f051e37ec17341cc7fbc76073dea248afcf223aba5d`  
		Last Modified: Mon, 18 Oct 2021 21:44:10 GMT  
		Size: 57.7 MB (57733379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79bdbfa9a5540080db6017b27b917e7c21fbf947abefb068a974a0b55d481e`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a13bdd3b1cef3426a41cadec19b55904b133d95c31c10574f56b0419a93f72`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb034e6582742a188487a0bdde846bf28e29179005b5f423b7d465a2c4e368df`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae700626b8f4a7301ee4ec15808eb5b1b281fa56ecf42eb4a653b7f0b2a5f722`  
		Last Modified: Mon, 18 Oct 2021 21:45:15 GMT  
		Size: 6.7 MB (6739077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore`

```console
$ docker pull docker@sha256:e4eec512a2de95c6783851f85f38652b37fce108fb3171a6d7ace46e15f76047
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `docker:20-windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull docker@sha256:00d1af6859be90ae81443923948f91023c5d9c98c3b0cd509930967d25cc3ab9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737551444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:118b153058557f1f2ed347f423229e946823c10252f6f64941f859b7dcfe91bb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 12:02:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Oct 2021 02:43:13 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 14 Oct 2021 02:43:14 GMT
ENV DOCKER_VERSION=20.10.9
# Thu, 14 Oct 2021 02:43:15 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.9.zip
# Thu, 14 Oct 2021 02:44:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cc0c4e719f418d49c6a0fb87abd2e0e480c5b6fec1bacc3077cacfad9b4ab3e0`  
		Last Modified: Wed, 13 Oct 2021 12:18:09 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd874ac08ee111fe2cf114d0c6cde1f454b67345e21ce092adcb65291fa3d020`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 347.3 KB (347273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f858e26c2cf09cac487c279dce052648a24ae14d8277ac08dd52848b19b2667e`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4954d9c2f7e3575c7c1b370f79b942a39a290b5d8969aae868db3a4b859b0218`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bb3747e628070f796fc97248f1ffaf64c4dfbb3b02e00d9b52f4acdf6ec4e0`  
		Last Modified: Thu, 14 Oct 2021 02:45:09 GMT  
		Size: 50.9 MB (50881403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-1809`

```console
$ docker pull docker@sha256:e4eec512a2de95c6783851f85f38652b37fce108fb3171a6d7ace46e15f76047
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `docker:20-windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull docker@sha256:00d1af6859be90ae81443923948f91023c5d9c98c3b0cd509930967d25cc3ab9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737551444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:118b153058557f1f2ed347f423229e946823c10252f6f64941f859b7dcfe91bb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 12:02:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Oct 2021 02:43:13 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 14 Oct 2021 02:43:14 GMT
ENV DOCKER_VERSION=20.10.9
# Thu, 14 Oct 2021 02:43:15 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.9.zip
# Thu, 14 Oct 2021 02:44:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cc0c4e719f418d49c6a0fb87abd2e0e480c5b6fec1bacc3077cacfad9b4ab3e0`  
		Last Modified: Wed, 13 Oct 2021 12:18:09 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd874ac08ee111fe2cf114d0c6cde1f454b67345e21ce092adcb65291fa3d020`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 347.3 KB (347273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f858e26c2cf09cac487c279dce052648a24ae14d8277ac08dd52848b19b2667e`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4954d9c2f7e3575c7c1b370f79b942a39a290b5d8969aae868db3a4b859b0218`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bb3747e628070f796fc97248f1ffaf64c4dfbb3b02e00d9b52f4acdf6ec4e0`  
		Last Modified: Thu, 14 Oct 2021 02:45:09 GMT  
		Size: 50.9 MB (50881403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10`

```console
$ docker pull docker@sha256:938bcb85cf77db2b80d219abd5a1424ec15ce11a3adaea6423fa16cc9acfe926
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10` - linux; amd64

```console
$ docker pull docker@sha256:62302357e804b152e157d3603ce7a97c3f368a626ce027eee1d1e02b5ae924f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68441124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6448e722e510f9bb0bb5c2f65ef99295fc2321b656c00f088078ccf6564372b`
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
# Tue, 05 Oct 2021 17:32:23 GMT
ENV DOCKER_VERSION=20.10.9
# Tue, 05 Oct 2021 17:32:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Oct 2021 17:32:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 05 Oct 2021 17:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:31 GMT
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
	-	`sha256:c6e88c3a8ccafbb819665e363fc6947b47a896d85170e8b267c6c12176385b3c`  
		Last Modified: Tue, 05 Oct 2021 17:33:31 GMT  
		Size: 63.7 MB (63689714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e00801cfc09a8e327c9cced9fbc94f179e9f03caf50d0ac1c01ae1ca92c3b`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a43c1017099b38ffcabb7b27169d9ca7821bbfea77b15059c969020a0acfd`  
		Last Modified: Tue, 05 Oct 2021 17:33:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52f4e484f770e1039348c98519c8610f67ba16969fb9ab93afae3f4421f7d1`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1710b19ecaa7eba8537ea64a35ddec333ff128cda5f2f19b7c4cd6e3a4e0daf7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62356500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c324afd4ac0437589f8f6e825c2fed8ef663773f55ac7c8e85cd589f554239d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:40:48 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 18 Oct 2021 21:40:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:59 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bacb27c3d6ff01f6e8f051e37ec17341cc7fbc76073dea248afcf223aba5d`  
		Last Modified: Mon, 18 Oct 2021 21:44:10 GMT  
		Size: 57.7 MB (57733379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79bdbfa9a5540080db6017b27b917e7c21fbf947abefb068a974a0b55d481e`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a13bdd3b1cef3426a41cadec19b55904b133d95c31c10574f56b0419a93f72`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb034e6582742a188487a0bdde846bf28e29179005b5f423b7d465a2c4e368df`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind`

```console
$ docker pull docker@sha256:d842418d21545fde57c2512681d9bdc4ce0e54f2e0305a293ee20a9b6166932b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind` - linux; amd64

```console
$ docker pull docker@sha256:24628ded7711e48db56af875236ac30a8950305ac461332955b3375ac5a87e1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (74967424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1efbbff84703848e1c787073a954e8e3f0146836d94673f2d54f3672296bf82f`
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
# Tue, 05 Oct 2021 17:32:23 GMT
ENV DOCKER_VERSION=20.10.9
# Tue, 05 Oct 2021 17:32:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Oct 2021 17:32:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 05 Oct 2021 17:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:31 GMT
CMD ["sh"]
# Tue, 05 Oct 2021 17:32:37 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 05 Oct 2021 17:32:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 05 Oct 2021 17:32:38 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 05 Oct 2021 17:32:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 05 Oct 2021 17:32:39 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:39 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Oct 2021 17:32:39 GMT
EXPOSE 2375 2376
# Tue, 05 Oct 2021 17:32:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:40 GMT
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
	-	`sha256:c6e88c3a8ccafbb819665e363fc6947b47a896d85170e8b267c6c12176385b3c`  
		Last Modified: Tue, 05 Oct 2021 17:33:31 GMT  
		Size: 63.7 MB (63689714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e00801cfc09a8e327c9cced9fbc94f179e9f03caf50d0ac1c01ae1ca92c3b`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a43c1017099b38ffcabb7b27169d9ca7821bbfea77b15059c969020a0acfd`  
		Last Modified: Tue, 05 Oct 2021 17:33:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52f4e484f770e1039348c98519c8610f67ba16969fb9ab93afae3f4421f7d1`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec67a583a94bdc153dacab38a9b85a032e58cd332069a169388b45727d5a03c`  
		Last Modified: Tue, 05 Oct 2021 17:33:49 GMT  
		Size: 6.5 MB (6521405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a20c97b2389ddc8160afed72508ba7d5ae1464e5837dd19905c4e7130c4e5`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170df0071614602fcd5820d60cc7c9a73f8e10a616928d111e25041951c3507d`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfeb3c70a4f70f3868998e1000a4907ec50a8303595dbf0e96bdd03d59e086c`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:3ba0867a449ca78b731e3251ddeb677fa893dc500293ab0e303a8188b9e4d106
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68779801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6144797d483747bee375b8607893579ff8b6d6ff47e83b10ed4827e4123f549e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:40:48 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 18 Oct 2021 21:40:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:59 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:41:08 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 18 Oct 2021 21:41:08 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:41:09 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 18 Oct 2021 21:41:10 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 18 Oct 2021 21:41:12 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:41:12 GMT
VOLUME [/var/lib/docker]
# Mon, 18 Oct 2021 21:41:13 GMT
EXPOSE 2375 2376
# Mon, 18 Oct 2021 21:41:14 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 18 Oct 2021 21:41:15 GMT
CMD []
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bacb27c3d6ff01f6e8f051e37ec17341cc7fbc76073dea248afcf223aba5d`  
		Last Modified: Mon, 18 Oct 2021 21:44:10 GMT  
		Size: 57.7 MB (57733379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79bdbfa9a5540080db6017b27b917e7c21fbf947abefb068a974a0b55d481e`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a13bdd3b1cef3426a41cadec19b55904b133d95c31c10574f56b0419a93f72`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb034e6582742a188487a0bdde846bf28e29179005b5f423b7d465a2c4e368df`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e8bdd67624c83a9918b7d0bb7d24f84d32a306b3453ac55e213380ee17335d`  
		Last Modified: Mon, 18 Oct 2021 21:44:31 GMT  
		Size: 6.4 MB (6418437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9e9de043d240e7a3e0baf2f1a9bd6bd1da52fd1a1df9db1d97b50b294c98b8`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b746a27963c477864e414004aab19efff02e763e88444128d5bbf735410a4f`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c17f756b76c3b8328ed61cc3fef72a62229860b3a7fefcc6e94edda353b7d3a`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 2.6 KB (2615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind-rootless`

```console
$ docker pull docker@sha256:51cd937b2ad1a1d32179f2e9acc01ea46d4e127cdaf493a533172b1fb019af15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:75acfc77a83d9b4d557aab529432058b78ac6d629325c9d61c385cd2fc48fe7c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 MB (95235937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b4aec2427ffe9836431bca031ae4354053a010dae4736917b174d52da90dba`
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
# Tue, 05 Oct 2021 17:32:23 GMT
ENV DOCKER_VERSION=20.10.9
# Tue, 05 Oct 2021 17:32:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Oct 2021 17:32:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 05 Oct 2021 17:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:31 GMT
CMD ["sh"]
# Tue, 05 Oct 2021 17:32:37 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 05 Oct 2021 17:32:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 05 Oct 2021 17:32:38 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 05 Oct 2021 17:32:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 05 Oct 2021 17:32:39 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:39 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Oct 2021 17:32:39 GMT
EXPOSE 2375 2376
# Tue, 05 Oct 2021 17:32:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:40 GMT
CMD []
# Tue, 05 Oct 2021 17:32:44 GMT
RUN apk add --no-cache iproute2
# Tue, 05 Oct 2021 17:32:45 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 05 Oct 2021 17:32:46 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 05 Oct 2021 17:32:48 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 05 Oct 2021 17:32:49 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 05 Oct 2021 17:32:50 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 05 Oct 2021 17:32:50 GMT
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
	-	`sha256:c6e88c3a8ccafbb819665e363fc6947b47a896d85170e8b267c6c12176385b3c`  
		Last Modified: Tue, 05 Oct 2021 17:33:31 GMT  
		Size: 63.7 MB (63689714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e00801cfc09a8e327c9cced9fbc94f179e9f03caf50d0ac1c01ae1ca92c3b`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a43c1017099b38ffcabb7b27169d9ca7821bbfea77b15059c969020a0acfd`  
		Last Modified: Tue, 05 Oct 2021 17:33:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52f4e484f770e1039348c98519c8610f67ba16969fb9ab93afae3f4421f7d1`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec67a583a94bdc153dacab38a9b85a032e58cd332069a169388b45727d5a03c`  
		Last Modified: Tue, 05 Oct 2021 17:33:49 GMT  
		Size: 6.5 MB (6521405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a20c97b2389ddc8160afed72508ba7d5ae1464e5837dd19905c4e7130c4e5`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170df0071614602fcd5820d60cc7c9a73f8e10a616928d111e25041951c3507d`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfeb3c70a4f70f3868998e1000a4907ec50a8303595dbf0e96bdd03d59e086c`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418f850bf44d36d532f71a72ed317e54531b904953d99821dd316e73e777d23c`  
		Last Modified: Tue, 05 Oct 2021 17:34:08 GMT  
		Size: 1.1 MB (1148745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03facf1a1e41afef60e2e7bad46f0fbd44f5b2b3a3328337c3e0a6049120dd8`  
		Last Modified: Tue, 05 Oct 2021 17:34:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f919e685bb3723d38cd895248bb1c99de9588af3aba7f57ef5cb72eca54106a9`  
		Last Modified: Tue, 05 Oct 2021 17:34:08 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79573e4e685e01787d1e021ea1cecb99cdbf78577b160037c6ed2c7f8f2b304`  
		Last Modified: Tue, 05 Oct 2021 17:34:11 GMT  
		Size: 19.1 MB (19118054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7054ab8c007ff95ebed9750aae6c97b9f692ed317ea464234611c57db8601634`  
		Last Modified: Tue, 05 Oct 2021 17:34:08 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:eb9feb96a9c979384276b169446b5134c441625461108344fde1f18fdee9ce75
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.0 MB (91045261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a26cf3ffc31a4748452e2da3ca2a290c3354e441650e7617aaf4a9fbf6d1750`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:40:48 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 18 Oct 2021 21:40:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:59 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:41:08 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 18 Oct 2021 21:41:08 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:41:09 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 18 Oct 2021 21:41:10 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 18 Oct 2021 21:41:12 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:41:12 GMT
VOLUME [/var/lib/docker]
# Mon, 18 Oct 2021 21:41:13 GMT
EXPOSE 2375 2376
# Mon, 18 Oct 2021 21:41:14 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 18 Oct 2021 21:41:15 GMT
CMD []
# Mon, 18 Oct 2021 21:41:23 GMT
RUN apk add --no-cache iproute2
# Mon, 18 Oct 2021 21:41:24 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 18 Oct 2021 21:41:25 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:41:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 18 Oct 2021 21:41:29 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 18 Oct 2021 21:41:30 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 18 Oct 2021 21:41:31 GMT
USER rootless
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bacb27c3d6ff01f6e8f051e37ec17341cc7fbc76073dea248afcf223aba5d`  
		Last Modified: Mon, 18 Oct 2021 21:44:10 GMT  
		Size: 57.7 MB (57733379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79bdbfa9a5540080db6017b27b917e7c21fbf947abefb068a974a0b55d481e`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a13bdd3b1cef3426a41cadec19b55904b133d95c31c10574f56b0419a93f72`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb034e6582742a188487a0bdde846bf28e29179005b5f423b7d465a2c4e368df`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e8bdd67624c83a9918b7d0bb7d24f84d32a306b3453ac55e213380ee17335d`  
		Last Modified: Mon, 18 Oct 2021 21:44:31 GMT  
		Size: 6.4 MB (6418437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9e9de043d240e7a3e0baf2f1a9bd6bd1da52fd1a1df9db1d97b50b294c98b8`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b746a27963c477864e414004aab19efff02e763e88444128d5bbf735410a4f`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c17f756b76c3b8328ed61cc3fef72a62229860b3a7fefcc6e94edda353b7d3a`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 2.6 KB (2615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da73c72dcad0b534b2f4febbace9688a2f4a30bf46b188501e200b3be5977b03`  
		Last Modified: Mon, 18 Oct 2021 21:44:52 GMT  
		Size: 1.2 MB (1167836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff4316d7dcf66341a4e5a7a7519ed9d36f902bb95d2169ebc26549a0f95849`  
		Last Modified: Mon, 18 Oct 2021 21:44:52 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba611fb139d8c880c857badbc205cee357e35952ae811c52e90139e68f959d57`  
		Last Modified: Mon, 18 Oct 2021 21:44:52 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098b6fcc42aecdd56305fc4ceba9415e977d589f359ff58a7ee2c72612859ce9`  
		Last Modified: Mon, 18 Oct 2021 21:44:55 GMT  
		Size: 21.1 MB (21096004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeef11aee822059479265f63f55446205a437ef50e49fbfb586c607571b58574`  
		Last Modified: Mon, 18 Oct 2021 21:44:53 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-git`

```console
$ docker pull docker@sha256:370cbd65cbf44658bc2ce46c8b606213d9e3e3ea04a7d53a0243d67ca6db95aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-git` - linux; amd64

```console
$ docker pull docker@sha256:3bf13c54edb2a2b817bcad4ae459bf6d8b867930b5026d1f51d4593f598495fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75071530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed61dfae734a45e9440fbd932eeb2b244f0079a45398e33dd1478f62a4f3be3`
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
# Tue, 05 Oct 2021 17:32:23 GMT
ENV DOCKER_VERSION=20.10.9
# Tue, 05 Oct 2021 17:32:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Oct 2021 17:32:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 05 Oct 2021 17:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:31 GMT
CMD ["sh"]
# Tue, 05 Oct 2021 17:32:54 GMT
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
	-	`sha256:c6e88c3a8ccafbb819665e363fc6947b47a896d85170e8b267c6c12176385b3c`  
		Last Modified: Tue, 05 Oct 2021 17:33:31 GMT  
		Size: 63.7 MB (63689714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e00801cfc09a8e327c9cced9fbc94f179e9f03caf50d0ac1c01ae1ca92c3b`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a43c1017099b38ffcabb7b27169d9ca7821bbfea77b15059c969020a0acfd`  
		Last Modified: Tue, 05 Oct 2021 17:33:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52f4e484f770e1039348c98519c8610f67ba16969fb9ab93afae3f4421f7d1`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e22895e9057604af4145b328a599ef34ed98eee9085de276ad33fe1adf50f5f`  
		Last Modified: Tue, 05 Oct 2021 17:34:29 GMT  
		Size: 6.6 MB (6630406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:6f7fe91a5a952fb482822be280a9c17313785627cdf33330c1980bf4404d6787
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69095577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b1ae00454f4fd0beeab581baa00fe5961ae9b97bae5802e58bc1d0e49636a41`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:40:48 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 18 Oct 2021 21:40:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:59 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:41:38 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bacb27c3d6ff01f6e8f051e37ec17341cc7fbc76073dea248afcf223aba5d`  
		Last Modified: Mon, 18 Oct 2021 21:44:10 GMT  
		Size: 57.7 MB (57733379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79bdbfa9a5540080db6017b27b917e7c21fbf947abefb068a974a0b55d481e`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a13bdd3b1cef3426a41cadec19b55904b133d95c31c10574f56b0419a93f72`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb034e6582742a188487a0bdde846bf28e29179005b5f423b7d465a2c4e368df`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae700626b8f4a7301ee4ec15808eb5b1b281fa56ecf42eb4a653b7f0b2a5f722`  
		Last Modified: Mon, 18 Oct 2021 21:45:15 GMT  
		Size: 6.7 MB (6739077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-rc`

```console
$ docker pull docker@sha256:abd9743f601c58c12db87ba997758a7a22d37b2800d15d7a0a90d4a777f4d86e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-rc` - linux; amd64

```console
$ docker pull docker@sha256:3769dd5e09b1795718cec653d648d55558244ebd8fe13955e02e83bba97bb495
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (74032061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b076b43daf1313e0b147059fa86500a35771815f9413671c44aceca8c3905722`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:15:43 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 22 Oct 2020 03:15:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Dec 2020 01:19:40 GMT
ENV DOCKER_VERSION=20.10.0-rc2
# Thu, 03 Dec 2020 01:19:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.0-rc2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.0-rc2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.0-rc2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.0-rc2.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Dec 2020 01:19:47 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Dec 2020 01:19:47 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Dec 2020 01:19:47 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Dec 2020 01:19:48 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Dec 2020 01:19:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Dec 2020 01:19:48 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7c675703d60dc4d757acb40557350159f600ca3d49e2e8d4c2039dd6b69457`  
		Last Modified: Thu, 22 Oct 2020 03:16:47 GMT  
		Size: 2.0 MB (2039054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8c12a437cbe4e104dcea425e0ce277a2442603e14551d22a948e11026ae658`  
		Last Modified: Thu, 22 Oct 2020 03:16:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0fd8b7f6d785daed3820c5e1498e61167583e9045feac86ffb7e44cc08a098`  
		Last Modified: Thu, 03 Dec 2020 01:21:03 GMT  
		Size: 69.2 MB (69194310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db597305dcaeb9a5ab05768839f670f942793156b7b3b3936ce746314bfca19`  
		Last Modified: Thu, 03 Dec 2020 01:20:49 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103a137d36f54bc2da72b6de7a354e8ac532e331da4fa7cea3061e707ee631d6`  
		Last Modified: Thu, 03 Dec 2020 01:20:49 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3157e29d9bca4123fa681ea84dd51dad3441b7f2ac7a8d8cb09865df9f7c7fbd`  
		Last Modified: Thu, 03 Dec 2020 01:20:50 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-rc` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:eab2a4f03c6f78fa775f16495d33d5bd9db312068b14db9caa3b631968f19f57
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62354582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cd1e6d54b025850351cefe3112edff43a74d0a46d04ad08066c1ba8d7e2ea9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:39:53 GMT
ENV DOCKER_VERSION=20.10.10-rc1
# Mon, 18 Oct 2021 21:39:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.10-rc1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.10-rc1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:02 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:04 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112f3374d6fabbfe7b2c992c077ac3658ff8d061a8e18265257b45cd60739c0d`  
		Last Modified: Mon, 18 Oct 2021 21:42:54 GMT  
		Size: 57.7 MB (57731459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ffe46428f8f4e7d13099151a78aa124e254522444b80d46bcec4e3e3fc41eb`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6699487bf567a986ddfb631b8655b487e6922d4a86ee9ff17b738d32ae342fa7`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4f64888be82e82dc404000ef04193fab09949191aa4a5abd16eb3f76de6422`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-rc-dind`

```console
$ docker pull docker@sha256:54a3e9071f9308d3643e44a0922f353ade496af29813d4bf6337ee31f98033fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-rc-dind` - linux; amd64

```console
$ docker pull docker@sha256:0805d140b875b9bc8ebfdbae9ea4b26ba60ee90640a636c575713b6825035f66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (79995526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1d8f7c2d7206c43f115c4af423e1637a1f435068bc08c12e23748f21e55af20`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:15:43 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 22 Oct 2020 03:15:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Dec 2020 01:19:40 GMT
ENV DOCKER_VERSION=20.10.0-rc2
# Thu, 03 Dec 2020 01:19:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.0-rc2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.0-rc2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.0-rc2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.0-rc2.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Dec 2020 01:19:47 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Dec 2020 01:19:47 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Dec 2020 01:19:47 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Dec 2020 01:19:48 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Dec 2020 01:19:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Dec 2020 01:19:48 GMT
CMD ["sh"]
# Thu, 03 Dec 2020 01:19:55 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 03 Dec 2020 01:19:56 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 03 Dec 2020 01:19:56 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Thu, 03 Dec 2020 01:19:57 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 03 Dec 2020 01:19:57 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Thu, 03 Dec 2020 01:19:57 GMT
VOLUME [/var/lib/docker]
# Thu, 03 Dec 2020 01:19:58 GMT
EXPOSE 2375 2376
# Thu, 03 Dec 2020 01:19:58 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 03 Dec 2020 01:19:58 GMT
CMD []
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7c675703d60dc4d757acb40557350159f600ca3d49e2e8d4c2039dd6b69457`  
		Last Modified: Thu, 22 Oct 2020 03:16:47 GMT  
		Size: 2.0 MB (2039054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8c12a437cbe4e104dcea425e0ce277a2442603e14551d22a948e11026ae658`  
		Last Modified: Thu, 22 Oct 2020 03:16:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0fd8b7f6d785daed3820c5e1498e61167583e9045feac86ffb7e44cc08a098`  
		Last Modified: Thu, 03 Dec 2020 01:21:03 GMT  
		Size: 69.2 MB (69194310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db597305dcaeb9a5ab05768839f670f942793156b7b3b3936ce746314bfca19`  
		Last Modified: Thu, 03 Dec 2020 01:20:49 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103a137d36f54bc2da72b6de7a354e8ac532e331da4fa7cea3061e707ee631d6`  
		Last Modified: Thu, 03 Dec 2020 01:20:49 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3157e29d9bca4123fa681ea84dd51dad3441b7f2ac7a8d8cb09865df9f7c7fbd`  
		Last Modified: Thu, 03 Dec 2020 01:20:50 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d41eb34354d9c453eb21d4d874b79246fdde42e242ce3b3946e3fb08cd77b1`  
		Last Modified: Thu, 03 Dec 2020 01:21:10 GMT  
		Size: 6.0 MB (5958742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e049752a368345c7b7d2d9539852eeac961803cd38f17028532ee69a4294dfa9`  
		Last Modified: Thu, 03 Dec 2020 01:21:10 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238431a551c0fd0e6304bda8ab6e3806b3407161b0ddaaa51d97ea7c01ee9172`  
		Last Modified: Thu, 03 Dec 2020 01:21:09 GMT  
		Size: 931.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff110f4494d28d0434d2149ac8619524c81c1701c64fce9a08150d3c6134704`  
		Last Modified: Thu, 03 Dec 2020 01:21:10 GMT  
		Size: 2.5 KB (2509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-rc-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:03f725eb2e70a25215590328677b3f23e21f5e5a620476f43d3ab036efee3343
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68777909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15a40ad8d21fe5b8d86077ad0f06de3c91a4b4cffc74c1be70fc259f15054b67`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:39:53 GMT
ENV DOCKER_VERSION=20.10.10-rc1
# Mon, 18 Oct 2021 21:39:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.10-rc1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.10-rc1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:02 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:04 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:40:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 18 Oct 2021 21:40:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:40:14 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 18 Oct 2021 21:40:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 18 Oct 2021 21:40:17 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:17 GMT
VOLUME [/var/lib/docker]
# Mon, 18 Oct 2021 21:40:18 GMT
EXPOSE 2375 2376
# Mon, 18 Oct 2021 21:40:19 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:20 GMT
CMD []
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112f3374d6fabbfe7b2c992c077ac3658ff8d061a8e18265257b45cd60739c0d`  
		Last Modified: Mon, 18 Oct 2021 21:42:54 GMT  
		Size: 57.7 MB (57731459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ffe46428f8f4e7d13099151a78aa124e254522444b80d46bcec4e3e3fc41eb`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6699487bf567a986ddfb631b8655b487e6922d4a86ee9ff17b738d32ae342fa7`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4f64888be82e82dc404000ef04193fab09949191aa4a5abd16eb3f76de6422`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6501ba4a4760252cf7cc02d607ee723591654cc0bb5f52520a6e33dc7a0edc25`  
		Last Modified: Mon, 18 Oct 2021 21:43:12 GMT  
		Size: 6.4 MB (6418461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a680b385ce15bb20e7ba5ac40667562dec340d2d81461023bdf90c3e3fabbebd`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f199395c417cc0c7e6398feae5d9baf39d65e2e0a7bb70170c70b89e589e8dfe`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1aee83547715d6f96b27af07d2631947e319c0f257cbebfed3719ab3e20529`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-rc-dind-rootless`

```console
$ docker pull docker@sha256:a2ad342f46ccf0daa32a00de0c18297b6fae7f26bbedf659379106326ba40a45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-rc-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:ba9a867298f514f0155fc0015a88624808e42c513196c562d22d8b37dda7e8a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101261107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:004b0ab8718ed6fab023f19e76b5bcd1db501061987c8a2d3fb61965d8a62c25`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:15:43 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 22 Oct 2020 03:15:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Dec 2020 01:19:40 GMT
ENV DOCKER_VERSION=20.10.0-rc2
# Thu, 03 Dec 2020 01:19:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.0-rc2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.0-rc2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.0-rc2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.0-rc2.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Dec 2020 01:19:47 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Dec 2020 01:19:47 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Dec 2020 01:19:47 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Dec 2020 01:19:48 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Dec 2020 01:19:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Dec 2020 01:19:48 GMT
CMD ["sh"]
# Thu, 03 Dec 2020 01:19:55 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 03 Dec 2020 01:19:56 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 03 Dec 2020 01:19:56 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Thu, 03 Dec 2020 01:19:57 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 03 Dec 2020 01:19:57 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Thu, 03 Dec 2020 01:19:57 GMT
VOLUME [/var/lib/docker]
# Thu, 03 Dec 2020 01:19:58 GMT
EXPOSE 2375 2376
# Thu, 03 Dec 2020 01:19:58 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 03 Dec 2020 01:19:58 GMT
CMD []
# Thu, 03 Dec 2020 01:20:03 GMT
RUN apk add --no-cache iproute2
# Thu, 03 Dec 2020 01:20:04 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 03 Dec 2020 01:20:05 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 03 Dec 2020 01:20:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-20.10.0-rc2.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 03 Dec 2020 01:20:08 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 03 Dec 2020 01:20:09 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 03 Dec 2020 01:20:09 GMT
USER rootless
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7c675703d60dc4d757acb40557350159f600ca3d49e2e8d4c2039dd6b69457`  
		Last Modified: Thu, 22 Oct 2020 03:16:47 GMT  
		Size: 2.0 MB (2039054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8c12a437cbe4e104dcea425e0ce277a2442603e14551d22a948e11026ae658`  
		Last Modified: Thu, 22 Oct 2020 03:16:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0fd8b7f6d785daed3820c5e1498e61167583e9045feac86ffb7e44cc08a098`  
		Last Modified: Thu, 03 Dec 2020 01:21:03 GMT  
		Size: 69.2 MB (69194310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db597305dcaeb9a5ab05768839f670f942793156b7b3b3936ce746314bfca19`  
		Last Modified: Thu, 03 Dec 2020 01:20:49 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103a137d36f54bc2da72b6de7a354e8ac532e331da4fa7cea3061e707ee631d6`  
		Last Modified: Thu, 03 Dec 2020 01:20:49 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3157e29d9bca4123fa681ea84dd51dad3441b7f2ac7a8d8cb09865df9f7c7fbd`  
		Last Modified: Thu, 03 Dec 2020 01:20:50 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d41eb34354d9c453eb21d4d874b79246fdde42e242ce3b3946e3fb08cd77b1`  
		Last Modified: Thu, 03 Dec 2020 01:21:10 GMT  
		Size: 6.0 MB (5958742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e049752a368345c7b7d2d9539852eeac961803cd38f17028532ee69a4294dfa9`  
		Last Modified: Thu, 03 Dec 2020 01:21:10 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238431a551c0fd0e6304bda8ab6e3806b3407161b0ddaaa51d97ea7c01ee9172`  
		Last Modified: Thu, 03 Dec 2020 01:21:09 GMT  
		Size: 931.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff110f4494d28d0434d2149ac8619524c81c1701c64fce9a08150d3c6134704`  
		Last Modified: Thu, 03 Dec 2020 01:21:10 GMT  
		Size: 2.5 KB (2509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20dbfa1b4e2ec98111aa0501360a509205fbf16bc526d399cfa670d0c35b6046`  
		Last Modified: Thu, 03 Dec 2020 01:21:17 GMT  
		Size: 1.1 MB (1092668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f728936c6fdb24935e0bb1366ed702b917e9581519d22efab93f8728513a259a`  
		Last Modified: Thu, 03 Dec 2020 01:21:17 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b638cd1abd59f9f12d28d5d6227cdb991c66c16fd6f9b00dc39564d1583b251`  
		Last Modified: Thu, 03 Dec 2020 01:21:17 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cac38aa50f31cfa5934d05e52f6ff76d5b8809a374846c9b36af98c8f5a822`  
		Last Modified: Thu, 03 Dec 2020 01:21:21 GMT  
		Size: 20.2 MB (20171300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbc24424926ce09c4f9387a3510fe8d83e0d537f83a25565d4d6f8eb4a43a50`  
		Last Modified: Thu, 03 Dec 2020 01:21:17 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-rc-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:036139df2869c66580cf19c3f5e10fbfcdc51e44e4c253dd52461dbaf8756d1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.0 MB (91048708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:592281427bbc8f0ac33cd2c8cc861023d89fe8804da4082b826bb8976bf55339`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:39:53 GMT
ENV DOCKER_VERSION=20.10.10-rc1
# Mon, 18 Oct 2021 21:39:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.10-rc1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.10-rc1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:02 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:04 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:40:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 18 Oct 2021 21:40:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:40:14 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 18 Oct 2021 21:40:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 18 Oct 2021 21:40:17 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:17 GMT
VOLUME [/var/lib/docker]
# Mon, 18 Oct 2021 21:40:18 GMT
EXPOSE 2375 2376
# Mon, 18 Oct 2021 21:40:19 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:20 GMT
CMD []
# Mon, 18 Oct 2021 21:40:27 GMT
RUN apk add --no-cache iproute2
# Mon, 18 Oct 2021 21:40:28 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 18 Oct 2021 21:40:29 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:40:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-rootless-extras-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 18 Oct 2021 21:40:33 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 18 Oct 2021 21:40:34 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 18 Oct 2021 21:40:35 GMT
USER rootless
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112f3374d6fabbfe7b2c992c077ac3658ff8d061a8e18265257b45cd60739c0d`  
		Last Modified: Mon, 18 Oct 2021 21:42:54 GMT  
		Size: 57.7 MB (57731459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ffe46428f8f4e7d13099151a78aa124e254522444b80d46bcec4e3e3fc41eb`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6699487bf567a986ddfb631b8655b487e6922d4a86ee9ff17b738d32ae342fa7`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4f64888be82e82dc404000ef04193fab09949191aa4a5abd16eb3f76de6422`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6501ba4a4760252cf7cc02d607ee723591654cc0bb5f52520a6e33dc7a0edc25`  
		Last Modified: Mon, 18 Oct 2021 21:43:12 GMT  
		Size: 6.4 MB (6418461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a680b385ce15bb20e7ba5ac40667562dec340d2d81461023bdf90c3e3fabbebd`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f199395c417cc0c7e6398feae5d9baf39d65e2e0a7bb70170c70b89e589e8dfe`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1aee83547715d6f96b27af07d2631947e319c0f257cbebfed3719ab3e20529`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375da3ba74accf4f4e776d8ea0d05c23a13b4b2b720c68351e5a106a84dda6e3`  
		Last Modified: Mon, 18 Oct 2021 21:43:29 GMT  
		Size: 1.2 MB (1167846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ac90cf496368c08bead07501a2fb6bcf1be125a482b1ba65545eb127ade900`  
		Last Modified: Mon, 18 Oct 2021 21:43:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1a7298291f6aaebb45b8b88842f7e71ac8c03b3ba86694de07dcba597dce8b`  
		Last Modified: Mon, 18 Oct 2021 21:43:29 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f92a9eb80f5eb157bb083cbb43ee01b129e3a55ba704b5f14a5e73d3957e05f`  
		Last Modified: Mon, 18 Oct 2021 21:43:32 GMT  
		Size: 21.1 MB (21101330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6559ad5989ef407de45b61e2a3ebc564a674911a70765ee6abc411c6c43b88b2`  
		Last Modified: Mon, 18 Oct 2021 21:43:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-rc-git`

```console
$ docker pull docker@sha256:2313c01f288bdcee76a986334f8e00f7b361442710f2b7cc1ced9f0983ce0825
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-rc-git` - linux; amd64

```console
$ docker pull docker@sha256:50da362dfee957933c12cf5c491ce74186d4649909508ea62d1071d6ca95d82e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.3 MB (82344149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f16515870a2368ced3032e3241b1ddcfef531d220a78ee33fe20dc4dae86f12`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:15:43 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 22 Oct 2020 03:15:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Dec 2020 01:19:40 GMT
ENV DOCKER_VERSION=20.10.0-rc2
# Thu, 03 Dec 2020 01:19:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.0-rc2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.0-rc2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.0-rc2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.0-rc2.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Dec 2020 01:19:47 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Dec 2020 01:19:47 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Dec 2020 01:19:47 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Dec 2020 01:19:48 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Dec 2020 01:19:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Dec 2020 01:19:48 GMT
CMD ["sh"]
# Thu, 03 Dec 2020 01:20:14 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7c675703d60dc4d757acb40557350159f600ca3d49e2e8d4c2039dd6b69457`  
		Last Modified: Thu, 22 Oct 2020 03:16:47 GMT  
		Size: 2.0 MB (2039054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8c12a437cbe4e104dcea425e0ce277a2442603e14551d22a948e11026ae658`  
		Last Modified: Thu, 22 Oct 2020 03:16:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0fd8b7f6d785daed3820c5e1498e61167583e9045feac86ffb7e44cc08a098`  
		Last Modified: Thu, 03 Dec 2020 01:21:03 GMT  
		Size: 69.2 MB (69194310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db597305dcaeb9a5ab05768839f670f942793156b7b3b3936ce746314bfca19`  
		Last Modified: Thu, 03 Dec 2020 01:20:49 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103a137d36f54bc2da72b6de7a354e8ac532e331da4fa7cea3061e707ee631d6`  
		Last Modified: Thu, 03 Dec 2020 01:20:49 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3157e29d9bca4123fa681ea84dd51dad3441b7f2ac7a8d8cb09865df9f7c7fbd`  
		Last Modified: Thu, 03 Dec 2020 01:20:50 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb412ed0bbeb7d18fa0721ca6ebdff49ee36167e163ff98e4340081383937f5`  
		Last Modified: Thu, 03 Dec 2020 01:21:29 GMT  
		Size: 8.3 MB (8312088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-rc-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:a85ba73189c3335850cce7608bd089cdcad6cb0c6131187d644f6d17f6ec6eac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69093629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638acbdc55fc536c4148cdf061e5ea335d61c5db1d7d75a467d1c96babf85bcb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:39:53 GMT
ENV DOCKER_VERSION=20.10.10-rc1
# Mon, 18 Oct 2021 21:39:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.10-rc1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.10-rc1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:02 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:04 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:40:42 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112f3374d6fabbfe7b2c992c077ac3658ff8d061a8e18265257b45cd60739c0d`  
		Last Modified: Mon, 18 Oct 2021 21:42:54 GMT  
		Size: 57.7 MB (57731459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ffe46428f8f4e7d13099151a78aa124e254522444b80d46bcec4e3e3fc41eb`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6699487bf567a986ddfb631b8655b487e6922d4a86ee9ff17b738d32ae342fa7`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4f64888be82e82dc404000ef04193fab09949191aa4a5abd16eb3f76de6422`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a7843f30ad6a2fa274b0b141d4ddbf161ab3f789f4de5d6f2132dba26513b8`  
		Last Modified: Mon, 18 Oct 2021 21:43:47 GMT  
		Size: 6.7 MB (6739047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-rc-windowsservercore`

```console
$ docker pull docker@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `docker:20.10-rc-windowsservercore-1809`

```console
$ docker pull docker@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `docker:20.10-windowsservercore`

```console
$ docker pull docker@sha256:e4eec512a2de95c6783851f85f38652b37fce108fb3171a6d7ace46e15f76047
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `docker:20.10-windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull docker@sha256:00d1af6859be90ae81443923948f91023c5d9c98c3b0cd509930967d25cc3ab9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737551444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:118b153058557f1f2ed347f423229e946823c10252f6f64941f859b7dcfe91bb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 12:02:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Oct 2021 02:43:13 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 14 Oct 2021 02:43:14 GMT
ENV DOCKER_VERSION=20.10.9
# Thu, 14 Oct 2021 02:43:15 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.9.zip
# Thu, 14 Oct 2021 02:44:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cc0c4e719f418d49c6a0fb87abd2e0e480c5b6fec1bacc3077cacfad9b4ab3e0`  
		Last Modified: Wed, 13 Oct 2021 12:18:09 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd874ac08ee111fe2cf114d0c6cde1f454b67345e21ce092adcb65291fa3d020`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 347.3 KB (347273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f858e26c2cf09cac487c279dce052648a24ae14d8277ac08dd52848b19b2667e`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4954d9c2f7e3575c7c1b370f79b942a39a290b5d8969aae868db3a4b859b0218`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bb3747e628070f796fc97248f1ffaf64c4dfbb3b02e00d9b52f4acdf6ec4e0`  
		Last Modified: Thu, 14 Oct 2021 02:45:09 GMT  
		Size: 50.9 MB (50881403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-1809`

```console
$ docker pull docker@sha256:e4eec512a2de95c6783851f85f38652b37fce108fb3171a6d7ace46e15f76047
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `docker:20.10-windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull docker@sha256:00d1af6859be90ae81443923948f91023c5d9c98c3b0cd509930967d25cc3ab9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737551444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:118b153058557f1f2ed347f423229e946823c10252f6f64941f859b7dcfe91bb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 12:02:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Oct 2021 02:43:13 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 14 Oct 2021 02:43:14 GMT
ENV DOCKER_VERSION=20.10.9
# Thu, 14 Oct 2021 02:43:15 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.9.zip
# Thu, 14 Oct 2021 02:44:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cc0c4e719f418d49c6a0fb87abd2e0e480c5b6fec1bacc3077cacfad9b4ab3e0`  
		Last Modified: Wed, 13 Oct 2021 12:18:09 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd874ac08ee111fe2cf114d0c6cde1f454b67345e21ce092adcb65291fa3d020`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 347.3 KB (347273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f858e26c2cf09cac487c279dce052648a24ae14d8277ac08dd52848b19b2667e`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4954d9c2f7e3575c7c1b370f79b942a39a290b5d8969aae868db3a4b859b0218`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bb3747e628070f796fc97248f1ffaf64c4dfbb3b02e00d9b52f4acdf6ec4e0`  
		Last Modified: Thu, 14 Oct 2021 02:45:09 GMT  
		Size: 50.9 MB (50881403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.10-rc1`

```console
$ docker pull docker@sha256:eaf841d3d1b95430681cacd56b716277510225470f047b0b92f8b43ebfa300b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `docker:20.10.10-rc1` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:eab2a4f03c6f78fa775f16495d33d5bd9db312068b14db9caa3b631968f19f57
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62354582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cd1e6d54b025850351cefe3112edff43a74d0a46d04ad08066c1ba8d7e2ea9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:39:53 GMT
ENV DOCKER_VERSION=20.10.10-rc1
# Mon, 18 Oct 2021 21:39:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.10-rc1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.10-rc1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:02 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:04 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112f3374d6fabbfe7b2c992c077ac3658ff8d061a8e18265257b45cd60739c0d`  
		Last Modified: Mon, 18 Oct 2021 21:42:54 GMT  
		Size: 57.7 MB (57731459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ffe46428f8f4e7d13099151a78aa124e254522444b80d46bcec4e3e3fc41eb`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6699487bf567a986ddfb631b8655b487e6922d4a86ee9ff17b738d32ae342fa7`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4f64888be82e82dc404000ef04193fab09949191aa4a5abd16eb3f76de6422`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.10-rc1-alpine3.14`

```console
$ docker pull docker@sha256:eaf841d3d1b95430681cacd56b716277510225470f047b0b92f8b43ebfa300b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `docker:20.10.10-rc1-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:eab2a4f03c6f78fa775f16495d33d5bd9db312068b14db9caa3b631968f19f57
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62354582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cd1e6d54b025850351cefe3112edff43a74d0a46d04ad08066c1ba8d7e2ea9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:39:53 GMT
ENV DOCKER_VERSION=20.10.10-rc1
# Mon, 18 Oct 2021 21:39:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.10-rc1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.10-rc1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:02 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:04 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112f3374d6fabbfe7b2c992c077ac3658ff8d061a8e18265257b45cd60739c0d`  
		Last Modified: Mon, 18 Oct 2021 21:42:54 GMT  
		Size: 57.7 MB (57731459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ffe46428f8f4e7d13099151a78aa124e254522444b80d46bcec4e3e3fc41eb`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6699487bf567a986ddfb631b8655b487e6922d4a86ee9ff17b738d32ae342fa7`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4f64888be82e82dc404000ef04193fab09949191aa4a5abd16eb3f76de6422`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.10-rc1-dind`

```console
$ docker pull docker@sha256:3d382f13546d43d0d388aa091b86a66ad5ed38bce6800d164c864a162ec2991b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `docker:20.10.10-rc1-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:03f725eb2e70a25215590328677b3f23e21f5e5a620476f43d3ab036efee3343
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68777909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15a40ad8d21fe5b8d86077ad0f06de3c91a4b4cffc74c1be70fc259f15054b67`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:39:53 GMT
ENV DOCKER_VERSION=20.10.10-rc1
# Mon, 18 Oct 2021 21:39:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.10-rc1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.10-rc1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:02 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:04 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:40:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 18 Oct 2021 21:40:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:40:14 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 18 Oct 2021 21:40:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 18 Oct 2021 21:40:17 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:17 GMT
VOLUME [/var/lib/docker]
# Mon, 18 Oct 2021 21:40:18 GMT
EXPOSE 2375 2376
# Mon, 18 Oct 2021 21:40:19 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:20 GMT
CMD []
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112f3374d6fabbfe7b2c992c077ac3658ff8d061a8e18265257b45cd60739c0d`  
		Last Modified: Mon, 18 Oct 2021 21:42:54 GMT  
		Size: 57.7 MB (57731459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ffe46428f8f4e7d13099151a78aa124e254522444b80d46bcec4e3e3fc41eb`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6699487bf567a986ddfb631b8655b487e6922d4a86ee9ff17b738d32ae342fa7`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4f64888be82e82dc404000ef04193fab09949191aa4a5abd16eb3f76de6422`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6501ba4a4760252cf7cc02d607ee723591654cc0bb5f52520a6e33dc7a0edc25`  
		Last Modified: Mon, 18 Oct 2021 21:43:12 GMT  
		Size: 6.4 MB (6418461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a680b385ce15bb20e7ba5ac40667562dec340d2d81461023bdf90c3e3fabbebd`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f199395c417cc0c7e6398feae5d9baf39d65e2e0a7bb70170c70b89e589e8dfe`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1aee83547715d6f96b27af07d2631947e319c0f257cbebfed3719ab3e20529`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.10-rc1-dind-alpine3.14`

```console
$ docker pull docker@sha256:3d382f13546d43d0d388aa091b86a66ad5ed38bce6800d164c864a162ec2991b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `docker:20.10.10-rc1-dind-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:03f725eb2e70a25215590328677b3f23e21f5e5a620476f43d3ab036efee3343
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68777909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15a40ad8d21fe5b8d86077ad0f06de3c91a4b4cffc74c1be70fc259f15054b67`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:39:53 GMT
ENV DOCKER_VERSION=20.10.10-rc1
# Mon, 18 Oct 2021 21:39:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.10-rc1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.10-rc1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:02 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:04 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:40:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 18 Oct 2021 21:40:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:40:14 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 18 Oct 2021 21:40:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 18 Oct 2021 21:40:17 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:17 GMT
VOLUME [/var/lib/docker]
# Mon, 18 Oct 2021 21:40:18 GMT
EXPOSE 2375 2376
# Mon, 18 Oct 2021 21:40:19 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:20 GMT
CMD []
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112f3374d6fabbfe7b2c992c077ac3658ff8d061a8e18265257b45cd60739c0d`  
		Last Modified: Mon, 18 Oct 2021 21:42:54 GMT  
		Size: 57.7 MB (57731459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ffe46428f8f4e7d13099151a78aa124e254522444b80d46bcec4e3e3fc41eb`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6699487bf567a986ddfb631b8655b487e6922d4a86ee9ff17b738d32ae342fa7`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4f64888be82e82dc404000ef04193fab09949191aa4a5abd16eb3f76de6422`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6501ba4a4760252cf7cc02d607ee723591654cc0bb5f52520a6e33dc7a0edc25`  
		Last Modified: Mon, 18 Oct 2021 21:43:12 GMT  
		Size: 6.4 MB (6418461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a680b385ce15bb20e7ba5ac40667562dec340d2d81461023bdf90c3e3fabbebd`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f199395c417cc0c7e6398feae5d9baf39d65e2e0a7bb70170c70b89e589e8dfe`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1aee83547715d6f96b27af07d2631947e319c0f257cbebfed3719ab3e20529`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.10-rc1-dind-rootless`

```console
$ docker pull docker@sha256:b4a76b8df0f30131e9ff4cbd85f2f7973a924c3f49309cf86a692d966e5029f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `docker:20.10.10-rc1-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:036139df2869c66580cf19c3f5e10fbfcdc51e44e4c253dd52461dbaf8756d1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.0 MB (91048708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:592281427bbc8f0ac33cd2c8cc861023d89fe8804da4082b826bb8976bf55339`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:39:53 GMT
ENV DOCKER_VERSION=20.10.10-rc1
# Mon, 18 Oct 2021 21:39:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.10-rc1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.10-rc1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:02 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:04 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:40:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 18 Oct 2021 21:40:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:40:14 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 18 Oct 2021 21:40:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 18 Oct 2021 21:40:17 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:17 GMT
VOLUME [/var/lib/docker]
# Mon, 18 Oct 2021 21:40:18 GMT
EXPOSE 2375 2376
# Mon, 18 Oct 2021 21:40:19 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:20 GMT
CMD []
# Mon, 18 Oct 2021 21:40:27 GMT
RUN apk add --no-cache iproute2
# Mon, 18 Oct 2021 21:40:28 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 18 Oct 2021 21:40:29 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:40:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-rootless-extras-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 18 Oct 2021 21:40:33 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 18 Oct 2021 21:40:34 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 18 Oct 2021 21:40:35 GMT
USER rootless
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112f3374d6fabbfe7b2c992c077ac3658ff8d061a8e18265257b45cd60739c0d`  
		Last Modified: Mon, 18 Oct 2021 21:42:54 GMT  
		Size: 57.7 MB (57731459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ffe46428f8f4e7d13099151a78aa124e254522444b80d46bcec4e3e3fc41eb`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6699487bf567a986ddfb631b8655b487e6922d4a86ee9ff17b738d32ae342fa7`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4f64888be82e82dc404000ef04193fab09949191aa4a5abd16eb3f76de6422`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6501ba4a4760252cf7cc02d607ee723591654cc0bb5f52520a6e33dc7a0edc25`  
		Last Modified: Mon, 18 Oct 2021 21:43:12 GMT  
		Size: 6.4 MB (6418461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a680b385ce15bb20e7ba5ac40667562dec340d2d81461023bdf90c3e3fabbebd`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f199395c417cc0c7e6398feae5d9baf39d65e2e0a7bb70170c70b89e589e8dfe`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1aee83547715d6f96b27af07d2631947e319c0f257cbebfed3719ab3e20529`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375da3ba74accf4f4e776d8ea0d05c23a13b4b2b720c68351e5a106a84dda6e3`  
		Last Modified: Mon, 18 Oct 2021 21:43:29 GMT  
		Size: 1.2 MB (1167846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ac90cf496368c08bead07501a2fb6bcf1be125a482b1ba65545eb127ade900`  
		Last Modified: Mon, 18 Oct 2021 21:43:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1a7298291f6aaebb45b8b88842f7e71ac8c03b3ba86694de07dcba597dce8b`  
		Last Modified: Mon, 18 Oct 2021 21:43:29 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f92a9eb80f5eb157bb083cbb43ee01b129e3a55ba704b5f14a5e73d3957e05f`  
		Last Modified: Mon, 18 Oct 2021 21:43:32 GMT  
		Size: 21.1 MB (21101330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6559ad5989ef407de45b61e2a3ebc564a674911a70765ee6abc411c6c43b88b2`  
		Last Modified: Mon, 18 Oct 2021 21:43:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.10-rc1-git`

```console
$ docker pull docker@sha256:d62aaad59b38ba571d761f4c68a732b5d312fbdb6686697047d79c9cc2dfe3b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `docker:20.10.10-rc1-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:a85ba73189c3335850cce7608bd089cdcad6cb0c6131187d644f6d17f6ec6eac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69093629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638acbdc55fc536c4148cdf061e5ea335d61c5db1d7d75a467d1c96babf85bcb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:39:53 GMT
ENV DOCKER_VERSION=20.10.10-rc1
# Mon, 18 Oct 2021 21:39:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.10-rc1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.10-rc1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:02 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:04 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:40:42 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112f3374d6fabbfe7b2c992c077ac3658ff8d061a8e18265257b45cd60739c0d`  
		Last Modified: Mon, 18 Oct 2021 21:42:54 GMT  
		Size: 57.7 MB (57731459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ffe46428f8f4e7d13099151a78aa124e254522444b80d46bcec4e3e3fc41eb`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6699487bf567a986ddfb631b8655b487e6922d4a86ee9ff17b738d32ae342fa7`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4f64888be82e82dc404000ef04193fab09949191aa4a5abd16eb3f76de6422`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a7843f30ad6a2fa274b0b141d4ddbf161ab3f789f4de5d6f2132dba26513b8`  
		Last Modified: Mon, 18 Oct 2021 21:43:47 GMT  
		Size: 6.7 MB (6739047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.10-rc1-windowsservercore`

```console
$ docker pull docker@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `docker:20.10.10-rc1-windowsservercore-1809`

```console
$ docker pull docker@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `docker:20.10.9`

```console
$ docker pull docker@sha256:938bcb85cf77db2b80d219abd5a1424ec15ce11a3adaea6423fa16cc9acfe926
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.9` - linux; amd64

```console
$ docker pull docker@sha256:62302357e804b152e157d3603ce7a97c3f368a626ce027eee1d1e02b5ae924f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68441124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6448e722e510f9bb0bb5c2f65ef99295fc2321b656c00f088078ccf6564372b`
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
# Tue, 05 Oct 2021 17:32:23 GMT
ENV DOCKER_VERSION=20.10.9
# Tue, 05 Oct 2021 17:32:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Oct 2021 17:32:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 05 Oct 2021 17:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:31 GMT
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
	-	`sha256:c6e88c3a8ccafbb819665e363fc6947b47a896d85170e8b267c6c12176385b3c`  
		Last Modified: Tue, 05 Oct 2021 17:33:31 GMT  
		Size: 63.7 MB (63689714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e00801cfc09a8e327c9cced9fbc94f179e9f03caf50d0ac1c01ae1ca92c3b`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a43c1017099b38ffcabb7b27169d9ca7821bbfea77b15059c969020a0acfd`  
		Last Modified: Tue, 05 Oct 2021 17:33:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52f4e484f770e1039348c98519c8610f67ba16969fb9ab93afae3f4421f7d1`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.9` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1710b19ecaa7eba8537ea64a35ddec333ff128cda5f2f19b7c4cd6e3a4e0daf7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62356500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c324afd4ac0437589f8f6e825c2fed8ef663773f55ac7c8e85cd589f554239d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:40:48 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 18 Oct 2021 21:40:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:59 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bacb27c3d6ff01f6e8f051e37ec17341cc7fbc76073dea248afcf223aba5d`  
		Last Modified: Mon, 18 Oct 2021 21:44:10 GMT  
		Size: 57.7 MB (57733379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79bdbfa9a5540080db6017b27b917e7c21fbf947abefb068a974a0b55d481e`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a13bdd3b1cef3426a41cadec19b55904b133d95c31c10574f56b0419a93f72`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb034e6582742a188487a0bdde846bf28e29179005b5f423b7d465a2c4e368df`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.9-alpine3.14`

```console
$ docker pull docker@sha256:938bcb85cf77db2b80d219abd5a1424ec15ce11a3adaea6423fa16cc9acfe926
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.9-alpine3.14` - linux; amd64

```console
$ docker pull docker@sha256:62302357e804b152e157d3603ce7a97c3f368a626ce027eee1d1e02b5ae924f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68441124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6448e722e510f9bb0bb5c2f65ef99295fc2321b656c00f088078ccf6564372b`
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
# Tue, 05 Oct 2021 17:32:23 GMT
ENV DOCKER_VERSION=20.10.9
# Tue, 05 Oct 2021 17:32:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Oct 2021 17:32:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 05 Oct 2021 17:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:31 GMT
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
	-	`sha256:c6e88c3a8ccafbb819665e363fc6947b47a896d85170e8b267c6c12176385b3c`  
		Last Modified: Tue, 05 Oct 2021 17:33:31 GMT  
		Size: 63.7 MB (63689714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e00801cfc09a8e327c9cced9fbc94f179e9f03caf50d0ac1c01ae1ca92c3b`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a43c1017099b38ffcabb7b27169d9ca7821bbfea77b15059c969020a0acfd`  
		Last Modified: Tue, 05 Oct 2021 17:33:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52f4e484f770e1039348c98519c8610f67ba16969fb9ab93afae3f4421f7d1`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.9-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1710b19ecaa7eba8537ea64a35ddec333ff128cda5f2f19b7c4cd6e3a4e0daf7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62356500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c324afd4ac0437589f8f6e825c2fed8ef663773f55ac7c8e85cd589f554239d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:40:48 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 18 Oct 2021 21:40:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:59 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bacb27c3d6ff01f6e8f051e37ec17341cc7fbc76073dea248afcf223aba5d`  
		Last Modified: Mon, 18 Oct 2021 21:44:10 GMT  
		Size: 57.7 MB (57733379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79bdbfa9a5540080db6017b27b917e7c21fbf947abefb068a974a0b55d481e`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a13bdd3b1cef3426a41cadec19b55904b133d95c31c10574f56b0419a93f72`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb034e6582742a188487a0bdde846bf28e29179005b5f423b7d465a2c4e368df`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.9-dind`

```console
$ docker pull docker@sha256:d842418d21545fde57c2512681d9bdc4ce0e54f2e0305a293ee20a9b6166932b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.9-dind` - linux; amd64

```console
$ docker pull docker@sha256:24628ded7711e48db56af875236ac30a8950305ac461332955b3375ac5a87e1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (74967424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1efbbff84703848e1c787073a954e8e3f0146836d94673f2d54f3672296bf82f`
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
# Tue, 05 Oct 2021 17:32:23 GMT
ENV DOCKER_VERSION=20.10.9
# Tue, 05 Oct 2021 17:32:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Oct 2021 17:32:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 05 Oct 2021 17:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:31 GMT
CMD ["sh"]
# Tue, 05 Oct 2021 17:32:37 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 05 Oct 2021 17:32:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 05 Oct 2021 17:32:38 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 05 Oct 2021 17:32:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 05 Oct 2021 17:32:39 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:39 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Oct 2021 17:32:39 GMT
EXPOSE 2375 2376
# Tue, 05 Oct 2021 17:32:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:40 GMT
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
	-	`sha256:c6e88c3a8ccafbb819665e363fc6947b47a896d85170e8b267c6c12176385b3c`  
		Last Modified: Tue, 05 Oct 2021 17:33:31 GMT  
		Size: 63.7 MB (63689714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e00801cfc09a8e327c9cced9fbc94f179e9f03caf50d0ac1c01ae1ca92c3b`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a43c1017099b38ffcabb7b27169d9ca7821bbfea77b15059c969020a0acfd`  
		Last Modified: Tue, 05 Oct 2021 17:33:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52f4e484f770e1039348c98519c8610f67ba16969fb9ab93afae3f4421f7d1`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec67a583a94bdc153dacab38a9b85a032e58cd332069a169388b45727d5a03c`  
		Last Modified: Tue, 05 Oct 2021 17:33:49 GMT  
		Size: 6.5 MB (6521405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a20c97b2389ddc8160afed72508ba7d5ae1464e5837dd19905c4e7130c4e5`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170df0071614602fcd5820d60cc7c9a73f8e10a616928d111e25041951c3507d`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfeb3c70a4f70f3868998e1000a4907ec50a8303595dbf0e96bdd03d59e086c`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.9-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:3ba0867a449ca78b731e3251ddeb677fa893dc500293ab0e303a8188b9e4d106
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68779801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6144797d483747bee375b8607893579ff8b6d6ff47e83b10ed4827e4123f549e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:40:48 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 18 Oct 2021 21:40:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:59 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:41:08 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 18 Oct 2021 21:41:08 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:41:09 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 18 Oct 2021 21:41:10 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 18 Oct 2021 21:41:12 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:41:12 GMT
VOLUME [/var/lib/docker]
# Mon, 18 Oct 2021 21:41:13 GMT
EXPOSE 2375 2376
# Mon, 18 Oct 2021 21:41:14 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 18 Oct 2021 21:41:15 GMT
CMD []
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bacb27c3d6ff01f6e8f051e37ec17341cc7fbc76073dea248afcf223aba5d`  
		Last Modified: Mon, 18 Oct 2021 21:44:10 GMT  
		Size: 57.7 MB (57733379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79bdbfa9a5540080db6017b27b917e7c21fbf947abefb068a974a0b55d481e`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a13bdd3b1cef3426a41cadec19b55904b133d95c31c10574f56b0419a93f72`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb034e6582742a188487a0bdde846bf28e29179005b5f423b7d465a2c4e368df`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e8bdd67624c83a9918b7d0bb7d24f84d32a306b3453ac55e213380ee17335d`  
		Last Modified: Mon, 18 Oct 2021 21:44:31 GMT  
		Size: 6.4 MB (6418437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9e9de043d240e7a3e0baf2f1a9bd6bd1da52fd1a1df9db1d97b50b294c98b8`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b746a27963c477864e414004aab19efff02e763e88444128d5bbf735410a4f`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c17f756b76c3b8328ed61cc3fef72a62229860b3a7fefcc6e94edda353b7d3a`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 2.6 KB (2615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.9-dind-alpine3.14`

```console
$ docker pull docker@sha256:d842418d21545fde57c2512681d9bdc4ce0e54f2e0305a293ee20a9b6166932b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.9-dind-alpine3.14` - linux; amd64

```console
$ docker pull docker@sha256:24628ded7711e48db56af875236ac30a8950305ac461332955b3375ac5a87e1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (74967424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1efbbff84703848e1c787073a954e8e3f0146836d94673f2d54f3672296bf82f`
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
# Tue, 05 Oct 2021 17:32:23 GMT
ENV DOCKER_VERSION=20.10.9
# Tue, 05 Oct 2021 17:32:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Oct 2021 17:32:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 05 Oct 2021 17:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:31 GMT
CMD ["sh"]
# Tue, 05 Oct 2021 17:32:37 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 05 Oct 2021 17:32:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 05 Oct 2021 17:32:38 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 05 Oct 2021 17:32:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 05 Oct 2021 17:32:39 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:39 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Oct 2021 17:32:39 GMT
EXPOSE 2375 2376
# Tue, 05 Oct 2021 17:32:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:40 GMT
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
	-	`sha256:c6e88c3a8ccafbb819665e363fc6947b47a896d85170e8b267c6c12176385b3c`  
		Last Modified: Tue, 05 Oct 2021 17:33:31 GMT  
		Size: 63.7 MB (63689714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e00801cfc09a8e327c9cced9fbc94f179e9f03caf50d0ac1c01ae1ca92c3b`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a43c1017099b38ffcabb7b27169d9ca7821bbfea77b15059c969020a0acfd`  
		Last Modified: Tue, 05 Oct 2021 17:33:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52f4e484f770e1039348c98519c8610f67ba16969fb9ab93afae3f4421f7d1`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec67a583a94bdc153dacab38a9b85a032e58cd332069a169388b45727d5a03c`  
		Last Modified: Tue, 05 Oct 2021 17:33:49 GMT  
		Size: 6.5 MB (6521405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a20c97b2389ddc8160afed72508ba7d5ae1464e5837dd19905c4e7130c4e5`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170df0071614602fcd5820d60cc7c9a73f8e10a616928d111e25041951c3507d`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfeb3c70a4f70f3868998e1000a4907ec50a8303595dbf0e96bdd03d59e086c`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.9-dind-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:3ba0867a449ca78b731e3251ddeb677fa893dc500293ab0e303a8188b9e4d106
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68779801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6144797d483747bee375b8607893579ff8b6d6ff47e83b10ed4827e4123f549e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:40:48 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 18 Oct 2021 21:40:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:59 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:41:08 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 18 Oct 2021 21:41:08 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:41:09 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 18 Oct 2021 21:41:10 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 18 Oct 2021 21:41:12 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:41:12 GMT
VOLUME [/var/lib/docker]
# Mon, 18 Oct 2021 21:41:13 GMT
EXPOSE 2375 2376
# Mon, 18 Oct 2021 21:41:14 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 18 Oct 2021 21:41:15 GMT
CMD []
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bacb27c3d6ff01f6e8f051e37ec17341cc7fbc76073dea248afcf223aba5d`  
		Last Modified: Mon, 18 Oct 2021 21:44:10 GMT  
		Size: 57.7 MB (57733379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79bdbfa9a5540080db6017b27b917e7c21fbf947abefb068a974a0b55d481e`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a13bdd3b1cef3426a41cadec19b55904b133d95c31c10574f56b0419a93f72`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb034e6582742a188487a0bdde846bf28e29179005b5f423b7d465a2c4e368df`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e8bdd67624c83a9918b7d0bb7d24f84d32a306b3453ac55e213380ee17335d`  
		Last Modified: Mon, 18 Oct 2021 21:44:31 GMT  
		Size: 6.4 MB (6418437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9e9de043d240e7a3e0baf2f1a9bd6bd1da52fd1a1df9db1d97b50b294c98b8`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b746a27963c477864e414004aab19efff02e763e88444128d5bbf735410a4f`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c17f756b76c3b8328ed61cc3fef72a62229860b3a7fefcc6e94edda353b7d3a`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 2.6 KB (2615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.9-dind-rootless`

```console
$ docker pull docker@sha256:51cd937b2ad1a1d32179f2e9acc01ea46d4e127cdaf493a533172b1fb019af15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.9-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:75acfc77a83d9b4d557aab529432058b78ac6d629325c9d61c385cd2fc48fe7c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 MB (95235937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b4aec2427ffe9836431bca031ae4354053a010dae4736917b174d52da90dba`
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
# Tue, 05 Oct 2021 17:32:23 GMT
ENV DOCKER_VERSION=20.10.9
# Tue, 05 Oct 2021 17:32:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Oct 2021 17:32:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 05 Oct 2021 17:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:31 GMT
CMD ["sh"]
# Tue, 05 Oct 2021 17:32:37 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 05 Oct 2021 17:32:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 05 Oct 2021 17:32:38 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 05 Oct 2021 17:32:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 05 Oct 2021 17:32:39 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:39 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Oct 2021 17:32:39 GMT
EXPOSE 2375 2376
# Tue, 05 Oct 2021 17:32:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:40 GMT
CMD []
# Tue, 05 Oct 2021 17:32:44 GMT
RUN apk add --no-cache iproute2
# Tue, 05 Oct 2021 17:32:45 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 05 Oct 2021 17:32:46 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 05 Oct 2021 17:32:48 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 05 Oct 2021 17:32:49 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 05 Oct 2021 17:32:50 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 05 Oct 2021 17:32:50 GMT
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
	-	`sha256:c6e88c3a8ccafbb819665e363fc6947b47a896d85170e8b267c6c12176385b3c`  
		Last Modified: Tue, 05 Oct 2021 17:33:31 GMT  
		Size: 63.7 MB (63689714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e00801cfc09a8e327c9cced9fbc94f179e9f03caf50d0ac1c01ae1ca92c3b`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a43c1017099b38ffcabb7b27169d9ca7821bbfea77b15059c969020a0acfd`  
		Last Modified: Tue, 05 Oct 2021 17:33:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52f4e484f770e1039348c98519c8610f67ba16969fb9ab93afae3f4421f7d1`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec67a583a94bdc153dacab38a9b85a032e58cd332069a169388b45727d5a03c`  
		Last Modified: Tue, 05 Oct 2021 17:33:49 GMT  
		Size: 6.5 MB (6521405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a20c97b2389ddc8160afed72508ba7d5ae1464e5837dd19905c4e7130c4e5`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170df0071614602fcd5820d60cc7c9a73f8e10a616928d111e25041951c3507d`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfeb3c70a4f70f3868998e1000a4907ec50a8303595dbf0e96bdd03d59e086c`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418f850bf44d36d532f71a72ed317e54531b904953d99821dd316e73e777d23c`  
		Last Modified: Tue, 05 Oct 2021 17:34:08 GMT  
		Size: 1.1 MB (1148745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03facf1a1e41afef60e2e7bad46f0fbd44f5b2b3a3328337c3e0a6049120dd8`  
		Last Modified: Tue, 05 Oct 2021 17:34:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f919e685bb3723d38cd895248bb1c99de9588af3aba7f57ef5cb72eca54106a9`  
		Last Modified: Tue, 05 Oct 2021 17:34:08 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79573e4e685e01787d1e021ea1cecb99cdbf78577b160037c6ed2c7f8f2b304`  
		Last Modified: Tue, 05 Oct 2021 17:34:11 GMT  
		Size: 19.1 MB (19118054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7054ab8c007ff95ebed9750aae6c97b9f692ed317ea464234611c57db8601634`  
		Last Modified: Tue, 05 Oct 2021 17:34:08 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.9-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:eb9feb96a9c979384276b169446b5134c441625461108344fde1f18fdee9ce75
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.0 MB (91045261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a26cf3ffc31a4748452e2da3ca2a290c3354e441650e7617aaf4a9fbf6d1750`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:40:48 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 18 Oct 2021 21:40:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:59 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:41:08 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 18 Oct 2021 21:41:08 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:41:09 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 18 Oct 2021 21:41:10 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 18 Oct 2021 21:41:12 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:41:12 GMT
VOLUME [/var/lib/docker]
# Mon, 18 Oct 2021 21:41:13 GMT
EXPOSE 2375 2376
# Mon, 18 Oct 2021 21:41:14 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 18 Oct 2021 21:41:15 GMT
CMD []
# Mon, 18 Oct 2021 21:41:23 GMT
RUN apk add --no-cache iproute2
# Mon, 18 Oct 2021 21:41:24 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 18 Oct 2021 21:41:25 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:41:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 18 Oct 2021 21:41:29 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 18 Oct 2021 21:41:30 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 18 Oct 2021 21:41:31 GMT
USER rootless
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bacb27c3d6ff01f6e8f051e37ec17341cc7fbc76073dea248afcf223aba5d`  
		Last Modified: Mon, 18 Oct 2021 21:44:10 GMT  
		Size: 57.7 MB (57733379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79bdbfa9a5540080db6017b27b917e7c21fbf947abefb068a974a0b55d481e`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a13bdd3b1cef3426a41cadec19b55904b133d95c31c10574f56b0419a93f72`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb034e6582742a188487a0bdde846bf28e29179005b5f423b7d465a2c4e368df`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e8bdd67624c83a9918b7d0bb7d24f84d32a306b3453ac55e213380ee17335d`  
		Last Modified: Mon, 18 Oct 2021 21:44:31 GMT  
		Size: 6.4 MB (6418437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9e9de043d240e7a3e0baf2f1a9bd6bd1da52fd1a1df9db1d97b50b294c98b8`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b746a27963c477864e414004aab19efff02e763e88444128d5bbf735410a4f`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c17f756b76c3b8328ed61cc3fef72a62229860b3a7fefcc6e94edda353b7d3a`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 2.6 KB (2615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da73c72dcad0b534b2f4febbace9688a2f4a30bf46b188501e200b3be5977b03`  
		Last Modified: Mon, 18 Oct 2021 21:44:52 GMT  
		Size: 1.2 MB (1167836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff4316d7dcf66341a4e5a7a7519ed9d36f902bb95d2169ebc26549a0f95849`  
		Last Modified: Mon, 18 Oct 2021 21:44:52 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba611fb139d8c880c857badbc205cee357e35952ae811c52e90139e68f959d57`  
		Last Modified: Mon, 18 Oct 2021 21:44:52 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098b6fcc42aecdd56305fc4ceba9415e977d589f359ff58a7ee2c72612859ce9`  
		Last Modified: Mon, 18 Oct 2021 21:44:55 GMT  
		Size: 21.1 MB (21096004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeef11aee822059479265f63f55446205a437ef50e49fbfb586c607571b58574`  
		Last Modified: Mon, 18 Oct 2021 21:44:53 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.9-git`

```console
$ docker pull docker@sha256:370cbd65cbf44658bc2ce46c8b606213d9e3e3ea04a7d53a0243d67ca6db95aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.9-git` - linux; amd64

```console
$ docker pull docker@sha256:3bf13c54edb2a2b817bcad4ae459bf6d8b867930b5026d1f51d4593f598495fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75071530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed61dfae734a45e9440fbd932eeb2b244f0079a45398e33dd1478f62a4f3be3`
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
# Tue, 05 Oct 2021 17:32:23 GMT
ENV DOCKER_VERSION=20.10.9
# Tue, 05 Oct 2021 17:32:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Oct 2021 17:32:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 05 Oct 2021 17:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:31 GMT
CMD ["sh"]
# Tue, 05 Oct 2021 17:32:54 GMT
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
	-	`sha256:c6e88c3a8ccafbb819665e363fc6947b47a896d85170e8b267c6c12176385b3c`  
		Last Modified: Tue, 05 Oct 2021 17:33:31 GMT  
		Size: 63.7 MB (63689714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e00801cfc09a8e327c9cced9fbc94f179e9f03caf50d0ac1c01ae1ca92c3b`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a43c1017099b38ffcabb7b27169d9ca7821bbfea77b15059c969020a0acfd`  
		Last Modified: Tue, 05 Oct 2021 17:33:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52f4e484f770e1039348c98519c8610f67ba16969fb9ab93afae3f4421f7d1`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e22895e9057604af4145b328a599ef34ed98eee9085de276ad33fe1adf50f5f`  
		Last Modified: Tue, 05 Oct 2021 17:34:29 GMT  
		Size: 6.6 MB (6630406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.9-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:6f7fe91a5a952fb482822be280a9c17313785627cdf33330c1980bf4404d6787
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69095577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b1ae00454f4fd0beeab581baa00fe5961ae9b97bae5802e58bc1d0e49636a41`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:40:48 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 18 Oct 2021 21:40:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:59 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:41:38 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bacb27c3d6ff01f6e8f051e37ec17341cc7fbc76073dea248afcf223aba5d`  
		Last Modified: Mon, 18 Oct 2021 21:44:10 GMT  
		Size: 57.7 MB (57733379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79bdbfa9a5540080db6017b27b917e7c21fbf947abefb068a974a0b55d481e`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a13bdd3b1cef3426a41cadec19b55904b133d95c31c10574f56b0419a93f72`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb034e6582742a188487a0bdde846bf28e29179005b5f423b7d465a2c4e368df`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae700626b8f4a7301ee4ec15808eb5b1b281fa56ecf42eb4a653b7f0b2a5f722`  
		Last Modified: Mon, 18 Oct 2021 21:45:15 GMT  
		Size: 6.7 MB (6739077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.9-windowsservercore`

```console
$ docker pull docker@sha256:e4eec512a2de95c6783851f85f38652b37fce108fb3171a6d7ace46e15f76047
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `docker:20.10.9-windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull docker@sha256:00d1af6859be90ae81443923948f91023c5d9c98c3b0cd509930967d25cc3ab9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737551444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:118b153058557f1f2ed347f423229e946823c10252f6f64941f859b7dcfe91bb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 12:02:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Oct 2021 02:43:13 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 14 Oct 2021 02:43:14 GMT
ENV DOCKER_VERSION=20.10.9
# Thu, 14 Oct 2021 02:43:15 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.9.zip
# Thu, 14 Oct 2021 02:44:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cc0c4e719f418d49c6a0fb87abd2e0e480c5b6fec1bacc3077cacfad9b4ab3e0`  
		Last Modified: Wed, 13 Oct 2021 12:18:09 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd874ac08ee111fe2cf114d0c6cde1f454b67345e21ce092adcb65291fa3d020`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 347.3 KB (347273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f858e26c2cf09cac487c279dce052648a24ae14d8277ac08dd52848b19b2667e`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4954d9c2f7e3575c7c1b370f79b942a39a290b5d8969aae868db3a4b859b0218`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bb3747e628070f796fc97248f1ffaf64c4dfbb3b02e00d9b52f4acdf6ec4e0`  
		Last Modified: Thu, 14 Oct 2021 02:45:09 GMT  
		Size: 50.9 MB (50881403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.9-windowsservercore-1809`

```console
$ docker pull docker@sha256:e4eec512a2de95c6783851f85f38652b37fce108fb3171a6d7ace46e15f76047
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `docker:20.10.9-windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull docker@sha256:00d1af6859be90ae81443923948f91023c5d9c98c3b0cd509930967d25cc3ab9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737551444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:118b153058557f1f2ed347f423229e946823c10252f6f64941f859b7dcfe91bb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 12:02:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Oct 2021 02:43:13 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 14 Oct 2021 02:43:14 GMT
ENV DOCKER_VERSION=20.10.9
# Thu, 14 Oct 2021 02:43:15 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.9.zip
# Thu, 14 Oct 2021 02:44:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cc0c4e719f418d49c6a0fb87abd2e0e480c5b6fec1bacc3077cacfad9b4ab3e0`  
		Last Modified: Wed, 13 Oct 2021 12:18:09 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd874ac08ee111fe2cf114d0c6cde1f454b67345e21ce092adcb65291fa3d020`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 347.3 KB (347273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f858e26c2cf09cac487c279dce052648a24ae14d8277ac08dd52848b19b2667e`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4954d9c2f7e3575c7c1b370f79b942a39a290b5d8969aae868db3a4b859b0218`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bb3747e628070f796fc97248f1ffaf64c4dfbb3b02e00d9b52f4acdf6ec4e0`  
		Last Modified: Thu, 14 Oct 2021 02:45:09 GMT  
		Size: 50.9 MB (50881403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:d842418d21545fde57c2512681d9bdc4ce0e54f2e0305a293ee20a9b6166932b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:24628ded7711e48db56af875236ac30a8950305ac461332955b3375ac5a87e1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (74967424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1efbbff84703848e1c787073a954e8e3f0146836d94673f2d54f3672296bf82f`
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
# Tue, 05 Oct 2021 17:32:23 GMT
ENV DOCKER_VERSION=20.10.9
# Tue, 05 Oct 2021 17:32:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Oct 2021 17:32:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 05 Oct 2021 17:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:31 GMT
CMD ["sh"]
# Tue, 05 Oct 2021 17:32:37 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 05 Oct 2021 17:32:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 05 Oct 2021 17:32:38 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 05 Oct 2021 17:32:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 05 Oct 2021 17:32:39 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:39 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Oct 2021 17:32:39 GMT
EXPOSE 2375 2376
# Tue, 05 Oct 2021 17:32:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:40 GMT
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
	-	`sha256:c6e88c3a8ccafbb819665e363fc6947b47a896d85170e8b267c6c12176385b3c`  
		Last Modified: Tue, 05 Oct 2021 17:33:31 GMT  
		Size: 63.7 MB (63689714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e00801cfc09a8e327c9cced9fbc94f179e9f03caf50d0ac1c01ae1ca92c3b`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a43c1017099b38ffcabb7b27169d9ca7821bbfea77b15059c969020a0acfd`  
		Last Modified: Tue, 05 Oct 2021 17:33:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52f4e484f770e1039348c98519c8610f67ba16969fb9ab93afae3f4421f7d1`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec67a583a94bdc153dacab38a9b85a032e58cd332069a169388b45727d5a03c`  
		Last Modified: Tue, 05 Oct 2021 17:33:49 GMT  
		Size: 6.5 MB (6521405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a20c97b2389ddc8160afed72508ba7d5ae1464e5837dd19905c4e7130c4e5`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170df0071614602fcd5820d60cc7c9a73f8e10a616928d111e25041951c3507d`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfeb3c70a4f70f3868998e1000a4907ec50a8303595dbf0e96bdd03d59e086c`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:3ba0867a449ca78b731e3251ddeb677fa893dc500293ab0e303a8188b9e4d106
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68779801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6144797d483747bee375b8607893579ff8b6d6ff47e83b10ed4827e4123f549e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:40:48 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 18 Oct 2021 21:40:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:59 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:41:08 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 18 Oct 2021 21:41:08 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:41:09 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 18 Oct 2021 21:41:10 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 18 Oct 2021 21:41:12 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:41:12 GMT
VOLUME [/var/lib/docker]
# Mon, 18 Oct 2021 21:41:13 GMT
EXPOSE 2375 2376
# Mon, 18 Oct 2021 21:41:14 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 18 Oct 2021 21:41:15 GMT
CMD []
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bacb27c3d6ff01f6e8f051e37ec17341cc7fbc76073dea248afcf223aba5d`  
		Last Modified: Mon, 18 Oct 2021 21:44:10 GMT  
		Size: 57.7 MB (57733379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79bdbfa9a5540080db6017b27b917e7c21fbf947abefb068a974a0b55d481e`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a13bdd3b1cef3426a41cadec19b55904b133d95c31c10574f56b0419a93f72`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb034e6582742a188487a0bdde846bf28e29179005b5f423b7d465a2c4e368df`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e8bdd67624c83a9918b7d0bb7d24f84d32a306b3453ac55e213380ee17335d`  
		Last Modified: Mon, 18 Oct 2021 21:44:31 GMT  
		Size: 6.4 MB (6418437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9e9de043d240e7a3e0baf2f1a9bd6bd1da52fd1a1df9db1d97b50b294c98b8`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b746a27963c477864e414004aab19efff02e763e88444128d5bbf735410a4f`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c17f756b76c3b8328ed61cc3fef72a62229860b3a7fefcc6e94edda353b7d3a`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 2.6 KB (2615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:51cd937b2ad1a1d32179f2e9acc01ea46d4e127cdaf493a533172b1fb019af15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:75acfc77a83d9b4d557aab529432058b78ac6d629325c9d61c385cd2fc48fe7c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 MB (95235937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b4aec2427ffe9836431bca031ae4354053a010dae4736917b174d52da90dba`
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
# Tue, 05 Oct 2021 17:32:23 GMT
ENV DOCKER_VERSION=20.10.9
# Tue, 05 Oct 2021 17:32:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Oct 2021 17:32:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 05 Oct 2021 17:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:31 GMT
CMD ["sh"]
# Tue, 05 Oct 2021 17:32:37 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 05 Oct 2021 17:32:37 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 05 Oct 2021 17:32:38 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 05 Oct 2021 17:32:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 05 Oct 2021 17:32:39 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:39 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Oct 2021 17:32:39 GMT
EXPOSE 2375 2376
# Tue, 05 Oct 2021 17:32:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:40 GMT
CMD []
# Tue, 05 Oct 2021 17:32:44 GMT
RUN apk add --no-cache iproute2
# Tue, 05 Oct 2021 17:32:45 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 05 Oct 2021 17:32:46 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 05 Oct 2021 17:32:48 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 05 Oct 2021 17:32:49 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 05 Oct 2021 17:32:50 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 05 Oct 2021 17:32:50 GMT
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
	-	`sha256:c6e88c3a8ccafbb819665e363fc6947b47a896d85170e8b267c6c12176385b3c`  
		Last Modified: Tue, 05 Oct 2021 17:33:31 GMT  
		Size: 63.7 MB (63689714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e00801cfc09a8e327c9cced9fbc94f179e9f03caf50d0ac1c01ae1ca92c3b`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a43c1017099b38ffcabb7b27169d9ca7821bbfea77b15059c969020a0acfd`  
		Last Modified: Tue, 05 Oct 2021 17:33:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52f4e484f770e1039348c98519c8610f67ba16969fb9ab93afae3f4421f7d1`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec67a583a94bdc153dacab38a9b85a032e58cd332069a169388b45727d5a03c`  
		Last Modified: Tue, 05 Oct 2021 17:33:49 GMT  
		Size: 6.5 MB (6521405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a20c97b2389ddc8160afed72508ba7d5ae1464e5837dd19905c4e7130c4e5`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170df0071614602fcd5820d60cc7c9a73f8e10a616928d111e25041951c3507d`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfeb3c70a4f70f3868998e1000a4907ec50a8303595dbf0e96bdd03d59e086c`  
		Last Modified: Tue, 05 Oct 2021 17:33:48 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418f850bf44d36d532f71a72ed317e54531b904953d99821dd316e73e777d23c`  
		Last Modified: Tue, 05 Oct 2021 17:34:08 GMT  
		Size: 1.1 MB (1148745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03facf1a1e41afef60e2e7bad46f0fbd44f5b2b3a3328337c3e0a6049120dd8`  
		Last Modified: Tue, 05 Oct 2021 17:34:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f919e685bb3723d38cd895248bb1c99de9588af3aba7f57ef5cb72eca54106a9`  
		Last Modified: Tue, 05 Oct 2021 17:34:08 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79573e4e685e01787d1e021ea1cecb99cdbf78577b160037c6ed2c7f8f2b304`  
		Last Modified: Tue, 05 Oct 2021 17:34:11 GMT  
		Size: 19.1 MB (19118054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7054ab8c007ff95ebed9750aae6c97b9f692ed317ea464234611c57db8601634`  
		Last Modified: Tue, 05 Oct 2021 17:34:08 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:eb9feb96a9c979384276b169446b5134c441625461108344fde1f18fdee9ce75
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.0 MB (91045261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a26cf3ffc31a4748452e2da3ca2a290c3354e441650e7617aaf4a9fbf6d1750`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:40:48 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 18 Oct 2021 21:40:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:59 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:41:08 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 18 Oct 2021 21:41:08 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:41:09 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 18 Oct 2021 21:41:10 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 18 Oct 2021 21:41:12 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:41:12 GMT
VOLUME [/var/lib/docker]
# Mon, 18 Oct 2021 21:41:13 GMT
EXPOSE 2375 2376
# Mon, 18 Oct 2021 21:41:14 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 18 Oct 2021 21:41:15 GMT
CMD []
# Mon, 18 Oct 2021 21:41:23 GMT
RUN apk add --no-cache iproute2
# Mon, 18 Oct 2021 21:41:24 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 18 Oct 2021 21:41:25 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:41:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 18 Oct 2021 21:41:29 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 18 Oct 2021 21:41:30 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 18 Oct 2021 21:41:31 GMT
USER rootless
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bacb27c3d6ff01f6e8f051e37ec17341cc7fbc76073dea248afcf223aba5d`  
		Last Modified: Mon, 18 Oct 2021 21:44:10 GMT  
		Size: 57.7 MB (57733379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79bdbfa9a5540080db6017b27b917e7c21fbf947abefb068a974a0b55d481e`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a13bdd3b1cef3426a41cadec19b55904b133d95c31c10574f56b0419a93f72`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb034e6582742a188487a0bdde846bf28e29179005b5f423b7d465a2c4e368df`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e8bdd67624c83a9918b7d0bb7d24f84d32a306b3453ac55e213380ee17335d`  
		Last Modified: Mon, 18 Oct 2021 21:44:31 GMT  
		Size: 6.4 MB (6418437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9e9de043d240e7a3e0baf2f1a9bd6bd1da52fd1a1df9db1d97b50b294c98b8`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b746a27963c477864e414004aab19efff02e763e88444128d5bbf735410a4f`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c17f756b76c3b8328ed61cc3fef72a62229860b3a7fefcc6e94edda353b7d3a`  
		Last Modified: Mon, 18 Oct 2021 21:44:30 GMT  
		Size: 2.6 KB (2615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da73c72dcad0b534b2f4febbace9688a2f4a30bf46b188501e200b3be5977b03`  
		Last Modified: Mon, 18 Oct 2021 21:44:52 GMT  
		Size: 1.2 MB (1167836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff4316d7dcf66341a4e5a7a7519ed9d36f902bb95d2169ebc26549a0f95849`  
		Last Modified: Mon, 18 Oct 2021 21:44:52 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba611fb139d8c880c857badbc205cee357e35952ae811c52e90139e68f959d57`  
		Last Modified: Mon, 18 Oct 2021 21:44:52 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098b6fcc42aecdd56305fc4ceba9415e977d589f359ff58a7ee2c72612859ce9`  
		Last Modified: Mon, 18 Oct 2021 21:44:55 GMT  
		Size: 21.1 MB (21096004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeef11aee822059479265f63f55446205a437ef50e49fbfb586c607571b58574`  
		Last Modified: Mon, 18 Oct 2021 21:44:53 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:370cbd65cbf44658bc2ce46c8b606213d9e3e3ea04a7d53a0243d67ca6db95aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:3bf13c54edb2a2b817bcad4ae459bf6d8b867930b5026d1f51d4593f598495fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75071530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed61dfae734a45e9440fbd932eeb2b244f0079a45398e33dd1478f62a4f3be3`
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
# Tue, 05 Oct 2021 17:32:23 GMT
ENV DOCKER_VERSION=20.10.9
# Tue, 05 Oct 2021 17:32:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Oct 2021 17:32:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 05 Oct 2021 17:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:31 GMT
CMD ["sh"]
# Tue, 05 Oct 2021 17:32:54 GMT
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
	-	`sha256:c6e88c3a8ccafbb819665e363fc6947b47a896d85170e8b267c6c12176385b3c`  
		Last Modified: Tue, 05 Oct 2021 17:33:31 GMT  
		Size: 63.7 MB (63689714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e00801cfc09a8e327c9cced9fbc94f179e9f03caf50d0ac1c01ae1ca92c3b`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a43c1017099b38ffcabb7b27169d9ca7821bbfea77b15059c969020a0acfd`  
		Last Modified: Tue, 05 Oct 2021 17:33:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52f4e484f770e1039348c98519c8610f67ba16969fb9ab93afae3f4421f7d1`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e22895e9057604af4145b328a599ef34ed98eee9085de276ad33fe1adf50f5f`  
		Last Modified: Tue, 05 Oct 2021 17:34:29 GMT  
		Size: 6.6 MB (6630406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:6f7fe91a5a952fb482822be280a9c17313785627cdf33330c1980bf4404d6787
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69095577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b1ae00454f4fd0beeab581baa00fe5961ae9b97bae5802e58bc1d0e49636a41`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:40:48 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 18 Oct 2021 21:40:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:59 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:41:38 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bacb27c3d6ff01f6e8f051e37ec17341cc7fbc76073dea248afcf223aba5d`  
		Last Modified: Mon, 18 Oct 2021 21:44:10 GMT  
		Size: 57.7 MB (57733379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79bdbfa9a5540080db6017b27b917e7c21fbf947abefb068a974a0b55d481e`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a13bdd3b1cef3426a41cadec19b55904b133d95c31c10574f56b0419a93f72`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb034e6582742a188487a0bdde846bf28e29179005b5f423b7d465a2c4e368df`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae700626b8f4a7301ee4ec15808eb5b1b281fa56ecf42eb4a653b7f0b2a5f722`  
		Last Modified: Mon, 18 Oct 2021 21:45:15 GMT  
		Size: 6.7 MB (6739077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:938bcb85cf77db2b80d219abd5a1424ec15ce11a3adaea6423fa16cc9acfe926
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:62302357e804b152e157d3603ce7a97c3f368a626ce027eee1d1e02b5ae924f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68441124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6448e722e510f9bb0bb5c2f65ef99295fc2321b656c00f088078ccf6564372b`
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
# Tue, 05 Oct 2021 17:32:23 GMT
ENV DOCKER_VERSION=20.10.9
# Tue, 05 Oct 2021 17:32:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 05 Oct 2021 17:32:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 05 Oct 2021 17:32:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Oct 2021 17:32:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 05 Oct 2021 17:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:32:31 GMT
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
	-	`sha256:c6e88c3a8ccafbb819665e363fc6947b47a896d85170e8b267c6c12176385b3c`  
		Last Modified: Tue, 05 Oct 2021 17:33:31 GMT  
		Size: 63.7 MB (63689714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e00801cfc09a8e327c9cced9fbc94f179e9f03caf50d0ac1c01ae1ca92c3b`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a43c1017099b38ffcabb7b27169d9ca7821bbfea77b15059c969020a0acfd`  
		Last Modified: Tue, 05 Oct 2021 17:33:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52f4e484f770e1039348c98519c8610f67ba16969fb9ab93afae3f4421f7d1`  
		Last Modified: Tue, 05 Oct 2021 17:33:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1710b19ecaa7eba8537ea64a35ddec333ff128cda5f2f19b7c4cd6e3a4e0daf7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62356500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c324afd4ac0437589f8f6e825c2fed8ef663773f55ac7c8e85cd589f554239d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:40:48 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 18 Oct 2021 21:40:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:59 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bacb27c3d6ff01f6e8f051e37ec17341cc7fbc76073dea248afcf223aba5d`  
		Last Modified: Mon, 18 Oct 2021 21:44:10 GMT  
		Size: 57.7 MB (57733379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79bdbfa9a5540080db6017b27b917e7c21fbf947abefb068a974a0b55d481e`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a13bdd3b1cef3426a41cadec19b55904b133d95c31c10574f56b0419a93f72`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb034e6582742a188487a0bdde846bf28e29179005b5f423b7d465a2c4e368df`  
		Last Modified: Mon, 18 Oct 2021 21:44:01 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:rc`

```console
$ docker pull docker@sha256:abd9743f601c58c12db87ba997758a7a22d37b2800d15d7a0a90d4a777f4d86e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:rc` - linux; amd64

```console
$ docker pull docker@sha256:3769dd5e09b1795718cec653d648d55558244ebd8fe13955e02e83bba97bb495
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (74032061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b076b43daf1313e0b147059fa86500a35771815f9413671c44aceca8c3905722`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:15:43 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 22 Oct 2020 03:15:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Dec 2020 01:19:40 GMT
ENV DOCKER_VERSION=20.10.0-rc2
# Thu, 03 Dec 2020 01:19:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.0-rc2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.0-rc2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.0-rc2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.0-rc2.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Dec 2020 01:19:47 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Dec 2020 01:19:47 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Dec 2020 01:19:47 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Dec 2020 01:19:48 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Dec 2020 01:19:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Dec 2020 01:19:48 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7c675703d60dc4d757acb40557350159f600ca3d49e2e8d4c2039dd6b69457`  
		Last Modified: Thu, 22 Oct 2020 03:16:47 GMT  
		Size: 2.0 MB (2039054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8c12a437cbe4e104dcea425e0ce277a2442603e14551d22a948e11026ae658`  
		Last Modified: Thu, 22 Oct 2020 03:16:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0fd8b7f6d785daed3820c5e1498e61167583e9045feac86ffb7e44cc08a098`  
		Last Modified: Thu, 03 Dec 2020 01:21:03 GMT  
		Size: 69.2 MB (69194310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db597305dcaeb9a5ab05768839f670f942793156b7b3b3936ce746314bfca19`  
		Last Modified: Thu, 03 Dec 2020 01:20:49 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103a137d36f54bc2da72b6de7a354e8ac532e331da4fa7cea3061e707ee631d6`  
		Last Modified: Thu, 03 Dec 2020 01:20:49 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3157e29d9bca4123fa681ea84dd51dad3441b7f2ac7a8d8cb09865df9f7c7fbd`  
		Last Modified: Thu, 03 Dec 2020 01:20:50 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:eab2a4f03c6f78fa775f16495d33d5bd9db312068b14db9caa3b631968f19f57
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62354582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cd1e6d54b025850351cefe3112edff43a74d0a46d04ad08066c1ba8d7e2ea9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:39:53 GMT
ENV DOCKER_VERSION=20.10.10-rc1
# Mon, 18 Oct 2021 21:39:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.10-rc1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.10-rc1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:02 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:04 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112f3374d6fabbfe7b2c992c077ac3658ff8d061a8e18265257b45cd60739c0d`  
		Last Modified: Mon, 18 Oct 2021 21:42:54 GMT  
		Size: 57.7 MB (57731459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ffe46428f8f4e7d13099151a78aa124e254522444b80d46bcec4e3e3fc41eb`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6699487bf567a986ddfb631b8655b487e6922d4a86ee9ff17b738d32ae342fa7`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4f64888be82e82dc404000ef04193fab09949191aa4a5abd16eb3f76de6422`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:rc-dind`

```console
$ docker pull docker@sha256:54a3e9071f9308d3643e44a0922f353ade496af29813d4bf6337ee31f98033fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:rc-dind` - linux; amd64

```console
$ docker pull docker@sha256:0805d140b875b9bc8ebfdbae9ea4b26ba60ee90640a636c575713b6825035f66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (79995526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1d8f7c2d7206c43f115c4af423e1637a1f435068bc08c12e23748f21e55af20`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:15:43 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 22 Oct 2020 03:15:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Dec 2020 01:19:40 GMT
ENV DOCKER_VERSION=20.10.0-rc2
# Thu, 03 Dec 2020 01:19:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.0-rc2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.0-rc2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.0-rc2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.0-rc2.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Dec 2020 01:19:47 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Dec 2020 01:19:47 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Dec 2020 01:19:47 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Dec 2020 01:19:48 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Dec 2020 01:19:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Dec 2020 01:19:48 GMT
CMD ["sh"]
# Thu, 03 Dec 2020 01:19:55 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 03 Dec 2020 01:19:56 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 03 Dec 2020 01:19:56 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Thu, 03 Dec 2020 01:19:57 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 03 Dec 2020 01:19:57 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Thu, 03 Dec 2020 01:19:57 GMT
VOLUME [/var/lib/docker]
# Thu, 03 Dec 2020 01:19:58 GMT
EXPOSE 2375 2376
# Thu, 03 Dec 2020 01:19:58 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 03 Dec 2020 01:19:58 GMT
CMD []
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7c675703d60dc4d757acb40557350159f600ca3d49e2e8d4c2039dd6b69457`  
		Last Modified: Thu, 22 Oct 2020 03:16:47 GMT  
		Size: 2.0 MB (2039054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8c12a437cbe4e104dcea425e0ce277a2442603e14551d22a948e11026ae658`  
		Last Modified: Thu, 22 Oct 2020 03:16:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0fd8b7f6d785daed3820c5e1498e61167583e9045feac86ffb7e44cc08a098`  
		Last Modified: Thu, 03 Dec 2020 01:21:03 GMT  
		Size: 69.2 MB (69194310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db597305dcaeb9a5ab05768839f670f942793156b7b3b3936ce746314bfca19`  
		Last Modified: Thu, 03 Dec 2020 01:20:49 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103a137d36f54bc2da72b6de7a354e8ac532e331da4fa7cea3061e707ee631d6`  
		Last Modified: Thu, 03 Dec 2020 01:20:49 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3157e29d9bca4123fa681ea84dd51dad3441b7f2ac7a8d8cb09865df9f7c7fbd`  
		Last Modified: Thu, 03 Dec 2020 01:20:50 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d41eb34354d9c453eb21d4d874b79246fdde42e242ce3b3946e3fb08cd77b1`  
		Last Modified: Thu, 03 Dec 2020 01:21:10 GMT  
		Size: 6.0 MB (5958742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e049752a368345c7b7d2d9539852eeac961803cd38f17028532ee69a4294dfa9`  
		Last Modified: Thu, 03 Dec 2020 01:21:10 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238431a551c0fd0e6304bda8ab6e3806b3407161b0ddaaa51d97ea7c01ee9172`  
		Last Modified: Thu, 03 Dec 2020 01:21:09 GMT  
		Size: 931.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff110f4494d28d0434d2149ac8619524c81c1701c64fce9a08150d3c6134704`  
		Last Modified: Thu, 03 Dec 2020 01:21:10 GMT  
		Size: 2.5 KB (2509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:03f725eb2e70a25215590328677b3f23e21f5e5a620476f43d3ab036efee3343
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68777909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15a40ad8d21fe5b8d86077ad0f06de3c91a4b4cffc74c1be70fc259f15054b67`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:39:53 GMT
ENV DOCKER_VERSION=20.10.10-rc1
# Mon, 18 Oct 2021 21:39:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.10-rc1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.10-rc1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:02 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:04 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:40:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 18 Oct 2021 21:40:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:40:14 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 18 Oct 2021 21:40:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 18 Oct 2021 21:40:17 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:17 GMT
VOLUME [/var/lib/docker]
# Mon, 18 Oct 2021 21:40:18 GMT
EXPOSE 2375 2376
# Mon, 18 Oct 2021 21:40:19 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:20 GMT
CMD []
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112f3374d6fabbfe7b2c992c077ac3658ff8d061a8e18265257b45cd60739c0d`  
		Last Modified: Mon, 18 Oct 2021 21:42:54 GMT  
		Size: 57.7 MB (57731459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ffe46428f8f4e7d13099151a78aa124e254522444b80d46bcec4e3e3fc41eb`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6699487bf567a986ddfb631b8655b487e6922d4a86ee9ff17b738d32ae342fa7`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4f64888be82e82dc404000ef04193fab09949191aa4a5abd16eb3f76de6422`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6501ba4a4760252cf7cc02d607ee723591654cc0bb5f52520a6e33dc7a0edc25`  
		Last Modified: Mon, 18 Oct 2021 21:43:12 GMT  
		Size: 6.4 MB (6418461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a680b385ce15bb20e7ba5ac40667562dec340d2d81461023bdf90c3e3fabbebd`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f199395c417cc0c7e6398feae5d9baf39d65e2e0a7bb70170c70b89e589e8dfe`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1aee83547715d6f96b27af07d2631947e319c0f257cbebfed3719ab3e20529`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:rc-dind-rootless`

```console
$ docker pull docker@sha256:a2ad342f46ccf0daa32a00de0c18297b6fae7f26bbedf659379106326ba40a45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:rc-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:ba9a867298f514f0155fc0015a88624808e42c513196c562d22d8b37dda7e8a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101261107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:004b0ab8718ed6fab023f19e76b5bcd1db501061987c8a2d3fb61965d8a62c25`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:15:43 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 22 Oct 2020 03:15:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Dec 2020 01:19:40 GMT
ENV DOCKER_VERSION=20.10.0-rc2
# Thu, 03 Dec 2020 01:19:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.0-rc2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.0-rc2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.0-rc2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.0-rc2.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Dec 2020 01:19:47 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Dec 2020 01:19:47 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Dec 2020 01:19:47 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Dec 2020 01:19:48 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Dec 2020 01:19:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Dec 2020 01:19:48 GMT
CMD ["sh"]
# Thu, 03 Dec 2020 01:19:55 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 03 Dec 2020 01:19:56 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 03 Dec 2020 01:19:56 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Thu, 03 Dec 2020 01:19:57 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 03 Dec 2020 01:19:57 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Thu, 03 Dec 2020 01:19:57 GMT
VOLUME [/var/lib/docker]
# Thu, 03 Dec 2020 01:19:58 GMT
EXPOSE 2375 2376
# Thu, 03 Dec 2020 01:19:58 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 03 Dec 2020 01:19:58 GMT
CMD []
# Thu, 03 Dec 2020 01:20:03 GMT
RUN apk add --no-cache iproute2
# Thu, 03 Dec 2020 01:20:04 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 03 Dec 2020 01:20:05 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 03 Dec 2020 01:20:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-20.10.0-rc2.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 03 Dec 2020 01:20:08 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 03 Dec 2020 01:20:09 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 03 Dec 2020 01:20:09 GMT
USER rootless
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7c675703d60dc4d757acb40557350159f600ca3d49e2e8d4c2039dd6b69457`  
		Last Modified: Thu, 22 Oct 2020 03:16:47 GMT  
		Size: 2.0 MB (2039054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8c12a437cbe4e104dcea425e0ce277a2442603e14551d22a948e11026ae658`  
		Last Modified: Thu, 22 Oct 2020 03:16:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0fd8b7f6d785daed3820c5e1498e61167583e9045feac86ffb7e44cc08a098`  
		Last Modified: Thu, 03 Dec 2020 01:21:03 GMT  
		Size: 69.2 MB (69194310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db597305dcaeb9a5ab05768839f670f942793156b7b3b3936ce746314bfca19`  
		Last Modified: Thu, 03 Dec 2020 01:20:49 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103a137d36f54bc2da72b6de7a354e8ac532e331da4fa7cea3061e707ee631d6`  
		Last Modified: Thu, 03 Dec 2020 01:20:49 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3157e29d9bca4123fa681ea84dd51dad3441b7f2ac7a8d8cb09865df9f7c7fbd`  
		Last Modified: Thu, 03 Dec 2020 01:20:50 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d41eb34354d9c453eb21d4d874b79246fdde42e242ce3b3946e3fb08cd77b1`  
		Last Modified: Thu, 03 Dec 2020 01:21:10 GMT  
		Size: 6.0 MB (5958742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e049752a368345c7b7d2d9539852eeac961803cd38f17028532ee69a4294dfa9`  
		Last Modified: Thu, 03 Dec 2020 01:21:10 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238431a551c0fd0e6304bda8ab6e3806b3407161b0ddaaa51d97ea7c01ee9172`  
		Last Modified: Thu, 03 Dec 2020 01:21:09 GMT  
		Size: 931.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff110f4494d28d0434d2149ac8619524c81c1701c64fce9a08150d3c6134704`  
		Last Modified: Thu, 03 Dec 2020 01:21:10 GMT  
		Size: 2.5 KB (2509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20dbfa1b4e2ec98111aa0501360a509205fbf16bc526d399cfa670d0c35b6046`  
		Last Modified: Thu, 03 Dec 2020 01:21:17 GMT  
		Size: 1.1 MB (1092668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f728936c6fdb24935e0bb1366ed702b917e9581519d22efab93f8728513a259a`  
		Last Modified: Thu, 03 Dec 2020 01:21:17 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b638cd1abd59f9f12d28d5d6227cdb991c66c16fd6f9b00dc39564d1583b251`  
		Last Modified: Thu, 03 Dec 2020 01:21:17 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cac38aa50f31cfa5934d05e52f6ff76d5b8809a374846c9b36af98c8f5a822`  
		Last Modified: Thu, 03 Dec 2020 01:21:21 GMT  
		Size: 20.2 MB (20171300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbc24424926ce09c4f9387a3510fe8d83e0d537f83a25565d4d6f8eb4a43a50`  
		Last Modified: Thu, 03 Dec 2020 01:21:17 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:036139df2869c66580cf19c3f5e10fbfcdc51e44e4c253dd52461dbaf8756d1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.0 MB (91048708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:592281427bbc8f0ac33cd2c8cc861023d89fe8804da4082b826bb8976bf55339`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:39:53 GMT
ENV DOCKER_VERSION=20.10.10-rc1
# Mon, 18 Oct 2021 21:39:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.10-rc1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.10-rc1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:02 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:04 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:40:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 18 Oct 2021 21:40:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:40:14 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 18 Oct 2021 21:40:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 18 Oct 2021 21:40:17 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:17 GMT
VOLUME [/var/lib/docker]
# Mon, 18 Oct 2021 21:40:18 GMT
EXPOSE 2375 2376
# Mon, 18 Oct 2021 21:40:19 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:20 GMT
CMD []
# Mon, 18 Oct 2021 21:40:27 GMT
RUN apk add --no-cache iproute2
# Mon, 18 Oct 2021 21:40:28 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 18 Oct 2021 21:40:29 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:40:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-rootless-extras-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 18 Oct 2021 21:40:33 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 18 Oct 2021 21:40:34 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 18 Oct 2021 21:40:35 GMT
USER rootless
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112f3374d6fabbfe7b2c992c077ac3658ff8d061a8e18265257b45cd60739c0d`  
		Last Modified: Mon, 18 Oct 2021 21:42:54 GMT  
		Size: 57.7 MB (57731459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ffe46428f8f4e7d13099151a78aa124e254522444b80d46bcec4e3e3fc41eb`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6699487bf567a986ddfb631b8655b487e6922d4a86ee9ff17b738d32ae342fa7`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4f64888be82e82dc404000ef04193fab09949191aa4a5abd16eb3f76de6422`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6501ba4a4760252cf7cc02d607ee723591654cc0bb5f52520a6e33dc7a0edc25`  
		Last Modified: Mon, 18 Oct 2021 21:43:12 GMT  
		Size: 6.4 MB (6418461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a680b385ce15bb20e7ba5ac40667562dec340d2d81461023bdf90c3e3fabbebd`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f199395c417cc0c7e6398feae5d9baf39d65e2e0a7bb70170c70b89e589e8dfe`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1aee83547715d6f96b27af07d2631947e319c0f257cbebfed3719ab3e20529`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375da3ba74accf4f4e776d8ea0d05c23a13b4b2b720c68351e5a106a84dda6e3`  
		Last Modified: Mon, 18 Oct 2021 21:43:29 GMT  
		Size: 1.2 MB (1167846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ac90cf496368c08bead07501a2fb6bcf1be125a482b1ba65545eb127ade900`  
		Last Modified: Mon, 18 Oct 2021 21:43:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1a7298291f6aaebb45b8b88842f7e71ac8c03b3ba86694de07dcba597dce8b`  
		Last Modified: Mon, 18 Oct 2021 21:43:29 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f92a9eb80f5eb157bb083cbb43ee01b129e3a55ba704b5f14a5e73d3957e05f`  
		Last Modified: Mon, 18 Oct 2021 21:43:32 GMT  
		Size: 21.1 MB (21101330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6559ad5989ef407de45b61e2a3ebc564a674911a70765ee6abc411c6c43b88b2`  
		Last Modified: Mon, 18 Oct 2021 21:43:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:rc-git`

```console
$ docker pull docker@sha256:2313c01f288bdcee76a986334f8e00f7b361442710f2b7cc1ced9f0983ce0825
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:rc-git` - linux; amd64

```console
$ docker pull docker@sha256:50da362dfee957933c12cf5c491ce74186d4649909508ea62d1071d6ca95d82e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.3 MB (82344149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f16515870a2368ced3032e3241b1ddcfef531d220a78ee33fe20dc4dae86f12`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:15:43 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 22 Oct 2020 03:15:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Dec 2020 01:19:40 GMT
ENV DOCKER_VERSION=20.10.0-rc2
# Thu, 03 Dec 2020 01:19:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.0-rc2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.0-rc2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.0-rc2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.0-rc2.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Dec 2020 01:19:47 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Dec 2020 01:19:47 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Dec 2020 01:19:47 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Dec 2020 01:19:48 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Dec 2020 01:19:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Dec 2020 01:19:48 GMT
CMD ["sh"]
# Thu, 03 Dec 2020 01:20:14 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7c675703d60dc4d757acb40557350159f600ca3d49e2e8d4c2039dd6b69457`  
		Last Modified: Thu, 22 Oct 2020 03:16:47 GMT  
		Size: 2.0 MB (2039054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8c12a437cbe4e104dcea425e0ce277a2442603e14551d22a948e11026ae658`  
		Last Modified: Thu, 22 Oct 2020 03:16:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0fd8b7f6d785daed3820c5e1498e61167583e9045feac86ffb7e44cc08a098`  
		Last Modified: Thu, 03 Dec 2020 01:21:03 GMT  
		Size: 69.2 MB (69194310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db597305dcaeb9a5ab05768839f670f942793156b7b3b3936ce746314bfca19`  
		Last Modified: Thu, 03 Dec 2020 01:20:49 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103a137d36f54bc2da72b6de7a354e8ac532e331da4fa7cea3061e707ee631d6`  
		Last Modified: Thu, 03 Dec 2020 01:20:49 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3157e29d9bca4123fa681ea84dd51dad3441b7f2ac7a8d8cb09865df9f7c7fbd`  
		Last Modified: Thu, 03 Dec 2020 01:20:50 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb412ed0bbeb7d18fa0721ca6ebdff49ee36167e163ff98e4340081383937f5`  
		Last Modified: Thu, 03 Dec 2020 01:21:29 GMT  
		Size: 8.3 MB (8312088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:a85ba73189c3335850cce7608bd089cdcad6cb0c6131187d644f6d17f6ec6eac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69093629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638acbdc55fc536c4148cdf061e5ea335d61c5db1d7d75a467d1c96babf85bcb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:39:53 GMT
ENV DOCKER_VERSION=20.10.10-rc1
# Mon, 18 Oct 2021 21:39:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.10-rc1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.10-rc1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:02 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:04 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:40:42 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112f3374d6fabbfe7b2c992c077ac3658ff8d061a8e18265257b45cd60739c0d`  
		Last Modified: Mon, 18 Oct 2021 21:42:54 GMT  
		Size: 57.7 MB (57731459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ffe46428f8f4e7d13099151a78aa124e254522444b80d46bcec4e3e3fc41eb`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6699487bf567a986ddfb631b8655b487e6922d4a86ee9ff17b738d32ae342fa7`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4f64888be82e82dc404000ef04193fab09949191aa4a5abd16eb3f76de6422`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a7843f30ad6a2fa274b0b141d4ddbf161ab3f789f4de5d6f2132dba26513b8`  
		Last Modified: Mon, 18 Oct 2021 21:43:47 GMT  
		Size: 6.7 MB (6739047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:rc-windowsservercore`

```console
$ docker pull docker@sha256:b93c815cb85b0b33bda3995458689c458b48600f7bebf504ae7819c5f2bb0d81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.1884; amd64

### `docker:rc-windowsservercore` - windows version 10.0.14393.1884; amd64

```console
$ docker pull docker@sha256:ecb33e06762179b8a50fc3204702e18b0d5631710f3c5f51e865103eea6a4413
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5372790933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03cd7d97ead7d0f7646b6c4466ae43a81295dbb77a1330ef15034c0a5df311fe`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 13 Nov 2017 21:42:13 GMT
RUN Install update 10.0.14393.1884
# Wed, 15 Nov 2017 03:14:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Nov 2017 19:27:10 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Nov 2017 19:27:11 GMT
ENV DOCKER_CHANNEL=test
# Wed, 15 Nov 2017 19:27:12 GMT
ENV DOCKER_VERSION=17.11.0-ce-rc3
# Wed, 15 Nov 2017 19:28:13 GMT
RUN $url = ('https://download.docker.com/win/static/{0}/x86_64/docker-{1}.zip' -f $env:DOCKER_CHANNEL, $env:DOCKER_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ead9f4ead3c5a712cb213a5318f4a8bf3604bc16e16ce4f7cf0b66f7d2073282`  
		Last Modified: Tue, 18 Sep 2018 00:42:16 GMT  
		Size: 1.3 GB (1286993027 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4bd6cd94ee2a374930b7554f113d83a6d2d7c4fc6059acd6f2f60e0f29d2f26`  
		Last Modified: Wed, 15 Nov 2017 10:26:12 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a6bca6ca4a5af1b9ecee7c5d06eed25aaf7d650400c816faf8118c069fcdc6`  
		Last Modified: Wed, 15 Nov 2017 19:30:54 GMT  
		Size: 4.9 MB (4876193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5674b5976285ba892ab4f5b91e7a35ff744c5cf8dbb16ed3b48c2218b651af0`  
		Last Modified: Wed, 15 Nov 2017 19:30:53 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7e6c9be57254dd1dd8a2fe6f99bf9322b4fdb1bc8e76149adf4d0e3619786b`  
		Last Modified: Wed, 15 Nov 2017 19:30:53 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a52471cc70e65173105c24345a376c017bf2459a5152685139bdca4ee598ff`  
		Last Modified: Wed, 15 Nov 2017 19:30:56 GMT  
		Size: 10.9 MB (10932220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:rc-windowsservercore-1809`

```console
$ docker pull docker@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `docker:windowsservercore`

```console
$ docker pull docker@sha256:e4eec512a2de95c6783851f85f38652b37fce108fb3171a6d7ace46e15f76047
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `docker:windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull docker@sha256:00d1af6859be90ae81443923948f91023c5d9c98c3b0cd509930967d25cc3ab9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737551444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:118b153058557f1f2ed347f423229e946823c10252f6f64941f859b7dcfe91bb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 12:02:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Oct 2021 02:43:13 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 14 Oct 2021 02:43:14 GMT
ENV DOCKER_VERSION=20.10.9
# Thu, 14 Oct 2021 02:43:15 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.9.zip
# Thu, 14 Oct 2021 02:44:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cc0c4e719f418d49c6a0fb87abd2e0e480c5b6fec1bacc3077cacfad9b4ab3e0`  
		Last Modified: Wed, 13 Oct 2021 12:18:09 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd874ac08ee111fe2cf114d0c6cde1f454b67345e21ce092adcb65291fa3d020`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 347.3 KB (347273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f858e26c2cf09cac487c279dce052648a24ae14d8277ac08dd52848b19b2667e`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4954d9c2f7e3575c7c1b370f79b942a39a290b5d8969aae868db3a4b859b0218`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bb3747e628070f796fc97248f1ffaf64c4dfbb3b02e00d9b52f4acdf6ec4e0`  
		Last Modified: Thu, 14 Oct 2021 02:45:09 GMT  
		Size: 50.9 MB (50881403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:e4eec512a2de95c6783851f85f38652b37fce108fb3171a6d7ace46e15f76047
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull docker@sha256:00d1af6859be90ae81443923948f91023c5d9c98c3b0cd509930967d25cc3ab9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737551444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:118b153058557f1f2ed347f423229e946823c10252f6f64941f859b7dcfe91bb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 12:02:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Oct 2021 02:43:13 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 14 Oct 2021 02:43:14 GMT
ENV DOCKER_VERSION=20.10.9
# Thu, 14 Oct 2021 02:43:15 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.9.zip
# Thu, 14 Oct 2021 02:44:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cc0c4e719f418d49c6a0fb87abd2e0e480c5b6fec1bacc3077cacfad9b4ab3e0`  
		Last Modified: Wed, 13 Oct 2021 12:18:09 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd874ac08ee111fe2cf114d0c6cde1f454b67345e21ce092adcb65291fa3d020`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 347.3 KB (347273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f858e26c2cf09cac487c279dce052648a24ae14d8277ac08dd52848b19b2667e`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4954d9c2f7e3575c7c1b370f79b942a39a290b5d8969aae868db3a4b859b0218`  
		Last Modified: Thu, 14 Oct 2021 02:44:58 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bb3747e628070f796fc97248f1ffaf64c4dfbb3b02e00d9b52f4acdf6ec4e0`  
		Last Modified: Thu, 14 Oct 2021 02:45:09 GMT  
		Size: 50.9 MB (50881403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
