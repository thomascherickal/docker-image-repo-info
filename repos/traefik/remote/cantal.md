## `traefik:cantal`

```console
$ docker pull traefik@sha256:825521d793f572a3944787c134468017fdd719340fba06be53c33382e33b5ed1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:cantal` - linux; amd64

```console
$ docker pull traefik@sha256:b648fb36b8b7a16c29b17098ab0d4e3d6b690f3743113d5715b476a86c0c6eb6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23078678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc73dafdaf77f021af5d6e11d26485ef404c9c448041d04e2ab64c02085b45fb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:23:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.7/traefik_v2.1.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:23:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:23:25 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:23:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:23:26 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:23:26 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c141e361698e17a696b4b6bccfed69dc1eb931474405e31a0c907c01f4e272a6`  
		Last Modified: Thu, 06 Feb 2020 23:44:04 GMT  
		Size: 694.2 KB (694182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23d352c6a6b6e399956a83e278cfbf4a6ee13202799f970464fb64a83191572`  
		Last Modified: Wed, 18 Mar 2020 21:24:15 GMT  
		Size: 19.6 MB (19581171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36778517a2cb14855119773806f3a6beab6c4e85b1dcf74981e652d0079561a9`  
		Last Modified: Wed, 18 Mar 2020 21:24:10 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:cantal` - linux; arm variant v6

```console
$ docker pull traefik@sha256:d4a0b779bb40f2148d63a9431422cdd9a641c74ef1fcea23de774e454d0aa433
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 MB (21652564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48ee9f0382c3f27923bbd3252f34486b585e3294b5b5825cf10dd3a21bd41d9c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 19 Mar 2020 23:23:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 19 Mar 2020 23:23:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 19 Mar 2020 23:23:51 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:23:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Mar 2020 23:23:55 GMT
CMD ["traefik"]
# Thu, 19 Mar 2020 23:23:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a045f3facd048d78ccec1317c0b8d3aa5e1b76f175b643f80c704ec2aa89f8`  
		Last Modified: Thu, 06 Feb 2020 22:51:40 GMT  
		Size: 698.0 KB (698013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53885d3a3b2b3c65397006830e2537614bdb892855376d49405c3d3f57b156f3`  
		Last Modified: Thu, 19 Mar 2020 23:24:51 GMT  
		Size: 18.3 MB (18336621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcd6f2d908241954732cb48c247880bdeaeb4c9941514c06bb5e01a406312c7`  
		Last Modified: Thu, 19 Mar 2020 23:24:45 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:cantal` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:064fbe4896c26fce414a7df2df0a3b0571ccefb73366b2739112b52612ebbf14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21453551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eaee0200df033a74b1986f9d77ef02c0efbe5323827d25b39c8481656d1a114`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 20 Mar 2020 01:08:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 20 Mar 2020 01:08:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 20 Mar 2020 01:08:51 GMT
EXPOSE 80
# Fri, 20 Mar 2020 01:09:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 Mar 2020 01:09:09 GMT
CMD ["traefik"]
# Fri, 20 Mar 2020 01:09:13 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5c788179332343fbcbc8b97673406752232ca36894176cc87ece20ee279754`  
		Last Modified: Thu, 06 Feb 2020 22:47:56 GMT  
		Size: 696.0 KB (696043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90c65e62bd1d8a41d60336854858745d85736586b37abe6790a7a6d6f5181ad`  
		Last Modified: Fri, 20 Mar 2020 01:10:09 GMT  
		Size: 18.0 MB (18034065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9bae08bcb1e759e95d0a6764537920273d6cb4815345c68f8682589d015a87`  
		Last Modified: Fri, 20 Mar 2020 01:10:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
