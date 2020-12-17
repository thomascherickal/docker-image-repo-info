## `docker:dind-rootless`

```console
$ docker pull docker@sha256:4943cc5bdd2f76f357abbc3bbfffa12502670bdc21f004022e8683368699b536
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:4c9081a5aa82d47e6d25242da1255c52939a3c720e4ec1a593768a2da6e34d27
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.6 MB (101564903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a0decd6352f07dd3329a8e291269ed11bae53216c7fbf35e8f9e51aacd43f95`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 12:37:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 17 Dec 2020 12:37:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 12:37:41 GMT
ENV DOCKER_VERSION=20.10.1
# Thu, 17 Dec 2020 12:37:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Dec 2020 12:37:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Dec 2020 12:37:50 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Dec 2020 12:37:50 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Dec 2020 12:37:51 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Dec 2020 12:37:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 12:37:51 GMT
CMD ["sh"]
# Thu, 17 Dec 2020 12:38:01 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 17 Dec 2020 12:38:03 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 17 Dec 2020 12:38:03 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Thu, 17 Dec 2020 12:38:05 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 17 Dec 2020 12:38:05 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Thu, 17 Dec 2020 12:38:05 GMT
VOLUME [/var/lib/docker]
# Thu, 17 Dec 2020 12:38:06 GMT
EXPOSE 2375 2376
# Thu, 17 Dec 2020 12:38:06 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 17 Dec 2020 12:38:06 GMT
CMD []
# Thu, 17 Dec 2020 12:38:14 GMT
RUN apk add --no-cache iproute2
# Thu, 17 Dec 2020 12:38:15 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 17 Dec 2020 12:38:17 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 17 Dec 2020 12:38:21 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 17 Dec 2020 12:38:22 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 17 Dec 2020 12:38:23 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 17 Dec 2020 12:38:23 GMT
USER rootless
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7dc993c79e722bfe2e7f64e7ae30964b200440f94deec6b702314e2c4e233a`  
		Last Modified: Thu, 17 Dec 2020 12:40:18 GMT  
		Size: 2.0 MB (2039162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39d95e4997fdf86ea798b96fad5c5eab74bed43cd512a3ecd5dfb4f48bc2371`  
		Last Modified: Thu, 17 Dec 2020 12:40:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cda4b703d87f5d062260330aa79bd174ca70549ef23c2f284d83aa7d36f7508`  
		Last Modified: Thu, 17 Dec 2020 12:40:35 GMT  
		Size: 69.5 MB (69456732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e5375350ea7018edc6b0935306c6df9a61fff1f7f37130d1b2d6c6b1dd3404`  
		Last Modified: Thu, 17 Dec 2020 12:40:15 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08cd1b3bb1bdaeb5122182eb4b4bc748d262194fcdd465cd8d789b241c116fb`  
		Last Modified: Thu, 17 Dec 2020 12:40:15 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e17d04e0c68820c8081496201fedef93af8edb4f5b1cf73e57959294b140f60`  
		Last Modified: Thu, 17 Dec 2020 12:40:15 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fab333a5ce91c4921b6ee687f61ae6ce3a8ad97f25dbeb882d62b6fd07c588`  
		Last Modified: Thu, 17 Dec 2020 12:40:46 GMT  
		Size: 6.0 MB (5997583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc477ada5f22b481a6edc6df8b2230b4772e776401a02fe2c768e83fb3a1e75`  
		Last Modified: Thu, 17 Dec 2020 12:40:46 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f57ce55fb4f023f15164a0f59b158c823b693a446df780638ef123a752c84aa`  
		Last Modified: Thu, 17 Dec 2020 12:40:44 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e22f9cd8f9fcb6f6da3aa140b3367e4ff154289a05a0bf86c7f57718559cce`  
		Last Modified: Thu, 17 Dec 2020 12:40:45 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3b3243eb4f6ea4312aa8e3bbc06fb355f1e337514c5f9975df3ebaf48d2c7a`  
		Last Modified: Thu, 17 Dec 2020 12:40:55 GMT  
		Size: 1.1 MB (1092840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81d89c022699c10767179f6f92d94caab77fb163fae189230bf796e1f0490be`  
		Last Modified: Thu, 17 Dec 2020 12:40:55 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e167115e3058c83b5e2ecb7423b7ed5cfa70ca5cd1f912e511bfd6c8f4f28b9`  
		Last Modified: Thu, 17 Dec 2020 12:40:55 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9e5cbb9f53ece24b94f5fd41faeabccb258150b38d8903540b0376b75513c4`  
		Last Modified: Thu, 17 Dec 2020 12:41:01 GMT  
		Size: 20.2 MB (20171366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b473ac371011cf55fc226f0b6fb746da0458af89482cc4e923c0fe9f67ecf3f8`  
		Last Modified: Thu, 17 Dec 2020 12:40:55 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
