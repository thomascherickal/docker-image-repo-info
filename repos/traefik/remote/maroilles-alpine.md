## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:3f2bc1ba1b3af0196f7ccc05598162d4a4af99eb3c6874aa73c91fa8074a10b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:6a5bf0d59212a73927e18da4a5b85ff7d02fb566283bcd10b3c307b8a39627a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25653523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:299327139165b0025a883c7a11747b5d04c4bc72f053601c0f763fee0ed761a1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:59 GMT
ADD file:a41bb436701fd0adf99a3157d19f172b3e54ea033f5c617009e2d1bdeac206d7 in / 
# Sat, 11 Feb 2023 04:46:59 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:05:46 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 14:05:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 14:05:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 14:05:51 GMT
EXPOSE 80
# Sat, 11 Feb 2023 14:05:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 14:05:52 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 14:05:52 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:d261077062b2aebb9ca8dc61f2b00e7e2b4e44179d3cfbe526c4ee0c5e41b26f`  
		Last Modified: Sat, 11 Feb 2023 04:47:49 GMT  
		Size: 2.8 MB (2829633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60fab313a1ca0ee79d027587c5edad5ff243a08e1cbd263abe2a17503c316d8b`  
		Last Modified: Sat, 11 Feb 2023 14:07:08 GMT  
		Size: 661.5 KB (661461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e550be36e43026c7c9214cf16b3b866de5ce1da12f14fcef46658c0def1d4a7`  
		Last Modified: Sat, 11 Feb 2023 14:07:12 GMT  
		Size: 22.2 MB (22162062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4561714fba29bd0d410fa9813afc75479ffef93714ffdad849a7943771d73544`  
		Last Modified: Sat, 11 Feb 2023 14:07:08 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:7f9dabda3415134f3c6c55aa1c6d4a9714df3e6c1b17c09fa6829518be40304e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23928182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989b6b4695cc561a8362ad5d755b293faf05ef51a2213c0f68940138fe65fd46`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:15 GMT
ADD file:1039802413c644346f599dac53a7c6dabd123027756231b9d8f64a1068c9779d in / 
# Wed, 29 Mar 2023 18:01:15 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:57 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 00:40:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 00:40:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 00:40:01 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:40:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 00:40:01 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 00:40:01 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ffeb76b9ee2f52d46487f4f9a7074ea62dea819a2dd53c9a2c6d703ca7b5aa06`  
		Last Modified: Wed, 29 Mar 2023 18:02:21 GMT  
		Size: 2.6 MB (2638259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b1182fcb4f775d878f0b8af17e60fdef00a0afb3a68f68731fdf08ca613566`  
		Last Modified: Thu, 30 Mar 2023 00:41:46 GMT  
		Size: 666.1 KB (666134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ace3e9b5f4c3d44312fca26e27d43459ab4671204cc813ae1a2d94bc295e24`  
		Last Modified: Thu, 30 Mar 2023 00:41:49 GMT  
		Size: 20.6 MB (20623422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec87c1bbd8ed5033ef249c444c828c0d4a024613f7c067d6408df986bd229a`  
		Last Modified: Thu, 30 Mar 2023 00:41:46 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:e23b8edb3c8a7f4a5ce7b2697e304f8e31d845474dccdbcd15b86e831c7bc69b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23519920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72dbaffc2f8e74c9ed9aa7a99d590e792ba2b318e8562992180335ba122958e3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:19 GMT
ADD file:50a841463966858f1c3ca87143cf96145d1d52f7349ef516adfbf21cdd5684fe in / 
# Fri, 10 Feb 2023 21:24:19 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:40:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 06:40:45 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 06:40:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 06:40:46 GMT
EXPOSE 80
# Sat, 11 Feb 2023 06:40:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 06:40:46 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 06:40:46 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6f0e733d82e26042c603e231c39b56abbabdad66673a736ec71c69c65be95f41`  
		Last Modified: Fri, 10 Feb 2023 21:25:10 GMT  
		Size: 2.7 MB (2725026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c8dd85906c92d3445ffeb0481950055e77c854095c4cbbd854f6951242a3c`  
		Last Modified: Sat, 11 Feb 2023 06:41:54 GMT  
		Size: 663.2 KB (663163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0994ad8baa5503f4c667ced5bb36b643eba7642f9791e4bf7975527de9f2c2ed`  
		Last Modified: Sat, 11 Feb 2023 06:41:57 GMT  
		Size: 20.1 MB (20131363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6a5a822a3369f9999a4da4bcb9718729d386c2dbf108fb8a8a52056eacc8d2`  
		Last Modified: Sat, 11 Feb 2023 06:41:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
