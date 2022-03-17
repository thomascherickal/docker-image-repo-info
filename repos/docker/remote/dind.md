## `docker:dind`

```console
$ docker pull docker@sha256:ca2744235df40f184843b2cb9f0245a6b64ae65065aad30285e80d5a266fe0c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:34c594c12507d24f66789978a90240d4addf3eb8fce22a7a9157ca9701afd46d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76152892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c05a8c965912fe35df9cce58ddb7aed725fb34d81772761a4ef7a373fd3271c1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Mar 2022 00:19:37 GMT
ENV DOCKER_VERSION=20.10.13
# Fri, 11 Mar 2022 00:19:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Mar 2022 00:19:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Mar 2022 00:19:42 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:42 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Mar 2022 00:19:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Mar 2022 00:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:42 GMT
CMD ["sh"]
# Fri, 11 Mar 2022 00:19:47 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Mar 2022 00:19:48 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Mar 2022 00:19:48 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 11 Mar 2022 00:19:48 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Mar 2022 00:19:48 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:19:48 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Mar 2022 00:19:49 GMT
EXPOSE 2375 2376
# Fri, 11 Mar 2022 00:19:49 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Mar 2022 00:19:49 GMT
CMD []
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea03e1895df432fba23ac2810a53a408fa25273ecf001276263d810107e1c81`  
		Last Modified: Wed, 15 Dec 2021 20:20:23 GMT  
		Size: 2.0 MB (1980404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff98835b05535c14c9bd8aa0449fd33d147a58c9a9fe7f21b76137065d0f4c5`  
		Last Modified: Wed, 15 Dec 2021 20:20:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbbd0a7b1dec526be119d73f0018052afa23e65ea79e09049a54a5954f2a374`  
		Last Modified: Fri, 11 Mar 2022 00:20:32 GMT  
		Size: 64.6 MB (64612571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317ecb07c86c68358ba3d763bea251b7baf1befde793d08f074abf2743a388dc`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52850491ed6a707afb12e76035b1a36f408c071e00d1de77b26ec2cb178c9a8a`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb2b84e11d9e63efd7d7cad8459ac6f5326f44d93991a59380b186824079bdf`  
		Last Modified: Fri, 11 Mar 2022 00:20:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd217e3dc5c63b9a21276d1a8b9b2c0a19dd9aeecf5c242902d63e8dd7c251f`  
		Last Modified: Fri, 11 Mar 2022 00:20:50 GMT  
		Size: 6.7 MB (6734617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f85497bc6212a4fbd95757776ba9f0cfc449ba5ec26f58dc4b48718582d256`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63824672dbc4b8bf906bba2cabad90a9964a4de17f7df52debc99611d2782d66`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330cf4336db2c7c1846de44144ed6eb30ac0942792712aeca3f5b38acbd16933`  
		Last Modified: Fri, 11 Mar 2022 00:20:49 GMT  
		Size: 2.7 KB (2747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e6222d4d8b30c439b883f691f52e8e405f6464852c86477f7b1577dee106ee6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69841345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ba71573c3cddc7fe6d1f68e3c7c55e13f7549be38cf07414563df801aa79e1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 06:44:43 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 17 Mar 2022 06:44:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 06:44:45 GMT
ENV DOCKER_VERSION=20.10.13
# Thu, 17 Mar 2022 06:44:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Mar 2022 06:44:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Mar 2022 06:44:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:44:51 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Mar 2022 06:44:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Mar 2022 06:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 06:44:54 GMT
CMD ["sh"]
# Thu, 17 Mar 2022 06:45:06 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 17 Mar 2022 06:45:07 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 17 Mar 2022 06:45:08 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 17 Mar 2022 06:45:09 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 17 Mar 2022 06:45:11 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 17 Mar 2022 06:45:11 GMT
VOLUME [/var/lib/docker]
# Thu, 17 Mar 2022 06:45:12 GMT
EXPOSE 2375 2376
# Thu, 17 Mar 2022 06:45:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 17 Mar 2022 06:45:14 GMT
CMD []
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bd6b2d67571b28ebbe22152f5536e3cff37d4346bc02a444b2ede9b5d71c6`  
		Last Modified: Thu, 17 Mar 2022 06:46:18 GMT  
		Size: 1.9 MB (1938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadc398c63809a7b7b0d60cee36c1a95c7dd031fb5987cb99246b289df77d64f`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fce163fc9e7e1d8912203364c303838e60da953ed77812572633504c2bd014`  
		Last Modified: Thu, 17 Mar 2022 06:46:25 GMT  
		Size: 58.6 MB (58565248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a0a3a69cb84240c8270720f964d7155438567aa97bb868bfe1adc07b5b977`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8be56eb060db5cad28d2359c143a7a7de20610f090073f5cbd7f1cfeafbd4`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746be13a2cb02a7014e32f66ba9fb3bb10e14bd43af45b7890fb09464fe2a830`  
		Last Modified: Thu, 17 Mar 2022 06:46:16 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb73bd4ce74defd0741f3f7922ffb261b2f91b45cf97e2225f65aaba2b4c42d6`  
		Last Modified: Thu, 17 Mar 2022 06:46:48 GMT  
		Size: 6.6 MB (6615563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e054635e9f383caa96af63cfbbc71098384c50f5c13efcc785d2a870ed8e4af9`  
		Last Modified: Thu, 17 Mar 2022 06:46:46 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791a50930d17375d4278a896defa85218b579b3efdd1455d1fa503e187676dfb`  
		Last Modified: Thu, 17 Mar 2022 06:46:46 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752ca04529521e0b4db8ded3d79d79f1629c7c725837b87fe79519f64bcb2e05`  
		Last Modified: Thu, 17 Mar 2022 06:46:47 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
