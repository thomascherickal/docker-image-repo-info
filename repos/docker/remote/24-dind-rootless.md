## `docker:24-dind-rootless`

```console
$ docker pull docker@sha256:09a3db31a598cfc7bf498078363a7a33429d8d1aff6abfce2e9e311df3845f5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:ab2735770ecf3f34b27e154b4fd0458c1e9f6f1e39017ac1360abd3caa9160bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137381447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c706618df85431b1ad32ff62dabfeabe04bdf2c2696ed6fdfeca19dfd3763350`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Fri, 19 May 2023 23:41:44 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Fri, 19 May 2023 23:41:44 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Fri, 19 May 2023 23:41:44 GMT
ENV DOCKER_VERSION=24.0.1
# Fri, 19 May 2023 23:41:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Fri, 19 May 2023 23:41:44 GMT
ENV DOCKER_BUILDX_VERSION=0.10.4
# Fri, 19 May 2023 23:41:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-amd64'; 			sha256='dbe68cdc537d0150fc83e3f30974cd0ca11c179dafbf27f32d6f063be26e869b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-arm-v6'; 			sha256='d50aa01a22a53e5a0eae9918274c9931b813b5336c0e30061a6b1904efb0c5eb'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-arm-v7'; 			sha256='aabc8cef5b9221ecbcb0af9846004a30591540be8668504d70814efe870448c8'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-arm64'; 			sha256='e8f666134cf4aa83ec2b1b6afef0c83b1ea1387984d7a40ae6657b7da4d82d91'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-ppc64le'; 			sha256='d107178f36e6c83286f3f9316e2f66b18f08306570cef209cb5840c880bd91ae'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-riscv64'; 			sha256='393db8518aeb442d0ca5f3ccf4800622dfc5eb8993c29bbfccb023cbfde6cdbc'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-s390x'; 			sha256='16ce9071c14293640e9bcd547ff01578c65cfc68fc6c154091abd81daaf10929'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Fri, 19 May 2023 23:41:44 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Fri, 19 May 2023 23:41:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Fri, 19 May 2023 23:41:44 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Fri, 19 May 2023 23:41:44 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 19 May 2023 23:41:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 19 May 2023 23:41:44 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Fri, 19 May 2023 23:41:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 May 2023 23:41:44 GMT
CMD ["sh"]
# Fri, 19 May 2023 23:41:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Fri, 19 May 2023 23:41:44 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Fri, 19 May 2023 23:41:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Fri, 19 May 2023 23:41:44 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 19 May 2023 23:41:44 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Fri, 19 May 2023 23:41:44 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 19 May 2023 23:41:44 GMT
VOLUME [/var/lib/docker]
# Fri, 19 May 2023 23:41:44 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Fri, 19 May 2023 23:41:44 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 19 May 2023 23:41:44 GMT
CMD []
# Fri, 19 May 2023 23:41:44 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Fri, 19 May 2023 23:41:44 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Fri, 19 May 2023 23:41:44 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Fri, 19 May 2023 23:41:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Fri, 19 May 2023 23:41:44 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Fri, 19 May 2023 23:41:44 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 19 May 2023 23:41:44 GMT
USER rootless
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb60e7f5d22cf3e06856538fbb2c518c629c1bbe07d62a60d16e3c7fefa06f4`  
		Last Modified: Thu, 11 May 2023 19:23:43 GMT  
		Size: 2.0 MB (2014357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74671f55a8da50720028684fd32ee90f4fdeb79ffcadf0e7213a90cd50ef5c3`  
		Last Modified: Thu, 11 May 2023 19:23:42 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75039dcfa57a7b4e9405dbd4aa6d212ea4202c813e54a727ccd1e54d545afc28`  
		Last Modified: Sat, 20 May 2023 00:20:31 GMT  
		Size: 16.4 MB (16376152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a22e3449daa86df0e5996848151b44321a93eb35c7b1955007f3a6335bfeba`  
		Last Modified: Sat, 20 May 2023 00:20:29 GMT  
		Size: 16.0 MB (16001743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4174c6dd601b702349d67f0ec402e10c1a11e61c46ce6b2c555ee089e95311`  
		Last Modified: Sat, 20 May 2023 00:20:30 GMT  
		Size: 16.4 MB (16398984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548fa0fa6487917c0e934aa5dfd5bfc32a006e0dc32892a9a55e0c036a9db1e4`  
		Last Modified: Sat, 20 May 2023 00:20:27 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce3b413b15210a3ccc6bd5e5f02809c368b9ece00a79281f47051c6c956e018`  
		Last Modified: Sat, 20 May 2023 00:20:27 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ecf18acb8bfbc53c5df3fbaaee8b8f4bf97076b2bda1157f18417f7889ade19`  
		Last Modified: Sat, 20 May 2023 00:20:27 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b211af78289a14cca1df1358fe6928252fa33b0111fcfb8fc5f2a1aab9ed06`  
		Last Modified: Sat, 20 May 2023 00:20:47 GMT  
		Size: 7.0 MB (7025215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c76e69021c44f28a2d40108ecc484e269768818214cf91dfec020144427987`  
		Last Modified: Sat, 20 May 2023 00:20:46 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e1c9b8d8308eb44a42f697d0c3a78c18cf2316c252f5705cafa5b711ede6b4`  
		Last Modified: Sat, 20 May 2023 00:20:53 GMT  
		Size: 54.1 MB (54148325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684530159b226af9dc9f82a9dd1f335103750f1ec991ccea176a77d34e734857`  
		Last Modified: Sat, 20 May 2023 00:20:46 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2980f78f4a0b2ed506b1af9f8978a27b257b6fc0c2cbbbe26943f6c8ba5d858e`  
		Last Modified: Sat, 20 May 2023 00:20:46 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e761efb48d5e3bcd653154cd8c543407f937de774570a77bc84e3c396f4052c3`  
		Last Modified: Sat, 20 May 2023 00:21:22 GMT  
		Size: 1.4 MB (1362357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400ddef134f0c67fd0058471efe2141098837f87b3255e3269dd6ca8257a168f`  
		Last Modified: Sat, 20 May 2023 00:21:22 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bec15fb251b6d4d68bb14a999e87e702621704655ac5173eee17a685b2b0803`  
		Last Modified: Sat, 20 May 2023 00:21:22 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39335e5237f39272d52f1eadc08bb36f9a0d0df505bed77732dc51a11bc7873`  
		Last Modified: Sat, 20 May 2023 00:21:25 GMT  
		Size: 20.6 MB (20648104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de54a89a23d3b007af441ec6f87feebed5d38f2025e5d3b03807cc0e367d1c16`  
		Last Modified: Sat, 20 May 2023 00:21:22 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:845e48fbc58b31427fd48341fe62f9d9e1cb1b82e51ce57408ff7cfbe872f577
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130662639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:312463247a36c36670d8ca58407f991abd23ee522b388ce4b48f8325d62120ac`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Fri, 19 May 2023 23:41:44 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Fri, 19 May 2023 23:41:44 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Fri, 19 May 2023 23:41:44 GMT
ENV DOCKER_VERSION=24.0.1
# Fri, 19 May 2023 23:41:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Fri, 19 May 2023 23:41:44 GMT
ENV DOCKER_BUILDX_VERSION=0.10.4
# Fri, 19 May 2023 23:41:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-amd64'; 			sha256='dbe68cdc537d0150fc83e3f30974cd0ca11c179dafbf27f32d6f063be26e869b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-arm-v6'; 			sha256='d50aa01a22a53e5a0eae9918274c9931b813b5336c0e30061a6b1904efb0c5eb'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-arm-v7'; 			sha256='aabc8cef5b9221ecbcb0af9846004a30591540be8668504d70814efe870448c8'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-arm64'; 			sha256='e8f666134cf4aa83ec2b1b6afef0c83b1ea1387984d7a40ae6657b7da4d82d91'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-ppc64le'; 			sha256='d107178f36e6c83286f3f9316e2f66b18f08306570cef209cb5840c880bd91ae'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-riscv64'; 			sha256='393db8518aeb442d0ca5f3ccf4800622dfc5eb8993c29bbfccb023cbfde6cdbc'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-s390x'; 			sha256='16ce9071c14293640e9bcd547ff01578c65cfc68fc6c154091abd81daaf10929'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Fri, 19 May 2023 23:41:44 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Fri, 19 May 2023 23:41:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Fri, 19 May 2023 23:41:44 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Fri, 19 May 2023 23:41:44 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 19 May 2023 23:41:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 19 May 2023 23:41:44 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Fri, 19 May 2023 23:41:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 May 2023 23:41:44 GMT
CMD ["sh"]
# Fri, 19 May 2023 23:41:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Fri, 19 May 2023 23:41:44 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Fri, 19 May 2023 23:41:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Fri, 19 May 2023 23:41:44 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 19 May 2023 23:41:44 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Fri, 19 May 2023 23:41:44 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 19 May 2023 23:41:44 GMT
VOLUME [/var/lib/docker]
# Fri, 19 May 2023 23:41:44 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Fri, 19 May 2023 23:41:44 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 19 May 2023 23:41:44 GMT
CMD []
# Fri, 19 May 2023 23:41:44 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Fri, 19 May 2023 23:41:44 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Fri, 19 May 2023 23:41:44 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Fri, 19 May 2023 23:41:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Fri, 19 May 2023 23:41:44 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Fri, 19 May 2023 23:41:44 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 19 May 2023 23:41:44 GMT
USER rootless
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf127bdc9f4f627525a187a7bf41c41f4706220fb1fe5b5c7d6cbc52114a9224`  
		Last Modified: Thu, 11 May 2023 19:42:22 GMT  
		Size: 2.0 MB (2024535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b4810136f4ceecd47a02cbf6a0c55b8d9de3b014cf917ac2bf8ee632787ba0`  
		Last Modified: Thu, 11 May 2023 19:42:22 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7805c665c512c9144fc4fa17be125272b027a57c3af9ecc374e51f661e6330`  
		Last Modified: Sat, 20 May 2023 00:40:13 GMT  
		Size: 15.4 MB (15422660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbd67a00da7691cf73e0cbbdd8b5070ecac2c3ed1436b9505ca99e74bc44bd5`  
		Last Modified: Sat, 20 May 2023 00:40:11 GMT  
		Size: 14.4 MB (14441544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c249a2b0348af58909a7ebc7f770df6507412de198ba536c1b7485a1b895acb3`  
		Last Modified: Sat, 20 May 2023 00:40:12 GMT  
		Size: 14.9 MB (14861193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32078c42a5cd335d34c6f6d9547560ca7add58173cca2f3547ac64946dccca5`  
		Last Modified: Sat, 20 May 2023 00:40:10 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2609f442dd15cae0be4698b5712b1becc841098c00622263fa755c49cda5df8c`  
		Last Modified: Sat, 20 May 2023 00:40:10 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3b98673d7e90887a606e4dee41dc7181da9ce2af21eefa02d8ae0fbd972e7f`  
		Last Modified: Sat, 20 May 2023 00:40:10 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef6520288bae68307ef36f9648aebc24ee4c252629bb1f9ddf42ad4f23008fd`  
		Last Modified: Sat, 20 May 2023 00:40:29 GMT  
		Size: 7.2 MB (7245041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d6c2010418c9b9114f385c4ceed9e4e27579e44cd1936e7bf44263962de233`  
		Last Modified: Sat, 20 May 2023 00:40:28 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1608e0260ec7379b82a9c1c77e0323d73131fa5c216f8de3b9b15fc6de4df938`  
		Last Modified: Sat, 20 May 2023 00:40:33 GMT  
		Size: 49.5 MB (49455581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8856b3ec9330196e88316f02312f18cfc8f7a5471537af942d2956b3790a57`  
		Last Modified: Sat, 20 May 2023 00:40:28 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12f6eec882e994024d5bef2227468a150b362417a1d6d7e60c5942d6afea410`  
		Last Modified: Sat, 20 May 2023 00:40:28 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1633bcd22f936d37c65df9260159328e12157718ca60c6fb7d368644a03a10c`  
		Last Modified: Sat, 20 May 2023 00:41:00 GMT  
		Size: 1.4 MB (1413232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec272657b2324ba8fe8ca1ac4498ba3a3738f4b8c930598acc1c21b9604bc351`  
		Last Modified: Sat, 20 May 2023 00:41:00 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4bc186d65eef743b521ca9502871df0e31d46880bb259db1db1590af80a596`  
		Last Modified: Sat, 20 May 2023 00:41:00 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0a794c6e8defd08696c6624853631dd5d843e84d68928bbeee59de4cabedac`  
		Last Modified: Sat, 20 May 2023 00:41:03 GMT  
		Size: 22.4 MB (22447272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30be9b827765e312c75527212247fd06f41191aca407b4a67920091ab7be1df9`  
		Last Modified: Sat, 20 May 2023 00:41:00 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
