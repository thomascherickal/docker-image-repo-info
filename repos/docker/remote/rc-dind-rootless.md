## `docker:rc-dind-rootless`

```console
$ docker pull docker@sha256:4bab8ea9681dfa72ba4a2bb5aaba2e02d928436f3f5977cdb05ff394ac2539eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:rc-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:0efa3bcf56d0e9070be1a7327c90341e3c58ecedebf4c599c362a73c57e7c3ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97526559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76db5f76af7c366a1f24263eeab75c37609d227b73f75613c0291b93147f483f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Jan 2020 19:20:00 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:44:57 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:45:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:45:07 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:45:08 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:08 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:45:10 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:10 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:45:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 02:45:21 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:45:21 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 02:45:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 02:45:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:24 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 02:45:24 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 02:45:24 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:25 GMT
CMD []
# Fri, 07 Feb 2020 02:45:32 GMT
RUN apk add --no-cache iproute2
# Fri, 07 Feb 2020 02:45:34 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 07 Feb 2020 02:45:35 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:45:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Fri, 07 Feb 2020 02:45:40 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Fri, 07 Feb 2020 02:46:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Fri, 07 Feb 2020 02:46:03 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 07 Feb 2020 02:46:04 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 07 Feb 2020 02:46:04 GMT
USER rootless
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caea7060abe9610714377bd4bba10bdc84753e6e62fa0e1ffdc5c4e12848b51e`  
		Last Modified: Fri, 07 Feb 2020 02:47:33 GMT  
		Size: 64.2 MB (64174865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b866925237283b42ccdf5500fced4225fc4ffa5aff8e5e797d8cee70997177`  
		Last Modified: Fri, 07 Feb 2020 02:47:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae0723913e410c295d4f5fedfe376630dd0a177f56989ef6b61b2e316e5884`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae024136251285a97bd4a3b789755dcbcc96f128f498429bfab5c8f4db8355e`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eea91a5b97173d5dd2f344bc5d0e72f82699953ef1c5f959d4a9b7774afa8cf`  
		Last Modified: Fri, 07 Feb 2020 02:47:43 GMT  
		Size: 5.6 MB (5587326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbb053638ea5610c62c318ca2e653ca9d0835c05411a1daaa83b82ec3c87b24`  
		Last Modified: Fri, 07 Feb 2020 02:47:42 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b363b8a24b99d588e888eeec2ff5552375c3d2abfa228cd2380f06f6335ee4f8`  
		Last Modified: Fri, 07 Feb 2020 02:47:41 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3d07de86fbe4cd8f0756a991706ead8e5663775b15af0d03643d133796463`  
		Last Modified: Fri, 07 Feb 2020 02:47:41 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342db616cce160fc08012aba5b09c05643f86f1a3619774e1f20d5284440ec73`  
		Last Modified: Fri, 07 Feb 2020 02:47:53 GMT  
		Size: 796.0 KB (795994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db756ea33c8791de85fefa909ce37b309704bd6a34f131ffb919d74f505ead3b`  
		Last Modified: Fri, 07 Feb 2020 02:47:51 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9703c78438112237598d40096ede1222152aad967dacbac9fd4582373c8d0688`  
		Last Modified: Fri, 07 Feb 2020 02:47:51 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d246c517d8c2448b88be1b032fb68bc6f86adcba1d8cf574a23c50fdadf6da`  
		Last Modified: Fri, 07 Feb 2020 02:48:00 GMT  
		Size: 9.1 MB (9109464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6270a09865bc1bbaa54e469241142ca426acd6eaea998dc82c435b066f527e7`  
		Last Modified: Fri, 07 Feb 2020 02:47:56 GMT  
		Size: 12.6 MB (12622787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fed64567b6f25fab4045c141d3665c9ea66a16c674a46ccca92ecea1bdaae6`  
		Last Modified: Fri, 07 Feb 2020 02:47:51 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
