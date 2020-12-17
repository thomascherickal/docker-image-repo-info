## `traefik:livarot`

```console
$ docker pull traefik@sha256:3a9a07795fae38994e905de5fc3c55e4210232dc31df2a5103702081e5ee6409
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:livarot` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0464505a5542f0c35a80906488d4f17acc8bc062ac5480abcdba5961e85dedef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27107202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a44b18ddf6ab462a4af8dbedfb58eaca6b7002622164563c3c18128b35078e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:26:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:26:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:26:02 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:26:03 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:26:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab096bb24791df9de14fbfc840265a32c0d9f7be463db3a782da6095c0e6ad5b`  
		Last Modified: Thu, 17 Dec 2020 00:27:24 GMT  
		Size: 674.9 KB (674902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a89144d2ec5013a820f4de949514c963d60f1eafac95fc5c0626ac3a5fca49`  
		Last Modified: Thu, 17 Dec 2020 00:27:32 GMT  
		Size: 23.8 MB (23811162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6633878abde02f77de69e78a3868c33a28300c0c47a47f81297473d9186bd156`  
		Last Modified: Thu, 17 Dec 2020 00:27:24 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:livarot` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:e1975275fbaf78b62a8a588b67d3ea3b72acc9ffcd47176cb4e987acf3f73c13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26736293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4646b0137cf051fe81afc86b698d2d8849446adda9ab81c8871f01b8c2e52d94`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:27:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:27:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:27:10 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:27:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:27:12 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:27:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278abd308a18c136f69dcabbba1dc64486ebdad665d4a2f4ab14d2826ec08b06`  
		Last Modified: Thu, 17 Dec 2020 00:28:38 GMT  
		Size: 673.2 KB (673246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c978289529e0d75adc45110a61b13d8d3791c39eda7bc74272d02afce9d584`  
		Last Modified: Thu, 17 Dec 2020 00:28:46 GMT  
		Size: 23.3 MB (23337462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade89e86f523ff8f8f95973a320cd860a913d5aac0df71602635b88f488a3567`  
		Last Modified: Thu, 17 Dec 2020 00:28:38 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
