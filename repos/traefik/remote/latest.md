## `traefik:latest`

```console
$ docker pull traefik@sha256:fdff55caa91ac7ff217ff03b93f3673844b3b88ad993e023ab43f6004021697c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:6354bfe99cf39164514ecca33ef4189361f0bf4eca8c16ffc1bae3623b99e8c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31023311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8345b2e8bee0c824835af0881cfdc602bbb351637c205cbebc76e7b74f813597`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:09:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:34:49 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:34:50 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:34:50 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:34:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:34:50 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:34:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07cb125bb766321ae78c2a558eb61358ea0c322871a963cc343f07b19a5dfe9f`  
		Last Modified: Tue, 24 May 2022 20:09:52 GMT  
		Size: 667.0 KB (667045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7643a4c688aef051e331797b6a1c3cf5a493b95e95e9a90502f34bb69543cf`  
		Last Modified: Mon, 13 Jun 2022 18:35:44 GMT  
		Size: 27.5 MB (27541339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5730b5ba9047bdf67c081e949f31b562532504f42b183afab9b38e82692c6a03`  
		Last Modified: Mon, 13 Jun 2022 18:35:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:b8e54b077cf2ffb132203d201519c7dae5dd885ea8cf6eb4b24f3bdd37eb0a6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29110783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc0175d61827f26689cebc311c086e4998894cb2370fa203eb6b0fc54626b7b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:16:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:01:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:01:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:01:08 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:01:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:01:09 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:01:10 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca500a6585c4382a3d0562172788318c2044142456377fdbf2c4b279334e26`  
		Last Modified: Tue, 24 May 2022 20:19:13 GMT  
		Size: 672.6 KB (672642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97f5f8fa2680bd0e85b1838bc88a1b3bad8ea5a158b18383f007e4c6b398e52`  
		Last Modified: Mon, 13 Jun 2022 18:04:09 GMT  
		Size: 25.8 MB (25815800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a11e8a929d0ad2e555c58f324df02cde6c468d2662ecf5414979893c990664`  
		Last Modified: Mon, 13 Jun 2022 18:03:52 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:f65b5a3b0de3d895385f85c41a180573a59d7dc4890d24e1b21c3fedd699ddf2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28492564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d1d1d829b444cff7a651cd13bdc6b2a66de794c8f21f75c5b7f204da37fdcb4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 21:18:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:19:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:19:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:19:35 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:19:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:19:37 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:19:38 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdde6df9c5c8f6328c1ce3fe2ca88cea0a7799584b83cafec0322b4d7235d0b7`  
		Last Modified: Tue, 24 May 2022 21:20:14 GMT  
		Size: 668.4 KB (668397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed46ebeb3f061a6426a51c9ce5d729ffe5bc2f3d8353303c30c35bff93ed4232`  
		Last Modified: Mon, 13 Jun 2022 18:21:04 GMT  
		Size: 25.1 MB (25107322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8683e30306089877837d12d61eaf9cc16d7ad0b3313d5b38dbff4cbc1685b057`  
		Last Modified: Mon, 13 Jun 2022 18:21:00 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; s390x

```console
$ docker pull traefik@sha256:9d7c6aa60ebe18d8257b0a02296eb18ac01e047675e48f4c20272c849c98669d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29788377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11de775752a6ad32f36bb166122916f9c84d52645b1d8c4274acb265af05d91`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:28:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:15:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:15:21 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:15:22 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:15:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:15:22 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:15:22 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f52582da22b0abbdbb4590735229191759cc22a1119ccdf5af9cd472103ffd`  
		Last Modified: Tue, 24 May 2022 20:29:51 GMT  
		Size: 672.6 KB (672603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0a8dab5f416aa3abd40293a95475c0df50231b6c94cf0b9c4fdbe5d2088c03`  
		Last Modified: Mon, 13 Jun 2022 18:16:12 GMT  
		Size: 26.5 MB (26515031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cc2efd66f301007736aaf33dcba85abe0fd187a08d11ce716f925b49440b20`  
		Last Modified: Mon, 13 Jun 2022 18:16:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
