## `docker:dind-rootless`

```console
$ docker pull docker@sha256:65d7a1b5b156c28a851ac653607043233fc1067dca85d3b6a550fb54d4d95614
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:8831f186343474659d0d46eea1d0e38b2efc6a34c4d81b95eafc410f308544d9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94538863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ef9bb7c8cb4398c7e24d5e040e6fa6221ae139846f5b6542009016162e17a0`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:13:44 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 24 Apr 2020 14:13:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:13:45 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 20 May 2020 17:19:38 GMT
ENV DOCKER_VERSION=19.03.9
# Wed, 20 May 2020 17:19:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 20 May 2020 17:19:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 20 May 2020 17:19:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 20 May 2020 17:19:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 20 May 2020 17:19:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 20 May 2020 17:19:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 May 2020 17:19:46 GMT
CMD ["sh"]
# Wed, 20 May 2020 17:19:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 20 May 2020 17:19:52 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 20 May 2020 17:19:52 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 20 May 2020 17:19:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 20 May 2020 17:19:53 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Wed, 20 May 2020 17:19:54 GMT
VOLUME [/var/lib/docker]
# Wed, 20 May 2020 17:19:54 GMT
EXPOSE 2375 2376
# Wed, 20 May 2020 17:19:54 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 20 May 2020 17:19:54 GMT
CMD []
# Wed, 20 May 2020 17:19:59 GMT
RUN apk add --no-cache iproute2
# Wed, 20 May 2020 17:20:00 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 20 May 2020 17:20:00 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 20 May 2020 17:20:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Wed, 20 May 2020 17:20:03 GMT
ENV ROOTLESSKIT_VERSION=0.9.1
# Wed, 20 May 2020 17:20:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Wed, 20 May 2020 17:20:16 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 20 May 2020 17:20:16 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 20 May 2020 17:20:16 GMT
USER rootless
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4c731d6eb3df3a5c5587aacd253a9f6d985fafb5a1c8ea03add752b00888ec`  
		Last Modified: Fri, 24 Apr 2020 14:14:46 GMT  
		Size: 2.0 MB (1994349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79d4ac3cd039c6e3f17d157c79b369e68a1a0d79c310a699cfd4835e283d48`  
		Last Modified: Fri, 24 Apr 2020 14:14:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be675782249ab1b51d43972b320944217f37cacc787750998b129f35bfb7c215`  
		Last Modified: Wed, 20 May 2020 17:20:49 GMT  
		Size: 61.2 MB (61173632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd3c8e333026edc4e004cf0e820757bb516e2e3a817400d16594a6ab4881f2f`  
		Last Modified: Wed, 20 May 2020 17:20:37 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcf4ec03a5025e14a3a4e456f6a72eb54a01407a916b8129b6f269f275ce099`  
		Last Modified: Wed, 20 May 2020 17:20:37 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be98e84f88b0a9fb4ae13634f8a848950e7ce60639773a0cc2cd947c420fdad1`  
		Last Modified: Wed, 20 May 2020 17:20:37 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638f17b62cf94a5f812d11c54a3fd26a0a64c7fa559df589a9e2c3efa2046a63`  
		Last Modified: Wed, 20 May 2020 17:20:58 GMT  
		Size: 5.5 MB (5544886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ce11980b0f907ff2cd4dbde55d47a4d497b03171766923503cf93f16832087`  
		Last Modified: Wed, 20 May 2020 17:20:57 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774579b7e8d28a8557ec65f6ec5720ea2b446ca8c0854c880fa7277bb8e35d59`  
		Last Modified: Wed, 20 May 2020 17:20:56 GMT  
		Size: 758.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee85d9eaa184694adc6f18b09857d5f75bc115d85655fc8915f5ad5381ea0a34`  
		Last Modified: Wed, 20 May 2020 17:20:56 GMT  
		Size: 2.5 KB (2509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39939050802959142f88b745e3e38b66b68444145b501d77ff2d86238a696f99`  
		Last Modified: Wed, 20 May 2020 17:21:06 GMT  
		Size: 737.9 KB (737893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f9e6c5301507a935bd38e602677868f0dae93fc3cc52b8d324b001d0fe1e65`  
		Last Modified: Wed, 20 May 2020 17:21:05 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f25708b92b308d249fc6cf101242d0099e0b8a75c29de84a2e2075a178eb79`  
		Last Modified: Wed, 20 May 2020 17:21:05 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b825013a315c700bb20caaaae973d0ac7b90cceb521b92adfbac544b48ba474`  
		Last Modified: Wed, 20 May 2020 17:21:08 GMT  
		Size: 9.1 MB (9109466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eaa1feefdd738b8eb4b7b0c2b32e33234f7f4652783e6935414695900dc36d3`  
		Last Modified: Wed, 20 May 2020 17:21:08 GMT  
		Size: 13.2 MB (13157329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e9a75b341cf61c58e01d831a02efd20a7e90be80cb11921f36c994c1541116`  
		Last Modified: Wed, 20 May 2020 17:21:05 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
