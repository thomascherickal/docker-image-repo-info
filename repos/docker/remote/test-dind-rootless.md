## `docker:test-dind-rootless`

```console
$ docker pull docker@sha256:4de1f97f33b062ff825c0aa13598746e490a845a49fd8e09fcd69afaf4ffcb5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:test-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:fa16519ce1fe1c391ea9f1c0227922b38e97da0e4241ff1efb655943bf8a3105
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.4 MB (95381693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d63201a95c763229aeb9888a47c23eb61b6af98e7449adb0ae0db81b8d0e352c`
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
# Thu, 25 Jun 2020 19:20:07 GMT
ENV DOCKER_VERSION=19.03.12
# Thu, 25 Jun 2020 19:20:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 25 Jun 2020 19:20:14 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 25 Jun 2020 19:20:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 25 Jun 2020 19:20:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 25 Jun 2020 19:20:15 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 25 Jun 2020 19:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:20:15 GMT
CMD ["sh"]
# Thu, 25 Jun 2020 19:20:21 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 25 Jun 2020 19:20:22 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 25 Jun 2020 19:20:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Thu, 25 Jun 2020 19:20:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 25 Jun 2020 19:20:23 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Thu, 25 Jun 2020 19:20:23 GMT
VOLUME [/var/lib/docker]
# Thu, 25 Jun 2020 19:20:23 GMT
EXPOSE 2375 2376
# Thu, 25 Jun 2020 19:20:24 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 25 Jun 2020 19:20:24 GMT
CMD []
# Thu, 25 Jun 2020 19:20:29 GMT
RUN apk add --no-cache iproute2
# Thu, 25 Jun 2020 19:20:30 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 25 Jun 2020 19:20:30 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 25 Jun 2020 19:20:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Thu, 25 Jun 2020 19:20:33 GMT
ENV ROOTLESSKIT_VERSION=0.9.1
# Thu, 25 Jun 2020 19:20:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Thu, 25 Jun 2020 19:20:46 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 25 Jun 2020 19:20:46 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 25 Jun 2020 19:20:46 GMT
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
	-	`sha256:46e300cec6696ac3fff5b87cd712918b3bc7ecc63b5d5b05a786ff273bad4389`  
		Last Modified: Thu, 25 Jun 2020 19:21:20 GMT  
		Size: 61.2 MB (61175765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63038576ad948ddc50187816ac3447b8b0ffc6d6d498fe6b1dba9c3eb8cb2a76`  
		Last Modified: Thu, 25 Jun 2020 19:21:08 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdb76c4706cd77e7b3c07fb9826679a2fede76c486d6ad54aad6accc0e1527f`  
		Last Modified: Thu, 25 Jun 2020 19:21:08 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7edeffdfd51334f1d2a83f7d1a18c92ed61aaf87faf2441538efd55174b3aa`  
		Last Modified: Thu, 25 Jun 2020 19:21:08 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc28bd76800fb343fc36656aed7256597354e11e3a565efd4666cb5a985078b3`  
		Last Modified: Thu, 25 Jun 2020 19:21:30 GMT  
		Size: 6.0 MB (5958689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54196fe38f7e182d1589488c3b679aa763ee9e92b88af5b1ce75566f5522acec`  
		Last Modified: Thu, 25 Jun 2020 19:21:28 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d269ba97d2166645c960223330a8dfbca59d7f3983f98dafb1a80971f95e87b`  
		Last Modified: Thu, 25 Jun 2020 19:21:28 GMT  
		Size: 758.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e35c09825f3f6569b4750828ec31d1461c13ff17c999b5d1d76478c08f01d7`  
		Last Modified: Thu, 25 Jun 2020 19:21:28 GMT  
		Size: 2.5 KB (2510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4da9d8f198f2639432c76e12dd8c2934cd7eb071dc92acd09e6084487c9bd07`  
		Last Modified: Thu, 25 Jun 2020 19:21:39 GMT  
		Size: 1.1 MB (1092690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402bb9de5ceec49bb959efce55c10df316bb4952db1e40c2b77c862fa49a2129`  
		Last Modified: Thu, 25 Jun 2020 19:21:38 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b866b65b4c03964cc41897970ca6131343903eb8e0a5162ea2a69543acc4b7a5`  
		Last Modified: Thu, 25 Jun 2020 19:21:38 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5131ad9393c8d6c881e716e85d676ae57bbcf8e6bde598b3428d2948768b5f5a`  
		Last Modified: Thu, 25 Jun 2020 19:21:40 GMT  
		Size: 9.1 MB (9109451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40f4a1aa60b99011fd34b0a43e6f8dabe781f6e91069f83d97bc5959d6d545e`  
		Last Modified: Thu, 25 Jun 2020 19:21:39 GMT  
		Size: 13.2 MB (13199304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426dc1387974ea55316aedc400c9b4904b162673e56892f4c897030911ade488`  
		Last Modified: Thu, 25 Jun 2020 19:21:37 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
