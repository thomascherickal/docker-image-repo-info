## `docker:latest`

```console
$ docker pull docker@sha256:e496f1729171f76a9b1a9b2a99431003e8e89e67168ed411ad25b95a73445d13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:35f612c47195c6e7c1e9ecc80c1b1a00402f3c039e768dd08b2ddb237fd5d0ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66151138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f67ee0b7de2f5cca0d60fe996f082ee6795d35fdd0c7823325b0f7855f57c342`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:26:39 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 00:26:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:26:40 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 00:26:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 00:26:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 00:26:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 00:26:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 00:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 00:26:48 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de31523ae09475f6d68e873b416f497c2bd9a92224d9dc9224e1ec4c0a6066e`  
		Last Modified: Wed, 01 Sep 2021 00:27:41 GMT  
		Size: 2.1 MB (2051151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856ddc4bf6a58ca53ceb6444141995979c00718b20dae8c849231fcf9bfae27`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2117e19917ef5839774785d348adb2ff996bccac5f12d461ca21ecfd58283314`  
		Last Modified: Wed, 01 Sep 2021 00:27:51 GMT  
		Size: 61.3 MB (61284048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53eeb058f8c3c25c5b9f9d12769ab386c353b9f48506daae8fdebd88a33a21`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9223565313e3813eda94fc3641a51cdd88a37775e7b9817ada2a57bd45050906`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa82c493f72cf1d33f4a0bd90320bdb1923957f3cb3b0d36596f52bad68ecb4`  
		Last Modified: Wed, 01 Sep 2021 00:27:38 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:cbad49f1637b08b224d3bb36e840cc869624bbe08b359763bd6ada7026165403
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60193296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51720a73bc2639cb36d62b9239b6db9903861e48a613e6202cfc1224065d5c3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 12:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 12:09:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 12:09:34 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 01 Sep 2021 12:09:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.8.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.8.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.8.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.8.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Sep 2021 12:09:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Sep 2021 12:09:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Sep 2021 12:09:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Sep 2021 12:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 12:09:39 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a21b349a3936e2b00dec57a9db1f448fc4a1a7a3f4ce187cab93819f045fb35`  
		Last Modified: Wed, 01 Sep 2021 12:11:04 GMT  
		Size: 2.1 MB (2058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd93908d94fd730b48322ef41072abf6ba75634aeca40153ef133aae9700fbf4`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2566d8104302856d2cfd150c099a6c900ecc92f214478aa574d755afc6ce191`  
		Last Modified: Wed, 01 Sep 2021 12:11:11 GMT  
		Size: 55.4 MB (55420371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0dc4a2cf61d4525db0351dcde1cc47f8005d1f7260470032b1b731c75757f6`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90454e11d6bb4b836cd9f026908873ed60d1f7e76b2cbcde812fcabe652fa8d`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a170ef51809d6a08fc091d84fc936b83c0aa5c141c7d0cf8ec41c885a79808`  
		Last Modified: Wed, 01 Sep 2021 12:11:01 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
