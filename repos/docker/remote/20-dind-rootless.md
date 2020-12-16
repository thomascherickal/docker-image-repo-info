## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:bc36ee50418f68b28bb5337fe4084c4db06436e5019bb65fe1a878625e27fbe7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:ba20ea6047ede4866cbb74c9ece64a69ab8aaff2e6ddd1c9ecc6069241ac4278
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.6 MB (101562918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c231d166fd1199c71fda54408e75113ceca394c05a1575e4e76c787093fa30e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Dec 2020 22:21:37 GMT
ENV DOCKER_VERSION=20.10.1
# Tue, 15 Dec 2020 22:21:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Dec 2020 22:21:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Dec 2020 22:21:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Dec 2020 22:21:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Dec 2020 22:21:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Dec 2020 22:21:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Dec 2020 22:21:45 GMT
CMD ["sh"]
# Tue, 15 Dec 2020 22:21:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 15 Dec 2020 22:21:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 15 Dec 2020 22:21:53 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 15 Dec 2020 22:21:54 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 15 Dec 2020 22:21:54 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 15 Dec 2020 22:21:54 GMT
VOLUME [/var/lib/docker]
# Tue, 15 Dec 2020 22:21:55 GMT
EXPOSE 2375 2376
# Tue, 15 Dec 2020 22:21:55 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 15 Dec 2020 22:21:55 GMT
CMD []
# Tue, 15 Dec 2020 22:22:00 GMT
RUN apk add --no-cache iproute2
# Tue, 15 Dec 2020 22:22:01 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 15 Dec 2020 22:22:03 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 15 Dec 2020 22:22:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 15 Dec 2020 22:22:06 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 15 Dec 2020 22:22:06 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 15 Dec 2020 22:22:06 GMT
USER rootless
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3104fdc50d02e0ce25e706d856e429c2c2b8296f5c0a9fff000d348e68021f4`  
		Last Modified: Tue, 15 Dec 2020 22:23:04 GMT  
		Size: 69.5 MB (69456740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e67d69e12ccdaf1f4ef6a7c0488b4f79f8a990ce16571bb6c5dd21718e508d`  
		Last Modified: Tue, 15 Dec 2020 22:22:50 GMT  
		Size: 538.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ede2b221ee48511ff2dc4b5d89f5fa4982cd016ac2bb8b0544d12ecdb83a05d`  
		Last Modified: Tue, 15 Dec 2020 22:22:51 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc74c0d5b7997aff9f0ba940d9f55335a2f665fcaba7d94de0e314f64d3ca793`  
		Last Modified: Tue, 15 Dec 2020 22:22:50 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a38d9b7fa1495ede4f541ad3e1d64d014e30a5cfa96367a2240d6f782faf7f`  
		Last Modified: Tue, 15 Dec 2020 22:23:14 GMT  
		Size: 6.0 MB (5997804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d878abb54a31ff5221da4f06fee86097a76d281f74e060089111d81fe241bd73`  
		Last Modified: Tue, 15 Dec 2020 22:23:14 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9478721dbc0d87887da131761e1d440c150b97dc72dad739e52b1ca1937ecf09`  
		Last Modified: Tue, 15 Dec 2020 22:23:12 GMT  
		Size: 935.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ee5b09a6bd1a070d04dde6b2515ef2a57e140d4f73d9f50ad83f6e8ce18b24`  
		Last Modified: Tue, 15 Dec 2020 22:23:14 GMT  
		Size: 2.5 KB (2511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08eada9a7bc7c63638ab2fcd5c61ed077a1f22a81291bd5f316209a4fe562389`  
		Last Modified: Tue, 15 Dec 2020 22:23:23 GMT  
		Size: 1.1 MB (1092849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0fbcf6d505937e2a317d503b0399e10ccb4ddcab4292a257f38c3702d31b11`  
		Last Modified: Tue, 15 Dec 2020 22:23:23 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2646423e5d17184a2ed078650c12782c170303e05dbf62659507b155bf555fcc`  
		Last Modified: Tue, 15 Dec 2020 22:23:23 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b0bfbf8e86d2acbedc1b3fb7473b827989a5c37400dc4a82287ce673d35d8c`  
		Last Modified: Tue, 15 Dec 2020 22:23:27 GMT  
		Size: 20.2 MB (20171376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a43da03684d4dff954c1c4393791ca8047cba0f83fa110427ce25707724465b`  
		Last Modified: Tue, 15 Dec 2020 22:23:23 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
