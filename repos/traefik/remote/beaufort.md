## `traefik:beaufort`

```console
$ docker pull traefik@sha256:83e7b36fbe4096887d144ba82c51b891893ad3eb5f891daf300f5cf49b9d61d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:beaufort` - linux; amd64

```console
$ docker pull traefik@sha256:a239deca1c7682fe9bb6a32e54364c7ff460205fa0e87c02bfeb66efb3f3a3d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42fc5a7c2d34a752fce6439cf3dc08ac747649d7712bc265c7dd7d1b38a2a45b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 02:37:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 02:37:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 02:37:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:37:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 02:37:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11624eb8d0cca298aa32848e39318bbc75ab1c404423d1d47c670fa60354e3`  
		Last Modified: Thu, 30 Mar 2023 02:38:16 GMT  
		Size: 661.1 KB (661099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9d40a9765a3ede8e4ec67030b20d484fedcea2ad98ee2b231ec3d86e6fd1b6`  
		Last Modified: Thu, 30 Mar 2023 02:38:21 GMT  
		Size: 37.1 MB (37074890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fca61e22e5a1dbbdeea08d3e394601c2c5492fc65d19af813ef66cc36a7d582`  
		Last Modified: Thu, 30 Mar 2023 02:38:15 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0e010dd7b60c3960f903b07854cae707e691496f1491f0447ca2635b5a374a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee0012c6d54cfd4da66d0da5e01f3dc4f70609eec928ce429e71a5efa02c96b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:32 GMT
ADD file:b987db82fa4ce6e623de49a50612c1fd91c5ab2209a62a5727ab3436c2923e91 in / 
# Wed, 14 Jun 2023 18:49:32 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:12:22 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Jun 2023 20:12:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Jun 2023 20:12:26 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Jun 2023 20:12:26 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:12:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:12:26 GMT
CMD ["traefik"]
# Wed, 14 Jun 2023 20:12:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:41c5c5b38e13af18def277385607129664fb24993d262d4b601a381e776482a9`  
		Last Modified: Wed, 14 Jun 2023 18:50:19 GMT  
		Size: 2.6 MB (2633060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718cfe2cb66c053a8fdb09adf88b20a52f260f22abd38cba68cc2838ee33e73d`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 666.3 KB (666349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b2cef5f2c79471c563b3c10376140084b51c097de00e9be0b758219ab95e5c`  
		Last Modified: Wed, 14 Jun 2023 20:12:52 GMT  
		Size: 35.0 MB (34989308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66078e59ed6730404193e57cea654480d0731663c7a068349344e0a681d1c660`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:529410986a68c6e7989a5a08afa53d087795a2f1406977d5d6b183bfdfab65dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37408212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e4bfdbd12bed1c2e46296bb16021a1eea4269055e03fdf9e30c035e5f9e8dc4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 03:26:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 03:26:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 03:26:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:26:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:26:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 03:26:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d019fab0470c352dfa2ff6c01be8f1d0344d43e9431a28656e78c5cabd03e67f`  
		Last Modified: Thu, 30 Mar 2023 03:27:17 GMT  
		Size: 662.3 KB (662323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ed46bb3966bf021d56f3bfda66ada1ddde7199ee9d3446ebcbeffec692004`  
		Last Modified: Thu, 30 Mar 2023 03:27:20 GMT  
		Size: 34.0 MB (34023520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a93ddfbde23c1aa20ccac6b7cd3dcbda52d11c2b1627d41dc7fa169bd46430`  
		Last Modified: Thu, 30 Mar 2023 03:27:16 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; s390x

```console
$ docker pull traefik@sha256:bbf1710b9a47f8ec5a04c849b5eabca1601d8c3d14771376db863d4bfb11267c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39132224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7797b8a6b1786adb45fd822e034429307f0e6d9835934dff30e1685c3d7253`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:07 GMT
ADD file:5cf392863cd9a0735de88f9e7dab93c9e74aca59ca05b792943cf3b621ea2c59 in / 
# Wed, 29 Mar 2023 17:42:07 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:57:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 09 May 2023 23:57:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 09 May 2023 23:57:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 09 May 2023 23:57:44 GMT
EXPOSE 80
# Tue, 09 May 2023 23:57:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 May 2023 23:57:44 GMT
CMD ["traefik"]
# Tue, 09 May 2023 23:57:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:1536575ac9c5f5fff4522c60d4610af0a52be584c36e652080c6c0ad169d4f27`  
		Last Modified: Wed, 29 Mar 2023 17:42:42 GMT  
		Size: 2.6 MB (2610636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7a4deefee64d3e0ac000d06c44544635381ead6c9ce624aad695fd76bdde33`  
		Last Modified: Tue, 09 May 2023 23:58:12 GMT  
		Size: 665.8 KB (665799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2ced6eac60c1c9707c57590d27e69315354f9d304ec2af3e7f07d5a2bec0b4`  
		Last Modified: Tue, 09 May 2023 23:58:18 GMT  
		Size: 35.9 MB (35855421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a1e76f2b69535b5f8ea9cdfda36f79ee2e5fd3194ee2e9ce12fd841672a09`  
		Last Modified: Tue, 09 May 2023 23:58:12 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
