## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:a5be418acbd9a1a3011242c27feadd440ca56afbec22a7763150202de397cb6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:178c67d6e375ce45264f1a47eef709bca9928ac85badaa8f0d877059d5f37b6a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24617292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa4204cec7f48d0cc16d69e25ac8a29074a4782bc92622e55ec94c3b11f5b479`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:45:50 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 22:23:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 22:23:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 22:23:45 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:23:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 22:23:45 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 22:23:45 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f365f1b91ebb32c62c3856cd602b14702103c16ede6873855d0c5a5faa874810`  
		Last Modified: Mon, 23 Mar 2020 23:47:03 GMT  
		Size: 694.1 KB (694143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cb6e408627ad0a100994d33c802c10828d8373fb7234572e0235fca9d7294c`  
		Last Modified: Wed, 25 Mar 2020 22:24:39 GMT  
		Size: 21.1 MB (21119525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5c0f262e2748518c0df991fbe02ea98c1eb9fc9a355c8eb8ca0c4cd4b43b55`  
		Last Modified: Wed, 25 Mar 2020 22:24:34 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:4f2a0e53c458ad8c389a40413c074135270a7bd2f82b1eb51a7dd0a5f093ec2b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23088245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd24e8f81b3e69a7b6eee14be566e2fd65f042b52389beb520915838d86f15e3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 03:43:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:49:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:49:53 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:49:54 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:49:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:49:55 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:49:55 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b73c299e24e9aa32bbbec493b7588c3a6592d11b52ccb01c156037b819aef46`  
		Last Modified: Tue, 24 Mar 2020 03:47:03 GMT  
		Size: 698.1 KB (698067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65b61609c3447263dc8c67420226770998aab72683c8da887882dda9a04761d`  
		Last Modified: Wed, 25 Mar 2020 21:50:48 GMT  
		Size: 19.8 MB (19771230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf34024959fde388d8f122f98686c98d2f26a6ee616fac255e9d24a7684480d`  
		Last Modified: Wed, 25 Mar 2020 21:50:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:2960a1bff52c4e20800f297ac9491661804f276e4c167c5f477cae56e45bf482
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22911054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10cc83f1529223ab41bc828bcbd1d0b3937e49b4786ab5851376c284cac448b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 05:52:48 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:44:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:44:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:44:07 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:44:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:44:08 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:44:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc893b889cb9ecb596775296ec01901b5ffcd52efc8691a608afb27fc5be6e6`  
		Last Modified: Tue, 24 Mar 2020 05:55:52 GMT  
		Size: 696.2 KB (696184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46883925a5415d0997e2373210f823fdb48428220d78047fe8ff251f7fc6810`  
		Last Modified: Wed, 25 Mar 2020 21:45:06 GMT  
		Size: 19.5 MB (19491362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09800e005e5decf1b215e0d6adfd8871dafad512432f8e624b6e59c927639d73`  
		Last Modified: Wed, 25 Mar 2020 21:44:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
