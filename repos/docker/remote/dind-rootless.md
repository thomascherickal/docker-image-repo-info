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
