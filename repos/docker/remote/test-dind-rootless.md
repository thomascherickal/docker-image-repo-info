## `docker:test-dind-rootless`

```console
$ docker pull docker@sha256:e597d2ff01152142af3f3c9300c68dece0b4c4dd239d0e7cc40c789249928f7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:test-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:39dd933a9abfb9d0930e3a53961ea7f3639d983ab04331f5c7275e8eadec45ad
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.0 MB (94996651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48dc2ea478ca8e83ea29b265ab180ed7120f5ee538f13c64ea3a1bc22c92e568`
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
# Tue, 02 Jun 2020 21:22:38 GMT
ENV DOCKER_VERSION=19.03.11
# Tue, 02 Jun 2020 21:22:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Jun 2020 21:22:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Jun 2020 21:22:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Jun 2020 21:22:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Jun 2020 21:22:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Jun 2020 21:22:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Jun 2020 21:22:46 GMT
CMD ["sh"]
# Tue, 02 Jun 2020 21:22:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Jun 2020 21:22:52 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Jun 2020 21:22:53 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Tue, 02 Jun 2020 21:22:54 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Jun 2020 21:22:54 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Jun 2020 21:22:54 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Jun 2020 21:22:54 GMT
EXPOSE 2375 2376
# Tue, 02 Jun 2020 21:22:54 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Jun 2020 21:22:55 GMT
CMD []
# Tue, 02 Jun 2020 21:22:59 GMT
RUN apk add --no-cache iproute2
# Tue, 02 Jun 2020 21:23:00 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 02 Jun 2020 21:23:01 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 02 Jun 2020 21:23:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Tue, 02 Jun 2020 21:23:03 GMT
ENV ROOTLESSKIT_VERSION=0.9.1
# Tue, 02 Jun 2020 21:23:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Tue, 02 Jun 2020 21:23:16 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 02 Jun 2020 21:23:16 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 02 Jun 2020 21:23:16 GMT
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
	-	`sha256:1d105a01b85c21ead141121d9c3f567f92b1818376a62de40bbd5420ea591a23`  
		Last Modified: Tue, 02 Jun 2020 21:23:45 GMT  
		Size: 61.2 MB (61178673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87316014961f16ae0d60f2eabe79bf9d28f90501dcbc98b566d896a770aa01a`  
		Last Modified: Tue, 02 Jun 2020 21:23:33 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7f709568fa5c5b38043c1e1e561290ce84f4cce0fee636f48336e0be474d2a`  
		Last Modified: Tue, 02 Jun 2020 21:23:33 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f9e63bc2f85b43fdac8f512daa5268fbcfa1d87b4935ae4f8493e1693160cc`  
		Last Modified: Tue, 02 Jun 2020 21:23:34 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9da4e3fe467cc0b910362c19c4cb7897d571f6cf4e20af9c6b46f7fca1ff15d`  
		Last Modified: Tue, 02 Jun 2020 21:23:53 GMT  
		Size: 6.0 MB (5958675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1e1be64f29f8b276cf2757c57455ca8539c2cc669b24c46105a4d877b65ae5`  
		Last Modified: Tue, 02 Jun 2020 21:23:53 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9314d7e899d7a3d81efa9866b7640d968716697797fee77d942f476641e8b0`  
		Last Modified: Tue, 02 Jun 2020 21:23:52 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d99f0faa015abeea40fd414f05b66084ba52f3c4f13d08c6e077adfa6dcfb29`  
		Last Modified: Tue, 02 Jun 2020 21:23:52 GMT  
		Size: 2.5 KB (2511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a72507cb2b0be8e5220de9f1fbb400363a672fa66d7a489c46f9e51727a70e`  
		Last Modified: Tue, 02 Jun 2020 21:24:02 GMT  
		Size: 1.1 MB (1092690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3e53c74e9a8c678848efdccdc5800ff8c0a52143701ba74104a2c9dd3e53bb`  
		Last Modified: Tue, 02 Jun 2020 21:24:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b40fee84f16da8198d7830a36c5888d4ba36d4af6ab5f0656561ee62b85dd58`  
		Last Modified: Tue, 02 Jun 2020 21:24:01 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5032ea5ffb0c6e3a08aad4fd5058fe3a7347a385a1fb8b18070bc0abae240a5c`  
		Last Modified: Tue, 02 Jun 2020 21:24:04 GMT  
		Size: 9.1 MB (9109451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165d36287938d8cb59e5bb7d3df47326cff1a0fb3e380f2f5c283b94dcf65075`  
		Last Modified: Tue, 02 Jun 2020 21:24:03 GMT  
		Size: 12.8 MB (12811367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044ec336c849629427d2d01d7e407d4ac1d14e408faf4c0d7571bba571c7fd16`  
		Last Modified: Tue, 02 Jun 2020 21:24:01 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
