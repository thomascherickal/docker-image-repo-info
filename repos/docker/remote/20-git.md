## `docker:20-git`

```console
$ docker pull docker@sha256:ab069d931ab449ce00eb935ffd4327bdb659b6b0d15f5725a6363d3f9c0e3d8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-git` - linux; amd64

```console
$ docker pull docker@sha256:2bec22e08c775d6e15f6e64878ed448d1d98bef0225c884a3c70a4274970c479
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.9 MB (80949262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdf48a660e89f8319289bc4a15ac35ef08e425ffb41770d8e0701247c47aef5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 21:43:03 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 17 Feb 2021 21:43:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 03 Mar 2021 01:19:43 GMT
ENV DOCKER_VERSION=20.10.5
# Wed, 03 Mar 2021 01:19:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.5.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 03 Mar 2021 01:19:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 03 Mar 2021 01:19:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 03 Mar 2021 01:19:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 03 Mar 2021 01:19:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 03 Mar 2021 01:19:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Mar 2021 01:19:53 GMT
CMD ["sh"]
# Wed, 03 Mar 2021 01:20:22 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94caa5d1da7043140e78e14956c22154f75708f44c1c1367ac20cc5a8be71e8b`  
		Last Modified: Wed, 17 Feb 2021 21:44:58 GMT  
		Size: 2.1 MB (2051413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10a29983da5ea49c724d6c132f4d3dc6c130fe7148e4dd9fc258c34fa210f0a`  
		Last Modified: Wed, 17 Feb 2021 21:44:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6ccddb7fa4ac3d17b73897072eb4e290f303073edb0964e6d5a3becb9a5a0b`  
		Last Modified: Wed, 03 Mar 2021 01:21:21 GMT  
		Size: 69.7 MB (69692167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1bef566495d7c6876dfecd14cbc9ee0b2a6e37c3d7ccfacd026b1a7ed66d45`  
		Last Modified: Wed, 03 Mar 2021 01:21:06 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201a9d1142eb86ee5a02feb68aee88cb069648aecc92331f7b4b3d6c9f18b90f`  
		Last Modified: Wed, 03 Mar 2021 01:21:07 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0806b78d1f4d9cfd8d904285a1c970d39cd203456efff5a95d56cc4e435618dd`  
		Last Modified: Wed, 03 Mar 2021 01:21:06 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664a0dc66ed65296bc5eb9cbda034c14add1ac170ea3a7db606cfc1835430778`  
		Last Modified: Wed, 03 Mar 2021 01:21:52 GMT  
		Size: 6.4 MB (6392196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:b6f8ebdda95e413f0118aedb37a7b6a08f8cc20fe02416d0a6ef3732b7cf3bfd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75033876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46be7269d18513d618ddadd3af99b8db787de2991471f97b892ffbb4907f58d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 20:58:21 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 17 Feb 2021 20:58:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 03 Mar 2021 00:39:43 GMT
ENV DOCKER_VERSION=20.10.5
# Wed, 03 Mar 2021 00:39:50 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.5.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 03 Mar 2021 00:39:52 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 03 Mar 2021 00:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 03 Mar 2021 00:39:53 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 03 Mar 2021 00:39:55 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 03 Mar 2021 00:39:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Mar 2021 00:39:56 GMT
CMD ["sh"]
# Wed, 03 Mar 2021 00:40:24 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73c8b9b1c8dd10c5e507fe99a317a8c9e76be18ce77b09351cae695d685c7b5`  
		Last Modified: Wed, 17 Feb 2021 21:00:33 GMT  
		Size: 2.1 MB (2067994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10cdebbd0f7f08e6238d70b00cc96942f37974ae2ad8d72478ccef46d019ff2`  
		Last Modified: Wed, 17 Feb 2021 21:00:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b94630c48ae2e6f574232450280da213e2c3da9f3b369599b6b8624c21925bb`  
		Last Modified: Wed, 03 Mar 2021 00:41:20 GMT  
		Size: 63.8 MB (63776776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482a2fdb559c47f0f0e45c4492cd6781fb854ce82bd97c22511924402d2e0a7e`  
		Last Modified: Wed, 03 Mar 2021 00:41:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead1daa99581cd5d7648abc46d6b31c0399613b68de92833fcbf2272928e715b`  
		Last Modified: Wed, 03 Mar 2021 00:41:02 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a0d231a5fae87ccbe93e7ae5c67890d1d21fc29d46c728d37bcb050ea5f3d5`  
		Last Modified: Wed, 03 Mar 2021 00:41:06 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647fb561b0a5199628a1cbe697dd372d88631bc60fc2410c6b17eb1b83904ca0`  
		Last Modified: Wed, 03 Mar 2021 00:41:43 GMT  
		Size: 6.5 MB (6475671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
