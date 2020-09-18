## `docker:dind-rootless`

```console
$ docker pull docker@sha256:adb853ec1f301f273ba4e03460150b5aecda03dc4dd92e53479a2672428e8bb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:0a7cb8c980134f575f5065931290e678e84e0e68445aea86cbb3880f48780be6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.9 MB (96934420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2e12918d0215db8d8d7c243e3adf110f4847b8a1c5e5e9ea8d2c8bed885bc52`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 21:22:37 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Jun 2020 21:22:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 21:22:38 GMT
ENV DOCKER_CHANNEL=stable
# Thu, 17 Sep 2020 23:21:13 GMT
ENV DOCKER_VERSION=19.03.13
# Thu, 17 Sep 2020 23:21:18 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 17 Sep 2020 23:21:18 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 17 Sep 2020 23:21:18 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 17 Sep 2020 23:21:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 17 Sep 2020 23:21:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 17 Sep 2020 23:21:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 23:21:19 GMT
CMD ["sh"]
# Thu, 17 Sep 2020 23:21:25 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 17 Sep 2020 23:21:26 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 17 Sep 2020 23:21:26 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Thu, 17 Sep 2020 23:21:27 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 17 Sep 2020 23:21:27 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Thu, 17 Sep 2020 23:21:28 GMT
VOLUME [/var/lib/docker]
# Thu, 17 Sep 2020 23:21:28 GMT
EXPOSE 2375 2376
# Thu, 17 Sep 2020 23:21:28 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 17 Sep 2020 23:21:28 GMT
CMD []
# Thu, 17 Sep 2020 23:21:33 GMT
RUN apk add --no-cache iproute2
# Thu, 17 Sep 2020 23:21:34 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 17 Sep 2020 23:21:35 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 17 Sep 2020 23:21:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Thu, 17 Sep 2020 23:21:37 GMT
ENV ROOTLESSKIT_VERSION=0.10.0
# Thu, 17 Sep 2020 23:21:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Thu, 17 Sep 2020 23:21:48 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 17 Sep 2020 23:21:48 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 17 Sep 2020 23:21:49 GMT
USER rootless
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ad7478873d1d5c57089f038747520fe46aa4e913cc6cf29273b3722ec45e53`  
		Last Modified: Tue, 02 Jun 2020 21:23:34 GMT  
		Size: 2.0 MB (2040260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4684f6177b5d290b3aa892c1dc44088aa89f9ea08a68f6ed98262c032aa2caa4`  
		Last Modified: Tue, 02 Jun 2020 21:23:33 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba584e970afe5db980fad9626244770514fa0667fdcde5cea2026e8530ed58a`  
		Last Modified: Thu, 17 Sep 2020 23:22:21 GMT  
		Size: 62.7 MB (62668331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cdc74d2b06dc3325760604f3119a68eb6ebdf2818ff2bfa17f2b43aefb185f7`  
		Last Modified: Thu, 17 Sep 2020 23:22:08 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5a0d07c1f8517115544072be65f194f72561d0ba214ad63537c8f25132464`  
		Last Modified: Thu, 17 Sep 2020 23:22:08 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca0ccc462d56fc24074f1918759e312745fd7bcf5c2791e5e464ba1180ef6e1`  
		Last Modified: Thu, 17 Sep 2020 23:22:08 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a08b8f1999516d805345343ae53d38576053a5310aead0479c7b915e4fa6305`  
		Last Modified: Thu, 17 Sep 2020 23:22:28 GMT  
		Size: 6.0 MB (5958779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60a2aec8c6b8d232554e9d47725616b33d281b189f4a1b26e5e383d1f5f9aea`  
		Last Modified: Thu, 17 Sep 2020 23:22:28 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84edc63b9e2e9b37d1c311747a4f882898fb37af5b058c3b7c7efb251a20dfe5`  
		Last Modified: Thu, 17 Sep 2020 23:22:27 GMT  
		Size: 931.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8919df01d067e3c586088e9fc4c32a5c41337896442e43d05b75fb352161261`  
		Last Modified: Thu, 17 Sep 2020 23:22:27 GMT  
		Size: 2.5 KB (2514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e41c4acd15f34c043f650b5817f41c59fc63ab5b208e01f6feadefefbac8d96`  
		Last Modified: Thu, 17 Sep 2020 23:22:36 GMT  
		Size: 1.1 MB (1092688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9daba13cec1e1c160b61b0f5159fbd4ccd0a0c6937518461c424490163513ae0`  
		Last Modified: Thu, 17 Sep 2020 23:22:35 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5e23dbfe67a22c03c82a4228ab070e4b241e0e67983f8abc5980bc10a2cbe6`  
		Last Modified: Thu, 17 Sep 2020 23:22:35 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cf6ba53e1ece18bf5ce4de921eb960cdf17433333941e7b221e55830e0c6f1`  
		Last Modified: Thu, 17 Sep 2020 23:22:37 GMT  
		Size: 9.1 MB (9109460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2140d2ce2ef33af0c84ce75d95490f5c6b55338780da6b1984e4f28642261b88`  
		Last Modified: Thu, 17 Sep 2020 23:22:37 GMT  
		Size: 13.3 MB (13259188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a14fa99b6b67584be5c5016b6df4b31c2ad42246ea682b9216c88ffd0a2c75f`  
		Last Modified: Thu, 17 Sep 2020 23:22:35 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
