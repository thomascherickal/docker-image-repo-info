## `docker:latest`

```console
$ docker pull docker@sha256:ddf0d732dcbc3e2087836e06e50cc97e21bfb002a49c7d0fe767f6c31e01d65f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:c9fe80d9eb030d771811e9cefcf2e3cb73aad845c24eee8e29b72b4429fae283
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66536142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51453dcdd9bd51e503f75e6d42a4071469ad2ba816321781985041b6bc7776db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:20:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:20:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:20:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:20:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:20:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:20:43 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:20:44 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:20:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:20:44 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b94fafbd542a8c279f4a08e81fef317862b0fe3f604febe2fc2138886ba1d7`  
		Last Modified: Wed, 04 Aug 2021 21:21:53 GMT  
		Size: 2.4 MB (2438245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e3c9e6c132861fd24ac22906718bb610ebcf3912ade5e48a791ba8f85e5799`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc990f87bf12a7b8fb86c3003977468a14fb1a31e5bb0b500e8127ee4e6beb5`  
		Last Modified: Wed, 04 Aug 2021 21:22:03 GMT  
		Size: 61.3 MB (61284061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1436504743cc47a166b7964d591792b69e34aa1e3e07ef5d91f481fdb11f948d`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c526f01240b836e9645a2b2b629051c5e488d60b309d5f253adab7f2c45ed7`  
		Last Modified: Wed, 04 Aug 2021 21:21:50 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d263b0ed3ea3116c812ca5c542c5175ccb0c99bee76b06db8c2340290057fa`  
		Last Modified: Wed, 04 Aug 2021 21:21:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:202f4fd8f1bc62e516f42f1f32d205a6d9dc12a5eddf42be5adda612331f7d99
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.6 MB (60592580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:917aa76b39804498915883c81d9c3f4616dafbae602e0e81597852ab6905bc77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 04 Aug 2021 21:40:35 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 04 Aug 2021 21:40:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 04 Aug 2021 21:40:35 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 04 Aug 2021 21:40:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Aug 2021 21:40:39 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:40:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Aug 2021 21:40:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Aug 2021 21:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:40:41 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d668eead8965ee8f4a1cd65de2a1cde9c49cfd2c2f06ac2290e0b90724ba4ea3`  
		Last Modified: Wed, 04 Aug 2021 21:42:32 GMT  
		Size: 2.5 MB (2458333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7010a04da6233aa993b677900fe12554cb30e4b12adeee36a2c884d5c0ec8965`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c06e26407aeefb6fd4953cb12e19c70695281c4c9ab4e9b8120734669094a8a`  
		Last Modified: Wed, 04 Aug 2021 21:42:39 GMT  
		Size: 55.4 MB (55420354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e4b73ac390f4f52af96ffa7e98228c80619fa25bd61e862485f64b509a849`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627ac7844e75fc94ea8963915c871cb5e376af3631da0ce14bf5a5662813175f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be33fcd733ebf68f8983483238e2245237efdc7751c83d98e9ce9b6a0f3069f`  
		Last Modified: Wed, 04 Aug 2021 21:42:29 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
