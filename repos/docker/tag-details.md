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
-	[`docker:20.10.12`](#docker201012)
-	[`docker:20.10.12-alpine3.15`](#docker201012-alpine315)
-	[`docker:20.10.12-dind`](#docker201012-dind)
-	[`docker:20.10.12-dind-alpine3.15`](#docker201012-dind-alpine315)
-	[`docker:20.10.12-dind-rootless`](#docker201012-dind-rootless)
-	[`docker:20.10.12-git`](#docker201012-git)
-	[`docker:20.10.12-windowsservercore`](#docker201012-windowsservercore)
-	[`docker:20.10.12-windowsservercore-1809`](#docker201012-windowsservercore-1809)
-	[`docker:20.10.12-windowsservercore-ltsc2022`](#docker201012-windowsservercore-ltsc2022)
-	[`docker:dind`](#dockerdind)
-	[`docker:dind-rootless`](#dockerdind-rootless)
-	[`docker:git`](#dockergit)
-	[`docker:latest`](#dockerlatest)
-	[`docker:windowsservercore`](#dockerwindowsservercore)
-	[`docker:windowsservercore-1809`](#dockerwindowsservercore-1809)
-	[`docker:windowsservercore-ltsc2022`](#dockerwindowsservercore-ltsc2022)

## `docker:20`

```console
$ docker pull docker@sha256:a729cce205a05b0b86dc8dca87823efaffc3f74979fe7dc86a707c2fbf631b61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20` - linux; amd64

```console
$ docker pull docker@sha256:b15efb5c932fd29acc764a2b8c0e6b1dfda4450f2a67d630c3b9f205785fdb2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68519144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15a9bc7c6340df2ac9d6c8196ca1d905180ddf2ca8b29a8d98f5422e2e5ccf85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 20:19:27 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 20:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:34 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 20:19:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 20:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:35 GMT
CMD ["sh"]
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
	-	`sha256:a3f2dd7b7d653d57dbfc55dcef38007cf7ae05a4c1a226f4465b3723cb2232ed`  
		Last Modified: Wed, 15 Dec 2021 20:20:32 GMT  
		Size: 63.7 MB (63718464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d182b62d4a3549bba88c6f8f32c2d7850ca927a7df0682d9a0de05d0c40095e2`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a57db2abd77c0b995c329d7812464e3734bc1af7b829bd1a42d461de77d3b7`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73490af52bd34939d0d8b02fe67c992943d062112c5a1cb41daf43146a25ae1b`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:17db01f277a58c2d70b2a40a8f46607c5319dd2f23c55dcf8c835cd25f7ff746
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62414023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4610f8d36c6766d145891417dd49f9b3e6535b43820bae79640d380fb88016b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 19:39:37 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 19:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 19:39:38 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 19:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 19:39:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 19:39:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:39:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 19:39:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 19:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 19:39:48 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1339a3be518a98fb1ef64708d14d86fd4039c4bb0a3d1db8c2d4a4c00fb8a2`  
		Last Modified: Wed, 15 Dec 2021 19:41:10 GMT  
		Size: 1.9 MB (1949540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353862b30dd70efe72e0bf55133d47f2a5b000e37f9cdb0e7e4a0178a5f076ec`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3190c06c4855888df747c4f505d0bc7aaecfbb0d9d4acaee685e28bddfb99b`  
		Last Modified: Wed, 15 Dec 2021 19:41:16 GMT  
		Size: 57.7 MB (57747213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e216c2ebb46ec0635d982e57890ab4c9025c95a940e79a81a0ed8b50c49b6`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46f33417cc9574bd0139314cc88909fae8f672527fc69f493d406dad1991e1`  
		Last Modified: Wed, 15 Dec 2021 19:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c99da1af64cbeec415a8ce2302a76874846814f574e07e7d9072e70ad00192`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind`

```console
$ docker pull docker@sha256:1f50d3a86f7035805843779f803e81e8f4ce96b62ed68fc70cdcf4922f43470b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind` - linux; amd64

```console
$ docker pull docker@sha256:4e04836731b7100e8bd5e0b35756f53d0b6211ddb3cc7ec326ae3640adcfa004
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75258135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:175122d895c3ac2d1a9e3eeaa4885972ffcf3cf86c6e14261fd58db58ca77139`
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
# Wed, 15 Dec 2021 20:19:27 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 20:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:34 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 20:19:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 20:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:35 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 20:19:42 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 15 Dec 2021 20:19:43 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 15 Dec 2021 20:19:43 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 15 Dec 2021 20:19:44 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 15 Dec 2021 20:19:44 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:44 GMT
VOLUME [/var/lib/docker]
# Wed, 15 Dec 2021 20:19:44 GMT
EXPOSE 2375 2376
# Wed, 15 Dec 2021 20:19:44 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:45 GMT
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
	-	`sha256:a3f2dd7b7d653d57dbfc55dcef38007cf7ae05a4c1a226f4465b3723cb2232ed`  
		Last Modified: Wed, 15 Dec 2021 20:20:32 GMT  
		Size: 63.7 MB (63718464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d182b62d4a3549bba88c6f8f32c2d7850ca927a7df0682d9a0de05d0c40095e2`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a57db2abd77c0b995c329d7812464e3734bc1af7b829bd1a42d461de77d3b7`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73490af52bd34939d0d8b02fe67c992943d062112c5a1cb41daf43146a25ae1b`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d28806efd0ea428cf206cb382a31cb6fba2972e2e6e870051723dab28340158`  
		Last Modified: Wed, 15 Dec 2021 20:20:55 GMT  
		Size: 6.7 MB (6734098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97fd78563ff48a3ea4d64328aac35a97ef969306734b403631f8f8fb36d16e5`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffaf1aff7f0b5974dc8e7b9ce5119cf168e186a2281887ebdb30b850059c51ec`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8eed8b923285e1979ee45a366bc2852d46843fc0ababa5c7de8d8009f25f757`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5ed82558a7494a410eb6777aef81cf618118517d352b34307ca40d1da8589a22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69031436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd9db4c317abc6701f11a378339752bf58a9371ae9dce469dd02627f373c2b97`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 19:39:37 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 19:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 19:39:38 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 19:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 19:39:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 19:39:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:39:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 19:39:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 19:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 19:39:48 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 19:39:58 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 15 Dec 2021 19:39:59 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 15 Dec 2021 19:40:00 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 15 Dec 2021 19:40:01 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 15 Dec 2021 19:40:03 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:40:03 GMT
VOLUME [/var/lib/docker]
# Wed, 15 Dec 2021 19:40:04 GMT
EXPOSE 2375 2376
# Wed, 15 Dec 2021 19:40:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 15 Dec 2021 19:40:06 GMT
CMD []
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1339a3be518a98fb1ef64708d14d86fd4039c4bb0a3d1db8c2d4a4c00fb8a2`  
		Last Modified: Wed, 15 Dec 2021 19:41:10 GMT  
		Size: 1.9 MB (1949540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353862b30dd70efe72e0bf55133d47f2a5b000e37f9cdb0e7e4a0178a5f076ec`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3190c06c4855888df747c4f505d0bc7aaecfbb0d9d4acaee685e28bddfb99b`  
		Last Modified: Wed, 15 Dec 2021 19:41:16 GMT  
		Size: 57.7 MB (57747213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e216c2ebb46ec0635d982e57890ab4c9025c95a940e79a81a0ed8b50c49b6`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46f33417cc9574bd0139314cc88909fae8f672527fc69f493d406dad1991e1`  
		Last Modified: Wed, 15 Dec 2021 19:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c99da1af64cbeec415a8ce2302a76874846814f574e07e7d9072e70ad00192`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12055a90557dd8852e5d26b75d39ee8c5bb53795e2df51b883cc60bf8d765aee`  
		Last Modified: Wed, 15 Dec 2021 19:41:39 GMT  
		Size: 6.6 MB (6612548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebd11f99968f9c201fb0dcc9d59bcd8653f16ef5b376446a563ca41ec400751`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a482d3fe6b24fb02fce911311cdbd9069d2a150c94dca0d5fcc85cf4b30b21b7`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7dc2dffdacf12cfe5762299899abbc48a89a3be50f8a7c62933935cdc3c9c2`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:88bd12875df6cb64ffd3965a3977feb9c3a0fd1c971b9521534492d8cc818f3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:c574820d5eabf3bd03e11a911791178a30d5b90ba7daafbb52635aece6ec18ba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95553909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18661e6d9122218fd4e0c88dc1e535ddbc477e8c2c64351efc251786a011e196`
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
# Wed, 15 Dec 2021 20:19:27 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 20:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:34 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 20:19:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 20:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:35 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 20:19:42 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 15 Dec 2021 20:19:43 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 15 Dec 2021 20:19:43 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 15 Dec 2021 20:19:44 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 15 Dec 2021 20:19:44 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:44 GMT
VOLUME [/var/lib/docker]
# Wed, 15 Dec 2021 20:19:44 GMT
EXPOSE 2375 2376
# Wed, 15 Dec 2021 20:19:44 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:45 GMT
CMD []
# Wed, 15 Dec 2021 20:19:48 GMT
RUN apk add --no-cache iproute2
# Wed, 15 Dec 2021 20:19:49 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 15 Dec 2021 20:19:50 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 15 Dec 2021 20:19:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 15 Dec 2021 20:19:53 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 15 Dec 2021 20:19:53 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 15 Dec 2021 20:19:54 GMT
USER rootless
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
	-	`sha256:a3f2dd7b7d653d57dbfc55dcef38007cf7ae05a4c1a226f4465b3723cb2232ed`  
		Last Modified: Wed, 15 Dec 2021 20:20:32 GMT  
		Size: 63.7 MB (63718464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d182b62d4a3549bba88c6f8f32c2d7850ca927a7df0682d9a0de05d0c40095e2`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a57db2abd77c0b995c329d7812464e3734bc1af7b829bd1a42d461de77d3b7`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73490af52bd34939d0d8b02fe67c992943d062112c5a1cb41daf43146a25ae1b`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d28806efd0ea428cf206cb382a31cb6fba2972e2e6e870051723dab28340158`  
		Last Modified: Wed, 15 Dec 2021 20:20:55 GMT  
		Size: 6.7 MB (6734098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97fd78563ff48a3ea4d64328aac35a97ef969306734b403631f8f8fb36d16e5`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffaf1aff7f0b5974dc8e7b9ce5119cf168e186a2281887ebdb30b850059c51ec`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8eed8b923285e1979ee45a366bc2852d46843fc0ababa5c7de8d8009f25f757`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4444124f7f8ff8ec85dd6ce1b2e709d524c897ac4115dee4d3fe112969a9e617`  
		Last Modified: Wed, 15 Dec 2021 20:21:20 GMT  
		Size: 1.2 MB (1162106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03e82f9fb8f6b548ad22baa5fc4b53ed561d820d967f4da8cc9bd05f79c07ce`  
		Last Modified: Wed, 15 Dec 2021 20:21:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dfe6db0ec7ad8e0fbf82c9af2fb052312f40985759a422df8c58d35e5a3635`  
		Last Modified: Wed, 15 Dec 2021 20:21:20 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32afcbc4731321210e9b6e0741bcd6b694b0159fb3ae1ba6d5a327a0f0086bb7`  
		Last Modified: Wed, 15 Dec 2021 20:21:23 GMT  
		Size: 19.1 MB (19131953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5902dceede3bc9a25497aeffa6125b18a89aea3e313b20a944f50f4f03d397c3`  
		Last Modified: Wed, 15 Dec 2021 20:21:20 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:0b938ec7ea96b1f40863ecc7b01be4cf348c84800b9ccd38bf86126655426da5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.3 MB (91316335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d4b842a15fcdb0104cacdbba294e63bcf3d1714af7ef34ddfbc5b8972f95bcd`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 19:39:37 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 19:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 19:39:38 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 19:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 19:39:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 19:39:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:39:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 19:39:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 19:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 19:39:48 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 19:39:58 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 15 Dec 2021 19:39:59 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 15 Dec 2021 19:40:00 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 15 Dec 2021 19:40:01 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 15 Dec 2021 19:40:03 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:40:03 GMT
VOLUME [/var/lib/docker]
# Wed, 15 Dec 2021 19:40:04 GMT
EXPOSE 2375 2376
# Wed, 15 Dec 2021 19:40:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 15 Dec 2021 19:40:06 GMT
CMD []
# Wed, 15 Dec 2021 19:40:14 GMT
RUN apk add --no-cache iproute2
# Wed, 15 Dec 2021 19:40:14 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 15 Dec 2021 19:40:15 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 15 Dec 2021 19:40:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 15 Dec 2021 19:40:18 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 15 Dec 2021 19:40:19 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 15 Dec 2021 19:40:20 GMT
USER rootless
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1339a3be518a98fb1ef64708d14d86fd4039c4bb0a3d1db8c2d4a4c00fb8a2`  
		Last Modified: Wed, 15 Dec 2021 19:41:10 GMT  
		Size: 1.9 MB (1949540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353862b30dd70efe72e0bf55133d47f2a5b000e37f9cdb0e7e4a0178a5f076ec`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3190c06c4855888df747c4f505d0bc7aaecfbb0d9d4acaee685e28bddfb99b`  
		Last Modified: Wed, 15 Dec 2021 19:41:16 GMT  
		Size: 57.7 MB (57747213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e216c2ebb46ec0635d982e57890ab4c9025c95a940e79a81a0ed8b50c49b6`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46f33417cc9574bd0139314cc88909fae8f672527fc69f493d406dad1991e1`  
		Last Modified: Wed, 15 Dec 2021 19:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c99da1af64cbeec415a8ce2302a76874846814f574e07e7d9072e70ad00192`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12055a90557dd8852e5d26b75d39ee8c5bb53795e2df51b883cc60bf8d765aee`  
		Last Modified: Wed, 15 Dec 2021 19:41:39 GMT  
		Size: 6.6 MB (6612548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebd11f99968f9c201fb0dcc9d59bcd8653f16ef5b376446a563ca41ec400751`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a482d3fe6b24fb02fce911311cdbd9069d2a150c94dca0d5fcc85cf4b30b21b7`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7dc2dffdacf12cfe5762299899abbc48a89a3be50f8a7c62933935cdc3c9c2`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d670443b55fd7ca190ef7e74937f339344c982fc891932721e85c0258f6a99`  
		Last Modified: Wed, 15 Dec 2021 19:42:00 GMT  
		Size: 1.2 MB (1178051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32d2d69d1f3c01aa88625f185c33e9d81afc49cae7c69e60188ea8e33edfb44`  
		Last Modified: Wed, 15 Dec 2021 19:42:00 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4374d2147deadc7d22f890fc9782880efb5b1f173e4c9532601ecc19dc672bc3`  
		Last Modified: Wed, 15 Dec 2021 19:42:00 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17554114a98827967270ad33a848b60df2da91189aa8f7b5e96d201e26e97347`  
		Last Modified: Wed, 15 Dec 2021 19:42:03 GMT  
		Size: 21.1 MB (21105227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a74d2bf287bf033007cdbf327593f6b8e1a14edf5106b8a6bd75474eb22c435`  
		Last Modified: Wed, 15 Dec 2021 19:42:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-git`

```console
$ docker pull docker@sha256:fe99b62ceb53a90c054c55e86440cf00d13b3ff2f3d99692a0bef4adc1b45c67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-git` - linux; amd64

```console
$ docker pull docker@sha256:44c9a5a828003f5276a952052dc4999b98b0243d0dd1bd7c8e85ea38352077b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75342928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:456c635446977ad70607efd5889908b1ccb8b727ae6244dca0569b72c2b63ead`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 20:19:27 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 20:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:34 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 20:19:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 20:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:35 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 20:19:58 GMT
RUN apk add --no-cache git
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
	-	`sha256:a3f2dd7b7d653d57dbfc55dcef38007cf7ae05a4c1a226f4465b3723cb2232ed`  
		Last Modified: Wed, 15 Dec 2021 20:20:32 GMT  
		Size: 63.7 MB (63718464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d182b62d4a3549bba88c6f8f32c2d7850ca927a7df0682d9a0de05d0c40095e2`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a57db2abd77c0b995c329d7812464e3734bc1af7b829bd1a42d461de77d3b7`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73490af52bd34939d0d8b02fe67c992943d062112c5a1cb41daf43146a25ae1b`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c28794b3e25128706cf6faa48515b023ea6f2d7bfacfe6493fa40b2f1436f1`  
		Last Modified: Wed, 15 Dec 2021 20:21:43 GMT  
		Size: 6.8 MB (6823784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:90c29958713df30b15a09c261d26cafc66bab0b23247300298267ef7f066fa67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69346856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab607b2188f06d49d5e0544631eb76703f41790b8928653d0ddb72808181c09`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 19:39:37 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 19:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 19:39:38 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 19:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 19:39:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 19:39:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:39:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 19:39:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 19:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 19:39:48 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 19:40:27 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1339a3be518a98fb1ef64708d14d86fd4039c4bb0a3d1db8c2d4a4c00fb8a2`  
		Last Modified: Wed, 15 Dec 2021 19:41:10 GMT  
		Size: 1.9 MB (1949540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353862b30dd70efe72e0bf55133d47f2a5b000e37f9cdb0e7e4a0178a5f076ec`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3190c06c4855888df747c4f505d0bc7aaecfbb0d9d4acaee685e28bddfb99b`  
		Last Modified: Wed, 15 Dec 2021 19:41:16 GMT  
		Size: 57.7 MB (57747213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e216c2ebb46ec0635d982e57890ab4c9025c95a940e79a81a0ed8b50c49b6`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46f33417cc9574bd0139314cc88909fae8f672527fc69f493d406dad1991e1`  
		Last Modified: Wed, 15 Dec 2021 19:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c99da1af64cbeec415a8ce2302a76874846814f574e07e7d9072e70ad00192`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973ec878c950532925c0e2a1d397edf1086a25b91f4af6344e9b56a4dbb000c9`  
		Last Modified: Wed, 15 Dec 2021 19:42:24 GMT  
		Size: 6.9 MB (6932833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore`

```console
$ docker pull docker@sha256:385c45deff3f6fd090ebbcaa19c2c4c7eb3ad8ee2e717b2cff3128b88154e116
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `docker:20-windowsservercore` - windows version 10.0.17763.2366; amd64

```console
$ docker pull docker@sha256:dda522f423b5f150997bb295498a0458b41f56ba7342754baffabaa57628cad4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2762195765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14c2d634d7d869aa8fd42835e537aa314d535b0c909a92cc26117284d1d84c9f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 18 Dec 2021 10:27:00 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 18 Dec 2021 10:27:01 GMT
ENV DOCKER_VERSION=20.10.12
# Sat, 18 Dec 2021 10:27:02 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.12.zip
# Sat, 18 Dec 2021 10:28:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd048ecae1fa585d9d38c625121cb1a8b3acb5c3d6413282e75b85193bfd151`  
		Last Modified: Sat, 18 Dec 2021 10:28:39 GMT  
		Size: 371.1 KB (371093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335bf6ad2e01acadc382163d2078d5e9a371ac3399fb5429befb22da359a6512`  
		Last Modified: Sat, 18 Dec 2021 10:28:38 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d37fa43c886f9824002edada19e4288dd79b3ca0048dccdbe1a4e1dcf1e850`  
		Last Modified: Sat, 18 Dec 2021 10:28:39 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280971e530a5c147ecc05e54d1dbb42f374f86e078c30f273150762f17ede482`  
		Last Modified: Sat, 18 Dec 2021 10:28:50 GMT  
		Size: 53.2 MB (53215955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-1809`

```console
$ docker pull docker@sha256:385c45deff3f6fd090ebbcaa19c2c4c7eb3ad8ee2e717b2cff3128b88154e116
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `docker:20-windowsservercore-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull docker@sha256:dda522f423b5f150997bb295498a0458b41f56ba7342754baffabaa57628cad4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2762195765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14c2d634d7d869aa8fd42835e537aa314d535b0c909a92cc26117284d1d84c9f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 18 Dec 2021 10:27:00 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 18 Dec 2021 10:27:01 GMT
ENV DOCKER_VERSION=20.10.12
# Sat, 18 Dec 2021 10:27:02 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.12.zip
# Sat, 18 Dec 2021 10:28:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd048ecae1fa585d9d38c625121cb1a8b3acb5c3d6413282e75b85193bfd151`  
		Last Modified: Sat, 18 Dec 2021 10:28:39 GMT  
		Size: 371.1 KB (371093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335bf6ad2e01acadc382163d2078d5e9a371ac3399fb5429befb22da359a6512`  
		Last Modified: Sat, 18 Dec 2021 10:28:38 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d37fa43c886f9824002edada19e4288dd79b3ca0048dccdbe1a4e1dcf1e850`  
		Last Modified: Sat, 18 Dec 2021 10:28:39 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280971e530a5c147ecc05e54d1dbb42f374f86e078c30f273150762f17ede482`  
		Last Modified: Sat, 18 Dec 2021 10:28:50 GMT  
		Size: 53.2 MB (53215955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `docker:20.10`

```console
$ docker pull docker@sha256:a729cce205a05b0b86dc8dca87823efaffc3f74979fe7dc86a707c2fbf631b61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10` - linux; amd64

```console
$ docker pull docker@sha256:b15efb5c932fd29acc764a2b8c0e6b1dfda4450f2a67d630c3b9f205785fdb2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68519144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15a9bc7c6340df2ac9d6c8196ca1d905180ddf2ca8b29a8d98f5422e2e5ccf85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 20:19:27 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 20:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:34 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 20:19:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 20:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:35 GMT
CMD ["sh"]
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
	-	`sha256:a3f2dd7b7d653d57dbfc55dcef38007cf7ae05a4c1a226f4465b3723cb2232ed`  
		Last Modified: Wed, 15 Dec 2021 20:20:32 GMT  
		Size: 63.7 MB (63718464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d182b62d4a3549bba88c6f8f32c2d7850ca927a7df0682d9a0de05d0c40095e2`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a57db2abd77c0b995c329d7812464e3734bc1af7b829bd1a42d461de77d3b7`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73490af52bd34939d0d8b02fe67c992943d062112c5a1cb41daf43146a25ae1b`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:17db01f277a58c2d70b2a40a8f46607c5319dd2f23c55dcf8c835cd25f7ff746
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62414023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4610f8d36c6766d145891417dd49f9b3e6535b43820bae79640d380fb88016b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 19:39:37 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 19:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 19:39:38 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 19:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 19:39:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 19:39:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:39:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 19:39:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 19:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 19:39:48 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1339a3be518a98fb1ef64708d14d86fd4039c4bb0a3d1db8c2d4a4c00fb8a2`  
		Last Modified: Wed, 15 Dec 2021 19:41:10 GMT  
		Size: 1.9 MB (1949540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353862b30dd70efe72e0bf55133d47f2a5b000e37f9cdb0e7e4a0178a5f076ec`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3190c06c4855888df747c4f505d0bc7aaecfbb0d9d4acaee685e28bddfb99b`  
		Last Modified: Wed, 15 Dec 2021 19:41:16 GMT  
		Size: 57.7 MB (57747213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e216c2ebb46ec0635d982e57890ab4c9025c95a940e79a81a0ed8b50c49b6`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46f33417cc9574bd0139314cc88909fae8f672527fc69f493d406dad1991e1`  
		Last Modified: Wed, 15 Dec 2021 19:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c99da1af64cbeec415a8ce2302a76874846814f574e07e7d9072e70ad00192`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind`

```console
$ docker pull docker@sha256:1f50d3a86f7035805843779f803e81e8f4ce96b62ed68fc70cdcf4922f43470b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind` - linux; amd64

```console
$ docker pull docker@sha256:4e04836731b7100e8bd5e0b35756f53d0b6211ddb3cc7ec326ae3640adcfa004
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75258135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:175122d895c3ac2d1a9e3eeaa4885972ffcf3cf86c6e14261fd58db58ca77139`
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
# Wed, 15 Dec 2021 20:19:27 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 20:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:34 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 20:19:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 20:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:35 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 20:19:42 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 15 Dec 2021 20:19:43 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 15 Dec 2021 20:19:43 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 15 Dec 2021 20:19:44 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 15 Dec 2021 20:19:44 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:44 GMT
VOLUME [/var/lib/docker]
# Wed, 15 Dec 2021 20:19:44 GMT
EXPOSE 2375 2376
# Wed, 15 Dec 2021 20:19:44 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:45 GMT
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
	-	`sha256:a3f2dd7b7d653d57dbfc55dcef38007cf7ae05a4c1a226f4465b3723cb2232ed`  
		Last Modified: Wed, 15 Dec 2021 20:20:32 GMT  
		Size: 63.7 MB (63718464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d182b62d4a3549bba88c6f8f32c2d7850ca927a7df0682d9a0de05d0c40095e2`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a57db2abd77c0b995c329d7812464e3734bc1af7b829bd1a42d461de77d3b7`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73490af52bd34939d0d8b02fe67c992943d062112c5a1cb41daf43146a25ae1b`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d28806efd0ea428cf206cb382a31cb6fba2972e2e6e870051723dab28340158`  
		Last Modified: Wed, 15 Dec 2021 20:20:55 GMT  
		Size: 6.7 MB (6734098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97fd78563ff48a3ea4d64328aac35a97ef969306734b403631f8f8fb36d16e5`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffaf1aff7f0b5974dc8e7b9ce5119cf168e186a2281887ebdb30b850059c51ec`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8eed8b923285e1979ee45a366bc2852d46843fc0ababa5c7de8d8009f25f757`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5ed82558a7494a410eb6777aef81cf618118517d352b34307ca40d1da8589a22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69031436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd9db4c317abc6701f11a378339752bf58a9371ae9dce469dd02627f373c2b97`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 19:39:37 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 19:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 19:39:38 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 19:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 19:39:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 19:39:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:39:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 19:39:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 19:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 19:39:48 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 19:39:58 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 15 Dec 2021 19:39:59 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 15 Dec 2021 19:40:00 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 15 Dec 2021 19:40:01 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 15 Dec 2021 19:40:03 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:40:03 GMT
VOLUME [/var/lib/docker]
# Wed, 15 Dec 2021 19:40:04 GMT
EXPOSE 2375 2376
# Wed, 15 Dec 2021 19:40:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 15 Dec 2021 19:40:06 GMT
CMD []
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1339a3be518a98fb1ef64708d14d86fd4039c4bb0a3d1db8c2d4a4c00fb8a2`  
		Last Modified: Wed, 15 Dec 2021 19:41:10 GMT  
		Size: 1.9 MB (1949540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353862b30dd70efe72e0bf55133d47f2a5b000e37f9cdb0e7e4a0178a5f076ec`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3190c06c4855888df747c4f505d0bc7aaecfbb0d9d4acaee685e28bddfb99b`  
		Last Modified: Wed, 15 Dec 2021 19:41:16 GMT  
		Size: 57.7 MB (57747213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e216c2ebb46ec0635d982e57890ab4c9025c95a940e79a81a0ed8b50c49b6`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46f33417cc9574bd0139314cc88909fae8f672527fc69f493d406dad1991e1`  
		Last Modified: Wed, 15 Dec 2021 19:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c99da1af64cbeec415a8ce2302a76874846814f574e07e7d9072e70ad00192`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12055a90557dd8852e5d26b75d39ee8c5bb53795e2df51b883cc60bf8d765aee`  
		Last Modified: Wed, 15 Dec 2021 19:41:39 GMT  
		Size: 6.6 MB (6612548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebd11f99968f9c201fb0dcc9d59bcd8653f16ef5b376446a563ca41ec400751`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a482d3fe6b24fb02fce911311cdbd9069d2a150c94dca0d5fcc85cf4b30b21b7`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7dc2dffdacf12cfe5762299899abbc48a89a3be50f8a7c62933935cdc3c9c2`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind-rootless`

```console
$ docker pull docker@sha256:88bd12875df6cb64ffd3965a3977feb9c3a0fd1c971b9521534492d8cc818f3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:c574820d5eabf3bd03e11a911791178a30d5b90ba7daafbb52635aece6ec18ba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95553909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18661e6d9122218fd4e0c88dc1e535ddbc477e8c2c64351efc251786a011e196`
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
# Wed, 15 Dec 2021 20:19:27 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 20:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:34 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 20:19:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 20:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:35 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 20:19:42 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 15 Dec 2021 20:19:43 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 15 Dec 2021 20:19:43 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 15 Dec 2021 20:19:44 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 15 Dec 2021 20:19:44 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:44 GMT
VOLUME [/var/lib/docker]
# Wed, 15 Dec 2021 20:19:44 GMT
EXPOSE 2375 2376
# Wed, 15 Dec 2021 20:19:44 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:45 GMT
CMD []
# Wed, 15 Dec 2021 20:19:48 GMT
RUN apk add --no-cache iproute2
# Wed, 15 Dec 2021 20:19:49 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 15 Dec 2021 20:19:50 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 15 Dec 2021 20:19:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 15 Dec 2021 20:19:53 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 15 Dec 2021 20:19:53 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 15 Dec 2021 20:19:54 GMT
USER rootless
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
	-	`sha256:a3f2dd7b7d653d57dbfc55dcef38007cf7ae05a4c1a226f4465b3723cb2232ed`  
		Last Modified: Wed, 15 Dec 2021 20:20:32 GMT  
		Size: 63.7 MB (63718464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d182b62d4a3549bba88c6f8f32c2d7850ca927a7df0682d9a0de05d0c40095e2`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a57db2abd77c0b995c329d7812464e3734bc1af7b829bd1a42d461de77d3b7`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73490af52bd34939d0d8b02fe67c992943d062112c5a1cb41daf43146a25ae1b`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d28806efd0ea428cf206cb382a31cb6fba2972e2e6e870051723dab28340158`  
		Last Modified: Wed, 15 Dec 2021 20:20:55 GMT  
		Size: 6.7 MB (6734098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97fd78563ff48a3ea4d64328aac35a97ef969306734b403631f8f8fb36d16e5`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffaf1aff7f0b5974dc8e7b9ce5119cf168e186a2281887ebdb30b850059c51ec`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8eed8b923285e1979ee45a366bc2852d46843fc0ababa5c7de8d8009f25f757`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4444124f7f8ff8ec85dd6ce1b2e709d524c897ac4115dee4d3fe112969a9e617`  
		Last Modified: Wed, 15 Dec 2021 20:21:20 GMT  
		Size: 1.2 MB (1162106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03e82f9fb8f6b548ad22baa5fc4b53ed561d820d967f4da8cc9bd05f79c07ce`  
		Last Modified: Wed, 15 Dec 2021 20:21:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dfe6db0ec7ad8e0fbf82c9af2fb052312f40985759a422df8c58d35e5a3635`  
		Last Modified: Wed, 15 Dec 2021 20:21:20 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32afcbc4731321210e9b6e0741bcd6b694b0159fb3ae1ba6d5a327a0f0086bb7`  
		Last Modified: Wed, 15 Dec 2021 20:21:23 GMT  
		Size: 19.1 MB (19131953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5902dceede3bc9a25497aeffa6125b18a89aea3e313b20a944f50f4f03d397c3`  
		Last Modified: Wed, 15 Dec 2021 20:21:20 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:0b938ec7ea96b1f40863ecc7b01be4cf348c84800b9ccd38bf86126655426da5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.3 MB (91316335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d4b842a15fcdb0104cacdbba294e63bcf3d1714af7ef34ddfbc5b8972f95bcd`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 19:39:37 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 19:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 19:39:38 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 19:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 19:39:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 19:39:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:39:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 19:39:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 19:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 19:39:48 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 19:39:58 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 15 Dec 2021 19:39:59 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 15 Dec 2021 19:40:00 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 15 Dec 2021 19:40:01 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 15 Dec 2021 19:40:03 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:40:03 GMT
VOLUME [/var/lib/docker]
# Wed, 15 Dec 2021 19:40:04 GMT
EXPOSE 2375 2376
# Wed, 15 Dec 2021 19:40:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 15 Dec 2021 19:40:06 GMT
CMD []
# Wed, 15 Dec 2021 19:40:14 GMT
RUN apk add --no-cache iproute2
# Wed, 15 Dec 2021 19:40:14 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 15 Dec 2021 19:40:15 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 15 Dec 2021 19:40:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 15 Dec 2021 19:40:18 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 15 Dec 2021 19:40:19 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 15 Dec 2021 19:40:20 GMT
USER rootless
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1339a3be518a98fb1ef64708d14d86fd4039c4bb0a3d1db8c2d4a4c00fb8a2`  
		Last Modified: Wed, 15 Dec 2021 19:41:10 GMT  
		Size: 1.9 MB (1949540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353862b30dd70efe72e0bf55133d47f2a5b000e37f9cdb0e7e4a0178a5f076ec`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3190c06c4855888df747c4f505d0bc7aaecfbb0d9d4acaee685e28bddfb99b`  
		Last Modified: Wed, 15 Dec 2021 19:41:16 GMT  
		Size: 57.7 MB (57747213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e216c2ebb46ec0635d982e57890ab4c9025c95a940e79a81a0ed8b50c49b6`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46f33417cc9574bd0139314cc88909fae8f672527fc69f493d406dad1991e1`  
		Last Modified: Wed, 15 Dec 2021 19:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c99da1af64cbeec415a8ce2302a76874846814f574e07e7d9072e70ad00192`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12055a90557dd8852e5d26b75d39ee8c5bb53795e2df51b883cc60bf8d765aee`  
		Last Modified: Wed, 15 Dec 2021 19:41:39 GMT  
		Size: 6.6 MB (6612548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebd11f99968f9c201fb0dcc9d59bcd8653f16ef5b376446a563ca41ec400751`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a482d3fe6b24fb02fce911311cdbd9069d2a150c94dca0d5fcc85cf4b30b21b7`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7dc2dffdacf12cfe5762299899abbc48a89a3be50f8a7c62933935cdc3c9c2`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d670443b55fd7ca190ef7e74937f339344c982fc891932721e85c0258f6a99`  
		Last Modified: Wed, 15 Dec 2021 19:42:00 GMT  
		Size: 1.2 MB (1178051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32d2d69d1f3c01aa88625f185c33e9d81afc49cae7c69e60188ea8e33edfb44`  
		Last Modified: Wed, 15 Dec 2021 19:42:00 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4374d2147deadc7d22f890fc9782880efb5b1f173e4c9532601ecc19dc672bc3`  
		Last Modified: Wed, 15 Dec 2021 19:42:00 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17554114a98827967270ad33a848b60df2da91189aa8f7b5e96d201e26e97347`  
		Last Modified: Wed, 15 Dec 2021 19:42:03 GMT  
		Size: 21.1 MB (21105227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a74d2bf287bf033007cdbf327593f6b8e1a14edf5106b8a6bd75474eb22c435`  
		Last Modified: Wed, 15 Dec 2021 19:42:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-git`

```console
$ docker pull docker@sha256:fe99b62ceb53a90c054c55e86440cf00d13b3ff2f3d99692a0bef4adc1b45c67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-git` - linux; amd64

```console
$ docker pull docker@sha256:44c9a5a828003f5276a952052dc4999b98b0243d0dd1bd7c8e85ea38352077b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75342928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:456c635446977ad70607efd5889908b1ccb8b727ae6244dca0569b72c2b63ead`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 20:19:27 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 20:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:34 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 20:19:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 20:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:35 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 20:19:58 GMT
RUN apk add --no-cache git
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
	-	`sha256:a3f2dd7b7d653d57dbfc55dcef38007cf7ae05a4c1a226f4465b3723cb2232ed`  
		Last Modified: Wed, 15 Dec 2021 20:20:32 GMT  
		Size: 63.7 MB (63718464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d182b62d4a3549bba88c6f8f32c2d7850ca927a7df0682d9a0de05d0c40095e2`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a57db2abd77c0b995c329d7812464e3734bc1af7b829bd1a42d461de77d3b7`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73490af52bd34939d0d8b02fe67c992943d062112c5a1cb41daf43146a25ae1b`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c28794b3e25128706cf6faa48515b023ea6f2d7bfacfe6493fa40b2f1436f1`  
		Last Modified: Wed, 15 Dec 2021 20:21:43 GMT  
		Size: 6.8 MB (6823784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:90c29958713df30b15a09c261d26cafc66bab0b23247300298267ef7f066fa67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69346856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab607b2188f06d49d5e0544631eb76703f41790b8928653d0ddb72808181c09`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 19:39:37 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 19:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 19:39:38 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 19:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 19:39:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 19:39:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:39:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 19:39:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 19:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 19:39:48 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 19:40:27 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1339a3be518a98fb1ef64708d14d86fd4039c4bb0a3d1db8c2d4a4c00fb8a2`  
		Last Modified: Wed, 15 Dec 2021 19:41:10 GMT  
		Size: 1.9 MB (1949540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353862b30dd70efe72e0bf55133d47f2a5b000e37f9cdb0e7e4a0178a5f076ec`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3190c06c4855888df747c4f505d0bc7aaecfbb0d9d4acaee685e28bddfb99b`  
		Last Modified: Wed, 15 Dec 2021 19:41:16 GMT  
		Size: 57.7 MB (57747213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e216c2ebb46ec0635d982e57890ab4c9025c95a940e79a81a0ed8b50c49b6`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46f33417cc9574bd0139314cc88909fae8f672527fc69f493d406dad1991e1`  
		Last Modified: Wed, 15 Dec 2021 19:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c99da1af64cbeec415a8ce2302a76874846814f574e07e7d9072e70ad00192`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973ec878c950532925c0e2a1d397edf1086a25b91f4af6344e9b56a4dbb000c9`  
		Last Modified: Wed, 15 Dec 2021 19:42:24 GMT  
		Size: 6.9 MB (6932833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore`

```console
$ docker pull docker@sha256:385c45deff3f6fd090ebbcaa19c2c4c7eb3ad8ee2e717b2cff3128b88154e116
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `docker:20.10-windowsservercore` - windows version 10.0.17763.2366; amd64

```console
$ docker pull docker@sha256:dda522f423b5f150997bb295498a0458b41f56ba7342754baffabaa57628cad4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2762195765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14c2d634d7d869aa8fd42835e537aa314d535b0c909a92cc26117284d1d84c9f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 18 Dec 2021 10:27:00 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 18 Dec 2021 10:27:01 GMT
ENV DOCKER_VERSION=20.10.12
# Sat, 18 Dec 2021 10:27:02 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.12.zip
# Sat, 18 Dec 2021 10:28:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd048ecae1fa585d9d38c625121cb1a8b3acb5c3d6413282e75b85193bfd151`  
		Last Modified: Sat, 18 Dec 2021 10:28:39 GMT  
		Size: 371.1 KB (371093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335bf6ad2e01acadc382163d2078d5e9a371ac3399fb5429befb22da359a6512`  
		Last Modified: Sat, 18 Dec 2021 10:28:38 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d37fa43c886f9824002edada19e4288dd79b3ca0048dccdbe1a4e1dcf1e850`  
		Last Modified: Sat, 18 Dec 2021 10:28:39 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280971e530a5c147ecc05e54d1dbb42f374f86e078c30f273150762f17ede482`  
		Last Modified: Sat, 18 Dec 2021 10:28:50 GMT  
		Size: 53.2 MB (53215955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-1809`

```console
$ docker pull docker@sha256:385c45deff3f6fd090ebbcaa19c2c4c7eb3ad8ee2e717b2cff3128b88154e116
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `docker:20.10-windowsservercore-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull docker@sha256:dda522f423b5f150997bb295498a0458b41f56ba7342754baffabaa57628cad4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2762195765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14c2d634d7d869aa8fd42835e537aa314d535b0c909a92cc26117284d1d84c9f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 18 Dec 2021 10:27:00 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 18 Dec 2021 10:27:01 GMT
ENV DOCKER_VERSION=20.10.12
# Sat, 18 Dec 2021 10:27:02 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.12.zip
# Sat, 18 Dec 2021 10:28:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd048ecae1fa585d9d38c625121cb1a8b3acb5c3d6413282e75b85193bfd151`  
		Last Modified: Sat, 18 Dec 2021 10:28:39 GMT  
		Size: 371.1 KB (371093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335bf6ad2e01acadc382163d2078d5e9a371ac3399fb5429befb22da359a6512`  
		Last Modified: Sat, 18 Dec 2021 10:28:38 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d37fa43c886f9824002edada19e4288dd79b3ca0048dccdbe1a4e1dcf1e850`  
		Last Modified: Sat, 18 Dec 2021 10:28:39 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280971e530a5c147ecc05e54d1dbb42f374f86e078c30f273150762f17ede482`  
		Last Modified: Sat, 18 Dec 2021 10:28:50 GMT  
		Size: 53.2 MB (53215955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `docker:20.10.12`

```console
$ docker pull docker@sha256:a729cce205a05b0b86dc8dca87823efaffc3f74979fe7dc86a707c2fbf631b61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.12` - linux; amd64

```console
$ docker pull docker@sha256:b15efb5c932fd29acc764a2b8c0e6b1dfda4450f2a67d630c3b9f205785fdb2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68519144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15a9bc7c6340df2ac9d6c8196ca1d905180ddf2ca8b29a8d98f5422e2e5ccf85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 20:19:27 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 20:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:34 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 20:19:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 20:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:35 GMT
CMD ["sh"]
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
	-	`sha256:a3f2dd7b7d653d57dbfc55dcef38007cf7ae05a4c1a226f4465b3723cb2232ed`  
		Last Modified: Wed, 15 Dec 2021 20:20:32 GMT  
		Size: 63.7 MB (63718464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d182b62d4a3549bba88c6f8f32c2d7850ca927a7df0682d9a0de05d0c40095e2`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a57db2abd77c0b995c329d7812464e3734bc1af7b829bd1a42d461de77d3b7`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73490af52bd34939d0d8b02fe67c992943d062112c5a1cb41daf43146a25ae1b`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.12` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:17db01f277a58c2d70b2a40a8f46607c5319dd2f23c55dcf8c835cd25f7ff746
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62414023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4610f8d36c6766d145891417dd49f9b3e6535b43820bae79640d380fb88016b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 19:39:37 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 19:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 19:39:38 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 19:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 19:39:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 19:39:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:39:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 19:39:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 19:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 19:39:48 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1339a3be518a98fb1ef64708d14d86fd4039c4bb0a3d1db8c2d4a4c00fb8a2`  
		Last Modified: Wed, 15 Dec 2021 19:41:10 GMT  
		Size: 1.9 MB (1949540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353862b30dd70efe72e0bf55133d47f2a5b000e37f9cdb0e7e4a0178a5f076ec`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3190c06c4855888df747c4f505d0bc7aaecfbb0d9d4acaee685e28bddfb99b`  
		Last Modified: Wed, 15 Dec 2021 19:41:16 GMT  
		Size: 57.7 MB (57747213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e216c2ebb46ec0635d982e57890ab4c9025c95a940e79a81a0ed8b50c49b6`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46f33417cc9574bd0139314cc88909fae8f672527fc69f493d406dad1991e1`  
		Last Modified: Wed, 15 Dec 2021 19:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c99da1af64cbeec415a8ce2302a76874846814f574e07e7d9072e70ad00192`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.12-alpine3.15`

```console
$ docker pull docker@sha256:a729cce205a05b0b86dc8dca87823efaffc3f74979fe7dc86a707c2fbf631b61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.12-alpine3.15` - linux; amd64

```console
$ docker pull docker@sha256:b15efb5c932fd29acc764a2b8c0e6b1dfda4450f2a67d630c3b9f205785fdb2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68519144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15a9bc7c6340df2ac9d6c8196ca1d905180ddf2ca8b29a8d98f5422e2e5ccf85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 20:19:27 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 20:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:34 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 20:19:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 20:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:35 GMT
CMD ["sh"]
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
	-	`sha256:a3f2dd7b7d653d57dbfc55dcef38007cf7ae05a4c1a226f4465b3723cb2232ed`  
		Last Modified: Wed, 15 Dec 2021 20:20:32 GMT  
		Size: 63.7 MB (63718464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d182b62d4a3549bba88c6f8f32c2d7850ca927a7df0682d9a0de05d0c40095e2`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a57db2abd77c0b995c329d7812464e3734bc1af7b829bd1a42d461de77d3b7`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73490af52bd34939d0d8b02fe67c992943d062112c5a1cb41daf43146a25ae1b`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.12-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:17db01f277a58c2d70b2a40a8f46607c5319dd2f23c55dcf8c835cd25f7ff746
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62414023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4610f8d36c6766d145891417dd49f9b3e6535b43820bae79640d380fb88016b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 19:39:37 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 19:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 19:39:38 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 19:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 19:39:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 19:39:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:39:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 19:39:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 19:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 19:39:48 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1339a3be518a98fb1ef64708d14d86fd4039c4bb0a3d1db8c2d4a4c00fb8a2`  
		Last Modified: Wed, 15 Dec 2021 19:41:10 GMT  
		Size: 1.9 MB (1949540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353862b30dd70efe72e0bf55133d47f2a5b000e37f9cdb0e7e4a0178a5f076ec`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3190c06c4855888df747c4f505d0bc7aaecfbb0d9d4acaee685e28bddfb99b`  
		Last Modified: Wed, 15 Dec 2021 19:41:16 GMT  
		Size: 57.7 MB (57747213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e216c2ebb46ec0635d982e57890ab4c9025c95a940e79a81a0ed8b50c49b6`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46f33417cc9574bd0139314cc88909fae8f672527fc69f493d406dad1991e1`  
		Last Modified: Wed, 15 Dec 2021 19:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c99da1af64cbeec415a8ce2302a76874846814f574e07e7d9072e70ad00192`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.12-dind`

```console
$ docker pull docker@sha256:1f50d3a86f7035805843779f803e81e8f4ce96b62ed68fc70cdcf4922f43470b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.12-dind` - linux; amd64

```console
$ docker pull docker@sha256:4e04836731b7100e8bd5e0b35756f53d0b6211ddb3cc7ec326ae3640adcfa004
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75258135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:175122d895c3ac2d1a9e3eeaa4885972ffcf3cf86c6e14261fd58db58ca77139`
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
# Wed, 15 Dec 2021 20:19:27 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 20:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:34 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 20:19:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 20:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:35 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 20:19:42 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 15 Dec 2021 20:19:43 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 15 Dec 2021 20:19:43 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 15 Dec 2021 20:19:44 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 15 Dec 2021 20:19:44 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:44 GMT
VOLUME [/var/lib/docker]
# Wed, 15 Dec 2021 20:19:44 GMT
EXPOSE 2375 2376
# Wed, 15 Dec 2021 20:19:44 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:45 GMT
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
	-	`sha256:a3f2dd7b7d653d57dbfc55dcef38007cf7ae05a4c1a226f4465b3723cb2232ed`  
		Last Modified: Wed, 15 Dec 2021 20:20:32 GMT  
		Size: 63.7 MB (63718464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d182b62d4a3549bba88c6f8f32c2d7850ca927a7df0682d9a0de05d0c40095e2`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a57db2abd77c0b995c329d7812464e3734bc1af7b829bd1a42d461de77d3b7`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73490af52bd34939d0d8b02fe67c992943d062112c5a1cb41daf43146a25ae1b`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d28806efd0ea428cf206cb382a31cb6fba2972e2e6e870051723dab28340158`  
		Last Modified: Wed, 15 Dec 2021 20:20:55 GMT  
		Size: 6.7 MB (6734098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97fd78563ff48a3ea4d64328aac35a97ef969306734b403631f8f8fb36d16e5`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffaf1aff7f0b5974dc8e7b9ce5119cf168e186a2281887ebdb30b850059c51ec`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8eed8b923285e1979ee45a366bc2852d46843fc0ababa5c7de8d8009f25f757`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.12-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5ed82558a7494a410eb6777aef81cf618118517d352b34307ca40d1da8589a22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69031436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd9db4c317abc6701f11a378339752bf58a9371ae9dce469dd02627f373c2b97`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 19:39:37 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 19:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 19:39:38 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 19:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 19:39:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 19:39:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:39:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 19:39:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 19:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 19:39:48 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 19:39:58 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 15 Dec 2021 19:39:59 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 15 Dec 2021 19:40:00 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 15 Dec 2021 19:40:01 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 15 Dec 2021 19:40:03 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:40:03 GMT
VOLUME [/var/lib/docker]
# Wed, 15 Dec 2021 19:40:04 GMT
EXPOSE 2375 2376
# Wed, 15 Dec 2021 19:40:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 15 Dec 2021 19:40:06 GMT
CMD []
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1339a3be518a98fb1ef64708d14d86fd4039c4bb0a3d1db8c2d4a4c00fb8a2`  
		Last Modified: Wed, 15 Dec 2021 19:41:10 GMT  
		Size: 1.9 MB (1949540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353862b30dd70efe72e0bf55133d47f2a5b000e37f9cdb0e7e4a0178a5f076ec`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3190c06c4855888df747c4f505d0bc7aaecfbb0d9d4acaee685e28bddfb99b`  
		Last Modified: Wed, 15 Dec 2021 19:41:16 GMT  
		Size: 57.7 MB (57747213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e216c2ebb46ec0635d982e57890ab4c9025c95a940e79a81a0ed8b50c49b6`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46f33417cc9574bd0139314cc88909fae8f672527fc69f493d406dad1991e1`  
		Last Modified: Wed, 15 Dec 2021 19:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c99da1af64cbeec415a8ce2302a76874846814f574e07e7d9072e70ad00192`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12055a90557dd8852e5d26b75d39ee8c5bb53795e2df51b883cc60bf8d765aee`  
		Last Modified: Wed, 15 Dec 2021 19:41:39 GMT  
		Size: 6.6 MB (6612548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebd11f99968f9c201fb0dcc9d59bcd8653f16ef5b376446a563ca41ec400751`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a482d3fe6b24fb02fce911311cdbd9069d2a150c94dca0d5fcc85cf4b30b21b7`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7dc2dffdacf12cfe5762299899abbc48a89a3be50f8a7c62933935cdc3c9c2`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.12-dind-alpine3.15`

```console
$ docker pull docker@sha256:1f50d3a86f7035805843779f803e81e8f4ce96b62ed68fc70cdcf4922f43470b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.12-dind-alpine3.15` - linux; amd64

```console
$ docker pull docker@sha256:4e04836731b7100e8bd5e0b35756f53d0b6211ddb3cc7ec326ae3640adcfa004
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75258135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:175122d895c3ac2d1a9e3eeaa4885972ffcf3cf86c6e14261fd58db58ca77139`
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
# Wed, 15 Dec 2021 20:19:27 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 20:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:34 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 20:19:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 20:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:35 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 20:19:42 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 15 Dec 2021 20:19:43 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 15 Dec 2021 20:19:43 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 15 Dec 2021 20:19:44 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 15 Dec 2021 20:19:44 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:44 GMT
VOLUME [/var/lib/docker]
# Wed, 15 Dec 2021 20:19:44 GMT
EXPOSE 2375 2376
# Wed, 15 Dec 2021 20:19:44 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:45 GMT
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
	-	`sha256:a3f2dd7b7d653d57dbfc55dcef38007cf7ae05a4c1a226f4465b3723cb2232ed`  
		Last Modified: Wed, 15 Dec 2021 20:20:32 GMT  
		Size: 63.7 MB (63718464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d182b62d4a3549bba88c6f8f32c2d7850ca927a7df0682d9a0de05d0c40095e2`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a57db2abd77c0b995c329d7812464e3734bc1af7b829bd1a42d461de77d3b7`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73490af52bd34939d0d8b02fe67c992943d062112c5a1cb41daf43146a25ae1b`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d28806efd0ea428cf206cb382a31cb6fba2972e2e6e870051723dab28340158`  
		Last Modified: Wed, 15 Dec 2021 20:20:55 GMT  
		Size: 6.7 MB (6734098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97fd78563ff48a3ea4d64328aac35a97ef969306734b403631f8f8fb36d16e5`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffaf1aff7f0b5974dc8e7b9ce5119cf168e186a2281887ebdb30b850059c51ec`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8eed8b923285e1979ee45a366bc2852d46843fc0ababa5c7de8d8009f25f757`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.12-dind-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5ed82558a7494a410eb6777aef81cf618118517d352b34307ca40d1da8589a22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69031436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd9db4c317abc6701f11a378339752bf58a9371ae9dce469dd02627f373c2b97`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 19:39:37 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 19:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 19:39:38 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 19:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 19:39:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 19:39:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:39:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 19:39:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 19:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 19:39:48 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 19:39:58 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 15 Dec 2021 19:39:59 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 15 Dec 2021 19:40:00 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 15 Dec 2021 19:40:01 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 15 Dec 2021 19:40:03 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:40:03 GMT
VOLUME [/var/lib/docker]
# Wed, 15 Dec 2021 19:40:04 GMT
EXPOSE 2375 2376
# Wed, 15 Dec 2021 19:40:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 15 Dec 2021 19:40:06 GMT
CMD []
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1339a3be518a98fb1ef64708d14d86fd4039c4bb0a3d1db8c2d4a4c00fb8a2`  
		Last Modified: Wed, 15 Dec 2021 19:41:10 GMT  
		Size: 1.9 MB (1949540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353862b30dd70efe72e0bf55133d47f2a5b000e37f9cdb0e7e4a0178a5f076ec`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3190c06c4855888df747c4f505d0bc7aaecfbb0d9d4acaee685e28bddfb99b`  
		Last Modified: Wed, 15 Dec 2021 19:41:16 GMT  
		Size: 57.7 MB (57747213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e216c2ebb46ec0635d982e57890ab4c9025c95a940e79a81a0ed8b50c49b6`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46f33417cc9574bd0139314cc88909fae8f672527fc69f493d406dad1991e1`  
		Last Modified: Wed, 15 Dec 2021 19:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c99da1af64cbeec415a8ce2302a76874846814f574e07e7d9072e70ad00192`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12055a90557dd8852e5d26b75d39ee8c5bb53795e2df51b883cc60bf8d765aee`  
		Last Modified: Wed, 15 Dec 2021 19:41:39 GMT  
		Size: 6.6 MB (6612548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebd11f99968f9c201fb0dcc9d59bcd8653f16ef5b376446a563ca41ec400751`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a482d3fe6b24fb02fce911311cdbd9069d2a150c94dca0d5fcc85cf4b30b21b7`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7dc2dffdacf12cfe5762299899abbc48a89a3be50f8a7c62933935cdc3c9c2`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.12-dind-rootless`

```console
$ docker pull docker@sha256:88bd12875df6cb64ffd3965a3977feb9c3a0fd1c971b9521534492d8cc818f3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.12-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:c574820d5eabf3bd03e11a911791178a30d5b90ba7daafbb52635aece6ec18ba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95553909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18661e6d9122218fd4e0c88dc1e535ddbc477e8c2c64351efc251786a011e196`
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
# Wed, 15 Dec 2021 20:19:27 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 20:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:34 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 20:19:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 20:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:35 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 20:19:42 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 15 Dec 2021 20:19:43 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 15 Dec 2021 20:19:43 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 15 Dec 2021 20:19:44 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 15 Dec 2021 20:19:44 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:44 GMT
VOLUME [/var/lib/docker]
# Wed, 15 Dec 2021 20:19:44 GMT
EXPOSE 2375 2376
# Wed, 15 Dec 2021 20:19:44 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:45 GMT
CMD []
# Wed, 15 Dec 2021 20:19:48 GMT
RUN apk add --no-cache iproute2
# Wed, 15 Dec 2021 20:19:49 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 15 Dec 2021 20:19:50 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 15 Dec 2021 20:19:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 15 Dec 2021 20:19:53 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 15 Dec 2021 20:19:53 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 15 Dec 2021 20:19:54 GMT
USER rootless
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
	-	`sha256:a3f2dd7b7d653d57dbfc55dcef38007cf7ae05a4c1a226f4465b3723cb2232ed`  
		Last Modified: Wed, 15 Dec 2021 20:20:32 GMT  
		Size: 63.7 MB (63718464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d182b62d4a3549bba88c6f8f32c2d7850ca927a7df0682d9a0de05d0c40095e2`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a57db2abd77c0b995c329d7812464e3734bc1af7b829bd1a42d461de77d3b7`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73490af52bd34939d0d8b02fe67c992943d062112c5a1cb41daf43146a25ae1b`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d28806efd0ea428cf206cb382a31cb6fba2972e2e6e870051723dab28340158`  
		Last Modified: Wed, 15 Dec 2021 20:20:55 GMT  
		Size: 6.7 MB (6734098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97fd78563ff48a3ea4d64328aac35a97ef969306734b403631f8f8fb36d16e5`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffaf1aff7f0b5974dc8e7b9ce5119cf168e186a2281887ebdb30b850059c51ec`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8eed8b923285e1979ee45a366bc2852d46843fc0ababa5c7de8d8009f25f757`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4444124f7f8ff8ec85dd6ce1b2e709d524c897ac4115dee4d3fe112969a9e617`  
		Last Modified: Wed, 15 Dec 2021 20:21:20 GMT  
		Size: 1.2 MB (1162106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03e82f9fb8f6b548ad22baa5fc4b53ed561d820d967f4da8cc9bd05f79c07ce`  
		Last Modified: Wed, 15 Dec 2021 20:21:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dfe6db0ec7ad8e0fbf82c9af2fb052312f40985759a422df8c58d35e5a3635`  
		Last Modified: Wed, 15 Dec 2021 20:21:20 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32afcbc4731321210e9b6e0741bcd6b694b0159fb3ae1ba6d5a327a0f0086bb7`  
		Last Modified: Wed, 15 Dec 2021 20:21:23 GMT  
		Size: 19.1 MB (19131953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5902dceede3bc9a25497aeffa6125b18a89aea3e313b20a944f50f4f03d397c3`  
		Last Modified: Wed, 15 Dec 2021 20:21:20 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.12-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:0b938ec7ea96b1f40863ecc7b01be4cf348c84800b9ccd38bf86126655426da5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.3 MB (91316335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d4b842a15fcdb0104cacdbba294e63bcf3d1714af7ef34ddfbc5b8972f95bcd`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 19:39:37 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 19:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 19:39:38 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 19:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 19:39:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 19:39:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:39:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 19:39:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 19:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 19:39:48 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 19:39:58 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 15 Dec 2021 19:39:59 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 15 Dec 2021 19:40:00 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 15 Dec 2021 19:40:01 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 15 Dec 2021 19:40:03 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:40:03 GMT
VOLUME [/var/lib/docker]
# Wed, 15 Dec 2021 19:40:04 GMT
EXPOSE 2375 2376
# Wed, 15 Dec 2021 19:40:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 15 Dec 2021 19:40:06 GMT
CMD []
# Wed, 15 Dec 2021 19:40:14 GMT
RUN apk add --no-cache iproute2
# Wed, 15 Dec 2021 19:40:14 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 15 Dec 2021 19:40:15 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 15 Dec 2021 19:40:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 15 Dec 2021 19:40:18 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 15 Dec 2021 19:40:19 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 15 Dec 2021 19:40:20 GMT
USER rootless
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1339a3be518a98fb1ef64708d14d86fd4039c4bb0a3d1db8c2d4a4c00fb8a2`  
		Last Modified: Wed, 15 Dec 2021 19:41:10 GMT  
		Size: 1.9 MB (1949540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353862b30dd70efe72e0bf55133d47f2a5b000e37f9cdb0e7e4a0178a5f076ec`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3190c06c4855888df747c4f505d0bc7aaecfbb0d9d4acaee685e28bddfb99b`  
		Last Modified: Wed, 15 Dec 2021 19:41:16 GMT  
		Size: 57.7 MB (57747213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e216c2ebb46ec0635d982e57890ab4c9025c95a940e79a81a0ed8b50c49b6`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46f33417cc9574bd0139314cc88909fae8f672527fc69f493d406dad1991e1`  
		Last Modified: Wed, 15 Dec 2021 19:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c99da1af64cbeec415a8ce2302a76874846814f574e07e7d9072e70ad00192`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12055a90557dd8852e5d26b75d39ee8c5bb53795e2df51b883cc60bf8d765aee`  
		Last Modified: Wed, 15 Dec 2021 19:41:39 GMT  
		Size: 6.6 MB (6612548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebd11f99968f9c201fb0dcc9d59bcd8653f16ef5b376446a563ca41ec400751`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a482d3fe6b24fb02fce911311cdbd9069d2a150c94dca0d5fcc85cf4b30b21b7`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7dc2dffdacf12cfe5762299899abbc48a89a3be50f8a7c62933935cdc3c9c2`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d670443b55fd7ca190ef7e74937f339344c982fc891932721e85c0258f6a99`  
		Last Modified: Wed, 15 Dec 2021 19:42:00 GMT  
		Size: 1.2 MB (1178051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32d2d69d1f3c01aa88625f185c33e9d81afc49cae7c69e60188ea8e33edfb44`  
		Last Modified: Wed, 15 Dec 2021 19:42:00 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4374d2147deadc7d22f890fc9782880efb5b1f173e4c9532601ecc19dc672bc3`  
		Last Modified: Wed, 15 Dec 2021 19:42:00 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17554114a98827967270ad33a848b60df2da91189aa8f7b5e96d201e26e97347`  
		Last Modified: Wed, 15 Dec 2021 19:42:03 GMT  
		Size: 21.1 MB (21105227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a74d2bf287bf033007cdbf327593f6b8e1a14edf5106b8a6bd75474eb22c435`  
		Last Modified: Wed, 15 Dec 2021 19:42:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.12-git`

```console
$ docker pull docker@sha256:fe99b62ceb53a90c054c55e86440cf00d13b3ff2f3d99692a0bef4adc1b45c67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.12-git` - linux; amd64

```console
$ docker pull docker@sha256:44c9a5a828003f5276a952052dc4999b98b0243d0dd1bd7c8e85ea38352077b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75342928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:456c635446977ad70607efd5889908b1ccb8b727ae6244dca0569b72c2b63ead`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 20:19:27 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 20:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:34 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 20:19:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 20:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:35 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 20:19:58 GMT
RUN apk add --no-cache git
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
	-	`sha256:a3f2dd7b7d653d57dbfc55dcef38007cf7ae05a4c1a226f4465b3723cb2232ed`  
		Last Modified: Wed, 15 Dec 2021 20:20:32 GMT  
		Size: 63.7 MB (63718464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d182b62d4a3549bba88c6f8f32c2d7850ca927a7df0682d9a0de05d0c40095e2`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a57db2abd77c0b995c329d7812464e3734bc1af7b829bd1a42d461de77d3b7`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73490af52bd34939d0d8b02fe67c992943d062112c5a1cb41daf43146a25ae1b`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c28794b3e25128706cf6faa48515b023ea6f2d7bfacfe6493fa40b2f1436f1`  
		Last Modified: Wed, 15 Dec 2021 20:21:43 GMT  
		Size: 6.8 MB (6823784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.12-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:90c29958713df30b15a09c261d26cafc66bab0b23247300298267ef7f066fa67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69346856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab607b2188f06d49d5e0544631eb76703f41790b8928653d0ddb72808181c09`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 19:39:37 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 19:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 19:39:38 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 19:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 19:39:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 19:39:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:39:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 19:39:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 19:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 19:39:48 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 19:40:27 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1339a3be518a98fb1ef64708d14d86fd4039c4bb0a3d1db8c2d4a4c00fb8a2`  
		Last Modified: Wed, 15 Dec 2021 19:41:10 GMT  
		Size: 1.9 MB (1949540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353862b30dd70efe72e0bf55133d47f2a5b000e37f9cdb0e7e4a0178a5f076ec`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3190c06c4855888df747c4f505d0bc7aaecfbb0d9d4acaee685e28bddfb99b`  
		Last Modified: Wed, 15 Dec 2021 19:41:16 GMT  
		Size: 57.7 MB (57747213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e216c2ebb46ec0635d982e57890ab4c9025c95a940e79a81a0ed8b50c49b6`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46f33417cc9574bd0139314cc88909fae8f672527fc69f493d406dad1991e1`  
		Last Modified: Wed, 15 Dec 2021 19:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c99da1af64cbeec415a8ce2302a76874846814f574e07e7d9072e70ad00192`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973ec878c950532925c0e2a1d397edf1086a25b91f4af6344e9b56a4dbb000c9`  
		Last Modified: Wed, 15 Dec 2021 19:42:24 GMT  
		Size: 6.9 MB (6932833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.12-windowsservercore`

```console
$ docker pull docker@sha256:385c45deff3f6fd090ebbcaa19c2c4c7eb3ad8ee2e717b2cff3128b88154e116
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `docker:20.10.12-windowsservercore` - windows version 10.0.17763.2366; amd64

```console
$ docker pull docker@sha256:dda522f423b5f150997bb295498a0458b41f56ba7342754baffabaa57628cad4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2762195765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14c2d634d7d869aa8fd42835e537aa314d535b0c909a92cc26117284d1d84c9f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 18 Dec 2021 10:27:00 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 18 Dec 2021 10:27:01 GMT
ENV DOCKER_VERSION=20.10.12
# Sat, 18 Dec 2021 10:27:02 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.12.zip
# Sat, 18 Dec 2021 10:28:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd048ecae1fa585d9d38c625121cb1a8b3acb5c3d6413282e75b85193bfd151`  
		Last Modified: Sat, 18 Dec 2021 10:28:39 GMT  
		Size: 371.1 KB (371093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335bf6ad2e01acadc382163d2078d5e9a371ac3399fb5429befb22da359a6512`  
		Last Modified: Sat, 18 Dec 2021 10:28:38 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d37fa43c886f9824002edada19e4288dd79b3ca0048dccdbe1a4e1dcf1e850`  
		Last Modified: Sat, 18 Dec 2021 10:28:39 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280971e530a5c147ecc05e54d1dbb42f374f86e078c30f273150762f17ede482`  
		Last Modified: Sat, 18 Dec 2021 10:28:50 GMT  
		Size: 53.2 MB (53215955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.12-windowsservercore-1809`

```console
$ docker pull docker@sha256:385c45deff3f6fd090ebbcaa19c2c4c7eb3ad8ee2e717b2cff3128b88154e116
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `docker:20.10.12-windowsservercore-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull docker@sha256:dda522f423b5f150997bb295498a0458b41f56ba7342754baffabaa57628cad4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2762195765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14c2d634d7d869aa8fd42835e537aa314d535b0c909a92cc26117284d1d84c9f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 18 Dec 2021 10:27:00 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 18 Dec 2021 10:27:01 GMT
ENV DOCKER_VERSION=20.10.12
# Sat, 18 Dec 2021 10:27:02 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.12.zip
# Sat, 18 Dec 2021 10:28:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd048ecae1fa585d9d38c625121cb1a8b3acb5c3d6413282e75b85193bfd151`  
		Last Modified: Sat, 18 Dec 2021 10:28:39 GMT  
		Size: 371.1 KB (371093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335bf6ad2e01acadc382163d2078d5e9a371ac3399fb5429befb22da359a6512`  
		Last Modified: Sat, 18 Dec 2021 10:28:38 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d37fa43c886f9824002edada19e4288dd79b3ca0048dccdbe1a4e1dcf1e850`  
		Last Modified: Sat, 18 Dec 2021 10:28:39 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280971e530a5c147ecc05e54d1dbb42f374f86e078c30f273150762f17ede482`  
		Last Modified: Sat, 18 Dec 2021 10:28:50 GMT  
		Size: 53.2 MB (53215955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.12-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `docker:dind`

```console
$ docker pull docker@sha256:1f50d3a86f7035805843779f803e81e8f4ce96b62ed68fc70cdcf4922f43470b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:4e04836731b7100e8bd5e0b35756f53d0b6211ddb3cc7ec326ae3640adcfa004
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75258135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:175122d895c3ac2d1a9e3eeaa4885972ffcf3cf86c6e14261fd58db58ca77139`
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
# Wed, 15 Dec 2021 20:19:27 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 20:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:34 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 20:19:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 20:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:35 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 20:19:42 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 15 Dec 2021 20:19:43 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 15 Dec 2021 20:19:43 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 15 Dec 2021 20:19:44 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 15 Dec 2021 20:19:44 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:44 GMT
VOLUME [/var/lib/docker]
# Wed, 15 Dec 2021 20:19:44 GMT
EXPOSE 2375 2376
# Wed, 15 Dec 2021 20:19:44 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:45 GMT
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
	-	`sha256:a3f2dd7b7d653d57dbfc55dcef38007cf7ae05a4c1a226f4465b3723cb2232ed`  
		Last Modified: Wed, 15 Dec 2021 20:20:32 GMT  
		Size: 63.7 MB (63718464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d182b62d4a3549bba88c6f8f32c2d7850ca927a7df0682d9a0de05d0c40095e2`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a57db2abd77c0b995c329d7812464e3734bc1af7b829bd1a42d461de77d3b7`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73490af52bd34939d0d8b02fe67c992943d062112c5a1cb41daf43146a25ae1b`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d28806efd0ea428cf206cb382a31cb6fba2972e2e6e870051723dab28340158`  
		Last Modified: Wed, 15 Dec 2021 20:20:55 GMT  
		Size: 6.7 MB (6734098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97fd78563ff48a3ea4d64328aac35a97ef969306734b403631f8f8fb36d16e5`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffaf1aff7f0b5974dc8e7b9ce5119cf168e186a2281887ebdb30b850059c51ec`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8eed8b923285e1979ee45a366bc2852d46843fc0ababa5c7de8d8009f25f757`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5ed82558a7494a410eb6777aef81cf618118517d352b34307ca40d1da8589a22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69031436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd9db4c317abc6701f11a378339752bf58a9371ae9dce469dd02627f373c2b97`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 19:39:37 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 19:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 19:39:38 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 19:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 19:39:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 19:39:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:39:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 19:39:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 19:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 19:39:48 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 19:39:58 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 15 Dec 2021 19:39:59 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 15 Dec 2021 19:40:00 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 15 Dec 2021 19:40:01 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 15 Dec 2021 19:40:03 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:40:03 GMT
VOLUME [/var/lib/docker]
# Wed, 15 Dec 2021 19:40:04 GMT
EXPOSE 2375 2376
# Wed, 15 Dec 2021 19:40:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 15 Dec 2021 19:40:06 GMT
CMD []
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1339a3be518a98fb1ef64708d14d86fd4039c4bb0a3d1db8c2d4a4c00fb8a2`  
		Last Modified: Wed, 15 Dec 2021 19:41:10 GMT  
		Size: 1.9 MB (1949540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353862b30dd70efe72e0bf55133d47f2a5b000e37f9cdb0e7e4a0178a5f076ec`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3190c06c4855888df747c4f505d0bc7aaecfbb0d9d4acaee685e28bddfb99b`  
		Last Modified: Wed, 15 Dec 2021 19:41:16 GMT  
		Size: 57.7 MB (57747213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e216c2ebb46ec0635d982e57890ab4c9025c95a940e79a81a0ed8b50c49b6`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46f33417cc9574bd0139314cc88909fae8f672527fc69f493d406dad1991e1`  
		Last Modified: Wed, 15 Dec 2021 19:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c99da1af64cbeec415a8ce2302a76874846814f574e07e7d9072e70ad00192`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12055a90557dd8852e5d26b75d39ee8c5bb53795e2df51b883cc60bf8d765aee`  
		Last Modified: Wed, 15 Dec 2021 19:41:39 GMT  
		Size: 6.6 MB (6612548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebd11f99968f9c201fb0dcc9d59bcd8653f16ef5b376446a563ca41ec400751`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a482d3fe6b24fb02fce911311cdbd9069d2a150c94dca0d5fcc85cf4b30b21b7`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7dc2dffdacf12cfe5762299899abbc48a89a3be50f8a7c62933935cdc3c9c2`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:88bd12875df6cb64ffd3965a3977feb9c3a0fd1c971b9521534492d8cc818f3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:c574820d5eabf3bd03e11a911791178a30d5b90ba7daafbb52635aece6ec18ba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95553909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18661e6d9122218fd4e0c88dc1e535ddbc477e8c2c64351efc251786a011e196`
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
# Wed, 15 Dec 2021 20:19:27 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 20:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:34 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 20:19:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 20:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:35 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 20:19:42 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 15 Dec 2021 20:19:43 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 15 Dec 2021 20:19:43 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 15 Dec 2021 20:19:44 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 15 Dec 2021 20:19:44 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:44 GMT
VOLUME [/var/lib/docker]
# Wed, 15 Dec 2021 20:19:44 GMT
EXPOSE 2375 2376
# Wed, 15 Dec 2021 20:19:44 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:45 GMT
CMD []
# Wed, 15 Dec 2021 20:19:48 GMT
RUN apk add --no-cache iproute2
# Wed, 15 Dec 2021 20:19:49 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 15 Dec 2021 20:19:50 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 15 Dec 2021 20:19:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 15 Dec 2021 20:19:53 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 15 Dec 2021 20:19:53 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 15 Dec 2021 20:19:54 GMT
USER rootless
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
	-	`sha256:a3f2dd7b7d653d57dbfc55dcef38007cf7ae05a4c1a226f4465b3723cb2232ed`  
		Last Modified: Wed, 15 Dec 2021 20:20:32 GMT  
		Size: 63.7 MB (63718464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d182b62d4a3549bba88c6f8f32c2d7850ca927a7df0682d9a0de05d0c40095e2`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a57db2abd77c0b995c329d7812464e3734bc1af7b829bd1a42d461de77d3b7`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73490af52bd34939d0d8b02fe67c992943d062112c5a1cb41daf43146a25ae1b`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d28806efd0ea428cf206cb382a31cb6fba2972e2e6e870051723dab28340158`  
		Last Modified: Wed, 15 Dec 2021 20:20:55 GMT  
		Size: 6.7 MB (6734098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97fd78563ff48a3ea4d64328aac35a97ef969306734b403631f8f8fb36d16e5`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffaf1aff7f0b5974dc8e7b9ce5119cf168e186a2281887ebdb30b850059c51ec`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8eed8b923285e1979ee45a366bc2852d46843fc0ababa5c7de8d8009f25f757`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4444124f7f8ff8ec85dd6ce1b2e709d524c897ac4115dee4d3fe112969a9e617`  
		Last Modified: Wed, 15 Dec 2021 20:21:20 GMT  
		Size: 1.2 MB (1162106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03e82f9fb8f6b548ad22baa5fc4b53ed561d820d967f4da8cc9bd05f79c07ce`  
		Last Modified: Wed, 15 Dec 2021 20:21:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dfe6db0ec7ad8e0fbf82c9af2fb052312f40985759a422df8c58d35e5a3635`  
		Last Modified: Wed, 15 Dec 2021 20:21:20 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32afcbc4731321210e9b6e0741bcd6b694b0159fb3ae1ba6d5a327a0f0086bb7`  
		Last Modified: Wed, 15 Dec 2021 20:21:23 GMT  
		Size: 19.1 MB (19131953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5902dceede3bc9a25497aeffa6125b18a89aea3e313b20a944f50f4f03d397c3`  
		Last Modified: Wed, 15 Dec 2021 20:21:20 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:0b938ec7ea96b1f40863ecc7b01be4cf348c84800b9ccd38bf86126655426da5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.3 MB (91316335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d4b842a15fcdb0104cacdbba294e63bcf3d1714af7ef34ddfbc5b8972f95bcd`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 19:39:37 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 19:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 19:39:38 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 19:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 19:39:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 19:39:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:39:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 19:39:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 19:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 19:39:48 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 19:39:58 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 15 Dec 2021 19:39:59 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 15 Dec 2021 19:40:00 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 15 Dec 2021 19:40:01 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 15 Dec 2021 19:40:03 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:40:03 GMT
VOLUME [/var/lib/docker]
# Wed, 15 Dec 2021 19:40:04 GMT
EXPOSE 2375 2376
# Wed, 15 Dec 2021 19:40:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 15 Dec 2021 19:40:06 GMT
CMD []
# Wed, 15 Dec 2021 19:40:14 GMT
RUN apk add --no-cache iproute2
# Wed, 15 Dec 2021 19:40:14 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 15 Dec 2021 19:40:15 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 15 Dec 2021 19:40:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 15 Dec 2021 19:40:18 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 15 Dec 2021 19:40:19 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 15 Dec 2021 19:40:20 GMT
USER rootless
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1339a3be518a98fb1ef64708d14d86fd4039c4bb0a3d1db8c2d4a4c00fb8a2`  
		Last Modified: Wed, 15 Dec 2021 19:41:10 GMT  
		Size: 1.9 MB (1949540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353862b30dd70efe72e0bf55133d47f2a5b000e37f9cdb0e7e4a0178a5f076ec`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3190c06c4855888df747c4f505d0bc7aaecfbb0d9d4acaee685e28bddfb99b`  
		Last Modified: Wed, 15 Dec 2021 19:41:16 GMT  
		Size: 57.7 MB (57747213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e216c2ebb46ec0635d982e57890ab4c9025c95a940e79a81a0ed8b50c49b6`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46f33417cc9574bd0139314cc88909fae8f672527fc69f493d406dad1991e1`  
		Last Modified: Wed, 15 Dec 2021 19:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c99da1af64cbeec415a8ce2302a76874846814f574e07e7d9072e70ad00192`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12055a90557dd8852e5d26b75d39ee8c5bb53795e2df51b883cc60bf8d765aee`  
		Last Modified: Wed, 15 Dec 2021 19:41:39 GMT  
		Size: 6.6 MB (6612548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebd11f99968f9c201fb0dcc9d59bcd8653f16ef5b376446a563ca41ec400751`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a482d3fe6b24fb02fce911311cdbd9069d2a150c94dca0d5fcc85cf4b30b21b7`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7dc2dffdacf12cfe5762299899abbc48a89a3be50f8a7c62933935cdc3c9c2`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d670443b55fd7ca190ef7e74937f339344c982fc891932721e85c0258f6a99`  
		Last Modified: Wed, 15 Dec 2021 19:42:00 GMT  
		Size: 1.2 MB (1178051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32d2d69d1f3c01aa88625f185c33e9d81afc49cae7c69e60188ea8e33edfb44`  
		Last Modified: Wed, 15 Dec 2021 19:42:00 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4374d2147deadc7d22f890fc9782880efb5b1f173e4c9532601ecc19dc672bc3`  
		Last Modified: Wed, 15 Dec 2021 19:42:00 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17554114a98827967270ad33a848b60df2da91189aa8f7b5e96d201e26e97347`  
		Last Modified: Wed, 15 Dec 2021 19:42:03 GMT  
		Size: 21.1 MB (21105227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a74d2bf287bf033007cdbf327593f6b8e1a14edf5106b8a6bd75474eb22c435`  
		Last Modified: Wed, 15 Dec 2021 19:42:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:fe99b62ceb53a90c054c55e86440cf00d13b3ff2f3d99692a0bef4adc1b45c67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:44c9a5a828003f5276a952052dc4999b98b0243d0dd1bd7c8e85ea38352077b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75342928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:456c635446977ad70607efd5889908b1ccb8b727ae6244dca0569b72c2b63ead`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 20:19:27 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 20:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:34 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 20:19:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 20:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:35 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 20:19:58 GMT
RUN apk add --no-cache git
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
	-	`sha256:a3f2dd7b7d653d57dbfc55dcef38007cf7ae05a4c1a226f4465b3723cb2232ed`  
		Last Modified: Wed, 15 Dec 2021 20:20:32 GMT  
		Size: 63.7 MB (63718464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d182b62d4a3549bba88c6f8f32c2d7850ca927a7df0682d9a0de05d0c40095e2`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a57db2abd77c0b995c329d7812464e3734bc1af7b829bd1a42d461de77d3b7`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73490af52bd34939d0d8b02fe67c992943d062112c5a1cb41daf43146a25ae1b`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c28794b3e25128706cf6faa48515b023ea6f2d7bfacfe6493fa40b2f1436f1`  
		Last Modified: Wed, 15 Dec 2021 20:21:43 GMT  
		Size: 6.8 MB (6823784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:90c29958713df30b15a09c261d26cafc66bab0b23247300298267ef7f066fa67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69346856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab607b2188f06d49d5e0544631eb76703f41790b8928653d0ddb72808181c09`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 19:39:37 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 19:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 19:39:38 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 19:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 19:39:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 19:39:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:39:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 19:39:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 19:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 19:39:48 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 19:40:27 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1339a3be518a98fb1ef64708d14d86fd4039c4bb0a3d1db8c2d4a4c00fb8a2`  
		Last Modified: Wed, 15 Dec 2021 19:41:10 GMT  
		Size: 1.9 MB (1949540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353862b30dd70efe72e0bf55133d47f2a5b000e37f9cdb0e7e4a0178a5f076ec`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3190c06c4855888df747c4f505d0bc7aaecfbb0d9d4acaee685e28bddfb99b`  
		Last Modified: Wed, 15 Dec 2021 19:41:16 GMT  
		Size: 57.7 MB (57747213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e216c2ebb46ec0635d982e57890ab4c9025c95a940e79a81a0ed8b50c49b6`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46f33417cc9574bd0139314cc88909fae8f672527fc69f493d406dad1991e1`  
		Last Modified: Wed, 15 Dec 2021 19:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c99da1af64cbeec415a8ce2302a76874846814f574e07e7d9072e70ad00192`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973ec878c950532925c0e2a1d397edf1086a25b91f4af6344e9b56a4dbb000c9`  
		Last Modified: Wed, 15 Dec 2021 19:42:24 GMT  
		Size: 6.9 MB (6932833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:a729cce205a05b0b86dc8dca87823efaffc3f74979fe7dc86a707c2fbf631b61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:b15efb5c932fd29acc764a2b8c0e6b1dfda4450f2a67d630c3b9f205785fdb2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68519144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15a9bc7c6340df2ac9d6c8196ca1d905180ddf2ca8b29a8d98f5422e2e5ccf85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 20:19:27 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 20:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:34 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 20:19:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 20:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:35 GMT
CMD ["sh"]
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
	-	`sha256:a3f2dd7b7d653d57dbfc55dcef38007cf7ae05a4c1a226f4465b3723cb2232ed`  
		Last Modified: Wed, 15 Dec 2021 20:20:32 GMT  
		Size: 63.7 MB (63718464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d182b62d4a3549bba88c6f8f32c2d7850ca927a7df0682d9a0de05d0c40095e2`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a57db2abd77c0b995c329d7812464e3734bc1af7b829bd1a42d461de77d3b7`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73490af52bd34939d0d8b02fe67c992943d062112c5a1cb41daf43146a25ae1b`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:17db01f277a58c2d70b2a40a8f46607c5319dd2f23c55dcf8c835cd25f7ff746
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62414023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4610f8d36c6766d145891417dd49f9b3e6535b43820bae79640d380fb88016b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 19:39:37 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 19:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 19:39:38 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 19:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 19:39:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 19:39:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:39:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 19:39:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 19:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 19:39:48 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1339a3be518a98fb1ef64708d14d86fd4039c4bb0a3d1db8c2d4a4c00fb8a2`  
		Last Modified: Wed, 15 Dec 2021 19:41:10 GMT  
		Size: 1.9 MB (1949540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353862b30dd70efe72e0bf55133d47f2a5b000e37f9cdb0e7e4a0178a5f076ec`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3190c06c4855888df747c4f505d0bc7aaecfbb0d9d4acaee685e28bddfb99b`  
		Last Modified: Wed, 15 Dec 2021 19:41:16 GMT  
		Size: 57.7 MB (57747213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e216c2ebb46ec0635d982e57890ab4c9025c95a940e79a81a0ed8b50c49b6`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46f33417cc9574bd0139314cc88909fae8f672527fc69f493d406dad1991e1`  
		Last Modified: Wed, 15 Dec 2021 19:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c99da1af64cbeec415a8ce2302a76874846814f574e07e7d9072e70ad00192`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore`

```console
$ docker pull docker@sha256:385c45deff3f6fd090ebbcaa19c2c4c7eb3ad8ee2e717b2cff3128b88154e116
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `docker:windowsservercore` - windows version 10.0.17763.2366; amd64

```console
$ docker pull docker@sha256:dda522f423b5f150997bb295498a0458b41f56ba7342754baffabaa57628cad4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2762195765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14c2d634d7d869aa8fd42835e537aa314d535b0c909a92cc26117284d1d84c9f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 18 Dec 2021 10:27:00 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 18 Dec 2021 10:27:01 GMT
ENV DOCKER_VERSION=20.10.12
# Sat, 18 Dec 2021 10:27:02 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.12.zip
# Sat, 18 Dec 2021 10:28:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd048ecae1fa585d9d38c625121cb1a8b3acb5c3d6413282e75b85193bfd151`  
		Last Modified: Sat, 18 Dec 2021 10:28:39 GMT  
		Size: 371.1 KB (371093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335bf6ad2e01acadc382163d2078d5e9a371ac3399fb5429befb22da359a6512`  
		Last Modified: Sat, 18 Dec 2021 10:28:38 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d37fa43c886f9824002edada19e4288dd79b3ca0048dccdbe1a4e1dcf1e850`  
		Last Modified: Sat, 18 Dec 2021 10:28:39 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280971e530a5c147ecc05e54d1dbb42f374f86e078c30f273150762f17ede482`  
		Last Modified: Sat, 18 Dec 2021 10:28:50 GMT  
		Size: 53.2 MB (53215955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:385c45deff3f6fd090ebbcaa19c2c4c7eb3ad8ee2e717b2cff3128b88154e116
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull docker@sha256:dda522f423b5f150997bb295498a0458b41f56ba7342754baffabaa57628cad4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2762195765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14c2d634d7d869aa8fd42835e537aa314d535b0c909a92cc26117284d1d84c9f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 18 Dec 2021 10:27:00 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 18 Dec 2021 10:27:01 GMT
ENV DOCKER_VERSION=20.10.12
# Sat, 18 Dec 2021 10:27:02 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.12.zip
# Sat, 18 Dec 2021 10:28:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd048ecae1fa585d9d38c625121cb1a8b3acb5c3d6413282e75b85193bfd151`  
		Last Modified: Sat, 18 Dec 2021 10:28:39 GMT  
		Size: 371.1 KB (371093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335bf6ad2e01acadc382163d2078d5e9a371ac3399fb5429befb22da359a6512`  
		Last Modified: Sat, 18 Dec 2021 10:28:38 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d37fa43c886f9824002edada19e4288dd79b3ca0048dccdbe1a4e1dcf1e850`  
		Last Modified: Sat, 18 Dec 2021 10:28:39 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280971e530a5c147ecc05e54d1dbb42f374f86e078c30f273150762f17ede482`  
		Last Modified: Sat, 18 Dec 2021 10:28:50 GMT  
		Size: 53.2 MB (53215955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0
