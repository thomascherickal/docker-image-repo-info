## `docker:20-git`

```console
$ docker pull docker@sha256:5b8f51320fb14ff3fbc45001d6477a8edc4155128fcd5dd4b7139294336e91fb
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
$ docker pull docker@sha256:7a2baddd024a7811ef67203d77de9ab3829ddca714ca6fe11f2ed2b3572fb5f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70154288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb42c0db861bb97af997256dc9ff427b43b0668bc7689aada6aa99ba4937b84e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:05:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 24 Mar 2022 05:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:05:37 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:05:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:05:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:05:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:05:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:05:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:05:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:05:48 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:06:28 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f777e60e93e1e25280d855dd6b0c8e7e7d1508b2cbd43b9678cd18b2bab72084`  
		Last Modified: Thu, 24 Mar 2022 05:07:13 GMT  
		Size: 1.9 MB (1938915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1b0eef4b739aafe07d37f6f0fc1850ff0b6f61ab14400a1b6348cd2c8b7186`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4e629eede4a3f517e93a1764b365c41b7b2d2554b27f9d6fa6c2e37473901`  
		Last Modified: Thu, 24 Mar 2022 05:07:20 GMT  
		Size: 58.6 MB (58565771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7213dc5eb38c445dc0cffd227536ad4e5265f45307b743d11d8eb43fbdd43c26`  
		Last Modified: Thu, 24 Mar 2022 05:07:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57979a88be1287b9ce5ca410359f13c10dea1b5859e7e42d1bed86fb996f2d6e`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44bdde740192774f34636311a0dbd2b1081ec88c6a24c81b246635938b65c1`  
		Last Modified: Thu, 24 Mar 2022 05:07:10 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a06e853d235302bea036f40c1af6580b1f35dccf8df3f8610cab630655e58ca`  
		Last Modified: Thu, 24 Mar 2022 05:08:26 GMT  
		Size: 6.9 MB (6933055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
