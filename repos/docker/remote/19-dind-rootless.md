## `docker:19-dind-rootless`

```console
$ docker pull docker@sha256:a6152484a8e8af2329cc26df57cace457d1052dbc2f44c51a44bc9083cb3a3e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:bd727ccfdb78901f0b8c5af62514ad5be08c3923af36d5aaf456798d353b98fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94876824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f69a27115b15433406b5620b969066c9e48e5e77109fc8e1b57ef3c206328101`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 07:56:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 26 Mar 2021 07:56:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 07:56:36 GMT
ENV DOCKER_VERSION=19.03.15
# Fri, 26 Mar 2021 07:56:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 26 Mar 2021 07:56:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 26 Mar 2021 07:56:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:56:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 26 Mar 2021 07:56:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 26 Mar 2021 07:56:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 07:56:42 GMT
CMD ["sh"]
# Fri, 26 Mar 2021 07:56:48 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 26 Mar 2021 07:56:49 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 26 Mar 2021 07:56:49 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 26 Mar 2021 07:56:50 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 26 Mar 2021 07:56:50 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:56:51 GMT
VOLUME [/var/lib/docker]
# Fri, 26 Mar 2021 07:56:51 GMT
EXPOSE 2375 2376
# Fri, 26 Mar 2021 07:56:51 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 26 Mar 2021 07:56:51 GMT
CMD []
# Fri, 26 Mar 2021 07:56:56 GMT
RUN apk add --no-cache iproute2
# Fri, 26 Mar 2021 07:56:57 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 26 Mar 2021 07:56:58 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 26 Mar 2021 07:57:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 26 Mar 2021 07:57:02 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 26 Mar 2021 07:57:02 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 26 Mar 2021 07:57:02 GMT
USER rootless
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8aba36c48bdd8a8a32e7d5f4a2f99baaf3cfcb07d9252c9c24ce06689a7152`  
		Last Modified: Fri, 26 Mar 2021 07:57:44 GMT  
		Size: 2.1 MB (2050069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42621afb2e170dae0ffca17d04117dcc72ee595bd65f98cb2346740a7281213`  
		Last Modified: Fri, 26 Mar 2021 07:57:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79bfa1e09b72cbe22b1b15c677bc84ceff4f5f16383a865a99bd0e04f6b2c27a`  
		Last Modified: Fri, 26 Mar 2021 07:59:24 GMT  
		Size: 62.9 MB (62882883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430fc81349c52eafdb1973bfb700cff202efb978dd184f56936d68f4754c835a`  
		Last Modified: Fri, 26 Mar 2021 07:59:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95f3b34476609ffc40451e019a41975f5fd573b230d16a2d70cdc2d31a2f22f`  
		Last Modified: Fri, 26 Mar 2021 07:59:12 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e3a3462c5bc415caac7ca73b74233461c5090e4c8bf72e532505ef7f4cf4dc`  
		Last Modified: Fri, 26 Mar 2021 07:59:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5749248f6d3090be71a5dfd9d919a071f5936744a87bc83a2773f38aac4e596`  
		Last Modified: Fri, 26 Mar 2021 07:59:38 GMT  
		Size: 6.6 MB (6569605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723c9d0b375aaa551dedf236094280c32f18070c65ac37f7e97fffb349a8131d`  
		Last Modified: Fri, 26 Mar 2021 07:59:37 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022372389676eced15d18f3e95c5be832fd2d3d8989e8907fbfef987ca909bbb`  
		Last Modified: Fri, 26 Mar 2021 07:59:38 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cf2688b2e31714c690359dd7773f5027e27da375f542460808cbed4c4841f4`  
		Last Modified: Fri, 26 Mar 2021 07:59:37 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed554b6c9e84215a1851a3ab05580c95edf8332ac6d96d08f867e854653d5e82`  
		Last Modified: Fri, 26 Mar 2021 07:59:56 GMT  
		Size: 1.1 MB (1131565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e56ae877c08df68055ee4b013eedaf284ff62847acc879a91cef4bb4078ed4f`  
		Last Modified: Fri, 26 Mar 2021 07:59:56 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67366e4fc018a763f8b42b20f9313e9fa5fd64433e6cd5e36a920ed76e8bfb1`  
		Last Modified: Fri, 26 Mar 2021 07:59:59 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb06fc7e4fcd089a36bf6b60d093eaf7597d9fc938ebdf3842d047dc757b90c`  
		Last Modified: Fri, 26 Mar 2021 08:00:00 GMT  
		Size: 19.4 MB (19422710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d28e7234f41cdf119798c5e50c10222a36086f7204a40483f3b622e230ca44d`  
		Last Modified: Fri, 26 Mar 2021 07:59:56 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
