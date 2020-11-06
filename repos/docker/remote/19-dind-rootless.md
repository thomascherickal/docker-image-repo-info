## `docker:19-dind-rootless`

```console
$ docker pull docker@sha256:b9cb0ce903f30dd0d92409c32cd57e96ae1f11320adf3655739622c1ae6bf629
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:6394789b569243613e397a6491bde5a7015a013f87e3c723697f7baaf477e3b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.6 MB (96601936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76688e5913de798a21eb564589a0b9f1c22c429111614af8e793e12a82a89752`
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
# Thu, 22 Oct 2020 03:15:44 GMT
ENV DOCKER_VERSION=19.03.13
# Thu, 22 Oct 2020 03:15:50 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.13.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.13.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.13.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 22 Oct 2020 03:15:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 22 Oct 2020 03:15:50 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 22 Oct 2020 03:15:50 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 22 Oct 2020 03:15:51 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 22 Oct 2020 03:15:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 03:15:51 GMT
CMD ["sh"]
# Thu, 22 Oct 2020 03:15:58 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 23 Oct 2020 17:17:54 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 23 Oct 2020 17:17:54 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 23 Oct 2020 17:17:56 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 23 Oct 2020 17:17:56 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 23 Oct 2020 17:17:56 GMT
VOLUME [/var/lib/docker]
# Fri, 23 Oct 2020 17:17:56 GMT
EXPOSE 2375 2376
# Fri, 23 Oct 2020 17:17:56 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 23 Oct 2020 17:17:57 GMT
CMD []
# Fri, 23 Oct 2020 17:18:02 GMT
RUN apk add --no-cache iproute2
# Fri, 23 Oct 2020 17:18:03 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 23 Oct 2020 17:18:03 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 23 Oct 2020 17:18:06 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-19.03.13.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Fri, 06 Nov 2020 18:20:16 GMT
ENV ROOTLESSKIT_VERSION=0.11.0
# Fri, 06 Nov 2020 18:20:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Fri, 06 Nov 2020 18:20:28 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 06 Nov 2020 18:20:28 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 06 Nov 2020 18:20:29 GMT
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
	-	`sha256:c5dafad2182aae29aeec9c17a0eb7b8a418902147a74d41a5408bd331ad7b61a`  
		Last Modified: Thu, 22 Oct 2020 03:16:58 GMT  
		Size: 62.7 MB (62668352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa711733414defdf599caa6bbb097b529419ba31f862069350c2c4e32c3bf04`  
		Last Modified: Thu, 22 Oct 2020 03:16:45 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058f73b55e4ba2b1e9c395241302653a08228f457e8c8adf0b51426de7c2cfef`  
		Last Modified: Thu, 22 Oct 2020 03:16:45 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9c664faf126b51772616bb78c98f55f404b3c3d9271621229cc765faa17bfb`  
		Last Modified: Thu, 22 Oct 2020 03:16:45 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0b6491c6e7d75eaa16d14ff8cc3de7012a35ff667afd4f77f65611c720a09a`  
		Last Modified: Thu, 22 Oct 2020 03:17:10 GMT  
		Size: 6.0 MB (5958697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab16b9777c1cbfd38119a9fa290b41b4fcdfe16c5edb8ccdd5e2d4977504b792`  
		Last Modified: Fri, 23 Oct 2020 17:19:30 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdea63f936d63b03276854ebc2fe824b807002174007ad17be14df00c1d4a3e5`  
		Last Modified: Fri, 23 Oct 2020 17:19:30 GMT  
		Size: 938.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b3f059d26fe2c26e4041f6797b4b79083813f3d43fb8add5c8e2ff8242962e`  
		Last Modified: Fri, 23 Oct 2020 17:19:30 GMT  
		Size: 2.5 KB (2509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08130c0d8458ee6f0108c1189bac44fe84507754c95b316ed51b625912139a5`  
		Last Modified: Fri, 23 Oct 2020 17:19:38 GMT  
		Size: 1.1 MB (1092665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3079cf4d76375226f813602fcbd435d700a6d66208648c71a5636b482184234f`  
		Last Modified: Fri, 23 Oct 2020 17:19:36 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d928ab0cdf166e0b4b8a33b366b9a60e8e8bc873520a5bff66cb519b1bfd4ee8`  
		Last Modified: Fri, 23 Oct 2020 17:19:36 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d740077150d7f5660e756b488b64db6481bb8550c9b759957825057c46bf8800`  
		Last Modified: Fri, 23 Oct 2020 17:19:39 GMT  
		Size: 9.1 MB (9109461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda9d7e22f0035a6e6dc814ab5476cf59c5490bc4f80a97f2edcb251f2493120`  
		Last Modified: Fri, 06 Nov 2020 18:21:09 GMT  
		Size: 12.9 MB (12928666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50490d9bc048dba07167cbe5365aac5c87fa6407b23ff6c6ecda749f4afaaaf`  
		Last Modified: Fri, 06 Nov 2020 18:21:07 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
