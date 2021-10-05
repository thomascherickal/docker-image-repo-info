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
-	[`docker:windowsservercore`](#dockerwindowsservercore)
-	[`docker:windowsservercore-1809`](#dockerwindowsservercore-1809)

## `docker:20`

```console
$ docker pull docker@sha256:e7c9c600322345ad23160a0cafde129426270f50ae83133f5354c3fe347a36c2
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
$ docker pull docker@sha256:3a95cba826396eb3fb4b07117bd1386e46bd982834e622a0a73a7c9d4af7e474
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62356071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4799c468fbdd4c40fd59367653432a1cd16b199c572b72cc7059f46d20130075`
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
# Mon, 04 Oct 2021 22:39:36 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:39:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 04 Oct 2021 22:39:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 04 Oct 2021 22:39:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:42 GMT
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
	-	`sha256:2addeb3702952172db1a24220381e0ef6580b99177900ac4d13119b213c2fcfc`  
		Last Modified: Mon, 04 Oct 2021 22:41:15 GMT  
		Size: 57.7 MB (57733347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb723bbe59439dde838001146817815fb936b405e719e023874e6c96f0a10c3f`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da7ad22416e3ba9ff03eac3fe069bd73b06cdac1fd584e932e9f35270fae50`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97dbd9a21f6258fbc117eeddf6fb34a1172588deb227ce6ffb2ab00321631af`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind`

```console
$ docker pull docker@sha256:d20f0866ee1aca6b0eb7bc8bdb0d0c938721c7f79219b1d3bc1aa58666928586
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
$ docker pull docker@sha256:25a2c533ed67819c4726fad3ccaa5a1fbcfd602149d1b63c663b620714ec13fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68779507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f4dc61e43a85443d5bc5759e6ddf1035da284ae045c44dd173830b798dbe53`
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
# Mon, 04 Oct 2021 22:39:36 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:39:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 04 Oct 2021 22:39:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 04 Oct 2021 22:39:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:42 GMT
CMD ["sh"]
# Mon, 04 Oct 2021 22:39:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 04 Oct 2021 22:39:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 04 Oct 2021 22:39:53 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 04 Oct 2021 22:39:54 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 04 Oct 2021 22:39:54 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:54 GMT
VOLUME [/var/lib/docker]
# Mon, 04 Oct 2021 22:39:54 GMT
EXPOSE 2375 2376
# Mon, 04 Oct 2021 22:39:55 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:55 GMT
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
	-	`sha256:2addeb3702952172db1a24220381e0ef6580b99177900ac4d13119b213c2fcfc`  
		Last Modified: Mon, 04 Oct 2021 22:41:15 GMT  
		Size: 57.7 MB (57733347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb723bbe59439dde838001146817815fb936b405e719e023874e6c96f0a10c3f`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da7ad22416e3ba9ff03eac3fe069bd73b06cdac1fd584e932e9f35270fae50`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97dbd9a21f6258fbc117eeddf6fb34a1172588deb227ce6ffb2ab00321631af`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6df64ef29bdc4a4edaabe9dba4c929323e0fb59f04d2c4157d1614bd477b4c`  
		Last Modified: Mon, 04 Oct 2021 22:41:38 GMT  
		Size: 6.4 MB (6418544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab2a956e5b959cab7be1b5014e743e67aa28c92a3a2b095fa35e0ad32dcb269`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c7d1ec1ea400226cdcfba7d06bc6bdf859f3f39fbf91d93258c1b90b37368`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eedd8c550c3dd9f5a5cb146b38007c1f143f1c3abc63edb69c622d288eb6cd`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:f06dfdfd278026427fb1ebf15e05d4bde89df85ff3ba2334fc964a71a705d16a
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
$ docker pull docker@sha256:81af51e044194e802cc9e2ff99144cfc2c4988731d4597bdeeeef6e5e7a583d3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.0 MB (91045329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6bf6ba3bce99fb59f75ec0438ad494b919f079b40ab77f41c7319cb0cacfd44`
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
# Mon, 04 Oct 2021 22:39:36 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:39:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 04 Oct 2021 22:39:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 04 Oct 2021 22:39:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:42 GMT
CMD ["sh"]
# Mon, 04 Oct 2021 22:39:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 04 Oct 2021 22:39:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 04 Oct 2021 22:39:53 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 04 Oct 2021 22:39:54 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 04 Oct 2021 22:39:54 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:54 GMT
VOLUME [/var/lib/docker]
# Mon, 04 Oct 2021 22:39:54 GMT
EXPOSE 2375 2376
# Mon, 04 Oct 2021 22:39:55 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:55 GMT
CMD []
# Mon, 04 Oct 2021 22:40:03 GMT
RUN apk add --no-cache iproute2
# Mon, 04 Oct 2021 22:40:04 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 04 Oct 2021 22:40:04 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 04 Oct 2021 22:40:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 04 Oct 2021 22:40:08 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 04 Oct 2021 22:40:08 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 04 Oct 2021 22:40:08 GMT
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
	-	`sha256:2addeb3702952172db1a24220381e0ef6580b99177900ac4d13119b213c2fcfc`  
		Last Modified: Mon, 04 Oct 2021 22:41:15 GMT  
		Size: 57.7 MB (57733347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb723bbe59439dde838001146817815fb936b405e719e023874e6c96f0a10c3f`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da7ad22416e3ba9ff03eac3fe069bd73b06cdac1fd584e932e9f35270fae50`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97dbd9a21f6258fbc117eeddf6fb34a1172588deb227ce6ffb2ab00321631af`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6df64ef29bdc4a4edaabe9dba4c929323e0fb59f04d2c4157d1614bd477b4c`  
		Last Modified: Mon, 04 Oct 2021 22:41:38 GMT  
		Size: 6.4 MB (6418544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab2a956e5b959cab7be1b5014e743e67aa28c92a3a2b095fa35e0ad32dcb269`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c7d1ec1ea400226cdcfba7d06bc6bdf859f3f39fbf91d93258c1b90b37368`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eedd8c550c3dd9f5a5cb146b38007c1f143f1c3abc63edb69c622d288eb6cd`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d22f8eb08ad02090048708d5c999c5952be4c8d02c6dcb805da08d4012c288c`  
		Last Modified: Mon, 04 Oct 2021 22:42:00 GMT  
		Size: 1.2 MB (1168110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a0714a4fdbcb6036fccf4cf380ac24fc7edd6c974ad7a5731f13c1966238bd`  
		Last Modified: Mon, 04 Oct 2021 22:42:00 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d79b658117c879c9103d01547357c7566fc262750d0b62c30966d4d49defab`  
		Last Modified: Mon, 04 Oct 2021 22:42:00 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc95b12a74fd36add08fa63f789816fb9cbea1ddc4bbef6a4406364b0c454f2`  
		Last Modified: Mon, 04 Oct 2021 22:42:04 GMT  
		Size: 21.1 MB (21095995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba365bba8d1721288d49e57f54c068465199da261e7f376686e5b2db5c06bf9`  
		Last Modified: Mon, 04 Oct 2021 22:42:00 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-git`

```console
$ docker pull docker@sha256:61f6baf32667fc13a9850b16bf6c6de6c8a1c1302ba23dda8350127430f48b17
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
$ docker pull docker@sha256:27b5d5b7687d6a932d2bc0230af9c258588b2d962d77de01b2553b121bbca2de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69095380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc52e2bf2a201533bcb1dcf4ac4284d848ef238ac5e9acda87bfaa02989e7f59`
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
# Mon, 04 Oct 2021 22:39:36 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:39:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 04 Oct 2021 22:39:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 04 Oct 2021 22:39:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:42 GMT
CMD ["sh"]
# Mon, 04 Oct 2021 22:40:16 GMT
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
	-	`sha256:2addeb3702952172db1a24220381e0ef6580b99177900ac4d13119b213c2fcfc`  
		Last Modified: Mon, 04 Oct 2021 22:41:15 GMT  
		Size: 57.7 MB (57733347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb723bbe59439dde838001146817815fb936b405e719e023874e6c96f0a10c3f`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da7ad22416e3ba9ff03eac3fe069bd73b06cdac1fd584e932e9f35270fae50`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97dbd9a21f6258fbc117eeddf6fb34a1172588deb227ce6ffb2ab00321631af`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bed24c5b37ab30374c66d0fb367cceeaaa68d6483601e0413a8fb1b97f86092`  
		Last Modified: Mon, 04 Oct 2021 22:42:24 GMT  
		Size: 6.7 MB (6739309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore`

```console
$ docker pull docker@sha256:b2cc2fdb94ee0637c9c04319f7d77d161f530672501ff22bf0e52504bf7af0cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `docker:20-windowsservercore` - windows version 10.0.17763.2183; amd64

```console
$ docker pull docker@sha256:aca950618ba0f6f9a7b717dab70a0b0eee15e6e02bf1b0606d8d5f78ee92d63d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737962479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:372be2a200c2f353972f63b2c2014a0c40ab15eb1448345a850fa2b8531d677f`
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
# Mon, 04 Oct 2021 22:15:14 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:15:15 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.9.zip
# Mon, 04 Oct 2021 22:16:46 GMT
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
	-	`sha256:39fb287d34302509d5512cdb0b97c37c3bd5779e0658467190f699cd58bee14a`  
		Last Modified: Mon, 04 Oct 2021 22:17:10 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8289de8bb44f7a333ffc1b0477844222cd20c2e87b3875b592a6b64eb2b901a`  
		Last Modified: Mon, 04 Oct 2021 22:17:10 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5965e430963578e6e1da8b37f105f899a73f13c1bf3ee436d2bc59d16c633b7`  
		Last Modified: Mon, 04 Oct 2021 22:17:22 GMT  
		Size: 50.9 MB (50906487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-1809`

```console
$ docker pull docker@sha256:b2cc2fdb94ee0637c9c04319f7d77d161f530672501ff22bf0e52504bf7af0cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `docker:20-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull docker@sha256:aca950618ba0f6f9a7b717dab70a0b0eee15e6e02bf1b0606d8d5f78ee92d63d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737962479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:372be2a200c2f353972f63b2c2014a0c40ab15eb1448345a850fa2b8531d677f`
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
# Mon, 04 Oct 2021 22:15:14 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:15:15 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.9.zip
# Mon, 04 Oct 2021 22:16:46 GMT
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
	-	`sha256:39fb287d34302509d5512cdb0b97c37c3bd5779e0658467190f699cd58bee14a`  
		Last Modified: Mon, 04 Oct 2021 22:17:10 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8289de8bb44f7a333ffc1b0477844222cd20c2e87b3875b592a6b64eb2b901a`  
		Last Modified: Mon, 04 Oct 2021 22:17:10 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5965e430963578e6e1da8b37f105f899a73f13c1bf3ee436d2bc59d16c633b7`  
		Last Modified: Mon, 04 Oct 2021 22:17:22 GMT  
		Size: 50.9 MB (50906487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10`

```console
$ docker pull docker@sha256:e7c9c600322345ad23160a0cafde129426270f50ae83133f5354c3fe347a36c2
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
$ docker pull docker@sha256:3a95cba826396eb3fb4b07117bd1386e46bd982834e622a0a73a7c9d4af7e474
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62356071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4799c468fbdd4c40fd59367653432a1cd16b199c572b72cc7059f46d20130075`
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
# Mon, 04 Oct 2021 22:39:36 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:39:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 04 Oct 2021 22:39:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 04 Oct 2021 22:39:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:42 GMT
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
	-	`sha256:2addeb3702952172db1a24220381e0ef6580b99177900ac4d13119b213c2fcfc`  
		Last Modified: Mon, 04 Oct 2021 22:41:15 GMT  
		Size: 57.7 MB (57733347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb723bbe59439dde838001146817815fb936b405e719e023874e6c96f0a10c3f`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da7ad22416e3ba9ff03eac3fe069bd73b06cdac1fd584e932e9f35270fae50`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97dbd9a21f6258fbc117eeddf6fb34a1172588deb227ce6ffb2ab00321631af`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind`

```console
$ docker pull docker@sha256:d20f0866ee1aca6b0eb7bc8bdb0d0c938721c7f79219b1d3bc1aa58666928586
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
$ docker pull docker@sha256:25a2c533ed67819c4726fad3ccaa5a1fbcfd602149d1b63c663b620714ec13fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68779507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f4dc61e43a85443d5bc5759e6ddf1035da284ae045c44dd173830b798dbe53`
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
# Mon, 04 Oct 2021 22:39:36 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:39:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 04 Oct 2021 22:39:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 04 Oct 2021 22:39:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:42 GMT
CMD ["sh"]
# Mon, 04 Oct 2021 22:39:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 04 Oct 2021 22:39:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 04 Oct 2021 22:39:53 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 04 Oct 2021 22:39:54 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 04 Oct 2021 22:39:54 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:54 GMT
VOLUME [/var/lib/docker]
# Mon, 04 Oct 2021 22:39:54 GMT
EXPOSE 2375 2376
# Mon, 04 Oct 2021 22:39:55 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:55 GMT
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
	-	`sha256:2addeb3702952172db1a24220381e0ef6580b99177900ac4d13119b213c2fcfc`  
		Last Modified: Mon, 04 Oct 2021 22:41:15 GMT  
		Size: 57.7 MB (57733347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb723bbe59439dde838001146817815fb936b405e719e023874e6c96f0a10c3f`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da7ad22416e3ba9ff03eac3fe069bd73b06cdac1fd584e932e9f35270fae50`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97dbd9a21f6258fbc117eeddf6fb34a1172588deb227ce6ffb2ab00321631af`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6df64ef29bdc4a4edaabe9dba4c929323e0fb59f04d2c4157d1614bd477b4c`  
		Last Modified: Mon, 04 Oct 2021 22:41:38 GMT  
		Size: 6.4 MB (6418544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab2a956e5b959cab7be1b5014e743e67aa28c92a3a2b095fa35e0ad32dcb269`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c7d1ec1ea400226cdcfba7d06bc6bdf859f3f39fbf91d93258c1b90b37368`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eedd8c550c3dd9f5a5cb146b38007c1f143f1c3abc63edb69c622d288eb6cd`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind-rootless`

```console
$ docker pull docker@sha256:f06dfdfd278026427fb1ebf15e05d4bde89df85ff3ba2334fc964a71a705d16a
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
$ docker pull docker@sha256:81af51e044194e802cc9e2ff99144cfc2c4988731d4597bdeeeef6e5e7a583d3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.0 MB (91045329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6bf6ba3bce99fb59f75ec0438ad494b919f079b40ab77f41c7319cb0cacfd44`
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
# Mon, 04 Oct 2021 22:39:36 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:39:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 04 Oct 2021 22:39:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 04 Oct 2021 22:39:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:42 GMT
CMD ["sh"]
# Mon, 04 Oct 2021 22:39:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 04 Oct 2021 22:39:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 04 Oct 2021 22:39:53 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 04 Oct 2021 22:39:54 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 04 Oct 2021 22:39:54 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:54 GMT
VOLUME [/var/lib/docker]
# Mon, 04 Oct 2021 22:39:54 GMT
EXPOSE 2375 2376
# Mon, 04 Oct 2021 22:39:55 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:55 GMT
CMD []
# Mon, 04 Oct 2021 22:40:03 GMT
RUN apk add --no-cache iproute2
# Mon, 04 Oct 2021 22:40:04 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 04 Oct 2021 22:40:04 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 04 Oct 2021 22:40:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 04 Oct 2021 22:40:08 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 04 Oct 2021 22:40:08 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 04 Oct 2021 22:40:08 GMT
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
	-	`sha256:2addeb3702952172db1a24220381e0ef6580b99177900ac4d13119b213c2fcfc`  
		Last Modified: Mon, 04 Oct 2021 22:41:15 GMT  
		Size: 57.7 MB (57733347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb723bbe59439dde838001146817815fb936b405e719e023874e6c96f0a10c3f`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da7ad22416e3ba9ff03eac3fe069bd73b06cdac1fd584e932e9f35270fae50`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97dbd9a21f6258fbc117eeddf6fb34a1172588deb227ce6ffb2ab00321631af`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6df64ef29bdc4a4edaabe9dba4c929323e0fb59f04d2c4157d1614bd477b4c`  
		Last Modified: Mon, 04 Oct 2021 22:41:38 GMT  
		Size: 6.4 MB (6418544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab2a956e5b959cab7be1b5014e743e67aa28c92a3a2b095fa35e0ad32dcb269`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c7d1ec1ea400226cdcfba7d06bc6bdf859f3f39fbf91d93258c1b90b37368`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eedd8c550c3dd9f5a5cb146b38007c1f143f1c3abc63edb69c622d288eb6cd`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d22f8eb08ad02090048708d5c999c5952be4c8d02c6dcb805da08d4012c288c`  
		Last Modified: Mon, 04 Oct 2021 22:42:00 GMT  
		Size: 1.2 MB (1168110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a0714a4fdbcb6036fccf4cf380ac24fc7edd6c974ad7a5731f13c1966238bd`  
		Last Modified: Mon, 04 Oct 2021 22:42:00 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d79b658117c879c9103d01547357c7566fc262750d0b62c30966d4d49defab`  
		Last Modified: Mon, 04 Oct 2021 22:42:00 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc95b12a74fd36add08fa63f789816fb9cbea1ddc4bbef6a4406364b0c454f2`  
		Last Modified: Mon, 04 Oct 2021 22:42:04 GMT  
		Size: 21.1 MB (21095995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba365bba8d1721288d49e57f54c068465199da261e7f376686e5b2db5c06bf9`  
		Last Modified: Mon, 04 Oct 2021 22:42:00 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-git`

```console
$ docker pull docker@sha256:61f6baf32667fc13a9850b16bf6c6de6c8a1c1302ba23dda8350127430f48b17
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
$ docker pull docker@sha256:27b5d5b7687d6a932d2bc0230af9c258588b2d962d77de01b2553b121bbca2de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69095380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc52e2bf2a201533bcb1dcf4ac4284d848ef238ac5e9acda87bfaa02989e7f59`
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
# Mon, 04 Oct 2021 22:39:36 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:39:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 04 Oct 2021 22:39:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 04 Oct 2021 22:39:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:42 GMT
CMD ["sh"]
# Mon, 04 Oct 2021 22:40:16 GMT
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
	-	`sha256:2addeb3702952172db1a24220381e0ef6580b99177900ac4d13119b213c2fcfc`  
		Last Modified: Mon, 04 Oct 2021 22:41:15 GMT  
		Size: 57.7 MB (57733347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb723bbe59439dde838001146817815fb936b405e719e023874e6c96f0a10c3f`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da7ad22416e3ba9ff03eac3fe069bd73b06cdac1fd584e932e9f35270fae50`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97dbd9a21f6258fbc117eeddf6fb34a1172588deb227ce6ffb2ab00321631af`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bed24c5b37ab30374c66d0fb367cceeaaa68d6483601e0413a8fb1b97f86092`  
		Last Modified: Mon, 04 Oct 2021 22:42:24 GMT  
		Size: 6.7 MB (6739309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore`

```console
$ docker pull docker@sha256:b2cc2fdb94ee0637c9c04319f7d77d161f530672501ff22bf0e52504bf7af0cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `docker:20.10-windowsservercore` - windows version 10.0.17763.2183; amd64

```console
$ docker pull docker@sha256:aca950618ba0f6f9a7b717dab70a0b0eee15e6e02bf1b0606d8d5f78ee92d63d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737962479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:372be2a200c2f353972f63b2c2014a0c40ab15eb1448345a850fa2b8531d677f`
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
# Mon, 04 Oct 2021 22:15:14 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:15:15 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.9.zip
# Mon, 04 Oct 2021 22:16:46 GMT
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
	-	`sha256:39fb287d34302509d5512cdb0b97c37c3bd5779e0658467190f699cd58bee14a`  
		Last Modified: Mon, 04 Oct 2021 22:17:10 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8289de8bb44f7a333ffc1b0477844222cd20c2e87b3875b592a6b64eb2b901a`  
		Last Modified: Mon, 04 Oct 2021 22:17:10 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5965e430963578e6e1da8b37f105f899a73f13c1bf3ee436d2bc59d16c633b7`  
		Last Modified: Mon, 04 Oct 2021 22:17:22 GMT  
		Size: 50.9 MB (50906487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-1809`

```console
$ docker pull docker@sha256:b2cc2fdb94ee0637c9c04319f7d77d161f530672501ff22bf0e52504bf7af0cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `docker:20.10-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull docker@sha256:aca950618ba0f6f9a7b717dab70a0b0eee15e6e02bf1b0606d8d5f78ee92d63d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737962479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:372be2a200c2f353972f63b2c2014a0c40ab15eb1448345a850fa2b8531d677f`
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
# Mon, 04 Oct 2021 22:15:14 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:15:15 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.9.zip
# Mon, 04 Oct 2021 22:16:46 GMT
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
	-	`sha256:39fb287d34302509d5512cdb0b97c37c3bd5779e0658467190f699cd58bee14a`  
		Last Modified: Mon, 04 Oct 2021 22:17:10 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8289de8bb44f7a333ffc1b0477844222cd20c2e87b3875b592a6b64eb2b901a`  
		Last Modified: Mon, 04 Oct 2021 22:17:10 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5965e430963578e6e1da8b37f105f899a73f13c1bf3ee436d2bc59d16c633b7`  
		Last Modified: Mon, 04 Oct 2021 22:17:22 GMT  
		Size: 50.9 MB (50906487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.9`

```console
$ docker pull docker@sha256:e7c9c600322345ad23160a0cafde129426270f50ae83133f5354c3fe347a36c2
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
$ docker pull docker@sha256:3a95cba826396eb3fb4b07117bd1386e46bd982834e622a0a73a7c9d4af7e474
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62356071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4799c468fbdd4c40fd59367653432a1cd16b199c572b72cc7059f46d20130075`
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
# Mon, 04 Oct 2021 22:39:36 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:39:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 04 Oct 2021 22:39:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 04 Oct 2021 22:39:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:42 GMT
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
	-	`sha256:2addeb3702952172db1a24220381e0ef6580b99177900ac4d13119b213c2fcfc`  
		Last Modified: Mon, 04 Oct 2021 22:41:15 GMT  
		Size: 57.7 MB (57733347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb723bbe59439dde838001146817815fb936b405e719e023874e6c96f0a10c3f`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da7ad22416e3ba9ff03eac3fe069bd73b06cdac1fd584e932e9f35270fae50`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97dbd9a21f6258fbc117eeddf6fb34a1172588deb227ce6ffb2ab00321631af`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.9-alpine3.14`

```console
$ docker pull docker@sha256:e7c9c600322345ad23160a0cafde129426270f50ae83133f5354c3fe347a36c2
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
$ docker pull docker@sha256:3a95cba826396eb3fb4b07117bd1386e46bd982834e622a0a73a7c9d4af7e474
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62356071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4799c468fbdd4c40fd59367653432a1cd16b199c572b72cc7059f46d20130075`
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
# Mon, 04 Oct 2021 22:39:36 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:39:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 04 Oct 2021 22:39:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 04 Oct 2021 22:39:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:42 GMT
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
	-	`sha256:2addeb3702952172db1a24220381e0ef6580b99177900ac4d13119b213c2fcfc`  
		Last Modified: Mon, 04 Oct 2021 22:41:15 GMT  
		Size: 57.7 MB (57733347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb723bbe59439dde838001146817815fb936b405e719e023874e6c96f0a10c3f`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da7ad22416e3ba9ff03eac3fe069bd73b06cdac1fd584e932e9f35270fae50`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97dbd9a21f6258fbc117eeddf6fb34a1172588deb227ce6ffb2ab00321631af`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.9-dind`

```console
$ docker pull docker@sha256:d20f0866ee1aca6b0eb7bc8bdb0d0c938721c7f79219b1d3bc1aa58666928586
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
$ docker pull docker@sha256:25a2c533ed67819c4726fad3ccaa5a1fbcfd602149d1b63c663b620714ec13fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68779507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f4dc61e43a85443d5bc5759e6ddf1035da284ae045c44dd173830b798dbe53`
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
# Mon, 04 Oct 2021 22:39:36 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:39:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 04 Oct 2021 22:39:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 04 Oct 2021 22:39:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:42 GMT
CMD ["sh"]
# Mon, 04 Oct 2021 22:39:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 04 Oct 2021 22:39:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 04 Oct 2021 22:39:53 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 04 Oct 2021 22:39:54 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 04 Oct 2021 22:39:54 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:54 GMT
VOLUME [/var/lib/docker]
# Mon, 04 Oct 2021 22:39:54 GMT
EXPOSE 2375 2376
# Mon, 04 Oct 2021 22:39:55 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:55 GMT
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
	-	`sha256:2addeb3702952172db1a24220381e0ef6580b99177900ac4d13119b213c2fcfc`  
		Last Modified: Mon, 04 Oct 2021 22:41:15 GMT  
		Size: 57.7 MB (57733347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb723bbe59439dde838001146817815fb936b405e719e023874e6c96f0a10c3f`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da7ad22416e3ba9ff03eac3fe069bd73b06cdac1fd584e932e9f35270fae50`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97dbd9a21f6258fbc117eeddf6fb34a1172588deb227ce6ffb2ab00321631af`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6df64ef29bdc4a4edaabe9dba4c929323e0fb59f04d2c4157d1614bd477b4c`  
		Last Modified: Mon, 04 Oct 2021 22:41:38 GMT  
		Size: 6.4 MB (6418544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab2a956e5b959cab7be1b5014e743e67aa28c92a3a2b095fa35e0ad32dcb269`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c7d1ec1ea400226cdcfba7d06bc6bdf859f3f39fbf91d93258c1b90b37368`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eedd8c550c3dd9f5a5cb146b38007c1f143f1c3abc63edb69c622d288eb6cd`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.9-dind-alpine3.14`

```console
$ docker pull docker@sha256:d20f0866ee1aca6b0eb7bc8bdb0d0c938721c7f79219b1d3bc1aa58666928586
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
$ docker pull docker@sha256:25a2c533ed67819c4726fad3ccaa5a1fbcfd602149d1b63c663b620714ec13fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68779507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f4dc61e43a85443d5bc5759e6ddf1035da284ae045c44dd173830b798dbe53`
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
# Mon, 04 Oct 2021 22:39:36 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:39:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 04 Oct 2021 22:39:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 04 Oct 2021 22:39:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:42 GMT
CMD ["sh"]
# Mon, 04 Oct 2021 22:39:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 04 Oct 2021 22:39:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 04 Oct 2021 22:39:53 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 04 Oct 2021 22:39:54 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 04 Oct 2021 22:39:54 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:54 GMT
VOLUME [/var/lib/docker]
# Mon, 04 Oct 2021 22:39:54 GMT
EXPOSE 2375 2376
# Mon, 04 Oct 2021 22:39:55 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:55 GMT
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
	-	`sha256:2addeb3702952172db1a24220381e0ef6580b99177900ac4d13119b213c2fcfc`  
		Last Modified: Mon, 04 Oct 2021 22:41:15 GMT  
		Size: 57.7 MB (57733347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb723bbe59439dde838001146817815fb936b405e719e023874e6c96f0a10c3f`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da7ad22416e3ba9ff03eac3fe069bd73b06cdac1fd584e932e9f35270fae50`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97dbd9a21f6258fbc117eeddf6fb34a1172588deb227ce6ffb2ab00321631af`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6df64ef29bdc4a4edaabe9dba4c929323e0fb59f04d2c4157d1614bd477b4c`  
		Last Modified: Mon, 04 Oct 2021 22:41:38 GMT  
		Size: 6.4 MB (6418544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab2a956e5b959cab7be1b5014e743e67aa28c92a3a2b095fa35e0ad32dcb269`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c7d1ec1ea400226cdcfba7d06bc6bdf859f3f39fbf91d93258c1b90b37368`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eedd8c550c3dd9f5a5cb146b38007c1f143f1c3abc63edb69c622d288eb6cd`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.9-dind-rootless`

```console
$ docker pull docker@sha256:f06dfdfd278026427fb1ebf15e05d4bde89df85ff3ba2334fc964a71a705d16a
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
$ docker pull docker@sha256:81af51e044194e802cc9e2ff99144cfc2c4988731d4597bdeeeef6e5e7a583d3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.0 MB (91045329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6bf6ba3bce99fb59f75ec0438ad494b919f079b40ab77f41c7319cb0cacfd44`
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
# Mon, 04 Oct 2021 22:39:36 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:39:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 04 Oct 2021 22:39:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 04 Oct 2021 22:39:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:42 GMT
CMD ["sh"]
# Mon, 04 Oct 2021 22:39:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 04 Oct 2021 22:39:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 04 Oct 2021 22:39:53 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 04 Oct 2021 22:39:54 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 04 Oct 2021 22:39:54 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:54 GMT
VOLUME [/var/lib/docker]
# Mon, 04 Oct 2021 22:39:54 GMT
EXPOSE 2375 2376
# Mon, 04 Oct 2021 22:39:55 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:55 GMT
CMD []
# Mon, 04 Oct 2021 22:40:03 GMT
RUN apk add --no-cache iproute2
# Mon, 04 Oct 2021 22:40:04 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 04 Oct 2021 22:40:04 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 04 Oct 2021 22:40:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 04 Oct 2021 22:40:08 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 04 Oct 2021 22:40:08 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 04 Oct 2021 22:40:08 GMT
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
	-	`sha256:2addeb3702952172db1a24220381e0ef6580b99177900ac4d13119b213c2fcfc`  
		Last Modified: Mon, 04 Oct 2021 22:41:15 GMT  
		Size: 57.7 MB (57733347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb723bbe59439dde838001146817815fb936b405e719e023874e6c96f0a10c3f`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da7ad22416e3ba9ff03eac3fe069bd73b06cdac1fd584e932e9f35270fae50`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97dbd9a21f6258fbc117eeddf6fb34a1172588deb227ce6ffb2ab00321631af`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6df64ef29bdc4a4edaabe9dba4c929323e0fb59f04d2c4157d1614bd477b4c`  
		Last Modified: Mon, 04 Oct 2021 22:41:38 GMT  
		Size: 6.4 MB (6418544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab2a956e5b959cab7be1b5014e743e67aa28c92a3a2b095fa35e0ad32dcb269`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c7d1ec1ea400226cdcfba7d06bc6bdf859f3f39fbf91d93258c1b90b37368`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eedd8c550c3dd9f5a5cb146b38007c1f143f1c3abc63edb69c622d288eb6cd`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d22f8eb08ad02090048708d5c999c5952be4c8d02c6dcb805da08d4012c288c`  
		Last Modified: Mon, 04 Oct 2021 22:42:00 GMT  
		Size: 1.2 MB (1168110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a0714a4fdbcb6036fccf4cf380ac24fc7edd6c974ad7a5731f13c1966238bd`  
		Last Modified: Mon, 04 Oct 2021 22:42:00 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d79b658117c879c9103d01547357c7566fc262750d0b62c30966d4d49defab`  
		Last Modified: Mon, 04 Oct 2021 22:42:00 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc95b12a74fd36add08fa63f789816fb9cbea1ddc4bbef6a4406364b0c454f2`  
		Last Modified: Mon, 04 Oct 2021 22:42:04 GMT  
		Size: 21.1 MB (21095995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba365bba8d1721288d49e57f54c068465199da261e7f376686e5b2db5c06bf9`  
		Last Modified: Mon, 04 Oct 2021 22:42:00 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.9-git`

```console
$ docker pull docker@sha256:61f6baf32667fc13a9850b16bf6c6de6c8a1c1302ba23dda8350127430f48b17
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
$ docker pull docker@sha256:27b5d5b7687d6a932d2bc0230af9c258588b2d962d77de01b2553b121bbca2de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69095380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc52e2bf2a201533bcb1dcf4ac4284d848ef238ac5e9acda87bfaa02989e7f59`
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
# Mon, 04 Oct 2021 22:39:36 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:39:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 04 Oct 2021 22:39:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 04 Oct 2021 22:39:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:42 GMT
CMD ["sh"]
# Mon, 04 Oct 2021 22:40:16 GMT
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
	-	`sha256:2addeb3702952172db1a24220381e0ef6580b99177900ac4d13119b213c2fcfc`  
		Last Modified: Mon, 04 Oct 2021 22:41:15 GMT  
		Size: 57.7 MB (57733347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb723bbe59439dde838001146817815fb936b405e719e023874e6c96f0a10c3f`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da7ad22416e3ba9ff03eac3fe069bd73b06cdac1fd584e932e9f35270fae50`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97dbd9a21f6258fbc117eeddf6fb34a1172588deb227ce6ffb2ab00321631af`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bed24c5b37ab30374c66d0fb367cceeaaa68d6483601e0413a8fb1b97f86092`  
		Last Modified: Mon, 04 Oct 2021 22:42:24 GMT  
		Size: 6.7 MB (6739309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.9-windowsservercore`

```console
$ docker pull docker@sha256:b2cc2fdb94ee0637c9c04319f7d77d161f530672501ff22bf0e52504bf7af0cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `docker:20.10.9-windowsservercore` - windows version 10.0.17763.2183; amd64

```console
$ docker pull docker@sha256:aca950618ba0f6f9a7b717dab70a0b0eee15e6e02bf1b0606d8d5f78ee92d63d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737962479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:372be2a200c2f353972f63b2c2014a0c40ab15eb1448345a850fa2b8531d677f`
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
# Mon, 04 Oct 2021 22:15:14 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:15:15 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.9.zip
# Mon, 04 Oct 2021 22:16:46 GMT
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
	-	`sha256:39fb287d34302509d5512cdb0b97c37c3bd5779e0658467190f699cd58bee14a`  
		Last Modified: Mon, 04 Oct 2021 22:17:10 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8289de8bb44f7a333ffc1b0477844222cd20c2e87b3875b592a6b64eb2b901a`  
		Last Modified: Mon, 04 Oct 2021 22:17:10 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5965e430963578e6e1da8b37f105f899a73f13c1bf3ee436d2bc59d16c633b7`  
		Last Modified: Mon, 04 Oct 2021 22:17:22 GMT  
		Size: 50.9 MB (50906487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.9-windowsservercore-1809`

```console
$ docker pull docker@sha256:b2cc2fdb94ee0637c9c04319f7d77d161f530672501ff22bf0e52504bf7af0cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `docker:20.10.9-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull docker@sha256:aca950618ba0f6f9a7b717dab70a0b0eee15e6e02bf1b0606d8d5f78ee92d63d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737962479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:372be2a200c2f353972f63b2c2014a0c40ab15eb1448345a850fa2b8531d677f`
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
# Mon, 04 Oct 2021 22:15:14 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:15:15 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.9.zip
# Mon, 04 Oct 2021 22:16:46 GMT
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
	-	`sha256:39fb287d34302509d5512cdb0b97c37c3bd5779e0658467190f699cd58bee14a`  
		Last Modified: Mon, 04 Oct 2021 22:17:10 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8289de8bb44f7a333ffc1b0477844222cd20c2e87b3875b592a6b64eb2b901a`  
		Last Modified: Mon, 04 Oct 2021 22:17:10 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5965e430963578e6e1da8b37f105f899a73f13c1bf3ee436d2bc59d16c633b7`  
		Last Modified: Mon, 04 Oct 2021 22:17:22 GMT  
		Size: 50.9 MB (50906487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:d20f0866ee1aca6b0eb7bc8bdb0d0c938721c7f79219b1d3bc1aa58666928586
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
$ docker pull docker@sha256:25a2c533ed67819c4726fad3ccaa5a1fbcfd602149d1b63c663b620714ec13fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68779507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f4dc61e43a85443d5bc5759e6ddf1035da284ae045c44dd173830b798dbe53`
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
# Mon, 04 Oct 2021 22:39:36 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:39:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 04 Oct 2021 22:39:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 04 Oct 2021 22:39:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:42 GMT
CMD ["sh"]
# Mon, 04 Oct 2021 22:39:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 04 Oct 2021 22:39:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 04 Oct 2021 22:39:53 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 04 Oct 2021 22:39:54 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 04 Oct 2021 22:39:54 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:54 GMT
VOLUME [/var/lib/docker]
# Mon, 04 Oct 2021 22:39:54 GMT
EXPOSE 2375 2376
# Mon, 04 Oct 2021 22:39:55 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:55 GMT
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
	-	`sha256:2addeb3702952172db1a24220381e0ef6580b99177900ac4d13119b213c2fcfc`  
		Last Modified: Mon, 04 Oct 2021 22:41:15 GMT  
		Size: 57.7 MB (57733347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb723bbe59439dde838001146817815fb936b405e719e023874e6c96f0a10c3f`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da7ad22416e3ba9ff03eac3fe069bd73b06cdac1fd584e932e9f35270fae50`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97dbd9a21f6258fbc117eeddf6fb34a1172588deb227ce6ffb2ab00321631af`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6df64ef29bdc4a4edaabe9dba4c929323e0fb59f04d2c4157d1614bd477b4c`  
		Last Modified: Mon, 04 Oct 2021 22:41:38 GMT  
		Size: 6.4 MB (6418544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab2a956e5b959cab7be1b5014e743e67aa28c92a3a2b095fa35e0ad32dcb269`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c7d1ec1ea400226cdcfba7d06bc6bdf859f3f39fbf91d93258c1b90b37368`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eedd8c550c3dd9f5a5cb146b38007c1f143f1c3abc63edb69c622d288eb6cd`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:f06dfdfd278026427fb1ebf15e05d4bde89df85ff3ba2334fc964a71a705d16a
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
$ docker pull docker@sha256:81af51e044194e802cc9e2ff99144cfc2c4988731d4597bdeeeef6e5e7a583d3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.0 MB (91045329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6bf6ba3bce99fb59f75ec0438ad494b919f079b40ab77f41c7319cb0cacfd44`
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
# Mon, 04 Oct 2021 22:39:36 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:39:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 04 Oct 2021 22:39:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 04 Oct 2021 22:39:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:42 GMT
CMD ["sh"]
# Mon, 04 Oct 2021 22:39:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 04 Oct 2021 22:39:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 04 Oct 2021 22:39:53 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 04 Oct 2021 22:39:54 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 04 Oct 2021 22:39:54 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:54 GMT
VOLUME [/var/lib/docker]
# Mon, 04 Oct 2021 22:39:54 GMT
EXPOSE 2375 2376
# Mon, 04 Oct 2021 22:39:55 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:55 GMT
CMD []
# Mon, 04 Oct 2021 22:40:03 GMT
RUN apk add --no-cache iproute2
# Mon, 04 Oct 2021 22:40:04 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 04 Oct 2021 22:40:04 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 04 Oct 2021 22:40:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 04 Oct 2021 22:40:08 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 04 Oct 2021 22:40:08 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 04 Oct 2021 22:40:08 GMT
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
	-	`sha256:2addeb3702952172db1a24220381e0ef6580b99177900ac4d13119b213c2fcfc`  
		Last Modified: Mon, 04 Oct 2021 22:41:15 GMT  
		Size: 57.7 MB (57733347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb723bbe59439dde838001146817815fb936b405e719e023874e6c96f0a10c3f`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da7ad22416e3ba9ff03eac3fe069bd73b06cdac1fd584e932e9f35270fae50`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97dbd9a21f6258fbc117eeddf6fb34a1172588deb227ce6ffb2ab00321631af`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6df64ef29bdc4a4edaabe9dba4c929323e0fb59f04d2c4157d1614bd477b4c`  
		Last Modified: Mon, 04 Oct 2021 22:41:38 GMT  
		Size: 6.4 MB (6418544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab2a956e5b959cab7be1b5014e743e67aa28c92a3a2b095fa35e0ad32dcb269`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c7d1ec1ea400226cdcfba7d06bc6bdf859f3f39fbf91d93258c1b90b37368`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eedd8c550c3dd9f5a5cb146b38007c1f143f1c3abc63edb69c622d288eb6cd`  
		Last Modified: Mon, 04 Oct 2021 22:41:37 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d22f8eb08ad02090048708d5c999c5952be4c8d02c6dcb805da08d4012c288c`  
		Last Modified: Mon, 04 Oct 2021 22:42:00 GMT  
		Size: 1.2 MB (1168110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a0714a4fdbcb6036fccf4cf380ac24fc7edd6c974ad7a5731f13c1966238bd`  
		Last Modified: Mon, 04 Oct 2021 22:42:00 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d79b658117c879c9103d01547357c7566fc262750d0b62c30966d4d49defab`  
		Last Modified: Mon, 04 Oct 2021 22:42:00 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc95b12a74fd36add08fa63f789816fb9cbea1ddc4bbef6a4406364b0c454f2`  
		Last Modified: Mon, 04 Oct 2021 22:42:04 GMT  
		Size: 21.1 MB (21095995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba365bba8d1721288d49e57f54c068465199da261e7f376686e5b2db5c06bf9`  
		Last Modified: Mon, 04 Oct 2021 22:42:00 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:61f6baf32667fc13a9850b16bf6c6de6c8a1c1302ba23dda8350127430f48b17
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
$ docker pull docker@sha256:27b5d5b7687d6a932d2bc0230af9c258588b2d962d77de01b2553b121bbca2de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69095380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc52e2bf2a201533bcb1dcf4ac4284d848ef238ac5e9acda87bfaa02989e7f59`
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
# Mon, 04 Oct 2021 22:39:36 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:39:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 04 Oct 2021 22:39:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 04 Oct 2021 22:39:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:42 GMT
CMD ["sh"]
# Mon, 04 Oct 2021 22:40:16 GMT
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
	-	`sha256:2addeb3702952172db1a24220381e0ef6580b99177900ac4d13119b213c2fcfc`  
		Last Modified: Mon, 04 Oct 2021 22:41:15 GMT  
		Size: 57.7 MB (57733347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb723bbe59439dde838001146817815fb936b405e719e023874e6c96f0a10c3f`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da7ad22416e3ba9ff03eac3fe069bd73b06cdac1fd584e932e9f35270fae50`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97dbd9a21f6258fbc117eeddf6fb34a1172588deb227ce6ffb2ab00321631af`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bed24c5b37ab30374c66d0fb367cceeaaa68d6483601e0413a8fb1b97f86092`  
		Last Modified: Mon, 04 Oct 2021 22:42:24 GMT  
		Size: 6.7 MB (6739309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:e7c9c600322345ad23160a0cafde129426270f50ae83133f5354c3fe347a36c2
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
$ docker pull docker@sha256:3a95cba826396eb3fb4b07117bd1386e46bd982834e622a0a73a7c9d4af7e474
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62356071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4799c468fbdd4c40fd59367653432a1cd16b199c572b72cc7059f46d20130075`
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
# Mon, 04 Oct 2021 22:39:36 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:39:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.9.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.9.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.9.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.9.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 04 Oct 2021 22:39:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 04 Oct 2021 22:39:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 04 Oct 2021 22:39:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 04 Oct 2021 22:39:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Oct 2021 22:39:42 GMT
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
	-	`sha256:2addeb3702952172db1a24220381e0ef6580b99177900ac4d13119b213c2fcfc`  
		Last Modified: Mon, 04 Oct 2021 22:41:15 GMT  
		Size: 57.7 MB (57733347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb723bbe59439dde838001146817815fb936b405e719e023874e6c96f0a10c3f`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da7ad22416e3ba9ff03eac3fe069bd73b06cdac1fd584e932e9f35270fae50`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97dbd9a21f6258fbc117eeddf6fb34a1172588deb227ce6ffb2ab00321631af`  
		Last Modified: Mon, 04 Oct 2021 22:41:05 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore`

```console
$ docker pull docker@sha256:b2cc2fdb94ee0637c9c04319f7d77d161f530672501ff22bf0e52504bf7af0cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `docker:windowsservercore` - windows version 10.0.17763.2183; amd64

```console
$ docker pull docker@sha256:aca950618ba0f6f9a7b717dab70a0b0eee15e6e02bf1b0606d8d5f78ee92d63d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737962479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:372be2a200c2f353972f63b2c2014a0c40ab15eb1448345a850fa2b8531d677f`
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
# Mon, 04 Oct 2021 22:15:14 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:15:15 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.9.zip
# Mon, 04 Oct 2021 22:16:46 GMT
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
	-	`sha256:39fb287d34302509d5512cdb0b97c37c3bd5779e0658467190f699cd58bee14a`  
		Last Modified: Mon, 04 Oct 2021 22:17:10 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8289de8bb44f7a333ffc1b0477844222cd20c2e87b3875b592a6b64eb2b901a`  
		Last Modified: Mon, 04 Oct 2021 22:17:10 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5965e430963578e6e1da8b37f105f899a73f13c1bf3ee436d2bc59d16c633b7`  
		Last Modified: Mon, 04 Oct 2021 22:17:22 GMT  
		Size: 50.9 MB (50906487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:b2cc2fdb94ee0637c9c04319f7d77d161f530672501ff22bf0e52504bf7af0cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull docker@sha256:aca950618ba0f6f9a7b717dab70a0b0eee15e6e02bf1b0606d8d5f78ee92d63d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737962479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:372be2a200c2f353972f63b2c2014a0c40ab15eb1448345a850fa2b8531d677f`
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
# Mon, 04 Oct 2021 22:15:14 GMT
ENV DOCKER_VERSION=20.10.9
# Mon, 04 Oct 2021 22:15:15 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.9.zip
# Mon, 04 Oct 2021 22:16:46 GMT
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
	-	`sha256:39fb287d34302509d5512cdb0b97c37c3bd5779e0658467190f699cd58bee14a`  
		Last Modified: Mon, 04 Oct 2021 22:17:10 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8289de8bb44f7a333ffc1b0477844222cd20c2e87b3875b592a6b64eb2b901a`  
		Last Modified: Mon, 04 Oct 2021 22:17:10 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5965e430963578e6e1da8b37f105f899a73f13c1bf3ee436d2bc59d16c633b7`  
		Last Modified: Mon, 04 Oct 2021 22:17:22 GMT  
		Size: 50.9 MB (50906487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
