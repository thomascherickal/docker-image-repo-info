## `docker:20-git`

```console
$ docker pull docker@sha256:a15eae526cfdd27abd33ce9db6b5ee4fff5a1f38ff54b95348d9eea376d4c11c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-git` - linux; amd64

```console
$ docker pull docker@sha256:3728219f8cc46f4f397b330577000ca639d8324aa5a1556d0e6a5cf738ebe0ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76219858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b79097ab0874839ce4ef81b16354be702b88d942e0232d86af2acdc33e22b9bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:14:46 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 23 Mar 2022 16:14:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:19:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:19:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:19:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:19:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:19:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:38 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:19:57 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236b952b9466b604bbc4e060a2667d7a7a335bee006fd5104c151dbdb4bf787`  
		Last Modified: Wed, 23 Mar 2022 16:15:39 GMT  
		Size: 2.0 MB (1969538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580f7437ec44a9dd3670ee6fd964ecb068808106d1bd8b961e7a568ef3ceb4f`  
		Last Modified: Wed, 23 Mar 2022 16:15:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0577d395ae504f47fad1c4d36855a3577354d4f0eca32daf7e0b13cf768c17`  
		Last Modified: Thu, 24 Mar 2022 05:20:29 GMT  
		Size: 64.6 MB (64611627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a33444f604b483769f304acdb1c976a4ea78d16943f3be3f9814e1a1e495f`  
		Last Modified: Thu, 24 Mar 2022 05:20:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8453fa1b01e46b0305c4d091304622803430cc8d0b3edb47c7be3a951e62e3`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e8e864d7d32b260f5ca60b2065242e7c51ccaa371f2cc9807d0c32b2ec06f`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8260489be308ed8266d2c832c405abe7c01809d417bf17b473ec0f0f37339134`  
		Last Modified: Thu, 24 Mar 2022 05:21:32 GMT  
		Size: 6.8 MB (6824140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:dc915cbe95f635e80584b41c3d800a495fa492211fe98af0ba24868f73b1522c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70155890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1420a43cf047a2037e665447c200d167cec0cfd12cec229b21eaf5f7d1c9310c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:26:13 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 29 Mar 2022 08:26:14 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 08:26:15 GMT
ENV DOCKER_VERSION=20.10.14
# Tue, 29 Mar 2022 08:26:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 29 Mar 2022 08:26:23 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 29 Mar 2022 08:26:24 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 29 Mar 2022 08:26:24 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 29 Mar 2022 08:26:25 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 29 Mar 2022 08:26:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 08:26:27 GMT
CMD ["sh"]
# Tue, 29 Mar 2022 08:27:09 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab8992fcbba1f8070f63d991ae72bed38408b25db7ffa00f7221352fe9275c5`  
		Last Modified: Tue, 29 Mar 2022 08:27:55 GMT  
		Size: 1.9 MB (1938918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afedb10a1343d3055a1a213063d8f8f6ea1882b01069a44faf0453b0041a802d`  
		Last Modified: Tue, 29 Mar 2022 08:27:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f3009765e88f09be3c6e87a57258d5bea877cf248e4b0a6acd198692f300ef`  
		Last Modified: Tue, 29 Mar 2022 08:28:02 GMT  
		Size: 58.6 MB (58565750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae115253e7c71f61aa1bcdfde46cc38e0de6c3fb34bf4d1cebeca0b9bc91cc4`  
		Last Modified: Tue, 29 Mar 2022 08:27:52 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb3afcdfd642c0cd2ac3c0e03dfccaf3352874a7ccf06e91ce2e8c9d5a5a513`  
		Last Modified: Tue, 29 Mar 2022 08:27:52 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971d2cdfcd569d13d88d038acf7b68fdc926a532b0f7e7480c3c80ebcf05bd31`  
		Last Modified: Tue, 29 Mar 2022 08:27:52 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e84da3ac4c997d7b350e908b8516ae22d0523bf8b7c0844b94ae73a7079f50`  
		Last Modified: Tue, 29 Mar 2022 08:29:07 GMT  
		Size: 6.9 MB (6933045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
