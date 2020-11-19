## `docker:rc-dind-rootless`

```console
$ docker pull docker@sha256:3b9c83b077c87237b35ae7a745aae360d60412424a5c9168432c282c8f3a64c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:rc-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:b3ff9bb04af9c8792a5af4e544aac96b05d7428e21c73c5361fe7d47e538f84d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.7 MB (103704599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02576142c5f47a6bce85cd79b31c5286da7dc8e758851840452b282231bc35c5`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:15:43 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 22 Oct 2020 03:15:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 19 Nov 2020 07:37:54 GMT
ENV DOCKER_VERSION=20.10.0-rc1
# Thu, 19 Nov 2020 07:38:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.0-rc1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.0-rc1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.0-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.0-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 19 Nov 2020 07:38:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 19 Nov 2020 07:38:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 19 Nov 2020 07:38:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 19 Nov 2020 07:38:02 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 19 Nov 2020 07:38:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Nov 2020 07:38:02 GMT
CMD ["sh"]
# Thu, 19 Nov 2020 07:38:09 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 19 Nov 2020 07:38:10 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 19 Nov 2020 07:38:10 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Thu, 19 Nov 2020 07:38:11 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 19 Nov 2020 07:38:11 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Thu, 19 Nov 2020 07:38:12 GMT
VOLUME [/var/lib/docker]
# Thu, 19 Nov 2020 07:38:12 GMT
EXPOSE 2375 2376
# Thu, 19 Nov 2020 07:38:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 19 Nov 2020 07:38:12 GMT
CMD []
# Thu, 19 Nov 2020 07:38:18 GMT
RUN apk add --no-cache iproute2
# Thu, 19 Nov 2020 07:38:19 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 19 Nov 2020 07:38:20 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 19 Nov 2020 07:38:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-20.10.0-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Thu, 19 Nov 2020 07:38:23 GMT
ENV ROOTLESSKIT_VERSION=0.11.0
# Thu, 19 Nov 2020 07:38:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Thu, 19 Nov 2020 07:38:36 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 19 Nov 2020 07:38:36 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 19 Nov 2020 07:38:37 GMT
USER rootless
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7c675703d60dc4d757acb40557350159f600ca3d49e2e8d4c2039dd6b69457`  
		Last Modified: Thu, 22 Oct 2020 03:16:47 GMT  
		Size: 2.0 MB (2039054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8c12a437cbe4e104dcea425e0ce277a2442603e14551d22a948e11026ae658`  
		Last Modified: Thu, 22 Oct 2020 03:16:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6fa0586cfb6c5924e8edbb8d8f5523ad9adffff171d2931a942827c650fc2a0`  
		Last Modified: Thu, 19 Nov 2020 07:39:38 GMT  
		Size: 69.0 MB (69019262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e467ed24859bdb6a61ea4868f70a19b2cc04dbb288642693dd0161026f752ef4`  
		Last Modified: Thu, 19 Nov 2020 07:39:25 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4d023e83c4b34234560f672657470bf941327c2d1735ee0edc2a89d59d0ecd`  
		Last Modified: Thu, 19 Nov 2020 07:39:24 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352f35817c2a388754c79bb1967ae2078b3a4efcf3be0ee43ef8e38eb553652a`  
		Last Modified: Thu, 19 Nov 2020 07:39:25 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d7623eac95c311571301e30165f238a32aef69630d02e30ce51229446b1975`  
		Last Modified: Thu, 19 Nov 2020 07:39:51 GMT  
		Size: 6.0 MB (5958667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84238371d566e2d9ff5cbbcd2d8f7bd7188e7e6db61b25b21901e22173d7ad8b`  
		Last Modified: Thu, 19 Nov 2020 07:39:49 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc4c0ca8bf70af12ff734901b3b78880f73c7a796ed2167c994cf706fcb9313`  
		Last Modified: Thu, 19 Nov 2020 07:39:49 GMT  
		Size: 931.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bcb07ec5643c524f1fad066f97b23b45a65ff5b837b178e2636c60e69dfd39`  
		Last Modified: Thu, 19 Nov 2020 07:39:49 GMT  
		Size: 2.5 KB (2511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f18993919ba9d76198f233647f214d16a07346f6f4e042604cc2cd947ac7954`  
		Last Modified: Thu, 19 Nov 2020 07:39:57 GMT  
		Size: 1.1 MB (1092661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016fec4edfae6601a46a6c3316126abf8b96a74b890b299f33627e1a9372ccf0`  
		Last Modified: Thu, 19 Nov 2020 07:39:56 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d819179e26d202b1915d81534f8883b1226d0bf9d747c210b483d90e26c03e`  
		Last Modified: Thu, 19 Nov 2020 07:39:56 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beee953df4d562d41db45e3676d56e86f07cfa2d498ad4098fe8d4841af759fe`  
		Last Modified: Thu, 19 Nov 2020 07:39:58 GMT  
		Size: 9.9 MB (9861309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b063068313907fa155ae542bd7aa88fea531c837e496664e436fa7136373ff14`  
		Last Modified: Thu, 19 Nov 2020 07:39:58 GMT  
		Size: 12.9 MB (12928611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9165cddf4c0b627f34fd172c93b4da1086c336fdb4b11622dd9ef5bcf09de4f`  
		Last Modified: Thu, 19 Nov 2020 07:39:55 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
