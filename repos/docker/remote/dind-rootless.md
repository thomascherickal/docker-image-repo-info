## `docker:dind-rootless`

```console
$ docker pull docker@sha256:e90be351afbb3baf01bd108e8dfc98acd332fd051e921dd12f295302e491572c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:9ad12bb649463b45bb39481eba38b2f5c5cfe8471e571917329ee0c19171a71d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102536447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:caf7902297ee81e8f4a98bc43184eef9d19bf4952e03a7ccbbb840266a5c9976`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 21:43:03 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 17 Feb 2021 21:43:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 03 Mar 2021 01:19:43 GMT
ENV DOCKER_VERSION=20.10.5
# Wed, 03 Mar 2021 01:19:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.5.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 03 Mar 2021 01:19:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 03 Mar 2021 01:19:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 03 Mar 2021 01:19:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 03 Mar 2021 01:19:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 03 Mar 2021 01:19:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Mar 2021 01:19:53 GMT
CMD ["sh"]
# Wed, 03 Mar 2021 01:20:00 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 03 Mar 2021 01:20:01 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 03 Mar 2021 01:20:01 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Wed, 03 Mar 2021 01:20:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 03 Mar 2021 01:20:03 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Wed, 03 Mar 2021 01:20:03 GMT
VOLUME [/var/lib/docker]
# Wed, 03 Mar 2021 01:20:03 GMT
EXPOSE 2375 2376
# Wed, 03 Mar 2021 01:20:03 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 03 Mar 2021 01:20:03 GMT
CMD []
# Wed, 03 Mar 2021 01:20:10 GMT
RUN apk add --no-cache iproute2
# Wed, 03 Mar 2021 01:20:11 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 03 Mar 2021 01:20:12 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 03 Mar 2021 01:20:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.5.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 03 Mar 2021 01:20:15 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 03 Mar 2021 01:20:16 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 03 Mar 2021 01:20:16 GMT
USER rootless
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94caa5d1da7043140e78e14956c22154f75708f44c1c1367ac20cc5a8be71e8b`  
		Last Modified: Wed, 17 Feb 2021 21:44:58 GMT  
		Size: 2.1 MB (2051413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10a29983da5ea49c724d6c132f4d3dc6c130fe7148e4dd9fc258c34fa210f0a`  
		Last Modified: Wed, 17 Feb 2021 21:44:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6ccddb7fa4ac3d17b73897072eb4e290f303073edb0964e6d5a3becb9a5a0b`  
		Last Modified: Wed, 03 Mar 2021 01:21:21 GMT  
		Size: 69.7 MB (69692167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1bef566495d7c6876dfecd14cbc9ee0b2a6e37c3d7ccfacd026b1a7ed66d45`  
		Last Modified: Wed, 03 Mar 2021 01:21:06 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201a9d1142eb86ee5a02feb68aee88cb069648aecc92331f7b4b3d6c9f18b90f`  
		Last Modified: Wed, 03 Mar 2021 01:21:07 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0806b78d1f4d9cfd8d904285a1c970d39cd203456efff5a95d56cc4e435618dd`  
		Last Modified: Wed, 03 Mar 2021 01:21:06 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7487d64c1d39bfc63819823397c74bc5c52c38f37bb0c4ffcb33fc44ddc48f0f`  
		Last Modified: Wed, 03 Mar 2021 01:21:33 GMT  
		Size: 6.6 MB (6610330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3803ba42d066895fc25255ade0c56cf28fd9650f0063587c21999079e50bc679`  
		Last Modified: Wed, 03 Mar 2021 01:21:32 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b73e0fabdc06284aa9a34800e289cf9554d574088da3ff3deb4a793ee62b066`  
		Last Modified: Wed, 03 Mar 2021 01:21:34 GMT  
		Size: 936.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5243cc195ad1f275015542e2c511f843efcaa93fd8cbfcb7a8758e78b8a25ff2`  
		Last Modified: Wed, 03 Mar 2021 01:21:32 GMT  
		Size: 2.5 KB (2512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aeeb211d2628af12d3b579e655113e47922155c47bc5a07fbd342268eff00de`  
		Last Modified: Wed, 03 Mar 2021 01:21:41 GMT  
		Size: 1.1 MB (1131695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701f28e697dcd8ee0e8212ffa6682f93407d2a7d74a12ae5c3fd69cde5e37200`  
		Last Modified: Wed, 03 Mar 2021 01:21:40 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2436a5b1260df3d28fea105f34fb63adaca196a3550f623a23226e80d7163dd5`  
		Last Modified: Wed, 03 Mar 2021 01:21:41 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4328096dd57b14d68375e273f89aadd2dba6d9fece12047c33e2a5a657eb01`  
		Last Modified: Wed, 03 Mar 2021 01:21:44 GMT  
		Size: 20.2 MB (20231014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df05abb71f547db1b708838cb04c909b680f744921eceb2c67e3c212ffc545c`  
		Last Modified: Wed, 03 Mar 2021 01:21:40 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
