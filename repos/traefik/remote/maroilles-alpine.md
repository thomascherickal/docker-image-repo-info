## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:72a0a55d0421c747b7f032ac8ce8f7223aed5b9af84d8faa4a0e4d8fa28a4297
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:3cbe9e62ef26a9ac17b25702754dfbf56dd346850170be90eabd370f24190ef1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24634355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c36f69007d987e4ed093711f4f306b52ce63b1c19f5ffacd49a1aea1f717e527`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Jul 2020 00:20:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Jul 2020 00:20:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Jul 2020 00:20:25 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:20:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Jul 2020 00:20:26 GMT
CMD ["traefik"]
# Wed, 29 Jul 2020 00:20:26 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16506d32a25436b458a7f443ec1ca0d096d99d3479523c92c247856fc6148c0`  
		Last Modified: Fri, 24 Apr 2020 17:34:15 GMT  
		Size: 694.1 KB (694148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb03716fa366c58de14b0fc81a50daf51f39175c928558e3e82017b5999f233`  
		Last Modified: Wed, 29 Jul 2020 00:21:23 GMT  
		Size: 21.1 MB (21126524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c61f1414a3fbacefede004c9c340def8b1c393630a1c2241a0c9196692c574`  
		Last Modified: Wed, 29 Jul 2020 00:21:19 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0494095125ba05e297b154e0827115ae0618b70d40ccce4b1c496ce1666ce43d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23069021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6d3de75d11f16c38ae16a31868fe6680c4f4f196bcab0eab4ca1f85c3d9d6f0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:26:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:26:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:26:35 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:26:37 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:26:39 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8bed822566f883c529e4423ed5efb201104f66147671cd72a5a80db2e5609dce`  
		Last Modified: Thu, 17 Dec 2020 00:28:20 GMT  
		Size: 19.8 MB (19772981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c867ecec8c478367249ed7ccc513e1c496aa5d628bd9950ed8ad87e604f4d`  
		Last Modified: Thu, 17 Dec 2020 00:28:14 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:91c6f4a7270971b010691e5a21e487ac6d85bfbb85b83237a02dfb5c82f35055
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22891964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3f47993d5e498f1e77ebd9467c190b17085ea5862b5fb1049ebbaf278fcd434`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:27:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:27:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:27:44 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:27:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:27:46 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:27:47 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6be00c7721dc4a904b3531bfb7878ea6761d57116b3730c05eac3cb31e726a7e`  
		Last Modified: Thu, 17 Dec 2020 00:29:37 GMT  
		Size: 19.5 MB (19493133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d0080e4ada531446b01e45e014d2c9983281dc58b873e4162e1adb99b6f3ad`  
		Last Modified: Thu, 17 Dec 2020 00:29:20 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
