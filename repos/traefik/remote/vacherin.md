## `traefik:vacherin`

```console
$ docker pull traefik@sha256:b83c90bf6ca98416a19327310228b669845baad0649431313ac183fc787f7386
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:vacherin` - linux; amd64

```console
$ docker pull traefik@sha256:4fa5024ce4f5ff629dfdffe651d2852ea04691b4902950db143914c9d361af38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.6 MB (31574343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4524c3269b0f9f98fcfe42134d0e7635306344d010df01923d147a5e94a91746`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:24:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 10 Aug 2022 01:24:58 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.1/traefik_v2.8.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 10 Aug 2022 01:24:58 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 10 Aug 2022 01:24:58 GMT
EXPOSE 80
# Wed, 10 Aug 2022 01:24:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Aug 2022 01:24:59 GMT
CMD ["traefik"]
# Wed, 10 Aug 2022 01:24:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0448c16748457249205ca0475f796fa6c4661fdcbf2d618c5241bdf9c4b12f9a`  
		Last Modified: Wed, 10 Aug 2022 01:25:43 GMT  
		Size: 681.7 KB (681674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9daea7e8d20befadd56e6171d061ff95b92aa6d15a21a66c7bf3712e41e1b97`  
		Last Modified: Wed, 10 Aug 2022 01:25:48 GMT  
		Size: 28.1 MB (28068789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368b8fef87fb39558d7117f8ff523f5a059d950f5fac48cb0430f278bc147cdd`  
		Last Modified: Wed, 10 Aug 2022 01:25:43 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:vacherin` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8cccfda743dbf42c90e560c60a4a72c94ef9a3354cd8118dea8a973fde0c23aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.6 MB (29621226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7bc78eaaf0bf3a16361dab22ed73cbbb1e296920d964fc9b1bd0d38bc662035`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 19 Jul 2022 22:49:49 GMT
ADD file:4958b5356608921fe85d83047b74d1cb4a53de78c3465039ac4e60a68329da64 in / 
# Tue, 19 Jul 2022 22:49:50 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 06:49:03 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 20 Jul 2022 06:49:10 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.1/traefik_v2.8.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 20 Jul 2022 06:49:11 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 20 Jul 2022 06:49:11 GMT
EXPOSE 80
# Wed, 20 Jul 2022 06:49:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Jul 2022 06:49:12 GMT
CMD ["traefik"]
# Wed, 20 Jul 2022 06:49:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:fcc62ebebb3542c1aad49c3cc072a98cf619f67e914baba1ea7dfeadcb32cbdd`  
		Last Modified: Tue, 19 Jul 2022 22:51:27 GMT  
		Size: 2.6 MB (2622400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbb53b6078ca358e1d1c1586bd466779bd44926c0e2ff673b16039cb3eafb03`  
		Last Modified: Wed, 20 Jul 2022 06:51:22 GMT  
		Size: 672.6 KB (672638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b49dea69eb378a4033e87b7c333f6a9bbcb234b5dc843c5d33ada0cd2337f9a`  
		Last Modified: Wed, 20 Jul 2022 06:51:39 GMT  
		Size: 26.3 MB (26325819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d04e1f1c884b0bdc39e84736241a413fd9aa7746ef228c47de6b5ff9fd2b55`  
		Last Modified: Wed, 20 Jul 2022 06:51:21 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:vacherin` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:0af7be5efbf74fbb875686c1bff79d3403073008ff158f8cc493a0f1176d6198
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (28980932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25c1b8b23cabde96f187151b98d9e5d6af2e2b27db1af60bf8835c7c3cb9d3f1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:42 GMT
ADD file:158791ae9b4fb18e208925ce1ac7396322e741030bcd9bcae7e320e83f517dfe in / 
# Tue, 19 Jul 2022 22:39:42 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 05:51:06 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 20 Jul 2022 05:51:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.1/traefik_v2.8.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 20 Jul 2022 05:51:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 20 Jul 2022 05:51:12 GMT
EXPOSE 80
# Wed, 20 Jul 2022 05:51:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Jul 2022 05:51:14 GMT
CMD ["traefik"]
# Wed, 20 Jul 2022 05:51:15 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e0295fd11fe28fc9d5438734f4d9560cce203f9c2dc12b26e0cfd0c1c02548f7`  
		Last Modified: Tue, 19 Jul 2022 22:40:33 GMT  
		Size: 2.7 MB (2716890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c83ed61f2b6e81a94fc8cd3b45f4907c236ccf21eea420ad12565a7173d3bf`  
		Last Modified: Wed, 20 Jul 2022 05:52:23 GMT  
		Size: 668.4 KB (668407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18238a0191c876d3d7d620cf0a15bde5652dcc3adddce6ea511db69224bc730b`  
		Last Modified: Wed, 20 Jul 2022 05:52:27 GMT  
		Size: 25.6 MB (25595267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3327bca13bcc8f1ea384f76d0bfc5c218ba61bab0dfffccc724c6fb35fb1fcda`  
		Last Modified: Wed, 20 Jul 2022 05:52:23 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:vacherin` - linux; s390x

```console
$ docker pull traefik@sha256:4c24518f93d9c33aaac337c2abaf95c39c3ed4a5293c5edb4d3b4c2e371c3651
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30304413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fedbceaa29021adcf342427ae2641e95594b6809ce028c2b17a603298e267a18`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 19 Jul 2022 22:41:55 GMT
ADD file:9671b14d87fd7602279c1b3d1148babaa2c411e4ab0570d294d95324fa19210c in / 
# Tue, 19 Jul 2022 22:41:56 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 01:44:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 20 Jul 2022 01:44:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.1/traefik_v2.8.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 20 Jul 2022 01:44:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 20 Jul 2022 01:44:35 GMT
EXPOSE 80
# Wed, 20 Jul 2022 01:44:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Jul 2022 01:44:36 GMT
CMD ["traefik"]
# Wed, 20 Jul 2022 01:44:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ef614dc1febe442e84bcc0f287628aea0f6547a0f322d7bed0a46ffabd5e0a50`  
		Last Modified: Tue, 19 Jul 2022 22:43:17 GMT  
		Size: 2.6 MB (2600789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b79af282487d4dd2fe64cc2d5529f61de3c7f86ff71841f2a54452117c1f4a`  
		Last Modified: Wed, 20 Jul 2022 01:45:01 GMT  
		Size: 672.6 KB (672597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71eb729d3ee6a234a1296df8b97b82e847a58c7c8a4a966fc76bca83de8890ac`  
		Last Modified: Wed, 20 Jul 2022 01:45:06 GMT  
		Size: 27.0 MB (27030659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69245f1bfeb3ab0728514ea63fb3f9ed925bccce38455a77ccfed46332250a7d`  
		Last Modified: Wed, 20 Jul 2022 01:45:01 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
