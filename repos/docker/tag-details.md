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
-	[`docker:20.10.8`](#docker20108)
-	[`docker:20.10.8-dind`](#docker20108-dind)
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

## `docker:19`

```console
$ docker pull docker@sha256:ea1f0761c92b600417ad14bc9b2b3a30abf8e96e94895fee6cbb5353316f30b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
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
$ docker pull docker@sha256:c85365ad08c7f6e02ac962a8759c4a5b8512ea5c294d3bb9ed25fca52e9e22e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
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
$ docker pull docker@sha256:5fbf776b8bb0e431ff612631fb058c5d8d82736d29fedf068d91f7487a2c3587
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
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
$ docker pull docker@sha256:ea1f0761c92b600417ad14bc9b2b3a30abf8e96e94895fee6cbb5353316f30b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
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
$ docker pull docker@sha256:c85365ad08c7f6e02ac962a8759c4a5b8512ea5c294d3bb9ed25fca52e9e22e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
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
$ docker pull docker@sha256:5fbf776b8bb0e431ff612631fb058c5d8d82736d29fedf068d91f7487a2c3587
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
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
$ docker pull docker@sha256:ddf0d732dcbc3e2087836e06e50cc97e21bfb002a49c7d0fe767f6c31e01d65f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20` - linux; amd64

```console
$ docker pull docker@sha256:c9fe80d9eb030d771811e9cefcf2e3cb73aad845c24eee8e29b72b4429fae283
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66536142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51453dcdd9bd51e503f75e6d42a4071469ad2ba816321781985041b6bc7776db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:20:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:20:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:20:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:20:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:43 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:20:44 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:20:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:44 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b94fafbd542a8c279f4a08e81fef317862b0fe3f604febe2fc2138886ba1d7`  
		Last Modified: Wed, 04 Aug 2021 21:21:53 GMT  
		Size: 2.4 MB (2438245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e3c9e6c132861fd24ac22906718bb610ebcf3912ade5e48a791ba8f85e5799`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc990f87bf12a7b8fb86c3003977468a14fb1a31e5bb0b500e8127ee4e6beb5`  
		Last Modified: Wed, 04 Aug 2021 21:22:03 GMT  
		Size: 61.3 MB (61284061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1436504743cc47a166b7964d591792b69e34aa1e3e07ef5d91f481fdb11f948d`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c526f01240b836e9645a2b2b629051c5e488d60b309d5f253adab7f2c45ed7`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d263b0ed3ea3116c812ca5c542c5175ccb0c99bee76b06db8c2340290057fa`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:202f4fd8f1bc62e516f42f1f32d205a6d9dc12a5eddf42be5adda612331f7d99
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.6 MB (60592580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:917aa76b39804498915883c81d9c3f4616dafbae602e0e81597852ab6905bc77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:40:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:40:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:40:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:40:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:40:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:41 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d668eead8965ee8f4a1cd65de2a1cde9c49cfd2c2f06ac2290e0b90724ba4ea3`  
		Last Modified: Wed, 04 Aug 2021 21:42:32 GMT  
		Size: 2.5 MB (2458333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7010a04da6233aa993b677900fe12554cb30e4b12adeee36a2c884d5c0ec8965`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c06e26407aeefb6fd4953cb12e19c70695281c4c9ab4e9b8120734669094a8a`  
		Last Modified: Wed, 04 Aug 2021 21:42:39 GMT  
		Size: 55.4 MB (55420354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e4b73ac390f4f52af96ffa7e98228c80619fa25bd61e862485f64b509a849`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627ac7844e75fc94ea8963915c871cb5e376af3631da0ce14bf5a5662813175f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be33fcd733ebf68f8983483238e2245237efdc7751c83d98e9ce9b6a0f3069f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind`

```console
$ docker pull docker@sha256:c0aac52a0f704627c01dfd5177f3d0e5d9bf6e64f2b8a2c35b5b5087ebe94cfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind` - linux; amd64

```console
$ docker pull docker@sha256:5a0822246a7ba7596160e5ebde39840d7631be4a30cd4133aec47625e87a69bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73065601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ede8a8017c85b24213ab65dc802ae2d0042d755d5c301d397e110381d5f50e3b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:20:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:20:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:20:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:20:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:43 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:20:44 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:20:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:44 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:20:50 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Aug 2021 21:20:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:20:51 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 04 Aug 2021 21:20:52 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Aug 2021 21:20:52 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:52 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Aug 2021 21:20:52 GMT
EXPOSE 2375 2376
# Wed, 04 Aug 2021 21:20:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:53 GMT
CMD []
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b94fafbd542a8c279f4a08e81fef317862b0fe3f604febe2fc2138886ba1d7`  
		Last Modified: Wed, 04 Aug 2021 21:21:53 GMT  
		Size: 2.4 MB (2438245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e3c9e6c132861fd24ac22906718bb610ebcf3912ade5e48a791ba8f85e5799`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc990f87bf12a7b8fb86c3003977468a14fb1a31e5bb0b500e8127ee4e6beb5`  
		Last Modified: Wed, 04 Aug 2021 21:22:03 GMT  
		Size: 61.3 MB (61284061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1436504743cc47a166b7964d591792b69e34aa1e3e07ef5d91f481fdb11f948d`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c526f01240b836e9645a2b2b629051c5e488d60b309d5f253adab7f2c45ed7`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d263b0ed3ea3116c812ca5c542c5175ccb0c99bee76b06db8c2340290057fa`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323e02cdc2f5b38baeff0de98fb35ef0d98c8eb6ee03c82bad90c145c7fe31a5`  
		Last Modified: Wed, 04 Aug 2021 21:22:21 GMT  
		Size: 6.5 MB (6524551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278c396f7286d8283a874d8792049d325633fac7e850531740d22f560c955187`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8ecf0198691794c5ecaa8389e5beef5e882d6cfec101c6a09dd9ace85ab594`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 979.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2662824727357b53a9d351903bfd330007c20c9576b971e2a06c0018226c6c3b`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:45667bb65fd02bf020846511c1f59ef9267e2c16439b60509dcf44794307f4f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67013251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:819e5b46b4c03a38c8296417bbbb73b3654addd89381b617d1ffd72887fdb7d2`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:40:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:40:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:40:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:40:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:40:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:41 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:40:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Aug 2021 21:40:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:40:50 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 04 Aug 2021 21:40:51 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Aug 2021 21:40:51 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:52 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Aug 2021 21:40:52 GMT
EXPOSE 2375 2376
# Wed, 04 Aug 2021 21:40:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:52 GMT
CMD []
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d668eead8965ee8f4a1cd65de2a1cde9c49cfd2c2f06ac2290e0b90724ba4ea3`  
		Last Modified: Wed, 04 Aug 2021 21:42:32 GMT  
		Size: 2.5 MB (2458333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7010a04da6233aa993b677900fe12554cb30e4b12adeee36a2c884d5c0ec8965`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c06e26407aeefb6fd4953cb12e19c70695281c4c9ab4e9b8120734669094a8a`  
		Last Modified: Wed, 04 Aug 2021 21:42:39 GMT  
		Size: 55.4 MB (55420354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e4b73ac390f4f52af96ffa7e98228c80619fa25bd61e862485f64b509a849`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627ac7844e75fc94ea8963915c871cb5e376af3631da0ce14bf5a5662813175f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be33fcd733ebf68f8983483238e2245237efdc7751c83d98e9ce9b6a0f3069f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7be703642618a8d45d2234fbab8868b1139a87c1d15e9ed461b84c174d6a50`  
		Last Modified: Wed, 04 Aug 2021 21:42:59 GMT  
		Size: 6.4 MB (6415768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d505b30c548b9339cb05141edaeeb535a1f6957a797abe632d52f98cc323a97`  
		Last Modified: Wed, 04 Aug 2021 21:42:58 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4a4ed41a0a4416dc51a066b9e02ee59d31136060b4b70de974046278cbaf0f`  
		Last Modified: Wed, 04 Aug 2021 21:42:59 GMT  
		Size: 975.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88540cd1423a8caeac6757a720ddc1be1455af90c51f8242cc0039ca1f5d3b37`  
		Last Modified: Wed, 04 Aug 2021 21:42:58 GMT  
		Size: 2.6 KB (2615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:963579745bca14f3cbd0d13ccc9b1909864e735d180c585ec47aa1f7d2257fd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:124b738e215234286634752adb38a03fca0b5f4d46c291a1f77a84b0383a1e5e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.3 MB (93315315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7347a3756263d56fd413c805bf0cb3bc52910009c4dbc12a4c8e84ba4359ffe6`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:20:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:20:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:20:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:20:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:43 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:20:44 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:20:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:44 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:20:50 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Aug 2021 21:20:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:20:51 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 04 Aug 2021 21:20:52 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Aug 2021 21:20:52 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:52 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Aug 2021 21:20:52 GMT
EXPOSE 2375 2376
# Wed, 04 Aug 2021 21:20:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:53 GMT
CMD []
# Wed, 04 Aug 2021 21:20:57 GMT
RUN apk add --no-cache iproute2
# Wed, 04 Aug 2021 21:20:58 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 04 Aug 2021 21:20:58 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:21:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 04 Aug 2021 21:21:01 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 04 Aug 2021 21:21:01 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 04 Aug 2021 21:21:01 GMT
USER rootless
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b94fafbd542a8c279f4a08e81fef317862b0fe3f604febe2fc2138886ba1d7`  
		Last Modified: Wed, 04 Aug 2021 21:21:53 GMT  
		Size: 2.4 MB (2438245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e3c9e6c132861fd24ac22906718bb610ebcf3912ade5e48a791ba8f85e5799`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc990f87bf12a7b8fb86c3003977468a14fb1a31e5bb0b500e8127ee4e6beb5`  
		Last Modified: Wed, 04 Aug 2021 21:22:03 GMT  
		Size: 61.3 MB (61284061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1436504743cc47a166b7964d591792b69e34aa1e3e07ef5d91f481fdb11f948d`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c526f01240b836e9645a2b2b629051c5e488d60b309d5f253adab7f2c45ed7`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d263b0ed3ea3116c812ca5c542c5175ccb0c99bee76b06db8c2340290057fa`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323e02cdc2f5b38baeff0de98fb35ef0d98c8eb6ee03c82bad90c145c7fe31a5`  
		Last Modified: Wed, 04 Aug 2021 21:22:21 GMT  
		Size: 6.5 MB (6524551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278c396f7286d8283a874d8792049d325633fac7e850531740d22f560c955187`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8ecf0198691794c5ecaa8389e5beef5e882d6cfec101c6a09dd9ace85ab594`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 979.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2662824727357b53a9d351903bfd330007c20c9576b971e2a06c0018226c6c3b`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e6256c33c0ede1adebf65b20431decf86e9ee5ee75bc5dafdc97323eb00b14`  
		Last Modified: Wed, 04 Aug 2021 21:22:39 GMT  
		Size: 1.1 MB (1131912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ee6cc75d0fb6ad7733a1aff3c28f0f3f7e0b2fab5a6a3834b15f4448fafd63`  
		Last Modified: Wed, 04 Aug 2021 21:22:39 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53de6cbf547b0318998261b99b7a0a30bd3fcde67956de7983df1b2328af358`  
		Last Modified: Wed, 04 Aug 2021 21:22:39 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956907e972957db3a2ae0b2ea1caad912dbfeb36651f885dd48cd155e666de43`  
		Last Modified: Wed, 04 Aug 2021 21:22:42 GMT  
		Size: 19.1 MB (19116096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39800d8bc1636f365b4faf120564b96243d4c0cb880f893e9b561a609f4758d1`  
		Last Modified: Wed, 04 Aug 2021 21:22:39 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8798010c693f3e0ab32e9c78938345734472925bde322d6eb50d015729da5738
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.3 MB (89262967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:796d21eeac11e41216052d96f3f42968c38bd60d22c93a28c08f5c8b0adb6510`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:40:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:40:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:40:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:40:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:40:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:41 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:40:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Aug 2021 21:40:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:40:50 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 04 Aug 2021 21:40:51 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Aug 2021 21:40:51 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:52 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Aug 2021 21:40:52 GMT
EXPOSE 2375 2376
# Wed, 04 Aug 2021 21:40:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:52 GMT
CMD []
# Wed, 04 Aug 2021 21:40:59 GMT
RUN apk add --no-cache iproute2
# Wed, 04 Aug 2021 21:41:00 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 04 Aug 2021 21:41:01 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:41:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 04 Aug 2021 21:41:04 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 04 Aug 2021 21:41:04 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 04 Aug 2021 21:41:04 GMT
USER rootless
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d668eead8965ee8f4a1cd65de2a1cde9c49cfd2c2f06ac2290e0b90724ba4ea3`  
		Last Modified: Wed, 04 Aug 2021 21:42:32 GMT  
		Size: 2.5 MB (2458333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7010a04da6233aa993b677900fe12554cb30e4b12adeee36a2c884d5c0ec8965`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c06e26407aeefb6fd4953cb12e19c70695281c4c9ab4e9b8120734669094a8a`  
		Last Modified: Wed, 04 Aug 2021 21:42:39 GMT  
		Size: 55.4 MB (55420354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e4b73ac390f4f52af96ffa7e98228c80619fa25bd61e862485f64b509a849`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627ac7844e75fc94ea8963915c871cb5e376af3631da0ce14bf5a5662813175f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be33fcd733ebf68f8983483238e2245237efdc7751c83d98e9ce9b6a0f3069f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7be703642618a8d45d2234fbab8868b1139a87c1d15e9ed461b84c174d6a50`  
		Last Modified: Wed, 04 Aug 2021 21:42:59 GMT  
		Size: 6.4 MB (6415768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d505b30c548b9339cb05141edaeeb535a1f6957a797abe632d52f98cc323a97`  
		Last Modified: Wed, 04 Aug 2021 21:42:58 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4a4ed41a0a4416dc51a066b9e02ee59d31136060b4b70de974046278cbaf0f`  
		Last Modified: Wed, 04 Aug 2021 21:42:59 GMT  
		Size: 975.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88540cd1423a8caeac6757a720ddc1be1455af90c51f8242cc0039ca1f5d3b37`  
		Last Modified: Wed, 04 Aug 2021 21:42:58 GMT  
		Size: 2.6 KB (2615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca55d719f285c206e9d9b9f065be06c1921f50cd25f3410d55d34ef73917dcb8`  
		Last Modified: Wed, 04 Aug 2021 21:43:19 GMT  
		Size: 1.2 MB (1153199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af474eb81075318d6a880fdd4d20b5cd59cb8953dc8bdd3e0abee2d3f098d6cc`  
		Last Modified: Wed, 04 Aug 2021 21:43:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8c6d1e64a80e62654c56d0e7179e03154215e4d3a994c2986a5df58e4058df`  
		Last Modified: Wed, 04 Aug 2021 21:43:18 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39408337edbf619576a8236fe50df4b7600b1a2a69ff501d52acad3a4f3b5a07`  
		Last Modified: Wed, 04 Aug 2021 21:43:24 GMT  
		Size: 21.1 MB (21094815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9ccbcf888a167c7709e18d6a5636d0b5b1e7dbc0f476ae4f25a78642e923e2`  
		Last Modified: Wed, 04 Aug 2021 21:43:18 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-git`

```console
$ docker pull docker@sha256:1da454342f3c7a35f8d75c6e867ab6afcf0aecacea2495e26f868d82ad5dd788
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-git` - linux; amd64

```console
$ docker pull docker@sha256:c43f2419d2b2e4177c5df924893b251d7ef6be98c157c885f22bce4ecbd10b8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72938677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fda6f821f6eee066c490f4c12941c8ea6069ccb3f5b2974718337ebd4f563e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:20:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:20:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:20:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:20:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:43 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:20:44 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:20:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:44 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:21:06 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b94fafbd542a8c279f4a08e81fef317862b0fe3f604febe2fc2138886ba1d7`  
		Last Modified: Wed, 04 Aug 2021 21:21:53 GMT  
		Size: 2.4 MB (2438245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e3c9e6c132861fd24ac22906718bb610ebcf3912ade5e48a791ba8f85e5799`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc990f87bf12a7b8fb86c3003977468a14fb1a31e5bb0b500e8127ee4e6beb5`  
		Last Modified: Wed, 04 Aug 2021 21:22:03 GMT  
		Size: 61.3 MB (61284061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1436504743cc47a166b7964d591792b69e34aa1e3e07ef5d91f481fdb11f948d`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c526f01240b836e9645a2b2b629051c5e488d60b309d5f253adab7f2c45ed7`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d263b0ed3ea3116c812ca5c542c5175ccb0c99bee76b06db8c2340290057fa`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9165592365f0af3016a817877513f46b501c0a526c4ba8ef6f74c57ddd35084c`  
		Last Modified: Wed, 04 Aug 2021 21:23:01 GMT  
		Size: 6.4 MB (6402535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:0701658b47dccbe63590f3113fb29e922d172cfcd2a8968c8cccd5b862b406da
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67080075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e61c00dc1afbaadf09353e28ba9e0de2ddcef8ef8ca38ece4221421b45a306d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:40:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:40:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:40:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:40:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:40:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:41 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:41:12 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d668eead8965ee8f4a1cd65de2a1cde9c49cfd2c2f06ac2290e0b90724ba4ea3`  
		Last Modified: Wed, 04 Aug 2021 21:42:32 GMT  
		Size: 2.5 MB (2458333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7010a04da6233aa993b677900fe12554cb30e4b12adeee36a2c884d5c0ec8965`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c06e26407aeefb6fd4953cb12e19c70695281c4c9ab4e9b8120734669094a8a`  
		Last Modified: Wed, 04 Aug 2021 21:42:39 GMT  
		Size: 55.4 MB (55420354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e4b73ac390f4f52af96ffa7e98228c80619fa25bd61e862485f64b509a849`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627ac7844e75fc94ea8963915c871cb5e376af3631da0ce14bf5a5662813175f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be33fcd733ebf68f8983483238e2245237efdc7751c83d98e9ce9b6a0f3069f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc643a0ffa7d7ae60054634b94e2ea6799be888df2ed22e2dd0d369753ba11e`  
		Last Modified: Wed, 04 Aug 2021 21:43:45 GMT  
		Size: 6.5 MB (6487495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore`

```console
$ docker pull docker@sha256:e23c1097f4422e0afd160973bdf739969e3f554176a203e74c9516e578f93eb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `docker:20-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull docker@sha256:861ad32b4aea6ebcafe15263de5392e2b96e68ae72982bbe6c3ee5842a392d2d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2736709359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45b8a1ae2c2bd7da22c9fb3204f2d1906f3d638f0a4fe37d7f63041107380a9e`
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
# Wed, 04 Aug 2021 21:14:18 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:14:21 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Wed, 04 Aug 2021 21:15:34 GMT
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
	-	`sha256:261da88a9739468f39a6c5afea5001a7636ff158c9f6d3c55c781c7a5e25f03d`  
		Last Modified: Wed, 04 Aug 2021 21:15:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65914705f95c4725772744ad7f2007bde657f07e7e22b9fdd99ceee0e321b00d`  
		Last Modified: Wed, 04 Aug 2021 21:15:58 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649fb723a4e40f18c7aafb9c9da6b3cf4745259262599aad41308db2de8ed8c8`  
		Last Modified: Wed, 04 Aug 2021 21:16:09 GMT  
		Size: 50.9 MB (50889139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-1809`

```console
$ docker pull docker@sha256:e23c1097f4422e0afd160973bdf739969e3f554176a203e74c9516e578f93eb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `docker:20-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull docker@sha256:861ad32b4aea6ebcafe15263de5392e2b96e68ae72982bbe6c3ee5842a392d2d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2736709359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45b8a1ae2c2bd7da22c9fb3204f2d1906f3d638f0a4fe37d7f63041107380a9e`
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
# Wed, 04 Aug 2021 21:14:18 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:14:21 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Wed, 04 Aug 2021 21:15:34 GMT
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
	-	`sha256:261da88a9739468f39a6c5afea5001a7636ff158c9f6d3c55c781c7a5e25f03d`  
		Last Modified: Wed, 04 Aug 2021 21:15:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65914705f95c4725772744ad7f2007bde657f07e7e22b9fdd99ceee0e321b00d`  
		Last Modified: Wed, 04 Aug 2021 21:15:58 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649fb723a4e40f18c7aafb9c9da6b3cf4745259262599aad41308db2de8ed8c8`  
		Last Modified: Wed, 04 Aug 2021 21:16:09 GMT  
		Size: 50.9 MB (50889139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10`

```console
$ docker pull docker@sha256:ddf0d732dcbc3e2087836e06e50cc97e21bfb002a49c7d0fe767f6c31e01d65f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10` - linux; amd64

```console
$ docker pull docker@sha256:c9fe80d9eb030d771811e9cefcf2e3cb73aad845c24eee8e29b72b4429fae283
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66536142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51453dcdd9bd51e503f75e6d42a4071469ad2ba816321781985041b6bc7776db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:20:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:20:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:20:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:20:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:43 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:20:44 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:20:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:44 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b94fafbd542a8c279f4a08e81fef317862b0fe3f604febe2fc2138886ba1d7`  
		Last Modified: Wed, 04 Aug 2021 21:21:53 GMT  
		Size: 2.4 MB (2438245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e3c9e6c132861fd24ac22906718bb610ebcf3912ade5e48a791ba8f85e5799`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc990f87bf12a7b8fb86c3003977468a14fb1a31e5bb0b500e8127ee4e6beb5`  
		Last Modified: Wed, 04 Aug 2021 21:22:03 GMT  
		Size: 61.3 MB (61284061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1436504743cc47a166b7964d591792b69e34aa1e3e07ef5d91f481fdb11f948d`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c526f01240b836e9645a2b2b629051c5e488d60b309d5f253adab7f2c45ed7`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d263b0ed3ea3116c812ca5c542c5175ccb0c99bee76b06db8c2340290057fa`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:202f4fd8f1bc62e516f42f1f32d205a6d9dc12a5eddf42be5adda612331f7d99
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.6 MB (60592580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:917aa76b39804498915883c81d9c3f4616dafbae602e0e81597852ab6905bc77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:40:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:40:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:40:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:40:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:40:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:41 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d668eead8965ee8f4a1cd65de2a1cde9c49cfd2c2f06ac2290e0b90724ba4ea3`  
		Last Modified: Wed, 04 Aug 2021 21:42:32 GMT  
		Size: 2.5 MB (2458333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7010a04da6233aa993b677900fe12554cb30e4b12adeee36a2c884d5c0ec8965`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c06e26407aeefb6fd4953cb12e19c70695281c4c9ab4e9b8120734669094a8a`  
		Last Modified: Wed, 04 Aug 2021 21:42:39 GMT  
		Size: 55.4 MB (55420354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e4b73ac390f4f52af96ffa7e98228c80619fa25bd61e862485f64b509a849`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627ac7844e75fc94ea8963915c871cb5e376af3631da0ce14bf5a5662813175f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be33fcd733ebf68f8983483238e2245237efdc7751c83d98e9ce9b6a0f3069f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind`

```console
$ docker pull docker@sha256:c0aac52a0f704627c01dfd5177f3d0e5d9bf6e64f2b8a2c35b5b5087ebe94cfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind` - linux; amd64

```console
$ docker pull docker@sha256:5a0822246a7ba7596160e5ebde39840d7631be4a30cd4133aec47625e87a69bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73065601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ede8a8017c85b24213ab65dc802ae2d0042d755d5c301d397e110381d5f50e3b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:20:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:20:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:20:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:20:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:43 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:20:44 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:20:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:44 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:20:50 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Aug 2021 21:20:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:20:51 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 04 Aug 2021 21:20:52 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Aug 2021 21:20:52 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:52 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Aug 2021 21:20:52 GMT
EXPOSE 2375 2376
# Wed, 04 Aug 2021 21:20:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:53 GMT
CMD []
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b94fafbd542a8c279f4a08e81fef317862b0fe3f604febe2fc2138886ba1d7`  
		Last Modified: Wed, 04 Aug 2021 21:21:53 GMT  
		Size: 2.4 MB (2438245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e3c9e6c132861fd24ac22906718bb610ebcf3912ade5e48a791ba8f85e5799`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc990f87bf12a7b8fb86c3003977468a14fb1a31e5bb0b500e8127ee4e6beb5`  
		Last Modified: Wed, 04 Aug 2021 21:22:03 GMT  
		Size: 61.3 MB (61284061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1436504743cc47a166b7964d591792b69e34aa1e3e07ef5d91f481fdb11f948d`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c526f01240b836e9645a2b2b629051c5e488d60b309d5f253adab7f2c45ed7`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d263b0ed3ea3116c812ca5c542c5175ccb0c99bee76b06db8c2340290057fa`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323e02cdc2f5b38baeff0de98fb35ef0d98c8eb6ee03c82bad90c145c7fe31a5`  
		Last Modified: Wed, 04 Aug 2021 21:22:21 GMT  
		Size: 6.5 MB (6524551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278c396f7286d8283a874d8792049d325633fac7e850531740d22f560c955187`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8ecf0198691794c5ecaa8389e5beef5e882d6cfec101c6a09dd9ace85ab594`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 979.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2662824727357b53a9d351903bfd330007c20c9576b971e2a06c0018226c6c3b`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:45667bb65fd02bf020846511c1f59ef9267e2c16439b60509dcf44794307f4f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67013251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:819e5b46b4c03a38c8296417bbbb73b3654addd89381b617d1ffd72887fdb7d2`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:40:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:40:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:40:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:40:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:40:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:41 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:40:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Aug 2021 21:40:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:40:50 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 04 Aug 2021 21:40:51 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Aug 2021 21:40:51 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:52 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Aug 2021 21:40:52 GMT
EXPOSE 2375 2376
# Wed, 04 Aug 2021 21:40:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:52 GMT
CMD []
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d668eead8965ee8f4a1cd65de2a1cde9c49cfd2c2f06ac2290e0b90724ba4ea3`  
		Last Modified: Wed, 04 Aug 2021 21:42:32 GMT  
		Size: 2.5 MB (2458333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7010a04da6233aa993b677900fe12554cb30e4b12adeee36a2c884d5c0ec8965`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c06e26407aeefb6fd4953cb12e19c70695281c4c9ab4e9b8120734669094a8a`  
		Last Modified: Wed, 04 Aug 2021 21:42:39 GMT  
		Size: 55.4 MB (55420354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e4b73ac390f4f52af96ffa7e98228c80619fa25bd61e862485f64b509a849`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627ac7844e75fc94ea8963915c871cb5e376af3631da0ce14bf5a5662813175f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be33fcd733ebf68f8983483238e2245237efdc7751c83d98e9ce9b6a0f3069f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7be703642618a8d45d2234fbab8868b1139a87c1d15e9ed461b84c174d6a50`  
		Last Modified: Wed, 04 Aug 2021 21:42:59 GMT  
		Size: 6.4 MB (6415768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d505b30c548b9339cb05141edaeeb535a1f6957a797abe632d52f98cc323a97`  
		Last Modified: Wed, 04 Aug 2021 21:42:58 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4a4ed41a0a4416dc51a066b9e02ee59d31136060b4b70de974046278cbaf0f`  
		Last Modified: Wed, 04 Aug 2021 21:42:59 GMT  
		Size: 975.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88540cd1423a8caeac6757a720ddc1be1455af90c51f8242cc0039ca1f5d3b37`  
		Last Modified: Wed, 04 Aug 2021 21:42:58 GMT  
		Size: 2.6 KB (2615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind-rootless`

```console
$ docker pull docker@sha256:963579745bca14f3cbd0d13ccc9b1909864e735d180c585ec47aa1f7d2257fd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:124b738e215234286634752adb38a03fca0b5f4d46c291a1f77a84b0383a1e5e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.3 MB (93315315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7347a3756263d56fd413c805bf0cb3bc52910009c4dbc12a4c8e84ba4359ffe6`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:20:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:20:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:20:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:20:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:43 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:20:44 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:20:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:44 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:20:50 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Aug 2021 21:20:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:20:51 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 04 Aug 2021 21:20:52 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Aug 2021 21:20:52 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:52 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Aug 2021 21:20:52 GMT
EXPOSE 2375 2376
# Wed, 04 Aug 2021 21:20:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:53 GMT
CMD []
# Wed, 04 Aug 2021 21:20:57 GMT
RUN apk add --no-cache iproute2
# Wed, 04 Aug 2021 21:20:58 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 04 Aug 2021 21:20:58 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:21:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 04 Aug 2021 21:21:01 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 04 Aug 2021 21:21:01 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 04 Aug 2021 21:21:01 GMT
USER rootless
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b94fafbd542a8c279f4a08e81fef317862b0fe3f604febe2fc2138886ba1d7`  
		Last Modified: Wed, 04 Aug 2021 21:21:53 GMT  
		Size: 2.4 MB (2438245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e3c9e6c132861fd24ac22906718bb610ebcf3912ade5e48a791ba8f85e5799`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc990f87bf12a7b8fb86c3003977468a14fb1a31e5bb0b500e8127ee4e6beb5`  
		Last Modified: Wed, 04 Aug 2021 21:22:03 GMT  
		Size: 61.3 MB (61284061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1436504743cc47a166b7964d591792b69e34aa1e3e07ef5d91f481fdb11f948d`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c526f01240b836e9645a2b2b629051c5e488d60b309d5f253adab7f2c45ed7`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d263b0ed3ea3116c812ca5c542c5175ccb0c99bee76b06db8c2340290057fa`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323e02cdc2f5b38baeff0de98fb35ef0d98c8eb6ee03c82bad90c145c7fe31a5`  
		Last Modified: Wed, 04 Aug 2021 21:22:21 GMT  
		Size: 6.5 MB (6524551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278c396f7286d8283a874d8792049d325633fac7e850531740d22f560c955187`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8ecf0198691794c5ecaa8389e5beef5e882d6cfec101c6a09dd9ace85ab594`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 979.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2662824727357b53a9d351903bfd330007c20c9576b971e2a06c0018226c6c3b`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e6256c33c0ede1adebf65b20431decf86e9ee5ee75bc5dafdc97323eb00b14`  
		Last Modified: Wed, 04 Aug 2021 21:22:39 GMT  
		Size: 1.1 MB (1131912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ee6cc75d0fb6ad7733a1aff3c28f0f3f7e0b2fab5a6a3834b15f4448fafd63`  
		Last Modified: Wed, 04 Aug 2021 21:22:39 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53de6cbf547b0318998261b99b7a0a30bd3fcde67956de7983df1b2328af358`  
		Last Modified: Wed, 04 Aug 2021 21:22:39 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956907e972957db3a2ae0b2ea1caad912dbfeb36651f885dd48cd155e666de43`  
		Last Modified: Wed, 04 Aug 2021 21:22:42 GMT  
		Size: 19.1 MB (19116096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39800d8bc1636f365b4faf120564b96243d4c0cb880f893e9b561a609f4758d1`  
		Last Modified: Wed, 04 Aug 2021 21:22:39 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8798010c693f3e0ab32e9c78938345734472925bde322d6eb50d015729da5738
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.3 MB (89262967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:796d21eeac11e41216052d96f3f42968c38bd60d22c93a28c08f5c8b0adb6510`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:40:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:40:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:40:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:40:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:40:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:41 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:40:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Aug 2021 21:40:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:40:50 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 04 Aug 2021 21:40:51 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Aug 2021 21:40:51 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:52 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Aug 2021 21:40:52 GMT
EXPOSE 2375 2376
# Wed, 04 Aug 2021 21:40:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:52 GMT
CMD []
# Wed, 04 Aug 2021 21:40:59 GMT
RUN apk add --no-cache iproute2
# Wed, 04 Aug 2021 21:41:00 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 04 Aug 2021 21:41:01 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:41:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 04 Aug 2021 21:41:04 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 04 Aug 2021 21:41:04 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 04 Aug 2021 21:41:04 GMT
USER rootless
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d668eead8965ee8f4a1cd65de2a1cde9c49cfd2c2f06ac2290e0b90724ba4ea3`  
		Last Modified: Wed, 04 Aug 2021 21:42:32 GMT  
		Size: 2.5 MB (2458333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7010a04da6233aa993b677900fe12554cb30e4b12adeee36a2c884d5c0ec8965`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c06e26407aeefb6fd4953cb12e19c70695281c4c9ab4e9b8120734669094a8a`  
		Last Modified: Wed, 04 Aug 2021 21:42:39 GMT  
		Size: 55.4 MB (55420354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e4b73ac390f4f52af96ffa7e98228c80619fa25bd61e862485f64b509a849`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627ac7844e75fc94ea8963915c871cb5e376af3631da0ce14bf5a5662813175f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be33fcd733ebf68f8983483238e2245237efdc7751c83d98e9ce9b6a0f3069f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7be703642618a8d45d2234fbab8868b1139a87c1d15e9ed461b84c174d6a50`  
		Last Modified: Wed, 04 Aug 2021 21:42:59 GMT  
		Size: 6.4 MB (6415768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d505b30c548b9339cb05141edaeeb535a1f6957a797abe632d52f98cc323a97`  
		Last Modified: Wed, 04 Aug 2021 21:42:58 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4a4ed41a0a4416dc51a066b9e02ee59d31136060b4b70de974046278cbaf0f`  
		Last Modified: Wed, 04 Aug 2021 21:42:59 GMT  
		Size: 975.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88540cd1423a8caeac6757a720ddc1be1455af90c51f8242cc0039ca1f5d3b37`  
		Last Modified: Wed, 04 Aug 2021 21:42:58 GMT  
		Size: 2.6 KB (2615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca55d719f285c206e9d9b9f065be06c1921f50cd25f3410d55d34ef73917dcb8`  
		Last Modified: Wed, 04 Aug 2021 21:43:19 GMT  
		Size: 1.2 MB (1153199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af474eb81075318d6a880fdd4d20b5cd59cb8953dc8bdd3e0abee2d3f098d6cc`  
		Last Modified: Wed, 04 Aug 2021 21:43:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8c6d1e64a80e62654c56d0e7179e03154215e4d3a994c2986a5df58e4058df`  
		Last Modified: Wed, 04 Aug 2021 21:43:18 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39408337edbf619576a8236fe50df4b7600b1a2a69ff501d52acad3a4f3b5a07`  
		Last Modified: Wed, 04 Aug 2021 21:43:24 GMT  
		Size: 21.1 MB (21094815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9ccbcf888a167c7709e18d6a5636d0b5b1e7dbc0f476ae4f25a78642e923e2`  
		Last Modified: Wed, 04 Aug 2021 21:43:18 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-git`

```console
$ docker pull docker@sha256:1da454342f3c7a35f8d75c6e867ab6afcf0aecacea2495e26f868d82ad5dd788
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-git` - linux; amd64

```console
$ docker pull docker@sha256:c43f2419d2b2e4177c5df924893b251d7ef6be98c157c885f22bce4ecbd10b8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72938677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fda6f821f6eee066c490f4c12941c8ea6069ccb3f5b2974718337ebd4f563e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:20:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:20:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:20:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:20:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:43 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:20:44 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:20:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:44 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:21:06 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b94fafbd542a8c279f4a08e81fef317862b0fe3f604febe2fc2138886ba1d7`  
		Last Modified: Wed, 04 Aug 2021 21:21:53 GMT  
		Size: 2.4 MB (2438245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e3c9e6c132861fd24ac22906718bb610ebcf3912ade5e48a791ba8f85e5799`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc990f87bf12a7b8fb86c3003977468a14fb1a31e5bb0b500e8127ee4e6beb5`  
		Last Modified: Wed, 04 Aug 2021 21:22:03 GMT  
		Size: 61.3 MB (61284061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1436504743cc47a166b7964d591792b69e34aa1e3e07ef5d91f481fdb11f948d`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c526f01240b836e9645a2b2b629051c5e488d60b309d5f253adab7f2c45ed7`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d263b0ed3ea3116c812ca5c542c5175ccb0c99bee76b06db8c2340290057fa`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9165592365f0af3016a817877513f46b501c0a526c4ba8ef6f74c57ddd35084c`  
		Last Modified: Wed, 04 Aug 2021 21:23:01 GMT  
		Size: 6.4 MB (6402535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:0701658b47dccbe63590f3113fb29e922d172cfcd2a8968c8cccd5b862b406da
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67080075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e61c00dc1afbaadf09353e28ba9e0de2ddcef8ef8ca38ece4221421b45a306d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:40:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:40:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:40:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:40:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:40:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:41 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:41:12 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d668eead8965ee8f4a1cd65de2a1cde9c49cfd2c2f06ac2290e0b90724ba4ea3`  
		Last Modified: Wed, 04 Aug 2021 21:42:32 GMT  
		Size: 2.5 MB (2458333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7010a04da6233aa993b677900fe12554cb30e4b12adeee36a2c884d5c0ec8965`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c06e26407aeefb6fd4953cb12e19c70695281c4c9ab4e9b8120734669094a8a`  
		Last Modified: Wed, 04 Aug 2021 21:42:39 GMT  
		Size: 55.4 MB (55420354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e4b73ac390f4f52af96ffa7e98228c80619fa25bd61e862485f64b509a849`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627ac7844e75fc94ea8963915c871cb5e376af3631da0ce14bf5a5662813175f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be33fcd733ebf68f8983483238e2245237efdc7751c83d98e9ce9b6a0f3069f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc643a0ffa7d7ae60054634b94e2ea6799be888df2ed22e2dd0d369753ba11e`  
		Last Modified: Wed, 04 Aug 2021 21:43:45 GMT  
		Size: 6.5 MB (6487495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore`

```console
$ docker pull docker@sha256:e23c1097f4422e0afd160973bdf739969e3f554176a203e74c9516e578f93eb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `docker:20.10-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull docker@sha256:861ad32b4aea6ebcafe15263de5392e2b96e68ae72982bbe6c3ee5842a392d2d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2736709359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45b8a1ae2c2bd7da22c9fb3204f2d1906f3d638f0a4fe37d7f63041107380a9e`
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
# Wed, 04 Aug 2021 21:14:18 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:14:21 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Wed, 04 Aug 2021 21:15:34 GMT
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
	-	`sha256:261da88a9739468f39a6c5afea5001a7636ff158c9f6d3c55c781c7a5e25f03d`  
		Last Modified: Wed, 04 Aug 2021 21:15:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65914705f95c4725772744ad7f2007bde657f07e7e22b9fdd99ceee0e321b00d`  
		Last Modified: Wed, 04 Aug 2021 21:15:58 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649fb723a4e40f18c7aafb9c9da6b3cf4745259262599aad41308db2de8ed8c8`  
		Last Modified: Wed, 04 Aug 2021 21:16:09 GMT  
		Size: 50.9 MB (50889139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-1809`

```console
$ docker pull docker@sha256:e23c1097f4422e0afd160973bdf739969e3f554176a203e74c9516e578f93eb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `docker:20.10-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull docker@sha256:861ad32b4aea6ebcafe15263de5392e2b96e68ae72982bbe6c3ee5842a392d2d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2736709359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45b8a1ae2c2bd7da22c9fb3204f2d1906f3d638f0a4fe37d7f63041107380a9e`
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
# Wed, 04 Aug 2021 21:14:18 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:14:21 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Wed, 04 Aug 2021 21:15:34 GMT
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
	-	`sha256:261da88a9739468f39a6c5afea5001a7636ff158c9f6d3c55c781c7a5e25f03d`  
		Last Modified: Wed, 04 Aug 2021 21:15:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65914705f95c4725772744ad7f2007bde657f07e7e22b9fdd99ceee0e321b00d`  
		Last Modified: Wed, 04 Aug 2021 21:15:58 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649fb723a4e40f18c7aafb9c9da6b3cf4745259262599aad41308db2de8ed8c8`  
		Last Modified: Wed, 04 Aug 2021 21:16:09 GMT  
		Size: 50.9 MB (50889139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8`

```console
$ docker pull docker@sha256:ddf0d732dcbc3e2087836e06e50cc97e21bfb002a49c7d0fe767f6c31e01d65f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.8` - linux; amd64

```console
$ docker pull docker@sha256:c9fe80d9eb030d771811e9cefcf2e3cb73aad845c24eee8e29b72b4429fae283
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66536142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51453dcdd9bd51e503f75e6d42a4071469ad2ba816321781985041b6bc7776db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:20:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:20:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:20:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:20:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:43 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:20:44 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:20:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:44 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b94fafbd542a8c279f4a08e81fef317862b0fe3f604febe2fc2138886ba1d7`  
		Last Modified: Wed, 04 Aug 2021 21:21:53 GMT  
		Size: 2.4 MB (2438245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e3c9e6c132861fd24ac22906718bb610ebcf3912ade5e48a791ba8f85e5799`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc990f87bf12a7b8fb86c3003977468a14fb1a31e5bb0b500e8127ee4e6beb5`  
		Last Modified: Wed, 04 Aug 2021 21:22:03 GMT  
		Size: 61.3 MB (61284061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1436504743cc47a166b7964d591792b69e34aa1e3e07ef5d91f481fdb11f948d`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c526f01240b836e9645a2b2b629051c5e488d60b309d5f253adab7f2c45ed7`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d263b0ed3ea3116c812ca5c542c5175ccb0c99bee76b06db8c2340290057fa`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.8` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:202f4fd8f1bc62e516f42f1f32d205a6d9dc12a5eddf42be5adda612331f7d99
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.6 MB (60592580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:917aa76b39804498915883c81d9c3f4616dafbae602e0e81597852ab6905bc77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:40:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:40:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:40:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:40:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:40:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:41 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d668eead8965ee8f4a1cd65de2a1cde9c49cfd2c2f06ac2290e0b90724ba4ea3`  
		Last Modified: Wed, 04 Aug 2021 21:42:32 GMT  
		Size: 2.5 MB (2458333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7010a04da6233aa993b677900fe12554cb30e4b12adeee36a2c884d5c0ec8965`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c06e26407aeefb6fd4953cb12e19c70695281c4c9ab4e9b8120734669094a8a`  
		Last Modified: Wed, 04 Aug 2021 21:42:39 GMT  
		Size: 55.4 MB (55420354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e4b73ac390f4f52af96ffa7e98228c80619fa25bd61e862485f64b509a849`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627ac7844e75fc94ea8963915c871cb5e376af3631da0ce14bf5a5662813175f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be33fcd733ebf68f8983483238e2245237efdc7751c83d98e9ce9b6a0f3069f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8-dind`

```console
$ docker pull docker@sha256:c0aac52a0f704627c01dfd5177f3d0e5d9bf6e64f2b8a2c35b5b5087ebe94cfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.8-dind` - linux; amd64

```console
$ docker pull docker@sha256:5a0822246a7ba7596160e5ebde39840d7631be4a30cd4133aec47625e87a69bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73065601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ede8a8017c85b24213ab65dc802ae2d0042d755d5c301d397e110381d5f50e3b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:20:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:20:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:20:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:20:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:43 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:20:44 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:20:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:44 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:20:50 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Aug 2021 21:20:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:20:51 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 04 Aug 2021 21:20:52 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Aug 2021 21:20:52 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:52 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Aug 2021 21:20:52 GMT
EXPOSE 2375 2376
# Wed, 04 Aug 2021 21:20:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:53 GMT
CMD []
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b94fafbd542a8c279f4a08e81fef317862b0fe3f604febe2fc2138886ba1d7`  
		Last Modified: Wed, 04 Aug 2021 21:21:53 GMT  
		Size: 2.4 MB (2438245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e3c9e6c132861fd24ac22906718bb610ebcf3912ade5e48a791ba8f85e5799`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc990f87bf12a7b8fb86c3003977468a14fb1a31e5bb0b500e8127ee4e6beb5`  
		Last Modified: Wed, 04 Aug 2021 21:22:03 GMT  
		Size: 61.3 MB (61284061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1436504743cc47a166b7964d591792b69e34aa1e3e07ef5d91f481fdb11f948d`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c526f01240b836e9645a2b2b629051c5e488d60b309d5f253adab7f2c45ed7`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d263b0ed3ea3116c812ca5c542c5175ccb0c99bee76b06db8c2340290057fa`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323e02cdc2f5b38baeff0de98fb35ef0d98c8eb6ee03c82bad90c145c7fe31a5`  
		Last Modified: Wed, 04 Aug 2021 21:22:21 GMT  
		Size: 6.5 MB (6524551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278c396f7286d8283a874d8792049d325633fac7e850531740d22f560c955187`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8ecf0198691794c5ecaa8389e5beef5e882d6cfec101c6a09dd9ace85ab594`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 979.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2662824727357b53a9d351903bfd330007c20c9576b971e2a06c0018226c6c3b`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.8-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:45667bb65fd02bf020846511c1f59ef9267e2c16439b60509dcf44794307f4f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67013251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:819e5b46b4c03a38c8296417bbbb73b3654addd89381b617d1ffd72887fdb7d2`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:40:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:40:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:40:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:40:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:40:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:41 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:40:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Aug 2021 21:40:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:40:50 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 04 Aug 2021 21:40:51 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Aug 2021 21:40:51 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:52 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Aug 2021 21:40:52 GMT
EXPOSE 2375 2376
# Wed, 04 Aug 2021 21:40:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:52 GMT
CMD []
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d668eead8965ee8f4a1cd65de2a1cde9c49cfd2c2f06ac2290e0b90724ba4ea3`  
		Last Modified: Wed, 04 Aug 2021 21:42:32 GMT  
		Size: 2.5 MB (2458333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7010a04da6233aa993b677900fe12554cb30e4b12adeee36a2c884d5c0ec8965`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c06e26407aeefb6fd4953cb12e19c70695281c4c9ab4e9b8120734669094a8a`  
		Last Modified: Wed, 04 Aug 2021 21:42:39 GMT  
		Size: 55.4 MB (55420354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e4b73ac390f4f52af96ffa7e98228c80619fa25bd61e862485f64b509a849`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627ac7844e75fc94ea8963915c871cb5e376af3631da0ce14bf5a5662813175f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be33fcd733ebf68f8983483238e2245237efdc7751c83d98e9ce9b6a0f3069f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7be703642618a8d45d2234fbab8868b1139a87c1d15e9ed461b84c174d6a50`  
		Last Modified: Wed, 04 Aug 2021 21:42:59 GMT  
		Size: 6.4 MB (6415768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d505b30c548b9339cb05141edaeeb535a1f6957a797abe632d52f98cc323a97`  
		Last Modified: Wed, 04 Aug 2021 21:42:58 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4a4ed41a0a4416dc51a066b9e02ee59d31136060b4b70de974046278cbaf0f`  
		Last Modified: Wed, 04 Aug 2021 21:42:59 GMT  
		Size: 975.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88540cd1423a8caeac6757a720ddc1be1455af90c51f8242cc0039ca1f5d3b37`  
		Last Modified: Wed, 04 Aug 2021 21:42:58 GMT  
		Size: 2.6 KB (2615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8-dind-rootless`

```console
$ docker pull docker@sha256:963579745bca14f3cbd0d13ccc9b1909864e735d180c585ec47aa1f7d2257fd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.8-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:124b738e215234286634752adb38a03fca0b5f4d46c291a1f77a84b0383a1e5e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.3 MB (93315315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7347a3756263d56fd413c805bf0cb3bc52910009c4dbc12a4c8e84ba4359ffe6`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:20:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:20:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:20:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:20:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:43 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:20:44 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:20:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:44 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:20:50 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Aug 2021 21:20:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:20:51 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 04 Aug 2021 21:20:52 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Aug 2021 21:20:52 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:52 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Aug 2021 21:20:52 GMT
EXPOSE 2375 2376
# Wed, 04 Aug 2021 21:20:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:53 GMT
CMD []
# Wed, 04 Aug 2021 21:20:57 GMT
RUN apk add --no-cache iproute2
# Wed, 04 Aug 2021 21:20:58 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 04 Aug 2021 21:20:58 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:21:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 04 Aug 2021 21:21:01 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 04 Aug 2021 21:21:01 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 04 Aug 2021 21:21:01 GMT
USER rootless
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b94fafbd542a8c279f4a08e81fef317862b0fe3f604febe2fc2138886ba1d7`  
		Last Modified: Wed, 04 Aug 2021 21:21:53 GMT  
		Size: 2.4 MB (2438245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e3c9e6c132861fd24ac22906718bb610ebcf3912ade5e48a791ba8f85e5799`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc990f87bf12a7b8fb86c3003977468a14fb1a31e5bb0b500e8127ee4e6beb5`  
		Last Modified: Wed, 04 Aug 2021 21:22:03 GMT  
		Size: 61.3 MB (61284061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1436504743cc47a166b7964d591792b69e34aa1e3e07ef5d91f481fdb11f948d`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c526f01240b836e9645a2b2b629051c5e488d60b309d5f253adab7f2c45ed7`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d263b0ed3ea3116c812ca5c542c5175ccb0c99bee76b06db8c2340290057fa`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323e02cdc2f5b38baeff0de98fb35ef0d98c8eb6ee03c82bad90c145c7fe31a5`  
		Last Modified: Wed, 04 Aug 2021 21:22:21 GMT  
		Size: 6.5 MB (6524551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278c396f7286d8283a874d8792049d325633fac7e850531740d22f560c955187`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8ecf0198691794c5ecaa8389e5beef5e882d6cfec101c6a09dd9ace85ab594`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 979.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2662824727357b53a9d351903bfd330007c20c9576b971e2a06c0018226c6c3b`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e6256c33c0ede1adebf65b20431decf86e9ee5ee75bc5dafdc97323eb00b14`  
		Last Modified: Wed, 04 Aug 2021 21:22:39 GMT  
		Size: 1.1 MB (1131912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ee6cc75d0fb6ad7733a1aff3c28f0f3f7e0b2fab5a6a3834b15f4448fafd63`  
		Last Modified: Wed, 04 Aug 2021 21:22:39 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53de6cbf547b0318998261b99b7a0a30bd3fcde67956de7983df1b2328af358`  
		Last Modified: Wed, 04 Aug 2021 21:22:39 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956907e972957db3a2ae0b2ea1caad912dbfeb36651f885dd48cd155e666de43`  
		Last Modified: Wed, 04 Aug 2021 21:22:42 GMT  
		Size: 19.1 MB (19116096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39800d8bc1636f365b4faf120564b96243d4c0cb880f893e9b561a609f4758d1`  
		Last Modified: Wed, 04 Aug 2021 21:22:39 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.8-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8798010c693f3e0ab32e9c78938345734472925bde322d6eb50d015729da5738
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.3 MB (89262967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:796d21eeac11e41216052d96f3f42968c38bd60d22c93a28c08f5c8b0adb6510`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:40:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:40:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:40:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:40:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:40:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:41 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:40:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Aug 2021 21:40:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:40:50 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 04 Aug 2021 21:40:51 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Aug 2021 21:40:51 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:52 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Aug 2021 21:40:52 GMT
EXPOSE 2375 2376
# Wed, 04 Aug 2021 21:40:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:52 GMT
CMD []
# Wed, 04 Aug 2021 21:40:59 GMT
RUN apk add --no-cache iproute2
# Wed, 04 Aug 2021 21:41:00 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 04 Aug 2021 21:41:01 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:41:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 04 Aug 2021 21:41:04 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 04 Aug 2021 21:41:04 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 04 Aug 2021 21:41:04 GMT
USER rootless
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d668eead8965ee8f4a1cd65de2a1cde9c49cfd2c2f06ac2290e0b90724ba4ea3`  
		Last Modified: Wed, 04 Aug 2021 21:42:32 GMT  
		Size: 2.5 MB (2458333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7010a04da6233aa993b677900fe12554cb30e4b12adeee36a2c884d5c0ec8965`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c06e26407aeefb6fd4953cb12e19c70695281c4c9ab4e9b8120734669094a8a`  
		Last Modified: Wed, 04 Aug 2021 21:42:39 GMT  
		Size: 55.4 MB (55420354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e4b73ac390f4f52af96ffa7e98228c80619fa25bd61e862485f64b509a849`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627ac7844e75fc94ea8963915c871cb5e376af3631da0ce14bf5a5662813175f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be33fcd733ebf68f8983483238e2245237efdc7751c83d98e9ce9b6a0f3069f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7be703642618a8d45d2234fbab8868b1139a87c1d15e9ed461b84c174d6a50`  
		Last Modified: Wed, 04 Aug 2021 21:42:59 GMT  
		Size: 6.4 MB (6415768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d505b30c548b9339cb05141edaeeb535a1f6957a797abe632d52f98cc323a97`  
		Last Modified: Wed, 04 Aug 2021 21:42:58 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4a4ed41a0a4416dc51a066b9e02ee59d31136060b4b70de974046278cbaf0f`  
		Last Modified: Wed, 04 Aug 2021 21:42:59 GMT  
		Size: 975.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88540cd1423a8caeac6757a720ddc1be1455af90c51f8242cc0039ca1f5d3b37`  
		Last Modified: Wed, 04 Aug 2021 21:42:58 GMT  
		Size: 2.6 KB (2615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca55d719f285c206e9d9b9f065be06c1921f50cd25f3410d55d34ef73917dcb8`  
		Last Modified: Wed, 04 Aug 2021 21:43:19 GMT  
		Size: 1.2 MB (1153199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af474eb81075318d6a880fdd4d20b5cd59cb8953dc8bdd3e0abee2d3f098d6cc`  
		Last Modified: Wed, 04 Aug 2021 21:43:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8c6d1e64a80e62654c56d0e7179e03154215e4d3a994c2986a5df58e4058df`  
		Last Modified: Wed, 04 Aug 2021 21:43:18 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39408337edbf619576a8236fe50df4b7600b1a2a69ff501d52acad3a4f3b5a07`  
		Last Modified: Wed, 04 Aug 2021 21:43:24 GMT  
		Size: 21.1 MB (21094815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9ccbcf888a167c7709e18d6a5636d0b5b1e7dbc0f476ae4f25a78642e923e2`  
		Last Modified: Wed, 04 Aug 2021 21:43:18 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8-git`

```console
$ docker pull docker@sha256:1da454342f3c7a35f8d75c6e867ab6afcf0aecacea2495e26f868d82ad5dd788
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.8-git` - linux; amd64

```console
$ docker pull docker@sha256:c43f2419d2b2e4177c5df924893b251d7ef6be98c157c885f22bce4ecbd10b8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72938677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fda6f821f6eee066c490f4c12941c8ea6069ccb3f5b2974718337ebd4f563e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:20:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:20:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:20:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:20:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:43 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:20:44 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:20:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:44 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:21:06 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b94fafbd542a8c279f4a08e81fef317862b0fe3f604febe2fc2138886ba1d7`  
		Last Modified: Wed, 04 Aug 2021 21:21:53 GMT  
		Size: 2.4 MB (2438245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e3c9e6c132861fd24ac22906718bb610ebcf3912ade5e48a791ba8f85e5799`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc990f87bf12a7b8fb86c3003977468a14fb1a31e5bb0b500e8127ee4e6beb5`  
		Last Modified: Wed, 04 Aug 2021 21:22:03 GMT  
		Size: 61.3 MB (61284061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1436504743cc47a166b7964d591792b69e34aa1e3e07ef5d91f481fdb11f948d`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c526f01240b836e9645a2b2b629051c5e488d60b309d5f253adab7f2c45ed7`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d263b0ed3ea3116c812ca5c542c5175ccb0c99bee76b06db8c2340290057fa`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9165592365f0af3016a817877513f46b501c0a526c4ba8ef6f74c57ddd35084c`  
		Last Modified: Wed, 04 Aug 2021 21:23:01 GMT  
		Size: 6.4 MB (6402535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.8-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:0701658b47dccbe63590f3113fb29e922d172cfcd2a8968c8cccd5b862b406da
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67080075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e61c00dc1afbaadf09353e28ba9e0de2ddcef8ef8ca38ece4221421b45a306d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:40:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:40:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:40:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:40:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:40:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:41 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:41:12 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d668eead8965ee8f4a1cd65de2a1cde9c49cfd2c2f06ac2290e0b90724ba4ea3`  
		Last Modified: Wed, 04 Aug 2021 21:42:32 GMT  
		Size: 2.5 MB (2458333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7010a04da6233aa993b677900fe12554cb30e4b12adeee36a2c884d5c0ec8965`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c06e26407aeefb6fd4953cb12e19c70695281c4c9ab4e9b8120734669094a8a`  
		Last Modified: Wed, 04 Aug 2021 21:42:39 GMT  
		Size: 55.4 MB (55420354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e4b73ac390f4f52af96ffa7e98228c80619fa25bd61e862485f64b509a849`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627ac7844e75fc94ea8963915c871cb5e376af3631da0ce14bf5a5662813175f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be33fcd733ebf68f8983483238e2245237efdc7751c83d98e9ce9b6a0f3069f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc643a0ffa7d7ae60054634b94e2ea6799be888df2ed22e2dd0d369753ba11e`  
		Last Modified: Wed, 04 Aug 2021 21:43:45 GMT  
		Size: 6.5 MB (6487495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8-windowsservercore`

```console
$ docker pull docker@sha256:e23c1097f4422e0afd160973bdf739969e3f554176a203e74c9516e578f93eb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `docker:20.10.8-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull docker@sha256:861ad32b4aea6ebcafe15263de5392e2b96e68ae72982bbe6c3ee5842a392d2d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2736709359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45b8a1ae2c2bd7da22c9fb3204f2d1906f3d638f0a4fe37d7f63041107380a9e`
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
# Wed, 04 Aug 2021 21:14:18 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:14:21 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Wed, 04 Aug 2021 21:15:34 GMT
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
	-	`sha256:261da88a9739468f39a6c5afea5001a7636ff158c9f6d3c55c781c7a5e25f03d`  
		Last Modified: Wed, 04 Aug 2021 21:15:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65914705f95c4725772744ad7f2007bde657f07e7e22b9fdd99ceee0e321b00d`  
		Last Modified: Wed, 04 Aug 2021 21:15:58 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649fb723a4e40f18c7aafb9c9da6b3cf4745259262599aad41308db2de8ed8c8`  
		Last Modified: Wed, 04 Aug 2021 21:16:09 GMT  
		Size: 50.9 MB (50889139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.8-windowsservercore-1809`

```console
$ docker pull docker@sha256:e23c1097f4422e0afd160973bdf739969e3f554176a203e74c9516e578f93eb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `docker:20.10.8-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull docker@sha256:861ad32b4aea6ebcafe15263de5392e2b96e68ae72982bbe6c3ee5842a392d2d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2736709359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45b8a1ae2c2bd7da22c9fb3204f2d1906f3d638f0a4fe37d7f63041107380a9e`
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
# Wed, 04 Aug 2021 21:14:18 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:14:21 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Wed, 04 Aug 2021 21:15:34 GMT
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
	-	`sha256:261da88a9739468f39a6c5afea5001a7636ff158c9f6d3c55c781c7a5e25f03d`  
		Last Modified: Wed, 04 Aug 2021 21:15:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65914705f95c4725772744ad7f2007bde657f07e7e22b9fdd99ceee0e321b00d`  
		Last Modified: Wed, 04 Aug 2021 21:15:58 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649fb723a4e40f18c7aafb9c9da6b3cf4745259262599aad41308db2de8ed8c8`  
		Last Modified: Wed, 04 Aug 2021 21:16:09 GMT  
		Size: 50.9 MB (50889139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:c0aac52a0f704627c01dfd5177f3d0e5d9bf6e64f2b8a2c35b5b5087ebe94cfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:5a0822246a7ba7596160e5ebde39840d7631be4a30cd4133aec47625e87a69bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73065601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ede8a8017c85b24213ab65dc802ae2d0042d755d5c301d397e110381d5f50e3b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:20:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:20:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:20:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:20:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:43 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:20:44 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:20:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:44 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:20:50 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Aug 2021 21:20:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:20:51 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 04 Aug 2021 21:20:52 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Aug 2021 21:20:52 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:52 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Aug 2021 21:20:52 GMT
EXPOSE 2375 2376
# Wed, 04 Aug 2021 21:20:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:53 GMT
CMD []
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b94fafbd542a8c279f4a08e81fef317862b0fe3f604febe2fc2138886ba1d7`  
		Last Modified: Wed, 04 Aug 2021 21:21:53 GMT  
		Size: 2.4 MB (2438245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e3c9e6c132861fd24ac22906718bb610ebcf3912ade5e48a791ba8f85e5799`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc990f87bf12a7b8fb86c3003977468a14fb1a31e5bb0b500e8127ee4e6beb5`  
		Last Modified: Wed, 04 Aug 2021 21:22:03 GMT  
		Size: 61.3 MB (61284061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1436504743cc47a166b7964d591792b69e34aa1e3e07ef5d91f481fdb11f948d`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c526f01240b836e9645a2b2b629051c5e488d60b309d5f253adab7f2c45ed7`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d263b0ed3ea3116c812ca5c542c5175ccb0c99bee76b06db8c2340290057fa`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323e02cdc2f5b38baeff0de98fb35ef0d98c8eb6ee03c82bad90c145c7fe31a5`  
		Last Modified: Wed, 04 Aug 2021 21:22:21 GMT  
		Size: 6.5 MB (6524551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278c396f7286d8283a874d8792049d325633fac7e850531740d22f560c955187`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8ecf0198691794c5ecaa8389e5beef5e882d6cfec101c6a09dd9ace85ab594`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 979.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2662824727357b53a9d351903bfd330007c20c9576b971e2a06c0018226c6c3b`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:45667bb65fd02bf020846511c1f59ef9267e2c16439b60509dcf44794307f4f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67013251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:819e5b46b4c03a38c8296417bbbb73b3654addd89381b617d1ffd72887fdb7d2`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:40:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:40:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:40:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:40:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:40:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:41 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:40:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Aug 2021 21:40:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:40:50 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 04 Aug 2021 21:40:51 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Aug 2021 21:40:51 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:52 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Aug 2021 21:40:52 GMT
EXPOSE 2375 2376
# Wed, 04 Aug 2021 21:40:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:52 GMT
CMD []
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d668eead8965ee8f4a1cd65de2a1cde9c49cfd2c2f06ac2290e0b90724ba4ea3`  
		Last Modified: Wed, 04 Aug 2021 21:42:32 GMT  
		Size: 2.5 MB (2458333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7010a04da6233aa993b677900fe12554cb30e4b12adeee36a2c884d5c0ec8965`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c06e26407aeefb6fd4953cb12e19c70695281c4c9ab4e9b8120734669094a8a`  
		Last Modified: Wed, 04 Aug 2021 21:42:39 GMT  
		Size: 55.4 MB (55420354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e4b73ac390f4f52af96ffa7e98228c80619fa25bd61e862485f64b509a849`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627ac7844e75fc94ea8963915c871cb5e376af3631da0ce14bf5a5662813175f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be33fcd733ebf68f8983483238e2245237efdc7751c83d98e9ce9b6a0f3069f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7be703642618a8d45d2234fbab8868b1139a87c1d15e9ed461b84c174d6a50`  
		Last Modified: Wed, 04 Aug 2021 21:42:59 GMT  
		Size: 6.4 MB (6415768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d505b30c548b9339cb05141edaeeb535a1f6957a797abe632d52f98cc323a97`  
		Last Modified: Wed, 04 Aug 2021 21:42:58 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4a4ed41a0a4416dc51a066b9e02ee59d31136060b4b70de974046278cbaf0f`  
		Last Modified: Wed, 04 Aug 2021 21:42:59 GMT  
		Size: 975.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88540cd1423a8caeac6757a720ddc1be1455af90c51f8242cc0039ca1f5d3b37`  
		Last Modified: Wed, 04 Aug 2021 21:42:58 GMT  
		Size: 2.6 KB (2615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:963579745bca14f3cbd0d13ccc9b1909864e735d180c585ec47aa1f7d2257fd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:124b738e215234286634752adb38a03fca0b5f4d46c291a1f77a84b0383a1e5e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.3 MB (93315315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7347a3756263d56fd413c805bf0cb3bc52910009c4dbc12a4c8e84ba4359ffe6`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:20:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:20:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:20:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:20:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:43 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:20:44 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:20:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:44 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:20:50 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Aug 2021 21:20:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:20:51 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 04 Aug 2021 21:20:52 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Aug 2021 21:20:52 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:52 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Aug 2021 21:20:52 GMT
EXPOSE 2375 2376
# Wed, 04 Aug 2021 21:20:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:53 GMT
CMD []
# Wed, 04 Aug 2021 21:20:57 GMT
RUN apk add --no-cache iproute2
# Wed, 04 Aug 2021 21:20:58 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 04 Aug 2021 21:20:58 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:21:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 04 Aug 2021 21:21:01 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 04 Aug 2021 21:21:01 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 04 Aug 2021 21:21:01 GMT
USER rootless
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b94fafbd542a8c279f4a08e81fef317862b0fe3f604febe2fc2138886ba1d7`  
		Last Modified: Wed, 04 Aug 2021 21:21:53 GMT  
		Size: 2.4 MB (2438245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e3c9e6c132861fd24ac22906718bb610ebcf3912ade5e48a791ba8f85e5799`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc990f87bf12a7b8fb86c3003977468a14fb1a31e5bb0b500e8127ee4e6beb5`  
		Last Modified: Wed, 04 Aug 2021 21:22:03 GMT  
		Size: 61.3 MB (61284061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1436504743cc47a166b7964d591792b69e34aa1e3e07ef5d91f481fdb11f948d`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c526f01240b836e9645a2b2b629051c5e488d60b309d5f253adab7f2c45ed7`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d263b0ed3ea3116c812ca5c542c5175ccb0c99bee76b06db8c2340290057fa`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323e02cdc2f5b38baeff0de98fb35ef0d98c8eb6ee03c82bad90c145c7fe31a5`  
		Last Modified: Wed, 04 Aug 2021 21:22:21 GMT  
		Size: 6.5 MB (6524551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278c396f7286d8283a874d8792049d325633fac7e850531740d22f560c955187`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8ecf0198691794c5ecaa8389e5beef5e882d6cfec101c6a09dd9ace85ab594`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 979.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2662824727357b53a9d351903bfd330007c20c9576b971e2a06c0018226c6c3b`  
		Last Modified: Wed, 04 Aug 2021 21:22:20 GMT  
		Size: 2.6 KB (2616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e6256c33c0ede1adebf65b20431decf86e9ee5ee75bc5dafdc97323eb00b14`  
		Last Modified: Wed, 04 Aug 2021 21:22:39 GMT  
		Size: 1.1 MB (1131912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ee6cc75d0fb6ad7733a1aff3c28f0f3f7e0b2fab5a6a3834b15f4448fafd63`  
		Last Modified: Wed, 04 Aug 2021 21:22:39 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53de6cbf547b0318998261b99b7a0a30bd3fcde67956de7983df1b2328af358`  
		Last Modified: Wed, 04 Aug 2021 21:22:39 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956907e972957db3a2ae0b2ea1caad912dbfeb36651f885dd48cd155e666de43`  
		Last Modified: Wed, 04 Aug 2021 21:22:42 GMT  
		Size: 19.1 MB (19116096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39800d8bc1636f365b4faf120564b96243d4c0cb880f893e9b561a609f4758d1`  
		Last Modified: Wed, 04 Aug 2021 21:22:39 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8798010c693f3e0ab32e9c78938345734472925bde322d6eb50d015729da5738
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.3 MB (89262967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:796d21eeac11e41216052d96f3f42968c38bd60d22c93a28c08f5c8b0adb6510`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:40:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:40:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:40:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:40:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:40:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:41 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:40:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Aug 2021 21:40:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:40:50 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 04 Aug 2021 21:40:51 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Aug 2021 21:40:51 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:52 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Aug 2021 21:40:52 GMT
EXPOSE 2375 2376
# Wed, 04 Aug 2021 21:40:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:52 GMT
CMD []
# Wed, 04 Aug 2021 21:40:59 GMT
RUN apk add --no-cache iproute2
# Wed, 04 Aug 2021 21:41:00 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 04 Aug 2021 21:41:01 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 04 Aug 2021 21:41:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 04 Aug 2021 21:41:04 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 04 Aug 2021 21:41:04 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 04 Aug 2021 21:41:04 GMT
USER rootless
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d668eead8965ee8f4a1cd65de2a1cde9c49cfd2c2f06ac2290e0b90724ba4ea3`  
		Last Modified: Wed, 04 Aug 2021 21:42:32 GMT  
		Size: 2.5 MB (2458333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7010a04da6233aa993b677900fe12554cb30e4b12adeee36a2c884d5c0ec8965`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c06e26407aeefb6fd4953cb12e19c70695281c4c9ab4e9b8120734669094a8a`  
		Last Modified: Wed, 04 Aug 2021 21:42:39 GMT  
		Size: 55.4 MB (55420354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e4b73ac390f4f52af96ffa7e98228c80619fa25bd61e862485f64b509a849`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627ac7844e75fc94ea8963915c871cb5e376af3631da0ce14bf5a5662813175f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be33fcd733ebf68f8983483238e2245237efdc7751c83d98e9ce9b6a0f3069f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7be703642618a8d45d2234fbab8868b1139a87c1d15e9ed461b84c174d6a50`  
		Last Modified: Wed, 04 Aug 2021 21:42:59 GMT  
		Size: 6.4 MB (6415768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d505b30c548b9339cb05141edaeeb535a1f6957a797abe632d52f98cc323a97`  
		Last Modified: Wed, 04 Aug 2021 21:42:58 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4a4ed41a0a4416dc51a066b9e02ee59d31136060b4b70de974046278cbaf0f`  
		Last Modified: Wed, 04 Aug 2021 21:42:59 GMT  
		Size: 975.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88540cd1423a8caeac6757a720ddc1be1455af90c51f8242cc0039ca1f5d3b37`  
		Last Modified: Wed, 04 Aug 2021 21:42:58 GMT  
		Size: 2.6 KB (2615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca55d719f285c206e9d9b9f065be06c1921f50cd25f3410d55d34ef73917dcb8`  
		Last Modified: Wed, 04 Aug 2021 21:43:19 GMT  
		Size: 1.2 MB (1153199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af474eb81075318d6a880fdd4d20b5cd59cb8953dc8bdd3e0abee2d3f098d6cc`  
		Last Modified: Wed, 04 Aug 2021 21:43:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8c6d1e64a80e62654c56d0e7179e03154215e4d3a994c2986a5df58e4058df`  
		Last Modified: Wed, 04 Aug 2021 21:43:18 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39408337edbf619576a8236fe50df4b7600b1a2a69ff501d52acad3a4f3b5a07`  
		Last Modified: Wed, 04 Aug 2021 21:43:24 GMT  
		Size: 21.1 MB (21094815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9ccbcf888a167c7709e18d6a5636d0b5b1e7dbc0f476ae4f25a78642e923e2`  
		Last Modified: Wed, 04 Aug 2021 21:43:18 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:1da454342f3c7a35f8d75c6e867ab6afcf0aecacea2495e26f868d82ad5dd788
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:c43f2419d2b2e4177c5df924893b251d7ef6be98c157c885f22bce4ecbd10b8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72938677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fda6f821f6eee066c490f4c12941c8ea6069ccb3f5b2974718337ebd4f563e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:20:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:20:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:20:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:20:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:43 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:20:44 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:20:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:44 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:21:06 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b94fafbd542a8c279f4a08e81fef317862b0fe3f604febe2fc2138886ba1d7`  
		Last Modified: Wed, 04 Aug 2021 21:21:53 GMT  
		Size: 2.4 MB (2438245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e3c9e6c132861fd24ac22906718bb610ebcf3912ade5e48a791ba8f85e5799`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc990f87bf12a7b8fb86c3003977468a14fb1a31e5bb0b500e8127ee4e6beb5`  
		Last Modified: Wed, 04 Aug 2021 21:22:03 GMT  
		Size: 61.3 MB (61284061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1436504743cc47a166b7964d591792b69e34aa1e3e07ef5d91f481fdb11f948d`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c526f01240b836e9645a2b2b629051c5e488d60b309d5f253adab7f2c45ed7`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d263b0ed3ea3116c812ca5c542c5175ccb0c99bee76b06db8c2340290057fa`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9165592365f0af3016a817877513f46b501c0a526c4ba8ef6f74c57ddd35084c`  
		Last Modified: Wed, 04 Aug 2021 21:23:01 GMT  
		Size: 6.4 MB (6402535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:0701658b47dccbe63590f3113fb29e922d172cfcd2a8968c8cccd5b862b406da
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67080075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e61c00dc1afbaadf09353e28ba9e0de2ddcef8ef8ca38ece4221421b45a306d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:40:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:40:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:40:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:40:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:40:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:41 GMT
CMD ["sh"]
# Wed, 04 Aug 2021 21:41:12 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d668eead8965ee8f4a1cd65de2a1cde9c49cfd2c2f06ac2290e0b90724ba4ea3`  
		Last Modified: Wed, 04 Aug 2021 21:42:32 GMT  
		Size: 2.5 MB (2458333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7010a04da6233aa993b677900fe12554cb30e4b12adeee36a2c884d5c0ec8965`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c06e26407aeefb6fd4953cb12e19c70695281c4c9ab4e9b8120734669094a8a`  
		Last Modified: Wed, 04 Aug 2021 21:42:39 GMT  
		Size: 55.4 MB (55420354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e4b73ac390f4f52af96ffa7e98228c80619fa25bd61e862485f64b509a849`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627ac7844e75fc94ea8963915c871cb5e376af3631da0ce14bf5a5662813175f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be33fcd733ebf68f8983483238e2245237efdc7751c83d98e9ce9b6a0f3069f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc643a0ffa7d7ae60054634b94e2ea6799be888df2ed22e2dd0d369753ba11e`  
		Last Modified: Wed, 04 Aug 2021 21:43:45 GMT  
		Size: 6.5 MB (6487495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:ddf0d732dcbc3e2087836e06e50cc97e21bfb002a49c7d0fe767f6c31e01d65f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:c9fe80d9eb030d771811e9cefcf2e3cb73aad845c24eee8e29b72b4429fae283
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66536142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51453dcdd9bd51e503f75e6d42a4071469ad2ba816321781985041b6bc7776db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:20:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:20:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:20:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:20:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:43 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:20:44 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:20:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:44 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b94fafbd542a8c279f4a08e81fef317862b0fe3f604febe2fc2138886ba1d7`  
		Last Modified: Wed, 04 Aug 2021 21:21:53 GMT  
		Size: 2.4 MB (2438245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e3c9e6c132861fd24ac22906718bb610ebcf3912ade5e48a791ba8f85e5799`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc990f87bf12a7b8fb86c3003977468a14fb1a31e5bb0b500e8127ee4e6beb5`  
		Last Modified: Wed, 04 Aug 2021 21:22:03 GMT  
		Size: 61.3 MB (61284061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1436504743cc47a166b7964d591792b69e34aa1e3e07ef5d91f481fdb11f948d`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c526f01240b836e9645a2b2b629051c5e488d60b309d5f253adab7f2c45ed7`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d263b0ed3ea3116c812ca5c542c5175ccb0c99bee76b06db8c2340290057fa`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:202f4fd8f1bc62e516f42f1f32d205a6d9dc12a5eddf42be5adda612331f7d99
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.6 MB (60592580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:917aa76b39804498915883c81d9c3f4616dafbae602e0e81597852ab6905bc77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:40:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:40:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:40:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:40:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:40:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:41 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d668eead8965ee8f4a1cd65de2a1cde9c49cfd2c2f06ac2290e0b90724ba4ea3`  
		Last Modified: Wed, 04 Aug 2021 21:42:32 GMT  
		Size: 2.5 MB (2458333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7010a04da6233aa993b677900fe12554cb30e4b12adeee36a2c884d5c0ec8965`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c06e26407aeefb6fd4953cb12e19c70695281c4c9ab4e9b8120734669094a8a`  
		Last Modified: Wed, 04 Aug 2021 21:42:39 GMT  
		Size: 55.4 MB (55420354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e4b73ac390f4f52af96ffa7e98228c80619fa25bd61e862485f64b509a849`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627ac7844e75fc94ea8963915c871cb5e376af3631da0ce14bf5a5662813175f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be33fcd733ebf68f8983483238e2245237efdc7751c83d98e9ce9b6a0f3069f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore`

```console
$ docker pull docker@sha256:e23c1097f4422e0afd160973bdf739969e3f554176a203e74c9516e578f93eb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `docker:windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull docker@sha256:861ad32b4aea6ebcafe15263de5392e2b96e68ae72982bbe6c3ee5842a392d2d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2736709359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45b8a1ae2c2bd7da22c9fb3204f2d1906f3d638f0a4fe37d7f63041107380a9e`
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
# Wed, 04 Aug 2021 21:14:18 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:14:21 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Wed, 04 Aug 2021 21:15:34 GMT
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
	-	`sha256:261da88a9739468f39a6c5afea5001a7636ff158c9f6d3c55c781c7a5e25f03d`  
		Last Modified: Wed, 04 Aug 2021 21:15:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65914705f95c4725772744ad7f2007bde657f07e7e22b9fdd99ceee0e321b00d`  
		Last Modified: Wed, 04 Aug 2021 21:15:58 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649fb723a4e40f18c7aafb9c9da6b3cf4745259262599aad41308db2de8ed8c8`  
		Last Modified: Wed, 04 Aug 2021 21:16:09 GMT  
		Size: 50.9 MB (50889139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:e23c1097f4422e0afd160973bdf739969e3f554176a203e74c9516e578f93eb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull docker@sha256:861ad32b4aea6ebcafe15263de5392e2b96e68ae72982bbe6c3ee5842a392d2d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2736709359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45b8a1ae2c2bd7da22c9fb3204f2d1906f3d638f0a4fe37d7f63041107380a9e`
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
# Wed, 04 Aug 2021 21:14:18 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:14:21 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Wed, 04 Aug 2021 21:15:34 GMT
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
	-	`sha256:261da88a9739468f39a6c5afea5001a7636ff158c9f6d3c55c781c7a5e25f03d`  
		Last Modified: Wed, 04 Aug 2021 21:15:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65914705f95c4725772744ad7f2007bde657f07e7e22b9fdd99ceee0e321b00d`  
		Last Modified: Wed, 04 Aug 2021 21:15:58 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649fb723a4e40f18c7aafb9c9da6b3cf4745259262599aad41308db2de8ed8c8`  
		Last Modified: Wed, 04 Aug 2021 21:16:09 GMT  
		Size: 50.9 MB (50889139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
