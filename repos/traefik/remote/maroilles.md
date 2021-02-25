## `traefik:maroilles`

```console
$ docker pull traefik@sha256:5325e0f4d374b9fd87550465b3145415c24ce90d56f839632e56875ce4072844
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:154e065982592220c9355925d9e60348eec6850418754ee76840f83501341b00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21553283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2d67ddf1c8b647742ebb1ea0d3edb163dff028640b772832fa325b6b7df830f`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:48:11 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:48:11 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Wed, 13 Jan 2021 22:29:46 GMT
COPY file:94b9997cc55c7732c9fc173c119f980e4a38eba20b96a90170a3d7fade75f0eb in / 
# Wed, 13 Jan 2021 22:29:47 GMT
EXPOSE 80
# Wed, 13 Jan 2021 22:29:47 GMT
VOLUME [/tmp]
# Wed, 13 Jan 2021 22:29:47 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Jan 2021 22:29:47 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79de75e85675fa9abbac17b57205d3e0dfcf2bd2fc4cbc194f2aaf917435425e`  
		Last Modified: Thu, 17 Dec 2020 00:49:17 GMT  
		Size: 130.9 KB (130872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0e925284bb6370a549da51637ed98a8e574317473e082cc4be745d87327c7f`  
		Last Modified: Thu, 17 Dec 2020 00:49:18 GMT  
		Size: 306.4 KB (306411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81848bd29c493bb51f93a0bf98cf3958436af2128b6890d7a28a35b7dfc352c0`  
		Last Modified: Wed, 13 Jan 2021 22:30:48 GMT  
		Size: 21.1 MB (21116000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:5eea4ce43832fb4fe06e6a76f4be2ee702cd7406bca2eeb28e7b8886b857fb60
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20207939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a16dc71c18edfa988002598f7753875525a253977c27360950d4277cb5a12afb`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 24 Feb 2021 23:34:19 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Wed, 24 Feb 2021 23:34:26 GMT
COPY file:3d9c1552db5b4c73ac7fe21268eeb20506f000d2e59d7be76697f45a50d32c64 in / 
# Wed, 24 Feb 2021 23:34:29 GMT
EXPOSE 80
# Wed, 24 Feb 2021 23:34:30 GMT
VOLUME [/tmp]
# Wed, 24 Feb 2021 23:34:31 GMT
ENTRYPOINT ["/traefik"]
# Wed, 24 Feb 2021 23:34:33 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:26c529e82b09c489524aa4f787754320793a95eb7aa7eaf306c517b76818ec25`  
		Last Modified: Thu, 17 Dec 2020 00:28:41 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e74b8526f2bdaa522f470d66d09f7ebbe9a1f060ce049ac91c0f7aad153e1be`  
		Last Modified: Wed, 24 Feb 2021 23:36:10 GMT  
		Size: 308.9 KB (308855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5b49b6d2a16c38104badd82447927b16f7ba253b84d47c329449b778bb19d`  
		Last Modified: Wed, 24 Feb 2021 23:36:21 GMT  
		Size: 19.8 MB (19768211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:468570d210f86c4366e666dac62c34b3054c230ee0b4d61c36e37ed276550b39
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19923388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13fff7cc610524cb77e4767eb66f534053cc0f45853e096fb250937594f9913d`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:27:58 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Wed, 13 Jan 2021 21:46:55 GMT
COPY file:6bab4a8fc3d272fc29bc5ff42634cb12785fea9e23b0cf50f077702217bb6c03 in / 
# Wed, 13 Jan 2021 21:46:56 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:46:56 GMT
VOLUME [/tmp]
# Wed, 13 Jan 2021 21:46:57 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Jan 2021 21:46:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7dccf22d113d483cac839141f2028cbf6ac2e0c6aa4a1716c5e7b575b162028c`  
		Last Modified: Thu, 17 Dec 2020 00:29:55 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c32c03119dbb32c844511340cb40a21ba5a56b90862cf603dec2e49cf5ab20d`  
		Last Modified: Thu, 17 Dec 2020 00:29:57 GMT  
		Size: 306.5 KB (306466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f7f3a967c907bfe4aeb896ba6da80cfaf9bce19fcb39b51a6378b00596760d`  
		Last Modified: Wed, 13 Jan 2021 21:47:50 GMT  
		Size: 19.5 MB (19486049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
