<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `docker`

-	[`docker:20`](#docker20)
-	[`docker:20-dind`](#docker20-dind)
-	[`docker:20-dind-rootless`](#docker20-dind-rootless)
-	[`docker:20-git`](#docker20-git)
-	[`docker:20-windowsservercore`](#docker20-windowsservercore)
-	[`docker:20-windowsservercore-1809`](#docker20-windowsservercore-1809)
-	[`docker:20-windowsservercore-ltsc2022`](#docker20-windowsservercore-ltsc2022)
-	[`docker:20.10`](#docker2010)
-	[`docker:20.10-dind`](#docker2010-dind)
-	[`docker:20.10-dind-rootless`](#docker2010-dind-rootless)
-	[`docker:20.10-git`](#docker2010-git)
-	[`docker:20.10-windowsservercore`](#docker2010-windowsservercore)
-	[`docker:20.10-windowsservercore-1809`](#docker2010-windowsservercore-1809)
-	[`docker:20.10-windowsservercore-ltsc2022`](#docker2010-windowsservercore-ltsc2022)
-	[`docker:20.10.17`](#docker201017)
-	[`docker:20.10.17-alpine3.16`](#docker201017-alpine316)
-	[`docker:20.10.17-dind`](#docker201017-dind)
-	[`docker:20.10.17-dind-alpine3.16`](#docker201017-dind-alpine316)
-	[`docker:20.10.17-dind-rootless`](#docker201017-dind-rootless)
-	[`docker:20.10.17-git`](#docker201017-git)
-	[`docker:20.10.17-windowsservercore`](#docker201017-windowsservercore)
-	[`docker:20.10.17-windowsservercore-1809`](#docker201017-windowsservercore-1809)
-	[`docker:20.10.17-windowsservercore-ltsc2022`](#docker201017-windowsservercore-ltsc2022)
-	[`docker:22.06-rc`](#docker2206-rc)
-	[`docker:22.06-rc-dind`](#docker2206-rc-dind)
-	[`docker:22.06-rc-dind-rootless`](#docker2206-rc-dind-rootless)
-	[`docker:22.06-rc-git`](#docker2206-rc-git)
-	[`docker:22.06-rc-windowsservercore`](#docker2206-rc-windowsservercore)
-	[`docker:22.06-rc-windowsservercore-1809`](#docker2206-rc-windowsservercore-1809)
-	[`docker:22.06-rc-windowsservercore-ltsc2022`](#docker2206-rc-windowsservercore-ltsc2022)
-	[`docker:22.06.0-beta.0`](#docker22060-beta0)
-	[`docker:22.06.0-beta.0-alpine3.16`](#docker22060-beta0-alpine316)
-	[`docker:22.06.0-beta.0-dind`](#docker22060-beta0-dind)
-	[`docker:22.06.0-beta.0-dind-alpine3.16`](#docker22060-beta0-dind-alpine316)
-	[`docker:22.06.0-beta.0-dind-rootless`](#docker22060-beta0-dind-rootless)
-	[`docker:22.06.0-beta.0-git`](#docker22060-beta0-git)
-	[`docker:22.06.0-beta.0-windowsservercore`](#docker22060-beta0-windowsservercore)
-	[`docker:22.06.0-beta.0-windowsservercore-1809`](#docker22060-beta0-windowsservercore-1809)
-	[`docker:22.06.0-beta.0-windowsservercore-ltsc2022`](#docker22060-beta0-windowsservercore-ltsc2022)
-	[`docker:dind`](#dockerdind)
-	[`docker:dind-rootless`](#dockerdind-rootless)
-	[`docker:git`](#dockergit)
-	[`docker:latest`](#dockerlatest)
-	[`docker:rc`](#dockerrc)
-	[`docker:rc-dind`](#dockerrc-dind)
-	[`docker:rc-dind-rootless`](#dockerrc-dind-rootless)
-	[`docker:rc-git`](#dockerrc-git)
-	[`docker:rc-windowsservercore`](#dockerrc-windowsservercore)
-	[`docker:rc-windowsservercore-1809`](#dockerrc-windowsservercore-1809)
-	[`docker:rc-windowsservercore-ltsc2022`](#dockerrc-windowsservercore-ltsc2022)
-	[`docker:windowsservercore`](#dockerwindowsservercore)
-	[`docker:windowsservercore-1809`](#dockerwindowsservercore-1809)
-	[`docker:windowsservercore-ltsc2022`](#dockerwindowsservercore-ltsc2022)

## `docker:20`

```console
$ docker pull docker@sha256:206fb7d9747e035b5fb0b12840d1117ccce38b7508c5967ddd66bfc1f8abc36a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20` - linux; amd64

```console
$ docker pull docker@sha256:d06e6924e1364a690ad454e7b51a75b38f01042cb43df2f9d51098bbbc5b836d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94244378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0208b15ab9702b6bf3b7ac59e6c1d7ebbd679b94bb27367f5763297681a61abc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:23:40 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:23:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:23:46 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:23:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:23:48 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:23:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:23:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:23:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:23:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:23:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:23:52 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a01eeb4b9660234932fe1a5ed6ee12b88476503688d1af44ef2cf5589db59c5`  
		Last Modified: Tue, 07 Jun 2022 18:25:11 GMT  
		Size: 65.5 MB (65511093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f16477544224c056335320872aa8dd6c2a404df9982484e1f62603e0f1f8e2a`  
		Last Modified: Tue, 07 Jun 2022 18:25:01 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e917105572c19bab12a64c5f1079e8d7b0a3e10899bd0398d1f136d41a4af191`  
		Last Modified: Tue, 07 Jun 2022 18:25:00 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709778230e46fbd5042dc9165462ac00b69b08da200fd164c4b55ee90d71ed6`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94076fc9c77a2ec8cd8737d8ee69c11882eaa16be0e46ea97b42763d6de07213`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0650593e055d90b3f09ecf2e61114a35929437150d1f25d6e9aea5e4d4ef57`  
		Last Modified: Tue, 07 Jun 2022 18:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4e95dfecee5f5f5a6ed920904149fdba4cbe725d149df62f88e556f6a64204f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.5 MB (86476390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065f5b92312ea447a580a243adb30727f02719699a6e80d668170755e50bf642`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:44:31 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:44:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:44:36 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:44:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:44:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:44:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:44:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:44:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:44:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:44:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:44:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:44:52 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208c9164699a390332f26552a4e3372cbba8153d21dd8c579d78b4820727447`  
		Last Modified: Tue, 07 Jun 2022 18:46:58 GMT  
		Size: 60.0 MB (60022171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd660eb6acfde977fdcc2e06e1f8b820b994c605f8d7c2a43c8043fee47a59`  
		Last Modified: Tue, 07 Jun 2022 18:46:49 GMT  
		Size: 13.1 MB (13097908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed4b77ab26353356aa5e47399b195759c104e1949f2c8552ed99141fcd5a8e6`  
		Last Modified: Tue, 07 Jun 2022 18:46:48 GMT  
		Size: 8.7 MB (8663386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e346f102da723c6d8f8709a20fe5d2b88c6efc5c31da9c1e7fba1007acd0ec1f`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97325db524006b151b2a34f2981b47567785b4362b383f8672aa4ccd00df3bfe`  
		Last Modified: Tue, 07 Jun 2022 18:46:47 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6e016098eef53d87f0df18ffe9c41bda01a822971b75a0d351d1787a4d59fb`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind`

```console
$ docker pull docker@sha256:a7a9383d0631b5f6b59f0a8138912d20b63c9320127e3fb065cb9ca0257a58b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind` - linux; amd64

```console
$ docker pull docker@sha256:8cdb600dd59001892484f7c4be06166e42a2952065b6822b98c5aa7b8ef2ce8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.1 MB (101111945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dbe252bd9afb23859f250989da416b2cd8ab30f4b61a2bc8fca6f9b05d7e665`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:23:40 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:23:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:23:46 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:23:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:23:48 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:23:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:23:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:23:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:23:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:23:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:23:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:24:02 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 07 Jun 2022 18:24:03 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:24:03 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 07 Jun 2022 18:24:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 07 Jun 2022 18:24:04 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:24:04 GMT
VOLUME [/var/lib/docker]
# Tue, 07 Jun 2022 18:24:04 GMT
EXPOSE 2375 2376
# Tue, 07 Jun 2022 18:24:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 07 Jun 2022 18:24:05 GMT
CMD []
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a01eeb4b9660234932fe1a5ed6ee12b88476503688d1af44ef2cf5589db59c5`  
		Last Modified: Tue, 07 Jun 2022 18:25:11 GMT  
		Size: 65.5 MB (65511093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f16477544224c056335320872aa8dd6c2a404df9982484e1f62603e0f1f8e2a`  
		Last Modified: Tue, 07 Jun 2022 18:25:01 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e917105572c19bab12a64c5f1079e8d7b0a3e10899bd0398d1f136d41a4af191`  
		Last Modified: Tue, 07 Jun 2022 18:25:00 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709778230e46fbd5042dc9165462ac00b69b08da200fd164c4b55ee90d71ed6`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94076fc9c77a2ec8cd8737d8ee69c11882eaa16be0e46ea97b42763d6de07213`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0650593e055d90b3f09ecf2e61114a35929437150d1f25d6e9aea5e4d4ef57`  
		Last Modified: Tue, 07 Jun 2022 18:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8739efbf33852756a9d17dd471ab7ab9d9a1f183df6185763c4f54d55f3e5ef`  
		Last Modified: Tue, 07 Jun 2022 18:25:31 GMT  
		Size: 6.9 MB (6862542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1528486149a1ec660cc13a105d322cbe384bf2fd0bb5b32436043928d35701e8`  
		Last Modified: Tue, 07 Jun 2022 18:25:30 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fce28207d4c0f42d2a8352f195f1551714dfa68bcc768565b63a0e030a46813`  
		Last Modified: Tue, 07 Jun 2022 18:25:29 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c6543c9821cdb12ce3c3b95bed6148272f6ee648fcaf31c1b5b6d7aa67c459`  
		Last Modified: Tue, 07 Jun 2022 18:25:29 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:c82526b54ad542830185247b1fd7cd75ca06c4b7379625a631193ebebbffceb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93216008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d2d13d30ebd3836c5760272dda377aa12d9253bf2aee7a175a1360773e2a9d9`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:44:31 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:44:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:44:36 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:44:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:44:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:44:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:44:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:44:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:44:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:44:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:44:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:44:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:45:01 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 07 Jun 2022 18:45:02 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:45:03 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 07 Jun 2022 18:45:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 07 Jun 2022 18:45:06 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:45:06 GMT
VOLUME [/var/lib/docker]
# Tue, 07 Jun 2022 18:45:07 GMT
EXPOSE 2375 2376
# Tue, 07 Jun 2022 18:45:08 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 07 Jun 2022 18:45:09 GMT
CMD []
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208c9164699a390332f26552a4e3372cbba8153d21dd8c579d78b4820727447`  
		Last Modified: Tue, 07 Jun 2022 18:46:58 GMT  
		Size: 60.0 MB (60022171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd660eb6acfde977fdcc2e06e1f8b820b994c605f8d7c2a43c8043fee47a59`  
		Last Modified: Tue, 07 Jun 2022 18:46:49 GMT  
		Size: 13.1 MB (13097908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed4b77ab26353356aa5e47399b195759c104e1949f2c8552ed99141fcd5a8e6`  
		Last Modified: Tue, 07 Jun 2022 18:46:48 GMT  
		Size: 8.7 MB (8663386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e346f102da723c6d8f8709a20fe5d2b88c6efc5c31da9c1e7fba1007acd0ec1f`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97325db524006b151b2a34f2981b47567785b4362b383f8672aa4ccd00df3bfe`  
		Last Modified: Tue, 07 Jun 2022 18:46:47 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6e016098eef53d87f0df18ffe9c41bda01a822971b75a0d351d1787a4d59fb`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e98490325d999d399e486a1107cbb821ef56e26e4b8e09cba42eab6de668f53`  
		Last Modified: Tue, 07 Jun 2022 18:47:20 GMT  
		Size: 6.7 MB (6734617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3937658d06fd0152ee0795e63b1ac2bef28cd0e08636738ed86cfb3f270efe87`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520215962f31f70fbe23340f593756dd36c602b6523c60d6edf47191a3366f70`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c038ae79644412f10a6fd71b2aeb63c3462ca53f5eba947465d067157abd1d`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 2.7 KB (2748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:9ff8f7cf745620a1d20cf27034f544f1ff7bca5a2abbcda2857962104e042bc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:96b2a2fefca7613f5b34629ac11cabaf527e8f440cbac8b7dc4c295c10b0e6cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.7 MB (121693146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8475d2a876361c1765ccfcd694b66a7a121b34b3d75a04f55d5b94a7437da1c3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:23:40 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:23:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:23:46 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:23:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:23:48 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:23:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:23:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:23:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:23:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:23:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:23:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:24:02 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 07 Jun 2022 18:24:03 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:24:03 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 07 Jun 2022 18:24:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 07 Jun 2022 18:24:04 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:24:04 GMT
VOLUME [/var/lib/docker]
# Tue, 07 Jun 2022 18:24:04 GMT
EXPOSE 2375 2376
# Tue, 07 Jun 2022 18:24:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 07 Jun 2022 18:24:05 GMT
CMD []
# Tue, 07 Jun 2022 18:24:11 GMT
RUN apk add --no-cache iproute2
# Tue, 07 Jun 2022 18:24:11 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 07 Jun 2022 18:24:12 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:24:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 07 Jun 2022 18:24:15 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 07 Jun 2022 18:24:15 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 07 Jun 2022 18:24:15 GMT
USER rootless
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a01eeb4b9660234932fe1a5ed6ee12b88476503688d1af44ef2cf5589db59c5`  
		Last Modified: Tue, 07 Jun 2022 18:25:11 GMT  
		Size: 65.5 MB (65511093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f16477544224c056335320872aa8dd6c2a404df9982484e1f62603e0f1f8e2a`  
		Last Modified: Tue, 07 Jun 2022 18:25:01 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e917105572c19bab12a64c5f1079e8d7b0a3e10899bd0398d1f136d41a4af191`  
		Last Modified: Tue, 07 Jun 2022 18:25:00 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709778230e46fbd5042dc9165462ac00b69b08da200fd164c4b55ee90d71ed6`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94076fc9c77a2ec8cd8737d8ee69c11882eaa16be0e46ea97b42763d6de07213`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0650593e055d90b3f09ecf2e61114a35929437150d1f25d6e9aea5e4d4ef57`  
		Last Modified: Tue, 07 Jun 2022 18:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8739efbf33852756a9d17dd471ab7ab9d9a1f183df6185763c4f54d55f3e5ef`  
		Last Modified: Tue, 07 Jun 2022 18:25:31 GMT  
		Size: 6.9 MB (6862542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1528486149a1ec660cc13a105d322cbe384bf2fd0bb5b32436043928d35701e8`  
		Last Modified: Tue, 07 Jun 2022 18:25:30 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fce28207d4c0f42d2a8352f195f1551714dfa68bcc768565b63a0e030a46813`  
		Last Modified: Tue, 07 Jun 2022 18:25:29 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c6543c9821cdb12ce3c3b95bed6148272f6ee648fcaf31c1b5b6d7aa67c459`  
		Last Modified: Tue, 07 Jun 2022 18:25:29 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a725abeedbfa4c33a7418f41fd875f275696b28eab0a79ba1aa544660a5e7b`  
		Last Modified: Tue, 07 Jun 2022 18:25:50 GMT  
		Size: 1.2 MB (1232609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6a3e20c8491b4d470b9c1a11dceab173fc5252f5fdb7deca56332f03d5b07d`  
		Last Modified: Tue, 07 Jun 2022 18:25:49 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c3ab7612a60e9dbcc8ef8900c43e8d03e0ee26e556f11ef6d7c7fa68ad5fcc`  
		Last Modified: Tue, 07 Jun 2022 18:25:49 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86880a2ebfe3428ec38a5d7146121cab83d10c47b662e08b7296300c5ba36b90`  
		Last Modified: Tue, 07 Jun 2022 18:25:53 GMT  
		Size: 19.3 MB (19346876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08bf902c5827b673ef106ed1a4eaa55f3b5df8409fea26c822f0b6369895c0b`  
		Last Modified: Tue, 07 Jun 2022 18:25:49 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:32882c77434b98c975ceb1b3b96dffe40acbf1cfe7a0af5d515331e4781d4541
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115640767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62f34441530bb8a901ae97f5ffd28037dfbe34695de70e1f8bd14c5e7d9b09ae`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:44:31 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:44:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:44:36 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:44:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:44:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:44:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:44:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:44:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:44:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:44:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:44:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:44:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:45:01 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 07 Jun 2022 18:45:02 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:45:03 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 07 Jun 2022 18:45:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 07 Jun 2022 18:45:06 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:45:06 GMT
VOLUME [/var/lib/docker]
# Tue, 07 Jun 2022 18:45:07 GMT
EXPOSE 2375 2376
# Tue, 07 Jun 2022 18:45:08 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 07 Jun 2022 18:45:09 GMT
CMD []
# Tue, 07 Jun 2022 18:45:17 GMT
RUN apk add --no-cache iproute2
# Tue, 07 Jun 2022 18:45:18 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 07 Jun 2022 18:45:19 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:45:21 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 07 Jun 2022 18:45:22 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 07 Jun 2022 18:45:23 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 07 Jun 2022 18:45:24 GMT
USER rootless
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208c9164699a390332f26552a4e3372cbba8153d21dd8c579d78b4820727447`  
		Last Modified: Tue, 07 Jun 2022 18:46:58 GMT  
		Size: 60.0 MB (60022171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd660eb6acfde977fdcc2e06e1f8b820b994c605f8d7c2a43c8043fee47a59`  
		Last Modified: Tue, 07 Jun 2022 18:46:49 GMT  
		Size: 13.1 MB (13097908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed4b77ab26353356aa5e47399b195759c104e1949f2c8552ed99141fcd5a8e6`  
		Last Modified: Tue, 07 Jun 2022 18:46:48 GMT  
		Size: 8.7 MB (8663386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e346f102da723c6d8f8709a20fe5d2b88c6efc5c31da9c1e7fba1007acd0ec1f`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97325db524006b151b2a34f2981b47567785b4362b383f8672aa4ccd00df3bfe`  
		Last Modified: Tue, 07 Jun 2022 18:46:47 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6e016098eef53d87f0df18ffe9c41bda01a822971b75a0d351d1787a4d59fb`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e98490325d999d399e486a1107cbb821ef56e26e4b8e09cba42eab6de668f53`  
		Last Modified: Tue, 07 Jun 2022 18:47:20 GMT  
		Size: 6.7 MB (6734617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3937658d06fd0152ee0795e63b1ac2bef28cd0e08636738ed86cfb3f270efe87`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520215962f31f70fbe23340f593756dd36c602b6523c60d6edf47191a3366f70`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c038ae79644412f10a6fd71b2aeb63c3462ca53f5eba947465d067157abd1d`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 2.7 KB (2748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a25f04457a8992aec9515a93b8e684c6308ac16e40609e4aea6e5e17e5a9831`  
		Last Modified: Tue, 07 Jun 2022 18:47:42 GMT  
		Size: 1.2 MB (1246089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4737bba435e3c5bf8e0bd36ea8549325126984e556f0383a65cd0780c17c41f3`  
		Last Modified: Tue, 07 Jun 2022 18:47:41 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153a758456f1bf14ac68b5cc4e5adf575663fbad6ee03e0056a9cd6162b45259`  
		Last Modified: Tue, 07 Jun 2022 18:47:42 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6ecdd375957217ed6f2887df5b1aede054583d798040f1fa03e2113584c479`  
		Last Modified: Tue, 07 Jun 2022 18:47:45 GMT  
		Size: 21.2 MB (21177045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e75e34fe059e0be78079a5bd13cfd80b8d414fad4f717402e56a2fa8343ed0`  
		Last Modified: Tue, 07 Jun 2022 18:47:41 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-git`

```console
$ docker pull docker@sha256:ae822531c5ce930bb49408e170ed0b1fd4efcf86da1777687c90f3471b6f73ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-git` - linux; amd64

```console
$ docker pull docker@sha256:fba3948c035af5fd3a4cbe953195dcbdab125581f254d44044d87b2e88aef8ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101178830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d39449ad493ed1d71480ba17d4dcd56af4c28605f7f5645a1429f077cd8513`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:23:40 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:23:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:23:46 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:23:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:23:48 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:23:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:23:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:23:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:23:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:23:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:23:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:24:19 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a01eeb4b9660234932fe1a5ed6ee12b88476503688d1af44ef2cf5589db59c5`  
		Last Modified: Tue, 07 Jun 2022 18:25:11 GMT  
		Size: 65.5 MB (65511093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f16477544224c056335320872aa8dd6c2a404df9982484e1f62603e0f1f8e2a`  
		Last Modified: Tue, 07 Jun 2022 18:25:01 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e917105572c19bab12a64c5f1079e8d7b0a3e10899bd0398d1f136d41a4af191`  
		Last Modified: Tue, 07 Jun 2022 18:25:00 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709778230e46fbd5042dc9165462ac00b69b08da200fd164c4b55ee90d71ed6`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94076fc9c77a2ec8cd8737d8ee69c11882eaa16be0e46ea97b42763d6de07213`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0650593e055d90b3f09ecf2e61114a35929437150d1f25d6e9aea5e4d4ef57`  
		Last Modified: Tue, 07 Jun 2022 18:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd116fbfcda7d014c42d3891e0c2d200795c968f665e123ee95a0e6d1e5c934`  
		Last Modified: Tue, 07 Jun 2022 18:26:11 GMT  
		Size: 6.9 MB (6934452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f633c11b5bfc875d87905074a8a032404ce2bfefb7e51f9f6919d36277e77393
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.5 MB (93521092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb6d61e7054c42bfa4ad4e5dca6aee71560f8fddb61b5a6a8101a66320730b1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:44:31 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:44:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:44:36 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:44:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:44:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:44:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:44:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:44:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:44:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:44:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:44:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:44:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:45:32 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208c9164699a390332f26552a4e3372cbba8153d21dd8c579d78b4820727447`  
		Last Modified: Tue, 07 Jun 2022 18:46:58 GMT  
		Size: 60.0 MB (60022171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd660eb6acfde977fdcc2e06e1f8b820b994c605f8d7c2a43c8043fee47a59`  
		Last Modified: Tue, 07 Jun 2022 18:46:49 GMT  
		Size: 13.1 MB (13097908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed4b77ab26353356aa5e47399b195759c104e1949f2c8552ed99141fcd5a8e6`  
		Last Modified: Tue, 07 Jun 2022 18:46:48 GMT  
		Size: 8.7 MB (8663386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e346f102da723c6d8f8709a20fe5d2b88c6efc5c31da9c1e7fba1007acd0ec1f`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97325db524006b151b2a34f2981b47567785b4362b383f8672aa4ccd00df3bfe`  
		Last Modified: Tue, 07 Jun 2022 18:46:47 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6e016098eef53d87f0df18ffe9c41bda01a822971b75a0d351d1787a4d59fb`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538445497cbaebac26dcea42aaadf26367e96ea7ccf5c022dcfd39bd1da7c882`  
		Last Modified: Tue, 07 Jun 2022 18:48:05 GMT  
		Size: 7.0 MB (7044702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore`

```console
$ docker pull docker@sha256:c46b51f81569a8528faf11ab678e415a9846ac53246ec6c2b11fc5a81e61674b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.768; amd64
	-	windows version 10.0.17763.3046; amd64

### `docker:20-windowsservercore` - windows version 10.0.20348.768; amd64

```console
$ docker pull docker@sha256:c92dc04a8ccb9c898c42318e134d11b4fe5e825349a870ec0af4d00a8aa32f30
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2331628569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbf9b630697f8843ffb9923fb2b24ec28ca80c582e396f4bc8ae9db8517438c8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 09 Jun 2022 04:32:50 GMT
RUN Install update 10.0.20348.768
# Wed, 15 Jun 2022 12:13:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:46:14 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:49:43 GMT
ENV DOCKER_VERSION=20.10.17
# Wed, 15 Jun 2022 22:49:44 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.17.zip
# Wed, 15 Jun 2022 22:50:20 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c71967ff41928927e4c407171e4ffbac3c9ab4221eb64f5ca5a34ff4c230567`  
		Size: 841.6 MB (841600427 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dec0338feaf01f35eb916b7fd9ecc08b719354163254885d5215e513c1a3eb2e`  
		Last Modified: Wed, 15 Jun 2022 12:49:26 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a162967ebe5da992f6dc4e9ebdd4ec9f402a84f6974c0c562cff1ed6f17dd39`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 630.9 KB (630886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6900080f685d53c251ad925dfa2391f7ea21ee77b7d5aa31e56e0d7a30666adc`  
		Last Modified: Wed, 15 Jun 2022 22:53:02 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79983762d3966bbf5de5e5397ea8b7173f7fa121d7ab01e2136817be07ae4e0f`  
		Last Modified: Wed, 15 Jun 2022 22:53:02 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7398906a7954731da34c295d4f50bdd50edb96f50ad88006b29eaa94662ccd2`  
		Last Modified: Wed, 15 Jun 2022 22:53:14 GMT  
		Size: 52.5 MB (52529382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-windowsservercore` - windows version 10.0.17763.3046; amd64

```console
$ docker pull docker@sha256:92b9efc4d05fc727177fa4d4f20e8ca35969778a932858c93dde72a69cafa065
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2715917945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:208e7e03e3e360a634a05b786e8043476d165cf2930fc4237e9c34c390385228`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:48:09 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:50:28 GMT
ENV DOCKER_VERSION=20.10.17
# Wed, 15 Jun 2022 22:50:29 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.17.zip
# Wed, 15 Jun 2022 22:51:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4c7110da70e07b37a00b3b05b18361572412287fee26eba04fcf23dcb75639`  
		Last Modified: Wed, 15 Jun 2022 22:52:48 GMT  
		Size: 352.2 KB (352228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a3fc52e3c402b1be6f7512b16405aaaba3edd6037ede2a7885b367bec19efd`  
		Last Modified: Wed, 15 Jun 2022 22:53:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92deca7aa7a34f968926e81414d0102042c2a2e85968fa9423cb1ceed71a9393`  
		Last Modified: Wed, 15 Jun 2022 22:53:28 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f346f796df4e8cb918a2d6f83dcf31d1544d3af9b283727e9757400a160423ab`  
		Last Modified: Wed, 15 Jun 2022 22:53:39 GMT  
		Size: 52.3 MB (52281684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-1809`

```console
$ docker pull docker@sha256:f8c99a477afebef2e0a504c1a2d40be47010d4e93cb99febe638d0eb20505199
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3046; amd64

### `docker:20-windowsservercore-1809` - windows version 10.0.17763.3046; amd64

```console
$ docker pull docker@sha256:92b9efc4d05fc727177fa4d4f20e8ca35969778a932858c93dde72a69cafa065
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2715917945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:208e7e03e3e360a634a05b786e8043476d165cf2930fc4237e9c34c390385228`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:48:09 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:50:28 GMT
ENV DOCKER_VERSION=20.10.17
# Wed, 15 Jun 2022 22:50:29 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.17.zip
# Wed, 15 Jun 2022 22:51:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4c7110da70e07b37a00b3b05b18361572412287fee26eba04fcf23dcb75639`  
		Last Modified: Wed, 15 Jun 2022 22:52:48 GMT  
		Size: 352.2 KB (352228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a3fc52e3c402b1be6f7512b16405aaaba3edd6037ede2a7885b367bec19efd`  
		Last Modified: Wed, 15 Jun 2022 22:53:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92deca7aa7a34f968926e81414d0102042c2a2e85968fa9423cb1ceed71a9393`  
		Last Modified: Wed, 15 Jun 2022 22:53:28 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f346f796df4e8cb918a2d6f83dcf31d1544d3af9b283727e9757400a160423ab`  
		Last Modified: Wed, 15 Jun 2022 22:53:39 GMT  
		Size: 52.3 MB (52281684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:cd3d27ef331e6abf4963d0f01313133f0ff610644838be15865103605feccd95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.768; amd64

### `docker:20-windowsservercore-ltsc2022` - windows version 10.0.20348.768; amd64

```console
$ docker pull docker@sha256:c92dc04a8ccb9c898c42318e134d11b4fe5e825349a870ec0af4d00a8aa32f30
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2331628569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbf9b630697f8843ffb9923fb2b24ec28ca80c582e396f4bc8ae9db8517438c8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 09 Jun 2022 04:32:50 GMT
RUN Install update 10.0.20348.768
# Wed, 15 Jun 2022 12:13:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:46:14 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:49:43 GMT
ENV DOCKER_VERSION=20.10.17
# Wed, 15 Jun 2022 22:49:44 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.17.zip
# Wed, 15 Jun 2022 22:50:20 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c71967ff41928927e4c407171e4ffbac3c9ab4221eb64f5ca5a34ff4c230567`  
		Size: 841.6 MB (841600427 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dec0338feaf01f35eb916b7fd9ecc08b719354163254885d5215e513c1a3eb2e`  
		Last Modified: Wed, 15 Jun 2022 12:49:26 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a162967ebe5da992f6dc4e9ebdd4ec9f402a84f6974c0c562cff1ed6f17dd39`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 630.9 KB (630886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6900080f685d53c251ad925dfa2391f7ea21ee77b7d5aa31e56e0d7a30666adc`  
		Last Modified: Wed, 15 Jun 2022 22:53:02 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79983762d3966bbf5de5e5397ea8b7173f7fa121d7ab01e2136817be07ae4e0f`  
		Last Modified: Wed, 15 Jun 2022 22:53:02 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7398906a7954731da34c295d4f50bdd50edb96f50ad88006b29eaa94662ccd2`  
		Last Modified: Wed, 15 Jun 2022 22:53:14 GMT  
		Size: 52.5 MB (52529382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10`

```console
$ docker pull docker@sha256:206fb7d9747e035b5fb0b12840d1117ccce38b7508c5967ddd66bfc1f8abc36a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10` - linux; amd64

```console
$ docker pull docker@sha256:d06e6924e1364a690ad454e7b51a75b38f01042cb43df2f9d51098bbbc5b836d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94244378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0208b15ab9702b6bf3b7ac59e6c1d7ebbd679b94bb27367f5763297681a61abc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:23:40 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:23:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:23:46 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:23:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:23:48 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:23:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:23:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:23:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:23:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:23:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:23:52 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a01eeb4b9660234932fe1a5ed6ee12b88476503688d1af44ef2cf5589db59c5`  
		Last Modified: Tue, 07 Jun 2022 18:25:11 GMT  
		Size: 65.5 MB (65511093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f16477544224c056335320872aa8dd6c2a404df9982484e1f62603e0f1f8e2a`  
		Last Modified: Tue, 07 Jun 2022 18:25:01 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e917105572c19bab12a64c5f1079e8d7b0a3e10899bd0398d1f136d41a4af191`  
		Last Modified: Tue, 07 Jun 2022 18:25:00 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709778230e46fbd5042dc9165462ac00b69b08da200fd164c4b55ee90d71ed6`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94076fc9c77a2ec8cd8737d8ee69c11882eaa16be0e46ea97b42763d6de07213`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0650593e055d90b3f09ecf2e61114a35929437150d1f25d6e9aea5e4d4ef57`  
		Last Modified: Tue, 07 Jun 2022 18:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4e95dfecee5f5f5a6ed920904149fdba4cbe725d149df62f88e556f6a64204f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.5 MB (86476390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065f5b92312ea447a580a243adb30727f02719699a6e80d668170755e50bf642`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:44:31 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:44:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:44:36 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:44:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:44:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:44:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:44:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:44:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:44:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:44:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:44:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:44:52 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208c9164699a390332f26552a4e3372cbba8153d21dd8c579d78b4820727447`  
		Last Modified: Tue, 07 Jun 2022 18:46:58 GMT  
		Size: 60.0 MB (60022171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd660eb6acfde977fdcc2e06e1f8b820b994c605f8d7c2a43c8043fee47a59`  
		Last Modified: Tue, 07 Jun 2022 18:46:49 GMT  
		Size: 13.1 MB (13097908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed4b77ab26353356aa5e47399b195759c104e1949f2c8552ed99141fcd5a8e6`  
		Last Modified: Tue, 07 Jun 2022 18:46:48 GMT  
		Size: 8.7 MB (8663386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e346f102da723c6d8f8709a20fe5d2b88c6efc5c31da9c1e7fba1007acd0ec1f`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97325db524006b151b2a34f2981b47567785b4362b383f8672aa4ccd00df3bfe`  
		Last Modified: Tue, 07 Jun 2022 18:46:47 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6e016098eef53d87f0df18ffe9c41bda01a822971b75a0d351d1787a4d59fb`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind`

```console
$ docker pull docker@sha256:a7a9383d0631b5f6b59f0a8138912d20b63c9320127e3fb065cb9ca0257a58b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind` - linux; amd64

```console
$ docker pull docker@sha256:8cdb600dd59001892484f7c4be06166e42a2952065b6822b98c5aa7b8ef2ce8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.1 MB (101111945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dbe252bd9afb23859f250989da416b2cd8ab30f4b61a2bc8fca6f9b05d7e665`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:23:40 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:23:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:23:46 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:23:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:23:48 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:23:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:23:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:23:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:23:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:23:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:23:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:24:02 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 07 Jun 2022 18:24:03 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:24:03 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 07 Jun 2022 18:24:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 07 Jun 2022 18:24:04 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:24:04 GMT
VOLUME [/var/lib/docker]
# Tue, 07 Jun 2022 18:24:04 GMT
EXPOSE 2375 2376
# Tue, 07 Jun 2022 18:24:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 07 Jun 2022 18:24:05 GMT
CMD []
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a01eeb4b9660234932fe1a5ed6ee12b88476503688d1af44ef2cf5589db59c5`  
		Last Modified: Tue, 07 Jun 2022 18:25:11 GMT  
		Size: 65.5 MB (65511093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f16477544224c056335320872aa8dd6c2a404df9982484e1f62603e0f1f8e2a`  
		Last Modified: Tue, 07 Jun 2022 18:25:01 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e917105572c19bab12a64c5f1079e8d7b0a3e10899bd0398d1f136d41a4af191`  
		Last Modified: Tue, 07 Jun 2022 18:25:00 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709778230e46fbd5042dc9165462ac00b69b08da200fd164c4b55ee90d71ed6`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94076fc9c77a2ec8cd8737d8ee69c11882eaa16be0e46ea97b42763d6de07213`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0650593e055d90b3f09ecf2e61114a35929437150d1f25d6e9aea5e4d4ef57`  
		Last Modified: Tue, 07 Jun 2022 18:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8739efbf33852756a9d17dd471ab7ab9d9a1f183df6185763c4f54d55f3e5ef`  
		Last Modified: Tue, 07 Jun 2022 18:25:31 GMT  
		Size: 6.9 MB (6862542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1528486149a1ec660cc13a105d322cbe384bf2fd0bb5b32436043928d35701e8`  
		Last Modified: Tue, 07 Jun 2022 18:25:30 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fce28207d4c0f42d2a8352f195f1551714dfa68bcc768565b63a0e030a46813`  
		Last Modified: Tue, 07 Jun 2022 18:25:29 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c6543c9821cdb12ce3c3b95bed6148272f6ee648fcaf31c1b5b6d7aa67c459`  
		Last Modified: Tue, 07 Jun 2022 18:25:29 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:c82526b54ad542830185247b1fd7cd75ca06c4b7379625a631193ebebbffceb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93216008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d2d13d30ebd3836c5760272dda377aa12d9253bf2aee7a175a1360773e2a9d9`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:44:31 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:44:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:44:36 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:44:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:44:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:44:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:44:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:44:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:44:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:44:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:44:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:44:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:45:01 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 07 Jun 2022 18:45:02 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:45:03 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 07 Jun 2022 18:45:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 07 Jun 2022 18:45:06 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:45:06 GMT
VOLUME [/var/lib/docker]
# Tue, 07 Jun 2022 18:45:07 GMT
EXPOSE 2375 2376
# Tue, 07 Jun 2022 18:45:08 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 07 Jun 2022 18:45:09 GMT
CMD []
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208c9164699a390332f26552a4e3372cbba8153d21dd8c579d78b4820727447`  
		Last Modified: Tue, 07 Jun 2022 18:46:58 GMT  
		Size: 60.0 MB (60022171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd660eb6acfde977fdcc2e06e1f8b820b994c605f8d7c2a43c8043fee47a59`  
		Last Modified: Tue, 07 Jun 2022 18:46:49 GMT  
		Size: 13.1 MB (13097908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed4b77ab26353356aa5e47399b195759c104e1949f2c8552ed99141fcd5a8e6`  
		Last Modified: Tue, 07 Jun 2022 18:46:48 GMT  
		Size: 8.7 MB (8663386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e346f102da723c6d8f8709a20fe5d2b88c6efc5c31da9c1e7fba1007acd0ec1f`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97325db524006b151b2a34f2981b47567785b4362b383f8672aa4ccd00df3bfe`  
		Last Modified: Tue, 07 Jun 2022 18:46:47 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6e016098eef53d87f0df18ffe9c41bda01a822971b75a0d351d1787a4d59fb`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e98490325d999d399e486a1107cbb821ef56e26e4b8e09cba42eab6de668f53`  
		Last Modified: Tue, 07 Jun 2022 18:47:20 GMT  
		Size: 6.7 MB (6734617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3937658d06fd0152ee0795e63b1ac2bef28cd0e08636738ed86cfb3f270efe87`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520215962f31f70fbe23340f593756dd36c602b6523c60d6edf47191a3366f70`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c038ae79644412f10a6fd71b2aeb63c3462ca53f5eba947465d067157abd1d`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 2.7 KB (2748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind-rootless`

```console
$ docker pull docker@sha256:9ff8f7cf745620a1d20cf27034f544f1ff7bca5a2abbcda2857962104e042bc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:96b2a2fefca7613f5b34629ac11cabaf527e8f440cbac8b7dc4c295c10b0e6cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.7 MB (121693146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8475d2a876361c1765ccfcd694b66a7a121b34b3d75a04f55d5b94a7437da1c3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:23:40 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:23:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:23:46 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:23:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:23:48 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:23:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:23:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:23:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:23:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:23:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:23:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:24:02 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 07 Jun 2022 18:24:03 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:24:03 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 07 Jun 2022 18:24:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 07 Jun 2022 18:24:04 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:24:04 GMT
VOLUME [/var/lib/docker]
# Tue, 07 Jun 2022 18:24:04 GMT
EXPOSE 2375 2376
# Tue, 07 Jun 2022 18:24:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 07 Jun 2022 18:24:05 GMT
CMD []
# Tue, 07 Jun 2022 18:24:11 GMT
RUN apk add --no-cache iproute2
# Tue, 07 Jun 2022 18:24:11 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 07 Jun 2022 18:24:12 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:24:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 07 Jun 2022 18:24:15 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 07 Jun 2022 18:24:15 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 07 Jun 2022 18:24:15 GMT
USER rootless
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a01eeb4b9660234932fe1a5ed6ee12b88476503688d1af44ef2cf5589db59c5`  
		Last Modified: Tue, 07 Jun 2022 18:25:11 GMT  
		Size: 65.5 MB (65511093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f16477544224c056335320872aa8dd6c2a404df9982484e1f62603e0f1f8e2a`  
		Last Modified: Tue, 07 Jun 2022 18:25:01 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e917105572c19bab12a64c5f1079e8d7b0a3e10899bd0398d1f136d41a4af191`  
		Last Modified: Tue, 07 Jun 2022 18:25:00 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709778230e46fbd5042dc9165462ac00b69b08da200fd164c4b55ee90d71ed6`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94076fc9c77a2ec8cd8737d8ee69c11882eaa16be0e46ea97b42763d6de07213`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0650593e055d90b3f09ecf2e61114a35929437150d1f25d6e9aea5e4d4ef57`  
		Last Modified: Tue, 07 Jun 2022 18:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8739efbf33852756a9d17dd471ab7ab9d9a1f183df6185763c4f54d55f3e5ef`  
		Last Modified: Tue, 07 Jun 2022 18:25:31 GMT  
		Size: 6.9 MB (6862542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1528486149a1ec660cc13a105d322cbe384bf2fd0bb5b32436043928d35701e8`  
		Last Modified: Tue, 07 Jun 2022 18:25:30 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fce28207d4c0f42d2a8352f195f1551714dfa68bcc768565b63a0e030a46813`  
		Last Modified: Tue, 07 Jun 2022 18:25:29 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c6543c9821cdb12ce3c3b95bed6148272f6ee648fcaf31c1b5b6d7aa67c459`  
		Last Modified: Tue, 07 Jun 2022 18:25:29 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a725abeedbfa4c33a7418f41fd875f275696b28eab0a79ba1aa544660a5e7b`  
		Last Modified: Tue, 07 Jun 2022 18:25:50 GMT  
		Size: 1.2 MB (1232609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6a3e20c8491b4d470b9c1a11dceab173fc5252f5fdb7deca56332f03d5b07d`  
		Last Modified: Tue, 07 Jun 2022 18:25:49 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c3ab7612a60e9dbcc8ef8900c43e8d03e0ee26e556f11ef6d7c7fa68ad5fcc`  
		Last Modified: Tue, 07 Jun 2022 18:25:49 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86880a2ebfe3428ec38a5d7146121cab83d10c47b662e08b7296300c5ba36b90`  
		Last Modified: Tue, 07 Jun 2022 18:25:53 GMT  
		Size: 19.3 MB (19346876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08bf902c5827b673ef106ed1a4eaa55f3b5df8409fea26c822f0b6369895c0b`  
		Last Modified: Tue, 07 Jun 2022 18:25:49 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:32882c77434b98c975ceb1b3b96dffe40acbf1cfe7a0af5d515331e4781d4541
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115640767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62f34441530bb8a901ae97f5ffd28037dfbe34695de70e1f8bd14c5e7d9b09ae`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:44:31 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:44:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:44:36 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:44:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:44:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:44:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:44:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:44:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:44:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:44:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:44:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:44:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:45:01 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 07 Jun 2022 18:45:02 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:45:03 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 07 Jun 2022 18:45:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 07 Jun 2022 18:45:06 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:45:06 GMT
VOLUME [/var/lib/docker]
# Tue, 07 Jun 2022 18:45:07 GMT
EXPOSE 2375 2376
# Tue, 07 Jun 2022 18:45:08 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 07 Jun 2022 18:45:09 GMT
CMD []
# Tue, 07 Jun 2022 18:45:17 GMT
RUN apk add --no-cache iproute2
# Tue, 07 Jun 2022 18:45:18 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 07 Jun 2022 18:45:19 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:45:21 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 07 Jun 2022 18:45:22 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 07 Jun 2022 18:45:23 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 07 Jun 2022 18:45:24 GMT
USER rootless
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208c9164699a390332f26552a4e3372cbba8153d21dd8c579d78b4820727447`  
		Last Modified: Tue, 07 Jun 2022 18:46:58 GMT  
		Size: 60.0 MB (60022171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd660eb6acfde977fdcc2e06e1f8b820b994c605f8d7c2a43c8043fee47a59`  
		Last Modified: Tue, 07 Jun 2022 18:46:49 GMT  
		Size: 13.1 MB (13097908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed4b77ab26353356aa5e47399b195759c104e1949f2c8552ed99141fcd5a8e6`  
		Last Modified: Tue, 07 Jun 2022 18:46:48 GMT  
		Size: 8.7 MB (8663386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e346f102da723c6d8f8709a20fe5d2b88c6efc5c31da9c1e7fba1007acd0ec1f`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97325db524006b151b2a34f2981b47567785b4362b383f8672aa4ccd00df3bfe`  
		Last Modified: Tue, 07 Jun 2022 18:46:47 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6e016098eef53d87f0df18ffe9c41bda01a822971b75a0d351d1787a4d59fb`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e98490325d999d399e486a1107cbb821ef56e26e4b8e09cba42eab6de668f53`  
		Last Modified: Tue, 07 Jun 2022 18:47:20 GMT  
		Size: 6.7 MB (6734617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3937658d06fd0152ee0795e63b1ac2bef28cd0e08636738ed86cfb3f270efe87`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520215962f31f70fbe23340f593756dd36c602b6523c60d6edf47191a3366f70`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c038ae79644412f10a6fd71b2aeb63c3462ca53f5eba947465d067157abd1d`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 2.7 KB (2748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a25f04457a8992aec9515a93b8e684c6308ac16e40609e4aea6e5e17e5a9831`  
		Last Modified: Tue, 07 Jun 2022 18:47:42 GMT  
		Size: 1.2 MB (1246089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4737bba435e3c5bf8e0bd36ea8549325126984e556f0383a65cd0780c17c41f3`  
		Last Modified: Tue, 07 Jun 2022 18:47:41 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153a758456f1bf14ac68b5cc4e5adf575663fbad6ee03e0056a9cd6162b45259`  
		Last Modified: Tue, 07 Jun 2022 18:47:42 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6ecdd375957217ed6f2887df5b1aede054583d798040f1fa03e2113584c479`  
		Last Modified: Tue, 07 Jun 2022 18:47:45 GMT  
		Size: 21.2 MB (21177045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e75e34fe059e0be78079a5bd13cfd80b8d414fad4f717402e56a2fa8343ed0`  
		Last Modified: Tue, 07 Jun 2022 18:47:41 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-git`

```console
$ docker pull docker@sha256:ae822531c5ce930bb49408e170ed0b1fd4efcf86da1777687c90f3471b6f73ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-git` - linux; amd64

```console
$ docker pull docker@sha256:fba3948c035af5fd3a4cbe953195dcbdab125581f254d44044d87b2e88aef8ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101178830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d39449ad493ed1d71480ba17d4dcd56af4c28605f7f5645a1429f077cd8513`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:23:40 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:23:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:23:46 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:23:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:23:48 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:23:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:23:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:23:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:23:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:23:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:23:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:24:19 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a01eeb4b9660234932fe1a5ed6ee12b88476503688d1af44ef2cf5589db59c5`  
		Last Modified: Tue, 07 Jun 2022 18:25:11 GMT  
		Size: 65.5 MB (65511093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f16477544224c056335320872aa8dd6c2a404df9982484e1f62603e0f1f8e2a`  
		Last Modified: Tue, 07 Jun 2022 18:25:01 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e917105572c19bab12a64c5f1079e8d7b0a3e10899bd0398d1f136d41a4af191`  
		Last Modified: Tue, 07 Jun 2022 18:25:00 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709778230e46fbd5042dc9165462ac00b69b08da200fd164c4b55ee90d71ed6`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94076fc9c77a2ec8cd8737d8ee69c11882eaa16be0e46ea97b42763d6de07213`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0650593e055d90b3f09ecf2e61114a35929437150d1f25d6e9aea5e4d4ef57`  
		Last Modified: Tue, 07 Jun 2022 18:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd116fbfcda7d014c42d3891e0c2d200795c968f665e123ee95a0e6d1e5c934`  
		Last Modified: Tue, 07 Jun 2022 18:26:11 GMT  
		Size: 6.9 MB (6934452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f633c11b5bfc875d87905074a8a032404ce2bfefb7e51f9f6919d36277e77393
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.5 MB (93521092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb6d61e7054c42bfa4ad4e5dca6aee71560f8fddb61b5a6a8101a66320730b1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:44:31 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:44:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:44:36 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:44:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:44:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:44:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:44:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:44:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:44:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:44:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:44:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:44:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:45:32 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208c9164699a390332f26552a4e3372cbba8153d21dd8c579d78b4820727447`  
		Last Modified: Tue, 07 Jun 2022 18:46:58 GMT  
		Size: 60.0 MB (60022171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd660eb6acfde977fdcc2e06e1f8b820b994c605f8d7c2a43c8043fee47a59`  
		Last Modified: Tue, 07 Jun 2022 18:46:49 GMT  
		Size: 13.1 MB (13097908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed4b77ab26353356aa5e47399b195759c104e1949f2c8552ed99141fcd5a8e6`  
		Last Modified: Tue, 07 Jun 2022 18:46:48 GMT  
		Size: 8.7 MB (8663386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e346f102da723c6d8f8709a20fe5d2b88c6efc5c31da9c1e7fba1007acd0ec1f`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97325db524006b151b2a34f2981b47567785b4362b383f8672aa4ccd00df3bfe`  
		Last Modified: Tue, 07 Jun 2022 18:46:47 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6e016098eef53d87f0df18ffe9c41bda01a822971b75a0d351d1787a4d59fb`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538445497cbaebac26dcea42aaadf26367e96ea7ccf5c022dcfd39bd1da7c882`  
		Last Modified: Tue, 07 Jun 2022 18:48:05 GMT  
		Size: 7.0 MB (7044702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore`

```console
$ docker pull docker@sha256:c46b51f81569a8528faf11ab678e415a9846ac53246ec6c2b11fc5a81e61674b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.768; amd64
	-	windows version 10.0.17763.3046; amd64

### `docker:20.10-windowsservercore` - windows version 10.0.20348.768; amd64

```console
$ docker pull docker@sha256:c92dc04a8ccb9c898c42318e134d11b4fe5e825349a870ec0af4d00a8aa32f30
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2331628569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbf9b630697f8843ffb9923fb2b24ec28ca80c582e396f4bc8ae9db8517438c8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 09 Jun 2022 04:32:50 GMT
RUN Install update 10.0.20348.768
# Wed, 15 Jun 2022 12:13:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:46:14 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:49:43 GMT
ENV DOCKER_VERSION=20.10.17
# Wed, 15 Jun 2022 22:49:44 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.17.zip
# Wed, 15 Jun 2022 22:50:20 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c71967ff41928927e4c407171e4ffbac3c9ab4221eb64f5ca5a34ff4c230567`  
		Size: 841.6 MB (841600427 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dec0338feaf01f35eb916b7fd9ecc08b719354163254885d5215e513c1a3eb2e`  
		Last Modified: Wed, 15 Jun 2022 12:49:26 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a162967ebe5da992f6dc4e9ebdd4ec9f402a84f6974c0c562cff1ed6f17dd39`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 630.9 KB (630886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6900080f685d53c251ad925dfa2391f7ea21ee77b7d5aa31e56e0d7a30666adc`  
		Last Modified: Wed, 15 Jun 2022 22:53:02 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79983762d3966bbf5de5e5397ea8b7173f7fa121d7ab01e2136817be07ae4e0f`  
		Last Modified: Wed, 15 Jun 2022 22:53:02 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7398906a7954731da34c295d4f50bdd50edb96f50ad88006b29eaa94662ccd2`  
		Last Modified: Wed, 15 Jun 2022 22:53:14 GMT  
		Size: 52.5 MB (52529382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-windowsservercore` - windows version 10.0.17763.3046; amd64

```console
$ docker pull docker@sha256:92b9efc4d05fc727177fa4d4f20e8ca35969778a932858c93dde72a69cafa065
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2715917945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:208e7e03e3e360a634a05b786e8043476d165cf2930fc4237e9c34c390385228`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:48:09 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:50:28 GMT
ENV DOCKER_VERSION=20.10.17
# Wed, 15 Jun 2022 22:50:29 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.17.zip
# Wed, 15 Jun 2022 22:51:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4c7110da70e07b37a00b3b05b18361572412287fee26eba04fcf23dcb75639`  
		Last Modified: Wed, 15 Jun 2022 22:52:48 GMT  
		Size: 352.2 KB (352228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a3fc52e3c402b1be6f7512b16405aaaba3edd6037ede2a7885b367bec19efd`  
		Last Modified: Wed, 15 Jun 2022 22:53:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92deca7aa7a34f968926e81414d0102042c2a2e85968fa9423cb1ceed71a9393`  
		Last Modified: Wed, 15 Jun 2022 22:53:28 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f346f796df4e8cb918a2d6f83dcf31d1544d3af9b283727e9757400a160423ab`  
		Last Modified: Wed, 15 Jun 2022 22:53:39 GMT  
		Size: 52.3 MB (52281684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-1809`

```console
$ docker pull docker@sha256:f8c99a477afebef2e0a504c1a2d40be47010d4e93cb99febe638d0eb20505199
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3046; amd64

### `docker:20.10-windowsservercore-1809` - windows version 10.0.17763.3046; amd64

```console
$ docker pull docker@sha256:92b9efc4d05fc727177fa4d4f20e8ca35969778a932858c93dde72a69cafa065
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2715917945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:208e7e03e3e360a634a05b786e8043476d165cf2930fc4237e9c34c390385228`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:48:09 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:50:28 GMT
ENV DOCKER_VERSION=20.10.17
# Wed, 15 Jun 2022 22:50:29 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.17.zip
# Wed, 15 Jun 2022 22:51:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4c7110da70e07b37a00b3b05b18361572412287fee26eba04fcf23dcb75639`  
		Last Modified: Wed, 15 Jun 2022 22:52:48 GMT  
		Size: 352.2 KB (352228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a3fc52e3c402b1be6f7512b16405aaaba3edd6037ede2a7885b367bec19efd`  
		Last Modified: Wed, 15 Jun 2022 22:53:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92deca7aa7a34f968926e81414d0102042c2a2e85968fa9423cb1ceed71a9393`  
		Last Modified: Wed, 15 Jun 2022 22:53:28 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f346f796df4e8cb918a2d6f83dcf31d1544d3af9b283727e9757400a160423ab`  
		Last Modified: Wed, 15 Jun 2022 22:53:39 GMT  
		Size: 52.3 MB (52281684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:cd3d27ef331e6abf4963d0f01313133f0ff610644838be15865103605feccd95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.768; amd64

### `docker:20.10-windowsservercore-ltsc2022` - windows version 10.0.20348.768; amd64

```console
$ docker pull docker@sha256:c92dc04a8ccb9c898c42318e134d11b4fe5e825349a870ec0af4d00a8aa32f30
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2331628569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbf9b630697f8843ffb9923fb2b24ec28ca80c582e396f4bc8ae9db8517438c8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 09 Jun 2022 04:32:50 GMT
RUN Install update 10.0.20348.768
# Wed, 15 Jun 2022 12:13:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:46:14 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:49:43 GMT
ENV DOCKER_VERSION=20.10.17
# Wed, 15 Jun 2022 22:49:44 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.17.zip
# Wed, 15 Jun 2022 22:50:20 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c71967ff41928927e4c407171e4ffbac3c9ab4221eb64f5ca5a34ff4c230567`  
		Size: 841.6 MB (841600427 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dec0338feaf01f35eb916b7fd9ecc08b719354163254885d5215e513c1a3eb2e`  
		Last Modified: Wed, 15 Jun 2022 12:49:26 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a162967ebe5da992f6dc4e9ebdd4ec9f402a84f6974c0c562cff1ed6f17dd39`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 630.9 KB (630886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6900080f685d53c251ad925dfa2391f7ea21ee77b7d5aa31e56e0d7a30666adc`  
		Last Modified: Wed, 15 Jun 2022 22:53:02 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79983762d3966bbf5de5e5397ea8b7173f7fa121d7ab01e2136817be07ae4e0f`  
		Last Modified: Wed, 15 Jun 2022 22:53:02 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7398906a7954731da34c295d4f50bdd50edb96f50ad88006b29eaa94662ccd2`  
		Last Modified: Wed, 15 Jun 2022 22:53:14 GMT  
		Size: 52.5 MB (52529382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.17`

```console
$ docker pull docker@sha256:206fb7d9747e035b5fb0b12840d1117ccce38b7508c5967ddd66bfc1f8abc36a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.17` - linux; amd64

```console
$ docker pull docker@sha256:d06e6924e1364a690ad454e7b51a75b38f01042cb43df2f9d51098bbbc5b836d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94244378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0208b15ab9702b6bf3b7ac59e6c1d7ebbd679b94bb27367f5763297681a61abc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:23:40 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:23:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:23:46 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:23:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:23:48 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:23:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:23:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:23:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:23:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:23:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:23:52 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a01eeb4b9660234932fe1a5ed6ee12b88476503688d1af44ef2cf5589db59c5`  
		Last Modified: Tue, 07 Jun 2022 18:25:11 GMT  
		Size: 65.5 MB (65511093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f16477544224c056335320872aa8dd6c2a404df9982484e1f62603e0f1f8e2a`  
		Last Modified: Tue, 07 Jun 2022 18:25:01 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e917105572c19bab12a64c5f1079e8d7b0a3e10899bd0398d1f136d41a4af191`  
		Last Modified: Tue, 07 Jun 2022 18:25:00 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709778230e46fbd5042dc9165462ac00b69b08da200fd164c4b55ee90d71ed6`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94076fc9c77a2ec8cd8737d8ee69c11882eaa16be0e46ea97b42763d6de07213`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0650593e055d90b3f09ecf2e61114a35929437150d1f25d6e9aea5e4d4ef57`  
		Last Modified: Tue, 07 Jun 2022 18:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.17` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4e95dfecee5f5f5a6ed920904149fdba4cbe725d149df62f88e556f6a64204f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.5 MB (86476390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065f5b92312ea447a580a243adb30727f02719699a6e80d668170755e50bf642`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:44:31 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:44:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:44:36 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:44:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:44:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:44:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:44:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:44:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:44:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:44:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:44:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:44:52 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208c9164699a390332f26552a4e3372cbba8153d21dd8c579d78b4820727447`  
		Last Modified: Tue, 07 Jun 2022 18:46:58 GMT  
		Size: 60.0 MB (60022171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd660eb6acfde977fdcc2e06e1f8b820b994c605f8d7c2a43c8043fee47a59`  
		Last Modified: Tue, 07 Jun 2022 18:46:49 GMT  
		Size: 13.1 MB (13097908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed4b77ab26353356aa5e47399b195759c104e1949f2c8552ed99141fcd5a8e6`  
		Last Modified: Tue, 07 Jun 2022 18:46:48 GMT  
		Size: 8.7 MB (8663386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e346f102da723c6d8f8709a20fe5d2b88c6efc5c31da9c1e7fba1007acd0ec1f`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97325db524006b151b2a34f2981b47567785b4362b383f8672aa4ccd00df3bfe`  
		Last Modified: Tue, 07 Jun 2022 18:46:47 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6e016098eef53d87f0df18ffe9c41bda01a822971b75a0d351d1787a4d59fb`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.17-alpine3.16`

```console
$ docker pull docker@sha256:206fb7d9747e035b5fb0b12840d1117ccce38b7508c5967ddd66bfc1f8abc36a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.17-alpine3.16` - linux; amd64

```console
$ docker pull docker@sha256:d06e6924e1364a690ad454e7b51a75b38f01042cb43df2f9d51098bbbc5b836d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94244378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0208b15ab9702b6bf3b7ac59e6c1d7ebbd679b94bb27367f5763297681a61abc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:23:40 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:23:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:23:46 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:23:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:23:48 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:23:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:23:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:23:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:23:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:23:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:23:52 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a01eeb4b9660234932fe1a5ed6ee12b88476503688d1af44ef2cf5589db59c5`  
		Last Modified: Tue, 07 Jun 2022 18:25:11 GMT  
		Size: 65.5 MB (65511093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f16477544224c056335320872aa8dd6c2a404df9982484e1f62603e0f1f8e2a`  
		Last Modified: Tue, 07 Jun 2022 18:25:01 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e917105572c19bab12a64c5f1079e8d7b0a3e10899bd0398d1f136d41a4af191`  
		Last Modified: Tue, 07 Jun 2022 18:25:00 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709778230e46fbd5042dc9165462ac00b69b08da200fd164c4b55ee90d71ed6`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94076fc9c77a2ec8cd8737d8ee69c11882eaa16be0e46ea97b42763d6de07213`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0650593e055d90b3f09ecf2e61114a35929437150d1f25d6e9aea5e4d4ef57`  
		Last Modified: Tue, 07 Jun 2022 18:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.17-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4e95dfecee5f5f5a6ed920904149fdba4cbe725d149df62f88e556f6a64204f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.5 MB (86476390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065f5b92312ea447a580a243adb30727f02719699a6e80d668170755e50bf642`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:44:31 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:44:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:44:36 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:44:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:44:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:44:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:44:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:44:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:44:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:44:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:44:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:44:52 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208c9164699a390332f26552a4e3372cbba8153d21dd8c579d78b4820727447`  
		Last Modified: Tue, 07 Jun 2022 18:46:58 GMT  
		Size: 60.0 MB (60022171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd660eb6acfde977fdcc2e06e1f8b820b994c605f8d7c2a43c8043fee47a59`  
		Last Modified: Tue, 07 Jun 2022 18:46:49 GMT  
		Size: 13.1 MB (13097908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed4b77ab26353356aa5e47399b195759c104e1949f2c8552ed99141fcd5a8e6`  
		Last Modified: Tue, 07 Jun 2022 18:46:48 GMT  
		Size: 8.7 MB (8663386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e346f102da723c6d8f8709a20fe5d2b88c6efc5c31da9c1e7fba1007acd0ec1f`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97325db524006b151b2a34f2981b47567785b4362b383f8672aa4ccd00df3bfe`  
		Last Modified: Tue, 07 Jun 2022 18:46:47 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6e016098eef53d87f0df18ffe9c41bda01a822971b75a0d351d1787a4d59fb`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.17-dind`

```console
$ docker pull docker@sha256:a7a9383d0631b5f6b59f0a8138912d20b63c9320127e3fb065cb9ca0257a58b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.17-dind` - linux; amd64

```console
$ docker pull docker@sha256:8cdb600dd59001892484f7c4be06166e42a2952065b6822b98c5aa7b8ef2ce8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.1 MB (101111945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dbe252bd9afb23859f250989da416b2cd8ab30f4b61a2bc8fca6f9b05d7e665`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:23:40 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:23:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:23:46 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:23:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:23:48 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:23:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:23:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:23:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:23:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:23:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:23:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:24:02 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 07 Jun 2022 18:24:03 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:24:03 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 07 Jun 2022 18:24:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 07 Jun 2022 18:24:04 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:24:04 GMT
VOLUME [/var/lib/docker]
# Tue, 07 Jun 2022 18:24:04 GMT
EXPOSE 2375 2376
# Tue, 07 Jun 2022 18:24:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 07 Jun 2022 18:24:05 GMT
CMD []
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a01eeb4b9660234932fe1a5ed6ee12b88476503688d1af44ef2cf5589db59c5`  
		Last Modified: Tue, 07 Jun 2022 18:25:11 GMT  
		Size: 65.5 MB (65511093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f16477544224c056335320872aa8dd6c2a404df9982484e1f62603e0f1f8e2a`  
		Last Modified: Tue, 07 Jun 2022 18:25:01 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e917105572c19bab12a64c5f1079e8d7b0a3e10899bd0398d1f136d41a4af191`  
		Last Modified: Tue, 07 Jun 2022 18:25:00 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709778230e46fbd5042dc9165462ac00b69b08da200fd164c4b55ee90d71ed6`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94076fc9c77a2ec8cd8737d8ee69c11882eaa16be0e46ea97b42763d6de07213`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0650593e055d90b3f09ecf2e61114a35929437150d1f25d6e9aea5e4d4ef57`  
		Last Modified: Tue, 07 Jun 2022 18:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8739efbf33852756a9d17dd471ab7ab9d9a1f183df6185763c4f54d55f3e5ef`  
		Last Modified: Tue, 07 Jun 2022 18:25:31 GMT  
		Size: 6.9 MB (6862542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1528486149a1ec660cc13a105d322cbe384bf2fd0bb5b32436043928d35701e8`  
		Last Modified: Tue, 07 Jun 2022 18:25:30 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fce28207d4c0f42d2a8352f195f1551714dfa68bcc768565b63a0e030a46813`  
		Last Modified: Tue, 07 Jun 2022 18:25:29 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c6543c9821cdb12ce3c3b95bed6148272f6ee648fcaf31c1b5b6d7aa67c459`  
		Last Modified: Tue, 07 Jun 2022 18:25:29 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.17-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:c82526b54ad542830185247b1fd7cd75ca06c4b7379625a631193ebebbffceb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93216008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d2d13d30ebd3836c5760272dda377aa12d9253bf2aee7a175a1360773e2a9d9`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:44:31 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:44:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:44:36 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:44:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:44:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:44:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:44:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:44:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:44:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:44:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:44:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:44:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:45:01 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 07 Jun 2022 18:45:02 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:45:03 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 07 Jun 2022 18:45:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 07 Jun 2022 18:45:06 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:45:06 GMT
VOLUME [/var/lib/docker]
# Tue, 07 Jun 2022 18:45:07 GMT
EXPOSE 2375 2376
# Tue, 07 Jun 2022 18:45:08 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 07 Jun 2022 18:45:09 GMT
CMD []
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208c9164699a390332f26552a4e3372cbba8153d21dd8c579d78b4820727447`  
		Last Modified: Tue, 07 Jun 2022 18:46:58 GMT  
		Size: 60.0 MB (60022171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd660eb6acfde977fdcc2e06e1f8b820b994c605f8d7c2a43c8043fee47a59`  
		Last Modified: Tue, 07 Jun 2022 18:46:49 GMT  
		Size: 13.1 MB (13097908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed4b77ab26353356aa5e47399b195759c104e1949f2c8552ed99141fcd5a8e6`  
		Last Modified: Tue, 07 Jun 2022 18:46:48 GMT  
		Size: 8.7 MB (8663386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e346f102da723c6d8f8709a20fe5d2b88c6efc5c31da9c1e7fba1007acd0ec1f`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97325db524006b151b2a34f2981b47567785b4362b383f8672aa4ccd00df3bfe`  
		Last Modified: Tue, 07 Jun 2022 18:46:47 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6e016098eef53d87f0df18ffe9c41bda01a822971b75a0d351d1787a4d59fb`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e98490325d999d399e486a1107cbb821ef56e26e4b8e09cba42eab6de668f53`  
		Last Modified: Tue, 07 Jun 2022 18:47:20 GMT  
		Size: 6.7 MB (6734617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3937658d06fd0152ee0795e63b1ac2bef28cd0e08636738ed86cfb3f270efe87`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520215962f31f70fbe23340f593756dd36c602b6523c60d6edf47191a3366f70`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c038ae79644412f10a6fd71b2aeb63c3462ca53f5eba947465d067157abd1d`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 2.7 KB (2748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.17-dind-alpine3.16`

```console
$ docker pull docker@sha256:a7a9383d0631b5f6b59f0a8138912d20b63c9320127e3fb065cb9ca0257a58b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.17-dind-alpine3.16` - linux; amd64

```console
$ docker pull docker@sha256:8cdb600dd59001892484f7c4be06166e42a2952065b6822b98c5aa7b8ef2ce8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.1 MB (101111945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dbe252bd9afb23859f250989da416b2cd8ab30f4b61a2bc8fca6f9b05d7e665`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:23:40 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:23:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:23:46 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:23:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:23:48 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:23:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:23:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:23:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:23:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:23:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:23:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:24:02 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 07 Jun 2022 18:24:03 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:24:03 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 07 Jun 2022 18:24:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 07 Jun 2022 18:24:04 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:24:04 GMT
VOLUME [/var/lib/docker]
# Tue, 07 Jun 2022 18:24:04 GMT
EXPOSE 2375 2376
# Tue, 07 Jun 2022 18:24:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 07 Jun 2022 18:24:05 GMT
CMD []
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a01eeb4b9660234932fe1a5ed6ee12b88476503688d1af44ef2cf5589db59c5`  
		Last Modified: Tue, 07 Jun 2022 18:25:11 GMT  
		Size: 65.5 MB (65511093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f16477544224c056335320872aa8dd6c2a404df9982484e1f62603e0f1f8e2a`  
		Last Modified: Tue, 07 Jun 2022 18:25:01 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e917105572c19bab12a64c5f1079e8d7b0a3e10899bd0398d1f136d41a4af191`  
		Last Modified: Tue, 07 Jun 2022 18:25:00 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709778230e46fbd5042dc9165462ac00b69b08da200fd164c4b55ee90d71ed6`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94076fc9c77a2ec8cd8737d8ee69c11882eaa16be0e46ea97b42763d6de07213`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0650593e055d90b3f09ecf2e61114a35929437150d1f25d6e9aea5e4d4ef57`  
		Last Modified: Tue, 07 Jun 2022 18:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8739efbf33852756a9d17dd471ab7ab9d9a1f183df6185763c4f54d55f3e5ef`  
		Last Modified: Tue, 07 Jun 2022 18:25:31 GMT  
		Size: 6.9 MB (6862542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1528486149a1ec660cc13a105d322cbe384bf2fd0bb5b32436043928d35701e8`  
		Last Modified: Tue, 07 Jun 2022 18:25:30 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fce28207d4c0f42d2a8352f195f1551714dfa68bcc768565b63a0e030a46813`  
		Last Modified: Tue, 07 Jun 2022 18:25:29 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c6543c9821cdb12ce3c3b95bed6148272f6ee648fcaf31c1b5b6d7aa67c459`  
		Last Modified: Tue, 07 Jun 2022 18:25:29 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.17-dind-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:c82526b54ad542830185247b1fd7cd75ca06c4b7379625a631193ebebbffceb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93216008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d2d13d30ebd3836c5760272dda377aa12d9253bf2aee7a175a1360773e2a9d9`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:44:31 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:44:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:44:36 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:44:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:44:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:44:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:44:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:44:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:44:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:44:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:44:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:44:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:45:01 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 07 Jun 2022 18:45:02 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:45:03 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 07 Jun 2022 18:45:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 07 Jun 2022 18:45:06 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:45:06 GMT
VOLUME [/var/lib/docker]
# Tue, 07 Jun 2022 18:45:07 GMT
EXPOSE 2375 2376
# Tue, 07 Jun 2022 18:45:08 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 07 Jun 2022 18:45:09 GMT
CMD []
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208c9164699a390332f26552a4e3372cbba8153d21dd8c579d78b4820727447`  
		Last Modified: Tue, 07 Jun 2022 18:46:58 GMT  
		Size: 60.0 MB (60022171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd660eb6acfde977fdcc2e06e1f8b820b994c605f8d7c2a43c8043fee47a59`  
		Last Modified: Tue, 07 Jun 2022 18:46:49 GMT  
		Size: 13.1 MB (13097908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed4b77ab26353356aa5e47399b195759c104e1949f2c8552ed99141fcd5a8e6`  
		Last Modified: Tue, 07 Jun 2022 18:46:48 GMT  
		Size: 8.7 MB (8663386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e346f102da723c6d8f8709a20fe5d2b88c6efc5c31da9c1e7fba1007acd0ec1f`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97325db524006b151b2a34f2981b47567785b4362b383f8672aa4ccd00df3bfe`  
		Last Modified: Tue, 07 Jun 2022 18:46:47 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6e016098eef53d87f0df18ffe9c41bda01a822971b75a0d351d1787a4d59fb`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e98490325d999d399e486a1107cbb821ef56e26e4b8e09cba42eab6de668f53`  
		Last Modified: Tue, 07 Jun 2022 18:47:20 GMT  
		Size: 6.7 MB (6734617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3937658d06fd0152ee0795e63b1ac2bef28cd0e08636738ed86cfb3f270efe87`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520215962f31f70fbe23340f593756dd36c602b6523c60d6edf47191a3366f70`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c038ae79644412f10a6fd71b2aeb63c3462ca53f5eba947465d067157abd1d`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 2.7 KB (2748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.17-dind-rootless`

```console
$ docker pull docker@sha256:9ff8f7cf745620a1d20cf27034f544f1ff7bca5a2abbcda2857962104e042bc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.17-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:96b2a2fefca7613f5b34629ac11cabaf527e8f440cbac8b7dc4c295c10b0e6cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.7 MB (121693146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8475d2a876361c1765ccfcd694b66a7a121b34b3d75a04f55d5b94a7437da1c3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:23:40 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:23:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:23:46 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:23:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:23:48 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:23:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:23:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:23:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:23:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:23:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:23:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:24:02 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 07 Jun 2022 18:24:03 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:24:03 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 07 Jun 2022 18:24:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 07 Jun 2022 18:24:04 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:24:04 GMT
VOLUME [/var/lib/docker]
# Tue, 07 Jun 2022 18:24:04 GMT
EXPOSE 2375 2376
# Tue, 07 Jun 2022 18:24:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 07 Jun 2022 18:24:05 GMT
CMD []
# Tue, 07 Jun 2022 18:24:11 GMT
RUN apk add --no-cache iproute2
# Tue, 07 Jun 2022 18:24:11 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 07 Jun 2022 18:24:12 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:24:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 07 Jun 2022 18:24:15 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 07 Jun 2022 18:24:15 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 07 Jun 2022 18:24:15 GMT
USER rootless
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a01eeb4b9660234932fe1a5ed6ee12b88476503688d1af44ef2cf5589db59c5`  
		Last Modified: Tue, 07 Jun 2022 18:25:11 GMT  
		Size: 65.5 MB (65511093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f16477544224c056335320872aa8dd6c2a404df9982484e1f62603e0f1f8e2a`  
		Last Modified: Tue, 07 Jun 2022 18:25:01 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e917105572c19bab12a64c5f1079e8d7b0a3e10899bd0398d1f136d41a4af191`  
		Last Modified: Tue, 07 Jun 2022 18:25:00 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709778230e46fbd5042dc9165462ac00b69b08da200fd164c4b55ee90d71ed6`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94076fc9c77a2ec8cd8737d8ee69c11882eaa16be0e46ea97b42763d6de07213`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0650593e055d90b3f09ecf2e61114a35929437150d1f25d6e9aea5e4d4ef57`  
		Last Modified: Tue, 07 Jun 2022 18:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8739efbf33852756a9d17dd471ab7ab9d9a1f183df6185763c4f54d55f3e5ef`  
		Last Modified: Tue, 07 Jun 2022 18:25:31 GMT  
		Size: 6.9 MB (6862542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1528486149a1ec660cc13a105d322cbe384bf2fd0bb5b32436043928d35701e8`  
		Last Modified: Tue, 07 Jun 2022 18:25:30 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fce28207d4c0f42d2a8352f195f1551714dfa68bcc768565b63a0e030a46813`  
		Last Modified: Tue, 07 Jun 2022 18:25:29 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c6543c9821cdb12ce3c3b95bed6148272f6ee648fcaf31c1b5b6d7aa67c459`  
		Last Modified: Tue, 07 Jun 2022 18:25:29 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a725abeedbfa4c33a7418f41fd875f275696b28eab0a79ba1aa544660a5e7b`  
		Last Modified: Tue, 07 Jun 2022 18:25:50 GMT  
		Size: 1.2 MB (1232609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6a3e20c8491b4d470b9c1a11dceab173fc5252f5fdb7deca56332f03d5b07d`  
		Last Modified: Tue, 07 Jun 2022 18:25:49 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c3ab7612a60e9dbcc8ef8900c43e8d03e0ee26e556f11ef6d7c7fa68ad5fcc`  
		Last Modified: Tue, 07 Jun 2022 18:25:49 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86880a2ebfe3428ec38a5d7146121cab83d10c47b662e08b7296300c5ba36b90`  
		Last Modified: Tue, 07 Jun 2022 18:25:53 GMT  
		Size: 19.3 MB (19346876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08bf902c5827b673ef106ed1a4eaa55f3b5df8409fea26c822f0b6369895c0b`  
		Last Modified: Tue, 07 Jun 2022 18:25:49 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.17-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:32882c77434b98c975ceb1b3b96dffe40acbf1cfe7a0af5d515331e4781d4541
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115640767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62f34441530bb8a901ae97f5ffd28037dfbe34695de70e1f8bd14c5e7d9b09ae`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:44:31 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:44:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:44:36 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:44:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:44:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:44:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:44:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:44:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:44:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:44:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:44:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:44:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:45:01 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 07 Jun 2022 18:45:02 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:45:03 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 07 Jun 2022 18:45:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 07 Jun 2022 18:45:06 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:45:06 GMT
VOLUME [/var/lib/docker]
# Tue, 07 Jun 2022 18:45:07 GMT
EXPOSE 2375 2376
# Tue, 07 Jun 2022 18:45:08 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 07 Jun 2022 18:45:09 GMT
CMD []
# Tue, 07 Jun 2022 18:45:17 GMT
RUN apk add --no-cache iproute2
# Tue, 07 Jun 2022 18:45:18 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 07 Jun 2022 18:45:19 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:45:21 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 07 Jun 2022 18:45:22 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 07 Jun 2022 18:45:23 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 07 Jun 2022 18:45:24 GMT
USER rootless
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208c9164699a390332f26552a4e3372cbba8153d21dd8c579d78b4820727447`  
		Last Modified: Tue, 07 Jun 2022 18:46:58 GMT  
		Size: 60.0 MB (60022171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd660eb6acfde977fdcc2e06e1f8b820b994c605f8d7c2a43c8043fee47a59`  
		Last Modified: Tue, 07 Jun 2022 18:46:49 GMT  
		Size: 13.1 MB (13097908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed4b77ab26353356aa5e47399b195759c104e1949f2c8552ed99141fcd5a8e6`  
		Last Modified: Tue, 07 Jun 2022 18:46:48 GMT  
		Size: 8.7 MB (8663386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e346f102da723c6d8f8709a20fe5d2b88c6efc5c31da9c1e7fba1007acd0ec1f`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97325db524006b151b2a34f2981b47567785b4362b383f8672aa4ccd00df3bfe`  
		Last Modified: Tue, 07 Jun 2022 18:46:47 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6e016098eef53d87f0df18ffe9c41bda01a822971b75a0d351d1787a4d59fb`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e98490325d999d399e486a1107cbb821ef56e26e4b8e09cba42eab6de668f53`  
		Last Modified: Tue, 07 Jun 2022 18:47:20 GMT  
		Size: 6.7 MB (6734617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3937658d06fd0152ee0795e63b1ac2bef28cd0e08636738ed86cfb3f270efe87`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520215962f31f70fbe23340f593756dd36c602b6523c60d6edf47191a3366f70`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c038ae79644412f10a6fd71b2aeb63c3462ca53f5eba947465d067157abd1d`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 2.7 KB (2748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a25f04457a8992aec9515a93b8e684c6308ac16e40609e4aea6e5e17e5a9831`  
		Last Modified: Tue, 07 Jun 2022 18:47:42 GMT  
		Size: 1.2 MB (1246089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4737bba435e3c5bf8e0bd36ea8549325126984e556f0383a65cd0780c17c41f3`  
		Last Modified: Tue, 07 Jun 2022 18:47:41 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153a758456f1bf14ac68b5cc4e5adf575663fbad6ee03e0056a9cd6162b45259`  
		Last Modified: Tue, 07 Jun 2022 18:47:42 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6ecdd375957217ed6f2887df5b1aede054583d798040f1fa03e2113584c479`  
		Last Modified: Tue, 07 Jun 2022 18:47:45 GMT  
		Size: 21.2 MB (21177045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e75e34fe059e0be78079a5bd13cfd80b8d414fad4f717402e56a2fa8343ed0`  
		Last Modified: Tue, 07 Jun 2022 18:47:41 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.17-git`

```console
$ docker pull docker@sha256:ae822531c5ce930bb49408e170ed0b1fd4efcf86da1777687c90f3471b6f73ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.17-git` - linux; amd64

```console
$ docker pull docker@sha256:fba3948c035af5fd3a4cbe953195dcbdab125581f254d44044d87b2e88aef8ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101178830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d39449ad493ed1d71480ba17d4dcd56af4c28605f7f5645a1429f077cd8513`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:23:40 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:23:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:23:46 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:23:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:23:48 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:23:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:23:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:23:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:23:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:23:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:23:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:24:19 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a01eeb4b9660234932fe1a5ed6ee12b88476503688d1af44ef2cf5589db59c5`  
		Last Modified: Tue, 07 Jun 2022 18:25:11 GMT  
		Size: 65.5 MB (65511093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f16477544224c056335320872aa8dd6c2a404df9982484e1f62603e0f1f8e2a`  
		Last Modified: Tue, 07 Jun 2022 18:25:01 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e917105572c19bab12a64c5f1079e8d7b0a3e10899bd0398d1f136d41a4af191`  
		Last Modified: Tue, 07 Jun 2022 18:25:00 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709778230e46fbd5042dc9165462ac00b69b08da200fd164c4b55ee90d71ed6`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94076fc9c77a2ec8cd8737d8ee69c11882eaa16be0e46ea97b42763d6de07213`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0650593e055d90b3f09ecf2e61114a35929437150d1f25d6e9aea5e4d4ef57`  
		Last Modified: Tue, 07 Jun 2022 18:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd116fbfcda7d014c42d3891e0c2d200795c968f665e123ee95a0e6d1e5c934`  
		Last Modified: Tue, 07 Jun 2022 18:26:11 GMT  
		Size: 6.9 MB (6934452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.17-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f633c11b5bfc875d87905074a8a032404ce2bfefb7e51f9f6919d36277e77393
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.5 MB (93521092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb6d61e7054c42bfa4ad4e5dca6aee71560f8fddb61b5a6a8101a66320730b1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:44:31 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:44:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:44:36 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:44:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:44:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:44:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:44:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:44:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:44:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:44:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:44:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:44:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:45:32 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208c9164699a390332f26552a4e3372cbba8153d21dd8c579d78b4820727447`  
		Last Modified: Tue, 07 Jun 2022 18:46:58 GMT  
		Size: 60.0 MB (60022171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd660eb6acfde977fdcc2e06e1f8b820b994c605f8d7c2a43c8043fee47a59`  
		Last Modified: Tue, 07 Jun 2022 18:46:49 GMT  
		Size: 13.1 MB (13097908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed4b77ab26353356aa5e47399b195759c104e1949f2c8552ed99141fcd5a8e6`  
		Last Modified: Tue, 07 Jun 2022 18:46:48 GMT  
		Size: 8.7 MB (8663386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e346f102da723c6d8f8709a20fe5d2b88c6efc5c31da9c1e7fba1007acd0ec1f`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97325db524006b151b2a34f2981b47567785b4362b383f8672aa4ccd00df3bfe`  
		Last Modified: Tue, 07 Jun 2022 18:46:47 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6e016098eef53d87f0df18ffe9c41bda01a822971b75a0d351d1787a4d59fb`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538445497cbaebac26dcea42aaadf26367e96ea7ccf5c022dcfd39bd1da7c882`  
		Last Modified: Tue, 07 Jun 2022 18:48:05 GMT  
		Size: 7.0 MB (7044702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.17-windowsservercore`

```console
$ docker pull docker@sha256:c46b51f81569a8528faf11ab678e415a9846ac53246ec6c2b11fc5a81e61674b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.768; amd64
	-	windows version 10.0.17763.3046; amd64

### `docker:20.10.17-windowsservercore` - windows version 10.0.20348.768; amd64

```console
$ docker pull docker@sha256:c92dc04a8ccb9c898c42318e134d11b4fe5e825349a870ec0af4d00a8aa32f30
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2331628569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbf9b630697f8843ffb9923fb2b24ec28ca80c582e396f4bc8ae9db8517438c8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 09 Jun 2022 04:32:50 GMT
RUN Install update 10.0.20348.768
# Wed, 15 Jun 2022 12:13:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:46:14 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:49:43 GMT
ENV DOCKER_VERSION=20.10.17
# Wed, 15 Jun 2022 22:49:44 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.17.zip
# Wed, 15 Jun 2022 22:50:20 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c71967ff41928927e4c407171e4ffbac3c9ab4221eb64f5ca5a34ff4c230567`  
		Size: 841.6 MB (841600427 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dec0338feaf01f35eb916b7fd9ecc08b719354163254885d5215e513c1a3eb2e`  
		Last Modified: Wed, 15 Jun 2022 12:49:26 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a162967ebe5da992f6dc4e9ebdd4ec9f402a84f6974c0c562cff1ed6f17dd39`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 630.9 KB (630886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6900080f685d53c251ad925dfa2391f7ea21ee77b7d5aa31e56e0d7a30666adc`  
		Last Modified: Wed, 15 Jun 2022 22:53:02 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79983762d3966bbf5de5e5397ea8b7173f7fa121d7ab01e2136817be07ae4e0f`  
		Last Modified: Wed, 15 Jun 2022 22:53:02 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7398906a7954731da34c295d4f50bdd50edb96f50ad88006b29eaa94662ccd2`  
		Last Modified: Wed, 15 Jun 2022 22:53:14 GMT  
		Size: 52.5 MB (52529382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.17-windowsservercore` - windows version 10.0.17763.3046; amd64

```console
$ docker pull docker@sha256:92b9efc4d05fc727177fa4d4f20e8ca35969778a932858c93dde72a69cafa065
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2715917945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:208e7e03e3e360a634a05b786e8043476d165cf2930fc4237e9c34c390385228`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:48:09 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:50:28 GMT
ENV DOCKER_VERSION=20.10.17
# Wed, 15 Jun 2022 22:50:29 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.17.zip
# Wed, 15 Jun 2022 22:51:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4c7110da70e07b37a00b3b05b18361572412287fee26eba04fcf23dcb75639`  
		Last Modified: Wed, 15 Jun 2022 22:52:48 GMT  
		Size: 352.2 KB (352228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a3fc52e3c402b1be6f7512b16405aaaba3edd6037ede2a7885b367bec19efd`  
		Last Modified: Wed, 15 Jun 2022 22:53:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92deca7aa7a34f968926e81414d0102042c2a2e85968fa9423cb1ceed71a9393`  
		Last Modified: Wed, 15 Jun 2022 22:53:28 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f346f796df4e8cb918a2d6f83dcf31d1544d3af9b283727e9757400a160423ab`  
		Last Modified: Wed, 15 Jun 2022 22:53:39 GMT  
		Size: 52.3 MB (52281684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.17-windowsservercore-1809`

```console
$ docker pull docker@sha256:f8c99a477afebef2e0a504c1a2d40be47010d4e93cb99febe638d0eb20505199
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3046; amd64

### `docker:20.10.17-windowsservercore-1809` - windows version 10.0.17763.3046; amd64

```console
$ docker pull docker@sha256:92b9efc4d05fc727177fa4d4f20e8ca35969778a932858c93dde72a69cafa065
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2715917945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:208e7e03e3e360a634a05b786e8043476d165cf2930fc4237e9c34c390385228`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:48:09 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:50:28 GMT
ENV DOCKER_VERSION=20.10.17
# Wed, 15 Jun 2022 22:50:29 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.17.zip
# Wed, 15 Jun 2022 22:51:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4c7110da70e07b37a00b3b05b18361572412287fee26eba04fcf23dcb75639`  
		Last Modified: Wed, 15 Jun 2022 22:52:48 GMT  
		Size: 352.2 KB (352228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a3fc52e3c402b1be6f7512b16405aaaba3edd6037ede2a7885b367bec19efd`  
		Last Modified: Wed, 15 Jun 2022 22:53:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92deca7aa7a34f968926e81414d0102042c2a2e85968fa9423cb1ceed71a9393`  
		Last Modified: Wed, 15 Jun 2022 22:53:28 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f346f796df4e8cb918a2d6f83dcf31d1544d3af9b283727e9757400a160423ab`  
		Last Modified: Wed, 15 Jun 2022 22:53:39 GMT  
		Size: 52.3 MB (52281684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.17-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:cd3d27ef331e6abf4963d0f01313133f0ff610644838be15865103605feccd95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.768; amd64

### `docker:20.10.17-windowsservercore-ltsc2022` - windows version 10.0.20348.768; amd64

```console
$ docker pull docker@sha256:c92dc04a8ccb9c898c42318e134d11b4fe5e825349a870ec0af4d00a8aa32f30
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2331628569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbf9b630697f8843ffb9923fb2b24ec28ca80c582e396f4bc8ae9db8517438c8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 09 Jun 2022 04:32:50 GMT
RUN Install update 10.0.20348.768
# Wed, 15 Jun 2022 12:13:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:46:14 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:49:43 GMT
ENV DOCKER_VERSION=20.10.17
# Wed, 15 Jun 2022 22:49:44 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.17.zip
# Wed, 15 Jun 2022 22:50:20 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c71967ff41928927e4c407171e4ffbac3c9ab4221eb64f5ca5a34ff4c230567`  
		Size: 841.6 MB (841600427 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dec0338feaf01f35eb916b7fd9ecc08b719354163254885d5215e513c1a3eb2e`  
		Last Modified: Wed, 15 Jun 2022 12:49:26 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a162967ebe5da992f6dc4e9ebdd4ec9f402a84f6974c0c562cff1ed6f17dd39`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 630.9 KB (630886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6900080f685d53c251ad925dfa2391f7ea21ee77b7d5aa31e56e0d7a30666adc`  
		Last Modified: Wed, 15 Jun 2022 22:53:02 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79983762d3966bbf5de5e5397ea8b7173f7fa121d7ab01e2136817be07ae4e0f`  
		Last Modified: Wed, 15 Jun 2022 22:53:02 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7398906a7954731da34c295d4f50bdd50edb96f50ad88006b29eaa94662ccd2`  
		Last Modified: Wed, 15 Jun 2022 22:53:14 GMT  
		Size: 52.5 MB (52529382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:22.06-rc`

```console
$ docker pull docker@sha256:0964ecc3084a4908f49afef17df539e7f355c5336969ad41ec9200182b919cb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:22.06-rc` - linux; amd64

```console
$ docker pull docker@sha256:b9614a53230d0a4c4f22f2d004e04362d9f147082898cd507de08736cfe744a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.8 MB (90771523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007fe5047a7c961c196b4479f8e4263e4da34c07677f92e330cf9749228dba4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 19:01:29 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 19:01:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 19:01:35 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 19:01:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 19:01:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 19:01:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 19:01:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 19:01:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:45 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99ba1e24152bfcd6f75ac7d03379a0d722bb011a60e4da292b3234ed0c229c5`  
		Last Modified: Mon, 06 Jun 2022 19:03:02 GMT  
		Size: 62.0 MB (62038242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d073b016bf56120f6f99463e72dfc1669ee2cf81aea28338e191dc3392b76c2`  
		Last Modified: Mon, 06 Jun 2022 19:02:53 GMT  
		Size: 14.5 MB (14454318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae7a7070ea618fa5d597e5c3d9fafb5531a4c0ba8b5f7f12e334175f7424643`  
		Last Modified: Mon, 06 Jun 2022 19:02:52 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b69fd3006304e4afc4226a31c41076934d97c9a0c8d536bc2acda02006dab5`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff67f9f388ec6907bd17f3fa9106924c548d5374d7e483e089076822e8759f9`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77709b39dac35a99fc73e9b30dab31b8e61f7729021558d7647d544c1eaa0f23`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:22.06-rc` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f1168269caf92da50e2c6c8781facff325d5a643079ef6534abf1b293d9cbfa7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.5 MB (83481513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3af4b446c8d50a9581547b8dc9a07922f7666fe639a1ffda87e9842bacadbf5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 18:36:44 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 18:36:50 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 18:36:50 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 18:36:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 18:36:55 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 18:36:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 18:37:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 18:37:02 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 18:37:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 18:37:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:05 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f1c4eb6753c4d8ca8abdc68946eaf136ebf43c3ba68b1e3f168d561a7a40e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:21 GMT  
		Size: 57.0 MB (57027293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8543d611571340a3ade0985e604f8050b3bd7c750ce108d248072285be716e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:13 GMT  
		Size: 13.1 MB (13097906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55bb534319c1b57528e0e77d4e31677b56a064afe3ef44ab80b3dcbb546fba69`  
		Last Modified: Mon, 06 Jun 2022 18:39:12 GMT  
		Size: 8.7 MB (8663389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596ba91569b21aa39db419bf97611342f554933900d729efaea259246e43c6c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8084d414abe81d6b025915fb786b9604e6c92ca873948a0840d95927314986bc`  
		Last Modified: Mon, 06 Jun 2022 18:39:11 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62b19d6f46e3b8b83902e63f8497def66bced996fd9b45792acf2c9d5afe0c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:22.06-rc-dind`

```console
$ docker pull docker@sha256:aac3ee54242eb33fddb238884878e0d5c059b2b227f6914086ddb183064f7314
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:22.06-rc-dind` - linux; amd64

```console
$ docker pull docker@sha256:ceb6d3f593b1d1a8991d661a78f9f46b35fd0c32f4e5ea95bd70505ab9141d6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.6 MB (97639097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60c88fe5471ef65f8032de6a0e7bf7162da118b90df5747a2b3b598b7d50a455`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 19:01:29 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 19:01:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 19:01:35 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 19:01:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 19:01:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 19:01:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 19:01:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 19:01:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:45 GMT
CMD ["sh"]
# Mon, 06 Jun 2022 19:01:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 06 Jun 2022 19:01:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 06 Jun 2022 19:01:53 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 06 Jun 2022 19:01:54 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 06 Jun 2022 19:01:54 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:54 GMT
VOLUME [/var/lib/docker]
# Mon, 06 Jun 2022 19:01:54 GMT
EXPOSE 2375 2376
# Mon, 06 Jun 2022 19:01:54 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:54 GMT
CMD []
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99ba1e24152bfcd6f75ac7d03379a0d722bb011a60e4da292b3234ed0c229c5`  
		Last Modified: Mon, 06 Jun 2022 19:03:02 GMT  
		Size: 62.0 MB (62038242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d073b016bf56120f6f99463e72dfc1669ee2cf81aea28338e191dc3392b76c2`  
		Last Modified: Mon, 06 Jun 2022 19:02:53 GMT  
		Size: 14.5 MB (14454318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae7a7070ea618fa5d597e5c3d9fafb5531a4c0ba8b5f7f12e334175f7424643`  
		Last Modified: Mon, 06 Jun 2022 19:02:52 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b69fd3006304e4afc4226a31c41076934d97c9a0c8d536bc2acda02006dab5`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff67f9f388ec6907bd17f3fa9106924c548d5374d7e483e089076822e8759f9`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77709b39dac35a99fc73e9b30dab31b8e61f7729021558d7647d544c1eaa0f23`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050708f4cb014b2395c1711989e46137eee788ff144f8a78fb7d27e8f6a54dc2`  
		Last Modified: Mon, 06 Jun 2022 19:03:18 GMT  
		Size: 6.9 MB (6862552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57437c337af006e3910175ac4b9f04054d69be2d790281e168f454cdb4d32301`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9320a07c879e2f8f96b6cb7f5ed2578bb1126537514c17728e6459ba3dbc35c`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f41b868a08905a9d2b14f2212edab168e71b841ca2db546976f5bd25bcd52e`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 2.7 KB (2745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:22.06-rc-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:7c7ec0aed8659021619bc24b0b9a7df51eb46ee8156bff5075a59a3f16c4eeda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90221146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cc869c8ebc6cae1fb3b1baabab00e9d8029967f6c7f60411689d8d53af8a7aa`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 18:36:44 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 18:36:50 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 18:36:50 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 18:36:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 18:36:55 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 18:36:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 18:37:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 18:37:02 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 18:37:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 18:37:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:05 GMT
CMD ["sh"]
# Mon, 06 Jun 2022 18:37:15 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 06 Jun 2022 18:37:16 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 06 Jun 2022 18:37:17 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 06 Jun 2022 18:37:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 06 Jun 2022 18:37:20 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:20 GMT
VOLUME [/var/lib/docker]
# Mon, 06 Jun 2022 18:37:21 GMT
EXPOSE 2375 2376
# Mon, 06 Jun 2022 18:37:22 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:23 GMT
CMD []
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f1c4eb6753c4d8ca8abdc68946eaf136ebf43c3ba68b1e3f168d561a7a40e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:21 GMT  
		Size: 57.0 MB (57027293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8543d611571340a3ade0985e604f8050b3bd7c750ce108d248072285be716e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:13 GMT  
		Size: 13.1 MB (13097906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55bb534319c1b57528e0e77d4e31677b56a064afe3ef44ab80b3dcbb546fba69`  
		Last Modified: Mon, 06 Jun 2022 18:39:12 GMT  
		Size: 8.7 MB (8663389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596ba91569b21aa39db419bf97611342f554933900d729efaea259246e43c6c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8084d414abe81d6b025915fb786b9604e6c92ca873948a0840d95927314986bc`  
		Last Modified: Mon, 06 Jun 2022 18:39:11 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62b19d6f46e3b8b83902e63f8497def66bced996fd9b45792acf2c9d5afe0c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c89092436ecc8615129e3f6851e1aeb6859cef0e5c8a99b5fe161c697d3b66a`  
		Last Modified: Mon, 06 Jun 2022 18:39:40 GMT  
		Size: 6.7 MB (6734638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b59828045492d626ecfdc53018fe98f86abbe1be9bf97a382026766e6680967`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731ca3affcf287405fe70a2a14535aea43776a755f4fa7701b780bd7773319fe`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59501b524a36d2a0f78ce443006bcfb2ce1c35a184836795fe0c527dbef3f02c`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:22.06-rc-dind-rootless`

```console
$ docker pull docker@sha256:5268e25e95d2380f29cbd313c117b47368679fb9bd823cb26405f881e0f96849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:22.06-rc-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:aa96a6309f6b63e8f5a04cfd9fd4dfca1b832a4464c213c5dcf08e51770b8e60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118791286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f868da0c728f57942c20154333eba26a5778c79a98b138498910d05d7543f0e1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 19:01:29 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 19:01:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 19:01:35 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 19:01:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 19:01:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 19:01:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 19:01:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 19:01:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:45 GMT
CMD ["sh"]
# Mon, 06 Jun 2022 19:01:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 06 Jun 2022 19:01:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 06 Jun 2022 19:01:53 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 06 Jun 2022 19:01:54 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 06 Jun 2022 19:01:54 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:54 GMT
VOLUME [/var/lib/docker]
# Mon, 06 Jun 2022 19:01:54 GMT
EXPOSE 2375 2376
# Mon, 06 Jun 2022 19:01:54 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:54 GMT
CMD []
# Mon, 06 Jun 2022 19:01:58 GMT
RUN apk add --no-cache iproute2
# Mon, 06 Jun 2022 19:01:59 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 06 Jun 2022 19:01:59 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 06 Jun 2022 19:02:02 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-rootless-extras-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 06 Jun 2022 19:02:03 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 06 Jun 2022 19:02:03 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 06 Jun 2022 19:02:03 GMT
USER rootless
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99ba1e24152bfcd6f75ac7d03379a0d722bb011a60e4da292b3234ed0c229c5`  
		Last Modified: Mon, 06 Jun 2022 19:03:02 GMT  
		Size: 62.0 MB (62038242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d073b016bf56120f6f99463e72dfc1669ee2cf81aea28338e191dc3392b76c2`  
		Last Modified: Mon, 06 Jun 2022 19:02:53 GMT  
		Size: 14.5 MB (14454318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae7a7070ea618fa5d597e5c3d9fafb5531a4c0ba8b5f7f12e334175f7424643`  
		Last Modified: Mon, 06 Jun 2022 19:02:52 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b69fd3006304e4afc4226a31c41076934d97c9a0c8d536bc2acda02006dab5`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff67f9f388ec6907bd17f3fa9106924c548d5374d7e483e089076822e8759f9`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77709b39dac35a99fc73e9b30dab31b8e61f7729021558d7647d544c1eaa0f23`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050708f4cb014b2395c1711989e46137eee788ff144f8a78fb7d27e8f6a54dc2`  
		Last Modified: Mon, 06 Jun 2022 19:03:18 GMT  
		Size: 6.9 MB (6862552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57437c337af006e3910175ac4b9f04054d69be2d790281e168f454cdb4d32301`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9320a07c879e2f8f96b6cb7f5ed2578bb1126537514c17728e6459ba3dbc35c`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f41b868a08905a9d2b14f2212edab168e71b841ca2db546976f5bd25bcd52e`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 2.7 KB (2745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc40b41e848d564c191097f81774cc897146ea1de2e76de308bb9269285f9b45`  
		Last Modified: Mon, 06 Jun 2022 19:03:34 GMT  
		Size: 1.2 MB (1232607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bfe48e653a7dc4eeb5579193ad0b4e6034a2b2586180a962e20bacab33624b`  
		Last Modified: Mon, 06 Jun 2022 19:03:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60e157845c0009309f2947508ada20712260eb7d8802f8ad3bd6025cb5da2eb`  
		Last Modified: Mon, 06 Jun 2022 19:03:34 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1838ba7dfdeda85348a3cf82992a7be7b26f4d9ff4d47609e2ca9e0cd1cf60`  
		Last Modified: Mon, 06 Jun 2022 19:03:37 GMT  
		Size: 19.9 MB (19917868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523494b3db69397e50326566071235673b0f24e5b1fcc42be82486b99fce41ca`  
		Last Modified: Mon, 06 Jun 2022 19:03:34 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:22.06-rc-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:54ee14edc9c35713cdafaced9e7fd525eb23e6b02fbf0d0f9b133b74b3a070ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.4 MB (113356240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f7b08a2a6cb290aa2d68a8d07cf52d8ed14e8e72121e6ce90fbeaf924d862ab`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 18:36:44 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 18:36:50 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 18:36:50 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 18:36:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 18:36:55 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 18:36:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 18:37:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 18:37:02 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 18:37:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 18:37:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:05 GMT
CMD ["sh"]
# Mon, 06 Jun 2022 18:37:15 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 06 Jun 2022 18:37:16 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 06 Jun 2022 18:37:17 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 06 Jun 2022 18:37:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 06 Jun 2022 18:37:20 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:20 GMT
VOLUME [/var/lib/docker]
# Mon, 06 Jun 2022 18:37:21 GMT
EXPOSE 2375 2376
# Mon, 06 Jun 2022 18:37:22 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:23 GMT
CMD []
# Mon, 06 Jun 2022 18:37:31 GMT
RUN apk add --no-cache iproute2
# Mon, 06 Jun 2022 18:37:32 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 06 Jun 2022 18:37:33 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 06 Jun 2022 18:37:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-rootless-extras-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 06 Jun 2022 18:37:37 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 06 Jun 2022 18:37:38 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 06 Jun 2022 18:37:39 GMT
USER rootless
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f1c4eb6753c4d8ca8abdc68946eaf136ebf43c3ba68b1e3f168d561a7a40e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:21 GMT  
		Size: 57.0 MB (57027293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8543d611571340a3ade0985e604f8050b3bd7c750ce108d248072285be716e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:13 GMT  
		Size: 13.1 MB (13097906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55bb534319c1b57528e0e77d4e31677b56a064afe3ef44ab80b3dcbb546fba69`  
		Last Modified: Mon, 06 Jun 2022 18:39:12 GMT  
		Size: 8.7 MB (8663389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596ba91569b21aa39db419bf97611342f554933900d729efaea259246e43c6c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8084d414abe81d6b025915fb786b9604e6c92ca873948a0840d95927314986bc`  
		Last Modified: Mon, 06 Jun 2022 18:39:11 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62b19d6f46e3b8b83902e63f8497def66bced996fd9b45792acf2c9d5afe0c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c89092436ecc8615129e3f6851e1aeb6859cef0e5c8a99b5fe161c697d3b66a`  
		Last Modified: Mon, 06 Jun 2022 18:39:40 GMT  
		Size: 6.7 MB (6734638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b59828045492d626ecfdc53018fe98f86abbe1be9bf97a382026766e6680967`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731ca3affcf287405fe70a2a14535aea43776a755f4fa7701b780bd7773319fe`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59501b524a36d2a0f78ce443006bcfb2ce1c35a184836795fe0c527dbef3f02c`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1349775e36852c48e984ab260b7262a05f902263a5488a8c3310a9e7ce84d612`  
		Last Modified: Mon, 06 Jun 2022 18:39:58 GMT  
		Size: 1.2 MB (1246071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ef4534bef24c4f8122f7275ee5a49000cbbeafeac66ecaa0c9e0d35c413eb5`  
		Last Modified: Mon, 06 Jun 2022 18:39:57 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4d33e0ed79838456d16cfbfcd8378818231b3cd82ee5630d58ac5e48a671fc`  
		Last Modified: Mon, 06 Jun 2022 18:39:58 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3433ce83674bad06b4dac071ea1995bdd1eb1014e83c23135e06971a450618dc`  
		Last Modified: Mon, 06 Jun 2022 18:40:01 GMT  
		Size: 21.9 MB (21887400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf27541a67b4884567ee908beefa5866a7295afe5d3eaa5ce8a04070fab57b6e`  
		Last Modified: Mon, 06 Jun 2022 18:39:58 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:22.06-rc-git`

```console
$ docker pull docker@sha256:79316cbde1069c03adef776435eb3624c5ae9866dd1df6a399b020146bec8a82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:22.06-rc-git` - linux; amd64

```console
$ docker pull docker@sha256:50d2107405e49b19cf4d72e886153f0679eb3abf48e2d3b3de4669d56d49f9eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.7 MB (97705984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcf6afb24ceadac365d6f10e98b0588eec5290ea19c9d8e76923ac45d134e3b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 19:01:29 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 19:01:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 19:01:35 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 19:01:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 19:01:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 19:01:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 19:01:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 19:01:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:45 GMT
CMD ["sh"]
# Mon, 06 Jun 2022 19:02:08 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99ba1e24152bfcd6f75ac7d03379a0d722bb011a60e4da292b3234ed0c229c5`  
		Last Modified: Mon, 06 Jun 2022 19:03:02 GMT  
		Size: 62.0 MB (62038242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d073b016bf56120f6f99463e72dfc1669ee2cf81aea28338e191dc3392b76c2`  
		Last Modified: Mon, 06 Jun 2022 19:02:53 GMT  
		Size: 14.5 MB (14454318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae7a7070ea618fa5d597e5c3d9fafb5531a4c0ba8b5f7f12e334175f7424643`  
		Last Modified: Mon, 06 Jun 2022 19:02:52 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b69fd3006304e4afc4226a31c41076934d97c9a0c8d536bc2acda02006dab5`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff67f9f388ec6907bd17f3fa9106924c548d5374d7e483e089076822e8759f9`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77709b39dac35a99fc73e9b30dab31b8e61f7729021558d7647d544c1eaa0f23`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4029b623e7cf6a5b9070d256c16adf13d0c929453290286bba377419aae00e`  
		Last Modified: Mon, 06 Jun 2022 19:04:05 GMT  
		Size: 6.9 MB (6934461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:22.06-rc-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f06691ad72c9fd7d3baaae7926667a6ea2e421dbcc613687d533ecdbdd0facae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.5 MB (90526228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb3d44d014348c6a18353b4dc9d6ef164e61a59e2dc8dc968e8ec25928b3a259`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 18:36:44 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 18:36:50 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 18:36:50 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 18:36:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 18:36:55 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 18:36:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 18:37:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 18:37:02 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 18:37:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 18:37:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:05 GMT
CMD ["sh"]
# Mon, 06 Jun 2022 18:37:46 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f1c4eb6753c4d8ca8abdc68946eaf136ebf43c3ba68b1e3f168d561a7a40e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:21 GMT  
		Size: 57.0 MB (57027293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8543d611571340a3ade0985e604f8050b3bd7c750ce108d248072285be716e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:13 GMT  
		Size: 13.1 MB (13097906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55bb534319c1b57528e0e77d4e31677b56a064afe3ef44ab80b3dcbb546fba69`  
		Last Modified: Mon, 06 Jun 2022 18:39:12 GMT  
		Size: 8.7 MB (8663389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596ba91569b21aa39db419bf97611342f554933900d729efaea259246e43c6c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8084d414abe81d6b025915fb786b9604e6c92ca873948a0840d95927314986bc`  
		Last Modified: Mon, 06 Jun 2022 18:39:11 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62b19d6f46e3b8b83902e63f8497def66bced996fd9b45792acf2c9d5afe0c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6266696465611c20778351065a15881b4a1edf1c9b4564e4d0779e0b7a3b6565`  
		Last Modified: Mon, 06 Jun 2022 18:40:33 GMT  
		Size: 7.0 MB (7044715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:22.06-rc-windowsservercore`

```console
$ docker pull docker@sha256:a34a08901b0c5a62d5638ae79160ad5cf955957f1ccf74b33c1863d15a9c2715
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.768; amd64
	-	windows version 10.0.17763.3046; amd64

### `docker:22.06-rc-windowsservercore` - windows version 10.0.20348.768; amd64

```console
$ docker pull docker@sha256:31b40cdc8e6e34d3869c35721212713e9d854c740003a20a1ca54262b4c6feab
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2288871549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6184a51f1d672575333cf01827c8883557519edbfbb7c8de596fd7b52760b768`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 09 Jun 2022 04:32:50 GMT
RUN Install update 10.0.20348.768
# Wed, 15 Jun 2022 12:13:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:46:14 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:46:15 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Wed, 15 Jun 2022 22:46:16 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/test/x86_64/docker-22.06.0-beta.0.zip
# Wed, 15 Jun 2022 22:46:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c71967ff41928927e4c407171e4ffbac3c9ab4221eb64f5ca5a34ff4c230567`  
		Size: 841.6 MB (841600427 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dec0338feaf01f35eb916b7fd9ecc08b719354163254885d5215e513c1a3eb2e`  
		Last Modified: Wed, 15 Jun 2022 12:49:26 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a162967ebe5da992f6dc4e9ebdd4ec9f402a84f6974c0c562cff1ed6f17dd39`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 630.9 KB (630886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7902af8cf06c7ef3cc0300bbdcd16b3d7610d4fb13025ded6e6d713b521b96`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b543c7ed7d518ed7e28b7429fa7638f623013abfb287c5e3de9ac6feadbcc964`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3eebb13fc88926962ee253a6b493aa8ac1b4eb3b24ac973a2443f8f50b5af00`  
		Last Modified: Wed, 15 Jun 2022 22:52:35 GMT  
		Size: 9.8 MB (9772337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:22.06-rc-windowsservercore` - windows version 10.0.17763.3046; amd64

```console
$ docker pull docker@sha256:493c7d58e2a74e217d0260db9fe2990755ad5d67b47d02c688277170415a1ceb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2673168277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97f8ec54ab6b0001e01fe57fce6bd7049a77d0b53f2a991dd90a46616ed565cf`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:48:09 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:48:10 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Wed, 15 Jun 2022 22:48:11 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/test/x86_64/docker-22.06.0-beta.0.zip
# Wed, 15 Jun 2022 22:49:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4c7110da70e07b37a00b3b05b18361572412287fee26eba04fcf23dcb75639`  
		Last Modified: Wed, 15 Jun 2022 22:52:48 GMT  
		Size: 352.2 KB (352228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c60272810a69a46255c487510637a80961c5d5bca4668b996bf20aa9d73896`  
		Last Modified: Wed, 15 Jun 2022 22:52:47 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3c712e062b5fcb69c4b6081c9c1d833fa38bb3e369b44b6b9347e43e1d58a5`  
		Last Modified: Wed, 15 Jun 2022 22:52:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766d5b06428cea8b3c37d65a9fb8d92a424c2dd2d36fb91835cc37ffda944128`  
		Last Modified: Wed, 15 Jun 2022 22:52:50 GMT  
		Size: 9.5 MB (9532028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:22.06-rc-windowsservercore-1809`

```console
$ docker pull docker@sha256:7688c18170e798ada2435ab1829e86c7a1256fdf29f4245cbf88d7a8efa21dcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3046; amd64

### `docker:22.06-rc-windowsservercore-1809` - windows version 10.0.17763.3046; amd64

```console
$ docker pull docker@sha256:493c7d58e2a74e217d0260db9fe2990755ad5d67b47d02c688277170415a1ceb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2673168277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97f8ec54ab6b0001e01fe57fce6bd7049a77d0b53f2a991dd90a46616ed565cf`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:48:09 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:48:10 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Wed, 15 Jun 2022 22:48:11 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/test/x86_64/docker-22.06.0-beta.0.zip
# Wed, 15 Jun 2022 22:49:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4c7110da70e07b37a00b3b05b18361572412287fee26eba04fcf23dcb75639`  
		Last Modified: Wed, 15 Jun 2022 22:52:48 GMT  
		Size: 352.2 KB (352228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c60272810a69a46255c487510637a80961c5d5bca4668b996bf20aa9d73896`  
		Last Modified: Wed, 15 Jun 2022 22:52:47 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3c712e062b5fcb69c4b6081c9c1d833fa38bb3e369b44b6b9347e43e1d58a5`  
		Last Modified: Wed, 15 Jun 2022 22:52:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766d5b06428cea8b3c37d65a9fb8d92a424c2dd2d36fb91835cc37ffda944128`  
		Last Modified: Wed, 15 Jun 2022 22:52:50 GMT  
		Size: 9.5 MB (9532028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:22.06-rc-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:1b711c5b73ae6926b7f7a1a6538af7de3e1c103ec4ee93ef127a952b50e9a52b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.768; amd64

### `docker:22.06-rc-windowsservercore-ltsc2022` - windows version 10.0.20348.768; amd64

```console
$ docker pull docker@sha256:31b40cdc8e6e34d3869c35721212713e9d854c740003a20a1ca54262b4c6feab
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2288871549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6184a51f1d672575333cf01827c8883557519edbfbb7c8de596fd7b52760b768`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 09 Jun 2022 04:32:50 GMT
RUN Install update 10.0.20348.768
# Wed, 15 Jun 2022 12:13:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:46:14 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:46:15 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Wed, 15 Jun 2022 22:46:16 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/test/x86_64/docker-22.06.0-beta.0.zip
# Wed, 15 Jun 2022 22:46:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c71967ff41928927e4c407171e4ffbac3c9ab4221eb64f5ca5a34ff4c230567`  
		Size: 841.6 MB (841600427 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dec0338feaf01f35eb916b7fd9ecc08b719354163254885d5215e513c1a3eb2e`  
		Last Modified: Wed, 15 Jun 2022 12:49:26 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a162967ebe5da992f6dc4e9ebdd4ec9f402a84f6974c0c562cff1ed6f17dd39`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 630.9 KB (630886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7902af8cf06c7ef3cc0300bbdcd16b3d7610d4fb13025ded6e6d713b521b96`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b543c7ed7d518ed7e28b7429fa7638f623013abfb287c5e3de9ac6feadbcc964`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3eebb13fc88926962ee253a6b493aa8ac1b4eb3b24ac973a2443f8f50b5af00`  
		Last Modified: Wed, 15 Jun 2022 22:52:35 GMT  
		Size: 9.8 MB (9772337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:22.06.0-beta.0`

```console
$ docker pull docker@sha256:0964ecc3084a4908f49afef17df539e7f355c5336969ad41ec9200182b919cb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:22.06.0-beta.0` - linux; amd64

```console
$ docker pull docker@sha256:b9614a53230d0a4c4f22f2d004e04362d9f147082898cd507de08736cfe744a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.8 MB (90771523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007fe5047a7c961c196b4479f8e4263e4da34c07677f92e330cf9749228dba4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 19:01:29 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 19:01:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 19:01:35 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 19:01:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 19:01:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 19:01:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 19:01:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 19:01:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:45 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99ba1e24152bfcd6f75ac7d03379a0d722bb011a60e4da292b3234ed0c229c5`  
		Last Modified: Mon, 06 Jun 2022 19:03:02 GMT  
		Size: 62.0 MB (62038242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d073b016bf56120f6f99463e72dfc1669ee2cf81aea28338e191dc3392b76c2`  
		Last Modified: Mon, 06 Jun 2022 19:02:53 GMT  
		Size: 14.5 MB (14454318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae7a7070ea618fa5d597e5c3d9fafb5531a4c0ba8b5f7f12e334175f7424643`  
		Last Modified: Mon, 06 Jun 2022 19:02:52 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b69fd3006304e4afc4226a31c41076934d97c9a0c8d536bc2acda02006dab5`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff67f9f388ec6907bd17f3fa9106924c548d5374d7e483e089076822e8759f9`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77709b39dac35a99fc73e9b30dab31b8e61f7729021558d7647d544c1eaa0f23`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:22.06.0-beta.0` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f1168269caf92da50e2c6c8781facff325d5a643079ef6534abf1b293d9cbfa7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.5 MB (83481513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3af4b446c8d50a9581547b8dc9a07922f7666fe639a1ffda87e9842bacadbf5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 18:36:44 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 18:36:50 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 18:36:50 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 18:36:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 18:36:55 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 18:36:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 18:37:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 18:37:02 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 18:37:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 18:37:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:05 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f1c4eb6753c4d8ca8abdc68946eaf136ebf43c3ba68b1e3f168d561a7a40e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:21 GMT  
		Size: 57.0 MB (57027293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8543d611571340a3ade0985e604f8050b3bd7c750ce108d248072285be716e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:13 GMT  
		Size: 13.1 MB (13097906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55bb534319c1b57528e0e77d4e31677b56a064afe3ef44ab80b3dcbb546fba69`  
		Last Modified: Mon, 06 Jun 2022 18:39:12 GMT  
		Size: 8.7 MB (8663389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596ba91569b21aa39db419bf97611342f554933900d729efaea259246e43c6c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8084d414abe81d6b025915fb786b9604e6c92ca873948a0840d95927314986bc`  
		Last Modified: Mon, 06 Jun 2022 18:39:11 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62b19d6f46e3b8b83902e63f8497def66bced996fd9b45792acf2c9d5afe0c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:22.06.0-beta.0-alpine3.16`

```console
$ docker pull docker@sha256:0964ecc3084a4908f49afef17df539e7f355c5336969ad41ec9200182b919cb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:22.06.0-beta.0-alpine3.16` - linux; amd64

```console
$ docker pull docker@sha256:b9614a53230d0a4c4f22f2d004e04362d9f147082898cd507de08736cfe744a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.8 MB (90771523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007fe5047a7c961c196b4479f8e4263e4da34c07677f92e330cf9749228dba4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 19:01:29 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 19:01:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 19:01:35 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 19:01:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 19:01:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 19:01:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 19:01:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 19:01:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:45 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99ba1e24152bfcd6f75ac7d03379a0d722bb011a60e4da292b3234ed0c229c5`  
		Last Modified: Mon, 06 Jun 2022 19:03:02 GMT  
		Size: 62.0 MB (62038242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d073b016bf56120f6f99463e72dfc1669ee2cf81aea28338e191dc3392b76c2`  
		Last Modified: Mon, 06 Jun 2022 19:02:53 GMT  
		Size: 14.5 MB (14454318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae7a7070ea618fa5d597e5c3d9fafb5531a4c0ba8b5f7f12e334175f7424643`  
		Last Modified: Mon, 06 Jun 2022 19:02:52 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b69fd3006304e4afc4226a31c41076934d97c9a0c8d536bc2acda02006dab5`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff67f9f388ec6907bd17f3fa9106924c548d5374d7e483e089076822e8759f9`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77709b39dac35a99fc73e9b30dab31b8e61f7729021558d7647d544c1eaa0f23`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:22.06.0-beta.0-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f1168269caf92da50e2c6c8781facff325d5a643079ef6534abf1b293d9cbfa7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.5 MB (83481513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3af4b446c8d50a9581547b8dc9a07922f7666fe639a1ffda87e9842bacadbf5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 18:36:44 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 18:36:50 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 18:36:50 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 18:36:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 18:36:55 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 18:36:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 18:37:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 18:37:02 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 18:37:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 18:37:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:05 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f1c4eb6753c4d8ca8abdc68946eaf136ebf43c3ba68b1e3f168d561a7a40e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:21 GMT  
		Size: 57.0 MB (57027293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8543d611571340a3ade0985e604f8050b3bd7c750ce108d248072285be716e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:13 GMT  
		Size: 13.1 MB (13097906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55bb534319c1b57528e0e77d4e31677b56a064afe3ef44ab80b3dcbb546fba69`  
		Last Modified: Mon, 06 Jun 2022 18:39:12 GMT  
		Size: 8.7 MB (8663389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596ba91569b21aa39db419bf97611342f554933900d729efaea259246e43c6c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8084d414abe81d6b025915fb786b9604e6c92ca873948a0840d95927314986bc`  
		Last Modified: Mon, 06 Jun 2022 18:39:11 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62b19d6f46e3b8b83902e63f8497def66bced996fd9b45792acf2c9d5afe0c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:22.06.0-beta.0-dind`

```console
$ docker pull docker@sha256:aac3ee54242eb33fddb238884878e0d5c059b2b227f6914086ddb183064f7314
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:22.06.0-beta.0-dind` - linux; amd64

```console
$ docker pull docker@sha256:ceb6d3f593b1d1a8991d661a78f9f46b35fd0c32f4e5ea95bd70505ab9141d6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.6 MB (97639097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60c88fe5471ef65f8032de6a0e7bf7162da118b90df5747a2b3b598b7d50a455`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 19:01:29 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 19:01:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 19:01:35 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 19:01:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 19:01:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 19:01:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 19:01:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 19:01:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:45 GMT
CMD ["sh"]
# Mon, 06 Jun 2022 19:01:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 06 Jun 2022 19:01:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 06 Jun 2022 19:01:53 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 06 Jun 2022 19:01:54 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 06 Jun 2022 19:01:54 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:54 GMT
VOLUME [/var/lib/docker]
# Mon, 06 Jun 2022 19:01:54 GMT
EXPOSE 2375 2376
# Mon, 06 Jun 2022 19:01:54 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:54 GMT
CMD []
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99ba1e24152bfcd6f75ac7d03379a0d722bb011a60e4da292b3234ed0c229c5`  
		Last Modified: Mon, 06 Jun 2022 19:03:02 GMT  
		Size: 62.0 MB (62038242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d073b016bf56120f6f99463e72dfc1669ee2cf81aea28338e191dc3392b76c2`  
		Last Modified: Mon, 06 Jun 2022 19:02:53 GMT  
		Size: 14.5 MB (14454318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae7a7070ea618fa5d597e5c3d9fafb5531a4c0ba8b5f7f12e334175f7424643`  
		Last Modified: Mon, 06 Jun 2022 19:02:52 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b69fd3006304e4afc4226a31c41076934d97c9a0c8d536bc2acda02006dab5`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff67f9f388ec6907bd17f3fa9106924c548d5374d7e483e089076822e8759f9`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77709b39dac35a99fc73e9b30dab31b8e61f7729021558d7647d544c1eaa0f23`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050708f4cb014b2395c1711989e46137eee788ff144f8a78fb7d27e8f6a54dc2`  
		Last Modified: Mon, 06 Jun 2022 19:03:18 GMT  
		Size: 6.9 MB (6862552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57437c337af006e3910175ac4b9f04054d69be2d790281e168f454cdb4d32301`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9320a07c879e2f8f96b6cb7f5ed2578bb1126537514c17728e6459ba3dbc35c`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f41b868a08905a9d2b14f2212edab168e71b841ca2db546976f5bd25bcd52e`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 2.7 KB (2745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:22.06.0-beta.0-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:7c7ec0aed8659021619bc24b0b9a7df51eb46ee8156bff5075a59a3f16c4eeda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90221146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cc869c8ebc6cae1fb3b1baabab00e9d8029967f6c7f60411689d8d53af8a7aa`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 18:36:44 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 18:36:50 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 18:36:50 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 18:36:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 18:36:55 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 18:36:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 18:37:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 18:37:02 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 18:37:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 18:37:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:05 GMT
CMD ["sh"]
# Mon, 06 Jun 2022 18:37:15 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 06 Jun 2022 18:37:16 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 06 Jun 2022 18:37:17 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 06 Jun 2022 18:37:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 06 Jun 2022 18:37:20 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:20 GMT
VOLUME [/var/lib/docker]
# Mon, 06 Jun 2022 18:37:21 GMT
EXPOSE 2375 2376
# Mon, 06 Jun 2022 18:37:22 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:23 GMT
CMD []
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f1c4eb6753c4d8ca8abdc68946eaf136ebf43c3ba68b1e3f168d561a7a40e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:21 GMT  
		Size: 57.0 MB (57027293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8543d611571340a3ade0985e604f8050b3bd7c750ce108d248072285be716e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:13 GMT  
		Size: 13.1 MB (13097906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55bb534319c1b57528e0e77d4e31677b56a064afe3ef44ab80b3dcbb546fba69`  
		Last Modified: Mon, 06 Jun 2022 18:39:12 GMT  
		Size: 8.7 MB (8663389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596ba91569b21aa39db419bf97611342f554933900d729efaea259246e43c6c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8084d414abe81d6b025915fb786b9604e6c92ca873948a0840d95927314986bc`  
		Last Modified: Mon, 06 Jun 2022 18:39:11 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62b19d6f46e3b8b83902e63f8497def66bced996fd9b45792acf2c9d5afe0c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c89092436ecc8615129e3f6851e1aeb6859cef0e5c8a99b5fe161c697d3b66a`  
		Last Modified: Mon, 06 Jun 2022 18:39:40 GMT  
		Size: 6.7 MB (6734638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b59828045492d626ecfdc53018fe98f86abbe1be9bf97a382026766e6680967`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731ca3affcf287405fe70a2a14535aea43776a755f4fa7701b780bd7773319fe`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59501b524a36d2a0f78ce443006bcfb2ce1c35a184836795fe0c527dbef3f02c`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:22.06.0-beta.0-dind-alpine3.16`

```console
$ docker pull docker@sha256:aac3ee54242eb33fddb238884878e0d5c059b2b227f6914086ddb183064f7314
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:22.06.0-beta.0-dind-alpine3.16` - linux; amd64

```console
$ docker pull docker@sha256:ceb6d3f593b1d1a8991d661a78f9f46b35fd0c32f4e5ea95bd70505ab9141d6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.6 MB (97639097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60c88fe5471ef65f8032de6a0e7bf7162da118b90df5747a2b3b598b7d50a455`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 19:01:29 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 19:01:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 19:01:35 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 19:01:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 19:01:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 19:01:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 19:01:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 19:01:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:45 GMT
CMD ["sh"]
# Mon, 06 Jun 2022 19:01:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 06 Jun 2022 19:01:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 06 Jun 2022 19:01:53 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 06 Jun 2022 19:01:54 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 06 Jun 2022 19:01:54 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:54 GMT
VOLUME [/var/lib/docker]
# Mon, 06 Jun 2022 19:01:54 GMT
EXPOSE 2375 2376
# Mon, 06 Jun 2022 19:01:54 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:54 GMT
CMD []
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99ba1e24152bfcd6f75ac7d03379a0d722bb011a60e4da292b3234ed0c229c5`  
		Last Modified: Mon, 06 Jun 2022 19:03:02 GMT  
		Size: 62.0 MB (62038242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d073b016bf56120f6f99463e72dfc1669ee2cf81aea28338e191dc3392b76c2`  
		Last Modified: Mon, 06 Jun 2022 19:02:53 GMT  
		Size: 14.5 MB (14454318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae7a7070ea618fa5d597e5c3d9fafb5531a4c0ba8b5f7f12e334175f7424643`  
		Last Modified: Mon, 06 Jun 2022 19:02:52 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b69fd3006304e4afc4226a31c41076934d97c9a0c8d536bc2acda02006dab5`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff67f9f388ec6907bd17f3fa9106924c548d5374d7e483e089076822e8759f9`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77709b39dac35a99fc73e9b30dab31b8e61f7729021558d7647d544c1eaa0f23`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050708f4cb014b2395c1711989e46137eee788ff144f8a78fb7d27e8f6a54dc2`  
		Last Modified: Mon, 06 Jun 2022 19:03:18 GMT  
		Size: 6.9 MB (6862552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57437c337af006e3910175ac4b9f04054d69be2d790281e168f454cdb4d32301`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9320a07c879e2f8f96b6cb7f5ed2578bb1126537514c17728e6459ba3dbc35c`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f41b868a08905a9d2b14f2212edab168e71b841ca2db546976f5bd25bcd52e`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 2.7 KB (2745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:22.06.0-beta.0-dind-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:7c7ec0aed8659021619bc24b0b9a7df51eb46ee8156bff5075a59a3f16c4eeda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90221146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cc869c8ebc6cae1fb3b1baabab00e9d8029967f6c7f60411689d8d53af8a7aa`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 18:36:44 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 18:36:50 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 18:36:50 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 18:36:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 18:36:55 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 18:36:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 18:37:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 18:37:02 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 18:37:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 18:37:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:05 GMT
CMD ["sh"]
# Mon, 06 Jun 2022 18:37:15 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 06 Jun 2022 18:37:16 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 06 Jun 2022 18:37:17 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 06 Jun 2022 18:37:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 06 Jun 2022 18:37:20 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:20 GMT
VOLUME [/var/lib/docker]
# Mon, 06 Jun 2022 18:37:21 GMT
EXPOSE 2375 2376
# Mon, 06 Jun 2022 18:37:22 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:23 GMT
CMD []
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f1c4eb6753c4d8ca8abdc68946eaf136ebf43c3ba68b1e3f168d561a7a40e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:21 GMT  
		Size: 57.0 MB (57027293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8543d611571340a3ade0985e604f8050b3bd7c750ce108d248072285be716e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:13 GMT  
		Size: 13.1 MB (13097906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55bb534319c1b57528e0e77d4e31677b56a064afe3ef44ab80b3dcbb546fba69`  
		Last Modified: Mon, 06 Jun 2022 18:39:12 GMT  
		Size: 8.7 MB (8663389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596ba91569b21aa39db419bf97611342f554933900d729efaea259246e43c6c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8084d414abe81d6b025915fb786b9604e6c92ca873948a0840d95927314986bc`  
		Last Modified: Mon, 06 Jun 2022 18:39:11 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62b19d6f46e3b8b83902e63f8497def66bced996fd9b45792acf2c9d5afe0c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c89092436ecc8615129e3f6851e1aeb6859cef0e5c8a99b5fe161c697d3b66a`  
		Last Modified: Mon, 06 Jun 2022 18:39:40 GMT  
		Size: 6.7 MB (6734638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b59828045492d626ecfdc53018fe98f86abbe1be9bf97a382026766e6680967`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731ca3affcf287405fe70a2a14535aea43776a755f4fa7701b780bd7773319fe`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59501b524a36d2a0f78ce443006bcfb2ce1c35a184836795fe0c527dbef3f02c`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:22.06.0-beta.0-dind-rootless`

```console
$ docker pull docker@sha256:5268e25e95d2380f29cbd313c117b47368679fb9bd823cb26405f881e0f96849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:22.06.0-beta.0-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:aa96a6309f6b63e8f5a04cfd9fd4dfca1b832a4464c213c5dcf08e51770b8e60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118791286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f868da0c728f57942c20154333eba26a5778c79a98b138498910d05d7543f0e1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 19:01:29 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 19:01:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 19:01:35 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 19:01:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 19:01:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 19:01:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 19:01:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 19:01:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:45 GMT
CMD ["sh"]
# Mon, 06 Jun 2022 19:01:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 06 Jun 2022 19:01:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 06 Jun 2022 19:01:53 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 06 Jun 2022 19:01:54 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 06 Jun 2022 19:01:54 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:54 GMT
VOLUME [/var/lib/docker]
# Mon, 06 Jun 2022 19:01:54 GMT
EXPOSE 2375 2376
# Mon, 06 Jun 2022 19:01:54 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:54 GMT
CMD []
# Mon, 06 Jun 2022 19:01:58 GMT
RUN apk add --no-cache iproute2
# Mon, 06 Jun 2022 19:01:59 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 06 Jun 2022 19:01:59 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 06 Jun 2022 19:02:02 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-rootless-extras-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 06 Jun 2022 19:02:03 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 06 Jun 2022 19:02:03 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 06 Jun 2022 19:02:03 GMT
USER rootless
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99ba1e24152bfcd6f75ac7d03379a0d722bb011a60e4da292b3234ed0c229c5`  
		Last Modified: Mon, 06 Jun 2022 19:03:02 GMT  
		Size: 62.0 MB (62038242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d073b016bf56120f6f99463e72dfc1669ee2cf81aea28338e191dc3392b76c2`  
		Last Modified: Mon, 06 Jun 2022 19:02:53 GMT  
		Size: 14.5 MB (14454318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae7a7070ea618fa5d597e5c3d9fafb5531a4c0ba8b5f7f12e334175f7424643`  
		Last Modified: Mon, 06 Jun 2022 19:02:52 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b69fd3006304e4afc4226a31c41076934d97c9a0c8d536bc2acda02006dab5`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff67f9f388ec6907bd17f3fa9106924c548d5374d7e483e089076822e8759f9`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77709b39dac35a99fc73e9b30dab31b8e61f7729021558d7647d544c1eaa0f23`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050708f4cb014b2395c1711989e46137eee788ff144f8a78fb7d27e8f6a54dc2`  
		Last Modified: Mon, 06 Jun 2022 19:03:18 GMT  
		Size: 6.9 MB (6862552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57437c337af006e3910175ac4b9f04054d69be2d790281e168f454cdb4d32301`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9320a07c879e2f8f96b6cb7f5ed2578bb1126537514c17728e6459ba3dbc35c`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f41b868a08905a9d2b14f2212edab168e71b841ca2db546976f5bd25bcd52e`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 2.7 KB (2745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc40b41e848d564c191097f81774cc897146ea1de2e76de308bb9269285f9b45`  
		Last Modified: Mon, 06 Jun 2022 19:03:34 GMT  
		Size: 1.2 MB (1232607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bfe48e653a7dc4eeb5579193ad0b4e6034a2b2586180a962e20bacab33624b`  
		Last Modified: Mon, 06 Jun 2022 19:03:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60e157845c0009309f2947508ada20712260eb7d8802f8ad3bd6025cb5da2eb`  
		Last Modified: Mon, 06 Jun 2022 19:03:34 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1838ba7dfdeda85348a3cf82992a7be7b26f4d9ff4d47609e2ca9e0cd1cf60`  
		Last Modified: Mon, 06 Jun 2022 19:03:37 GMT  
		Size: 19.9 MB (19917868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523494b3db69397e50326566071235673b0f24e5b1fcc42be82486b99fce41ca`  
		Last Modified: Mon, 06 Jun 2022 19:03:34 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:22.06.0-beta.0-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:54ee14edc9c35713cdafaced9e7fd525eb23e6b02fbf0d0f9b133b74b3a070ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.4 MB (113356240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f7b08a2a6cb290aa2d68a8d07cf52d8ed14e8e72121e6ce90fbeaf924d862ab`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 18:36:44 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 18:36:50 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 18:36:50 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 18:36:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 18:36:55 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 18:36:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 18:37:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 18:37:02 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 18:37:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 18:37:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:05 GMT
CMD ["sh"]
# Mon, 06 Jun 2022 18:37:15 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 06 Jun 2022 18:37:16 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 06 Jun 2022 18:37:17 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 06 Jun 2022 18:37:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 06 Jun 2022 18:37:20 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:20 GMT
VOLUME [/var/lib/docker]
# Mon, 06 Jun 2022 18:37:21 GMT
EXPOSE 2375 2376
# Mon, 06 Jun 2022 18:37:22 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:23 GMT
CMD []
# Mon, 06 Jun 2022 18:37:31 GMT
RUN apk add --no-cache iproute2
# Mon, 06 Jun 2022 18:37:32 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 06 Jun 2022 18:37:33 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 06 Jun 2022 18:37:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-rootless-extras-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 06 Jun 2022 18:37:37 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 06 Jun 2022 18:37:38 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 06 Jun 2022 18:37:39 GMT
USER rootless
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f1c4eb6753c4d8ca8abdc68946eaf136ebf43c3ba68b1e3f168d561a7a40e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:21 GMT  
		Size: 57.0 MB (57027293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8543d611571340a3ade0985e604f8050b3bd7c750ce108d248072285be716e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:13 GMT  
		Size: 13.1 MB (13097906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55bb534319c1b57528e0e77d4e31677b56a064afe3ef44ab80b3dcbb546fba69`  
		Last Modified: Mon, 06 Jun 2022 18:39:12 GMT  
		Size: 8.7 MB (8663389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596ba91569b21aa39db419bf97611342f554933900d729efaea259246e43c6c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8084d414abe81d6b025915fb786b9604e6c92ca873948a0840d95927314986bc`  
		Last Modified: Mon, 06 Jun 2022 18:39:11 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62b19d6f46e3b8b83902e63f8497def66bced996fd9b45792acf2c9d5afe0c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c89092436ecc8615129e3f6851e1aeb6859cef0e5c8a99b5fe161c697d3b66a`  
		Last Modified: Mon, 06 Jun 2022 18:39:40 GMT  
		Size: 6.7 MB (6734638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b59828045492d626ecfdc53018fe98f86abbe1be9bf97a382026766e6680967`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731ca3affcf287405fe70a2a14535aea43776a755f4fa7701b780bd7773319fe`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59501b524a36d2a0f78ce443006bcfb2ce1c35a184836795fe0c527dbef3f02c`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1349775e36852c48e984ab260b7262a05f902263a5488a8c3310a9e7ce84d612`  
		Last Modified: Mon, 06 Jun 2022 18:39:58 GMT  
		Size: 1.2 MB (1246071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ef4534bef24c4f8122f7275ee5a49000cbbeafeac66ecaa0c9e0d35c413eb5`  
		Last Modified: Mon, 06 Jun 2022 18:39:57 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4d33e0ed79838456d16cfbfcd8378818231b3cd82ee5630d58ac5e48a671fc`  
		Last Modified: Mon, 06 Jun 2022 18:39:58 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3433ce83674bad06b4dac071ea1995bdd1eb1014e83c23135e06971a450618dc`  
		Last Modified: Mon, 06 Jun 2022 18:40:01 GMT  
		Size: 21.9 MB (21887400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf27541a67b4884567ee908beefa5866a7295afe5d3eaa5ce8a04070fab57b6e`  
		Last Modified: Mon, 06 Jun 2022 18:39:58 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:22.06.0-beta.0-git`

```console
$ docker pull docker@sha256:79316cbde1069c03adef776435eb3624c5ae9866dd1df6a399b020146bec8a82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:22.06.0-beta.0-git` - linux; amd64

```console
$ docker pull docker@sha256:50d2107405e49b19cf4d72e886153f0679eb3abf48e2d3b3de4669d56d49f9eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.7 MB (97705984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcf6afb24ceadac365d6f10e98b0588eec5290ea19c9d8e76923ac45d134e3b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 19:01:29 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 19:01:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 19:01:35 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 19:01:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 19:01:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 19:01:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 19:01:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 19:01:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:45 GMT
CMD ["sh"]
# Mon, 06 Jun 2022 19:02:08 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99ba1e24152bfcd6f75ac7d03379a0d722bb011a60e4da292b3234ed0c229c5`  
		Last Modified: Mon, 06 Jun 2022 19:03:02 GMT  
		Size: 62.0 MB (62038242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d073b016bf56120f6f99463e72dfc1669ee2cf81aea28338e191dc3392b76c2`  
		Last Modified: Mon, 06 Jun 2022 19:02:53 GMT  
		Size: 14.5 MB (14454318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae7a7070ea618fa5d597e5c3d9fafb5531a4c0ba8b5f7f12e334175f7424643`  
		Last Modified: Mon, 06 Jun 2022 19:02:52 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b69fd3006304e4afc4226a31c41076934d97c9a0c8d536bc2acda02006dab5`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff67f9f388ec6907bd17f3fa9106924c548d5374d7e483e089076822e8759f9`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77709b39dac35a99fc73e9b30dab31b8e61f7729021558d7647d544c1eaa0f23`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4029b623e7cf6a5b9070d256c16adf13d0c929453290286bba377419aae00e`  
		Last Modified: Mon, 06 Jun 2022 19:04:05 GMT  
		Size: 6.9 MB (6934461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:22.06.0-beta.0-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f06691ad72c9fd7d3baaae7926667a6ea2e421dbcc613687d533ecdbdd0facae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.5 MB (90526228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb3d44d014348c6a18353b4dc9d6ef164e61a59e2dc8dc968e8ec25928b3a259`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 18:36:44 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 18:36:50 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 18:36:50 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 18:36:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 18:36:55 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 18:36:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 18:37:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 18:37:02 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 18:37:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 18:37:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:05 GMT
CMD ["sh"]
# Mon, 06 Jun 2022 18:37:46 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f1c4eb6753c4d8ca8abdc68946eaf136ebf43c3ba68b1e3f168d561a7a40e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:21 GMT  
		Size: 57.0 MB (57027293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8543d611571340a3ade0985e604f8050b3bd7c750ce108d248072285be716e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:13 GMT  
		Size: 13.1 MB (13097906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55bb534319c1b57528e0e77d4e31677b56a064afe3ef44ab80b3dcbb546fba69`  
		Last Modified: Mon, 06 Jun 2022 18:39:12 GMT  
		Size: 8.7 MB (8663389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596ba91569b21aa39db419bf97611342f554933900d729efaea259246e43c6c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8084d414abe81d6b025915fb786b9604e6c92ca873948a0840d95927314986bc`  
		Last Modified: Mon, 06 Jun 2022 18:39:11 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62b19d6f46e3b8b83902e63f8497def66bced996fd9b45792acf2c9d5afe0c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6266696465611c20778351065a15881b4a1edf1c9b4564e4d0779e0b7a3b6565`  
		Last Modified: Mon, 06 Jun 2022 18:40:33 GMT  
		Size: 7.0 MB (7044715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:22.06.0-beta.0-windowsservercore`

```console
$ docker pull docker@sha256:a34a08901b0c5a62d5638ae79160ad5cf955957f1ccf74b33c1863d15a9c2715
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.768; amd64
	-	windows version 10.0.17763.3046; amd64

### `docker:22.06.0-beta.0-windowsservercore` - windows version 10.0.20348.768; amd64

```console
$ docker pull docker@sha256:31b40cdc8e6e34d3869c35721212713e9d854c740003a20a1ca54262b4c6feab
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2288871549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6184a51f1d672575333cf01827c8883557519edbfbb7c8de596fd7b52760b768`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 09 Jun 2022 04:32:50 GMT
RUN Install update 10.0.20348.768
# Wed, 15 Jun 2022 12:13:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:46:14 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:46:15 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Wed, 15 Jun 2022 22:46:16 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/test/x86_64/docker-22.06.0-beta.0.zip
# Wed, 15 Jun 2022 22:46:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c71967ff41928927e4c407171e4ffbac3c9ab4221eb64f5ca5a34ff4c230567`  
		Size: 841.6 MB (841600427 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dec0338feaf01f35eb916b7fd9ecc08b719354163254885d5215e513c1a3eb2e`  
		Last Modified: Wed, 15 Jun 2022 12:49:26 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a162967ebe5da992f6dc4e9ebdd4ec9f402a84f6974c0c562cff1ed6f17dd39`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 630.9 KB (630886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7902af8cf06c7ef3cc0300bbdcd16b3d7610d4fb13025ded6e6d713b521b96`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b543c7ed7d518ed7e28b7429fa7638f623013abfb287c5e3de9ac6feadbcc964`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3eebb13fc88926962ee253a6b493aa8ac1b4eb3b24ac973a2443f8f50b5af00`  
		Last Modified: Wed, 15 Jun 2022 22:52:35 GMT  
		Size: 9.8 MB (9772337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:22.06.0-beta.0-windowsservercore` - windows version 10.0.17763.3046; amd64

```console
$ docker pull docker@sha256:493c7d58e2a74e217d0260db9fe2990755ad5d67b47d02c688277170415a1ceb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2673168277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97f8ec54ab6b0001e01fe57fce6bd7049a77d0b53f2a991dd90a46616ed565cf`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:48:09 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:48:10 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Wed, 15 Jun 2022 22:48:11 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/test/x86_64/docker-22.06.0-beta.0.zip
# Wed, 15 Jun 2022 22:49:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4c7110da70e07b37a00b3b05b18361572412287fee26eba04fcf23dcb75639`  
		Last Modified: Wed, 15 Jun 2022 22:52:48 GMT  
		Size: 352.2 KB (352228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c60272810a69a46255c487510637a80961c5d5bca4668b996bf20aa9d73896`  
		Last Modified: Wed, 15 Jun 2022 22:52:47 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3c712e062b5fcb69c4b6081c9c1d833fa38bb3e369b44b6b9347e43e1d58a5`  
		Last Modified: Wed, 15 Jun 2022 22:52:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766d5b06428cea8b3c37d65a9fb8d92a424c2dd2d36fb91835cc37ffda944128`  
		Last Modified: Wed, 15 Jun 2022 22:52:50 GMT  
		Size: 9.5 MB (9532028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:22.06.0-beta.0-windowsservercore-1809`

```console
$ docker pull docker@sha256:7688c18170e798ada2435ab1829e86c7a1256fdf29f4245cbf88d7a8efa21dcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3046; amd64

### `docker:22.06.0-beta.0-windowsservercore-1809` - windows version 10.0.17763.3046; amd64

```console
$ docker pull docker@sha256:493c7d58e2a74e217d0260db9fe2990755ad5d67b47d02c688277170415a1ceb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2673168277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97f8ec54ab6b0001e01fe57fce6bd7049a77d0b53f2a991dd90a46616ed565cf`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:48:09 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:48:10 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Wed, 15 Jun 2022 22:48:11 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/test/x86_64/docker-22.06.0-beta.0.zip
# Wed, 15 Jun 2022 22:49:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4c7110da70e07b37a00b3b05b18361572412287fee26eba04fcf23dcb75639`  
		Last Modified: Wed, 15 Jun 2022 22:52:48 GMT  
		Size: 352.2 KB (352228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c60272810a69a46255c487510637a80961c5d5bca4668b996bf20aa9d73896`  
		Last Modified: Wed, 15 Jun 2022 22:52:47 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3c712e062b5fcb69c4b6081c9c1d833fa38bb3e369b44b6b9347e43e1d58a5`  
		Last Modified: Wed, 15 Jun 2022 22:52:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766d5b06428cea8b3c37d65a9fb8d92a424c2dd2d36fb91835cc37ffda944128`  
		Last Modified: Wed, 15 Jun 2022 22:52:50 GMT  
		Size: 9.5 MB (9532028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:22.06.0-beta.0-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:1b711c5b73ae6926b7f7a1a6538af7de3e1c103ec4ee93ef127a952b50e9a52b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.768; amd64

### `docker:22.06.0-beta.0-windowsservercore-ltsc2022` - windows version 10.0.20348.768; amd64

```console
$ docker pull docker@sha256:31b40cdc8e6e34d3869c35721212713e9d854c740003a20a1ca54262b4c6feab
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2288871549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6184a51f1d672575333cf01827c8883557519edbfbb7c8de596fd7b52760b768`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 09 Jun 2022 04:32:50 GMT
RUN Install update 10.0.20348.768
# Wed, 15 Jun 2022 12:13:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:46:14 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:46:15 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Wed, 15 Jun 2022 22:46:16 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/test/x86_64/docker-22.06.0-beta.0.zip
# Wed, 15 Jun 2022 22:46:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c71967ff41928927e4c407171e4ffbac3c9ab4221eb64f5ca5a34ff4c230567`  
		Size: 841.6 MB (841600427 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dec0338feaf01f35eb916b7fd9ecc08b719354163254885d5215e513c1a3eb2e`  
		Last Modified: Wed, 15 Jun 2022 12:49:26 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a162967ebe5da992f6dc4e9ebdd4ec9f402a84f6974c0c562cff1ed6f17dd39`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 630.9 KB (630886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7902af8cf06c7ef3cc0300bbdcd16b3d7610d4fb13025ded6e6d713b521b96`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b543c7ed7d518ed7e28b7429fa7638f623013abfb287c5e3de9ac6feadbcc964`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3eebb13fc88926962ee253a6b493aa8ac1b4eb3b24ac973a2443f8f50b5af00`  
		Last Modified: Wed, 15 Jun 2022 22:52:35 GMT  
		Size: 9.8 MB (9772337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:a7a9383d0631b5f6b59f0a8138912d20b63c9320127e3fb065cb9ca0257a58b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:8cdb600dd59001892484f7c4be06166e42a2952065b6822b98c5aa7b8ef2ce8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.1 MB (101111945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dbe252bd9afb23859f250989da416b2cd8ab30f4b61a2bc8fca6f9b05d7e665`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:23:40 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:23:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:23:46 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:23:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:23:48 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:23:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:23:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:23:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:23:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:23:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:23:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:24:02 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 07 Jun 2022 18:24:03 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:24:03 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 07 Jun 2022 18:24:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 07 Jun 2022 18:24:04 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:24:04 GMT
VOLUME [/var/lib/docker]
# Tue, 07 Jun 2022 18:24:04 GMT
EXPOSE 2375 2376
# Tue, 07 Jun 2022 18:24:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 07 Jun 2022 18:24:05 GMT
CMD []
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a01eeb4b9660234932fe1a5ed6ee12b88476503688d1af44ef2cf5589db59c5`  
		Last Modified: Tue, 07 Jun 2022 18:25:11 GMT  
		Size: 65.5 MB (65511093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f16477544224c056335320872aa8dd6c2a404df9982484e1f62603e0f1f8e2a`  
		Last Modified: Tue, 07 Jun 2022 18:25:01 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e917105572c19bab12a64c5f1079e8d7b0a3e10899bd0398d1f136d41a4af191`  
		Last Modified: Tue, 07 Jun 2022 18:25:00 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709778230e46fbd5042dc9165462ac00b69b08da200fd164c4b55ee90d71ed6`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94076fc9c77a2ec8cd8737d8ee69c11882eaa16be0e46ea97b42763d6de07213`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0650593e055d90b3f09ecf2e61114a35929437150d1f25d6e9aea5e4d4ef57`  
		Last Modified: Tue, 07 Jun 2022 18:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8739efbf33852756a9d17dd471ab7ab9d9a1f183df6185763c4f54d55f3e5ef`  
		Last Modified: Tue, 07 Jun 2022 18:25:31 GMT  
		Size: 6.9 MB (6862542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1528486149a1ec660cc13a105d322cbe384bf2fd0bb5b32436043928d35701e8`  
		Last Modified: Tue, 07 Jun 2022 18:25:30 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fce28207d4c0f42d2a8352f195f1551714dfa68bcc768565b63a0e030a46813`  
		Last Modified: Tue, 07 Jun 2022 18:25:29 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c6543c9821cdb12ce3c3b95bed6148272f6ee648fcaf31c1b5b6d7aa67c459`  
		Last Modified: Tue, 07 Jun 2022 18:25:29 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:c82526b54ad542830185247b1fd7cd75ca06c4b7379625a631193ebebbffceb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93216008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d2d13d30ebd3836c5760272dda377aa12d9253bf2aee7a175a1360773e2a9d9`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:44:31 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:44:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:44:36 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:44:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:44:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:44:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:44:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:44:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:44:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:44:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:44:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:44:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:45:01 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 07 Jun 2022 18:45:02 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:45:03 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 07 Jun 2022 18:45:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 07 Jun 2022 18:45:06 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:45:06 GMT
VOLUME [/var/lib/docker]
# Tue, 07 Jun 2022 18:45:07 GMT
EXPOSE 2375 2376
# Tue, 07 Jun 2022 18:45:08 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 07 Jun 2022 18:45:09 GMT
CMD []
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208c9164699a390332f26552a4e3372cbba8153d21dd8c579d78b4820727447`  
		Last Modified: Tue, 07 Jun 2022 18:46:58 GMT  
		Size: 60.0 MB (60022171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd660eb6acfde977fdcc2e06e1f8b820b994c605f8d7c2a43c8043fee47a59`  
		Last Modified: Tue, 07 Jun 2022 18:46:49 GMT  
		Size: 13.1 MB (13097908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed4b77ab26353356aa5e47399b195759c104e1949f2c8552ed99141fcd5a8e6`  
		Last Modified: Tue, 07 Jun 2022 18:46:48 GMT  
		Size: 8.7 MB (8663386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e346f102da723c6d8f8709a20fe5d2b88c6efc5c31da9c1e7fba1007acd0ec1f`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97325db524006b151b2a34f2981b47567785b4362b383f8672aa4ccd00df3bfe`  
		Last Modified: Tue, 07 Jun 2022 18:46:47 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6e016098eef53d87f0df18ffe9c41bda01a822971b75a0d351d1787a4d59fb`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e98490325d999d399e486a1107cbb821ef56e26e4b8e09cba42eab6de668f53`  
		Last Modified: Tue, 07 Jun 2022 18:47:20 GMT  
		Size: 6.7 MB (6734617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3937658d06fd0152ee0795e63b1ac2bef28cd0e08636738ed86cfb3f270efe87`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520215962f31f70fbe23340f593756dd36c602b6523c60d6edf47191a3366f70`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c038ae79644412f10a6fd71b2aeb63c3462ca53f5eba947465d067157abd1d`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 2.7 KB (2748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:9ff8f7cf745620a1d20cf27034f544f1ff7bca5a2abbcda2857962104e042bc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:96b2a2fefca7613f5b34629ac11cabaf527e8f440cbac8b7dc4c295c10b0e6cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.7 MB (121693146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8475d2a876361c1765ccfcd694b66a7a121b34b3d75a04f55d5b94a7437da1c3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:23:40 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:23:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:23:46 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:23:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:23:48 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:23:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:23:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:23:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:23:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:23:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:23:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:24:02 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 07 Jun 2022 18:24:03 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:24:03 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 07 Jun 2022 18:24:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 07 Jun 2022 18:24:04 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:24:04 GMT
VOLUME [/var/lib/docker]
# Tue, 07 Jun 2022 18:24:04 GMT
EXPOSE 2375 2376
# Tue, 07 Jun 2022 18:24:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 07 Jun 2022 18:24:05 GMT
CMD []
# Tue, 07 Jun 2022 18:24:11 GMT
RUN apk add --no-cache iproute2
# Tue, 07 Jun 2022 18:24:11 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 07 Jun 2022 18:24:12 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:24:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 07 Jun 2022 18:24:15 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 07 Jun 2022 18:24:15 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 07 Jun 2022 18:24:15 GMT
USER rootless
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a01eeb4b9660234932fe1a5ed6ee12b88476503688d1af44ef2cf5589db59c5`  
		Last Modified: Tue, 07 Jun 2022 18:25:11 GMT  
		Size: 65.5 MB (65511093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f16477544224c056335320872aa8dd6c2a404df9982484e1f62603e0f1f8e2a`  
		Last Modified: Tue, 07 Jun 2022 18:25:01 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e917105572c19bab12a64c5f1079e8d7b0a3e10899bd0398d1f136d41a4af191`  
		Last Modified: Tue, 07 Jun 2022 18:25:00 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709778230e46fbd5042dc9165462ac00b69b08da200fd164c4b55ee90d71ed6`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94076fc9c77a2ec8cd8737d8ee69c11882eaa16be0e46ea97b42763d6de07213`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0650593e055d90b3f09ecf2e61114a35929437150d1f25d6e9aea5e4d4ef57`  
		Last Modified: Tue, 07 Jun 2022 18:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8739efbf33852756a9d17dd471ab7ab9d9a1f183df6185763c4f54d55f3e5ef`  
		Last Modified: Tue, 07 Jun 2022 18:25:31 GMT  
		Size: 6.9 MB (6862542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1528486149a1ec660cc13a105d322cbe384bf2fd0bb5b32436043928d35701e8`  
		Last Modified: Tue, 07 Jun 2022 18:25:30 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fce28207d4c0f42d2a8352f195f1551714dfa68bcc768565b63a0e030a46813`  
		Last Modified: Tue, 07 Jun 2022 18:25:29 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c6543c9821cdb12ce3c3b95bed6148272f6ee648fcaf31c1b5b6d7aa67c459`  
		Last Modified: Tue, 07 Jun 2022 18:25:29 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a725abeedbfa4c33a7418f41fd875f275696b28eab0a79ba1aa544660a5e7b`  
		Last Modified: Tue, 07 Jun 2022 18:25:50 GMT  
		Size: 1.2 MB (1232609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6a3e20c8491b4d470b9c1a11dceab173fc5252f5fdb7deca56332f03d5b07d`  
		Last Modified: Tue, 07 Jun 2022 18:25:49 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c3ab7612a60e9dbcc8ef8900c43e8d03e0ee26e556f11ef6d7c7fa68ad5fcc`  
		Last Modified: Tue, 07 Jun 2022 18:25:49 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86880a2ebfe3428ec38a5d7146121cab83d10c47b662e08b7296300c5ba36b90`  
		Last Modified: Tue, 07 Jun 2022 18:25:53 GMT  
		Size: 19.3 MB (19346876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08bf902c5827b673ef106ed1a4eaa55f3b5df8409fea26c822f0b6369895c0b`  
		Last Modified: Tue, 07 Jun 2022 18:25:49 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:32882c77434b98c975ceb1b3b96dffe40acbf1cfe7a0af5d515331e4781d4541
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115640767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62f34441530bb8a901ae97f5ffd28037dfbe34695de70e1f8bd14c5e7d9b09ae`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:44:31 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:44:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:44:36 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:44:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:44:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:44:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:44:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:44:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:44:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:44:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:44:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:44:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:45:01 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 07 Jun 2022 18:45:02 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:45:03 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 07 Jun 2022 18:45:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 07 Jun 2022 18:45:06 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:45:06 GMT
VOLUME [/var/lib/docker]
# Tue, 07 Jun 2022 18:45:07 GMT
EXPOSE 2375 2376
# Tue, 07 Jun 2022 18:45:08 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 07 Jun 2022 18:45:09 GMT
CMD []
# Tue, 07 Jun 2022 18:45:17 GMT
RUN apk add --no-cache iproute2
# Tue, 07 Jun 2022 18:45:18 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 07 Jun 2022 18:45:19 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:45:21 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 07 Jun 2022 18:45:22 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 07 Jun 2022 18:45:23 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 07 Jun 2022 18:45:24 GMT
USER rootless
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208c9164699a390332f26552a4e3372cbba8153d21dd8c579d78b4820727447`  
		Last Modified: Tue, 07 Jun 2022 18:46:58 GMT  
		Size: 60.0 MB (60022171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd660eb6acfde977fdcc2e06e1f8b820b994c605f8d7c2a43c8043fee47a59`  
		Last Modified: Tue, 07 Jun 2022 18:46:49 GMT  
		Size: 13.1 MB (13097908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed4b77ab26353356aa5e47399b195759c104e1949f2c8552ed99141fcd5a8e6`  
		Last Modified: Tue, 07 Jun 2022 18:46:48 GMT  
		Size: 8.7 MB (8663386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e346f102da723c6d8f8709a20fe5d2b88c6efc5c31da9c1e7fba1007acd0ec1f`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97325db524006b151b2a34f2981b47567785b4362b383f8672aa4ccd00df3bfe`  
		Last Modified: Tue, 07 Jun 2022 18:46:47 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6e016098eef53d87f0df18ffe9c41bda01a822971b75a0d351d1787a4d59fb`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e98490325d999d399e486a1107cbb821ef56e26e4b8e09cba42eab6de668f53`  
		Last Modified: Tue, 07 Jun 2022 18:47:20 GMT  
		Size: 6.7 MB (6734617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3937658d06fd0152ee0795e63b1ac2bef28cd0e08636738ed86cfb3f270efe87`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520215962f31f70fbe23340f593756dd36c602b6523c60d6edf47191a3366f70`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c038ae79644412f10a6fd71b2aeb63c3462ca53f5eba947465d067157abd1d`  
		Last Modified: Tue, 07 Jun 2022 18:47:19 GMT  
		Size: 2.7 KB (2748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a25f04457a8992aec9515a93b8e684c6308ac16e40609e4aea6e5e17e5a9831`  
		Last Modified: Tue, 07 Jun 2022 18:47:42 GMT  
		Size: 1.2 MB (1246089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4737bba435e3c5bf8e0bd36ea8549325126984e556f0383a65cd0780c17c41f3`  
		Last Modified: Tue, 07 Jun 2022 18:47:41 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153a758456f1bf14ac68b5cc4e5adf575663fbad6ee03e0056a9cd6162b45259`  
		Last Modified: Tue, 07 Jun 2022 18:47:42 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6ecdd375957217ed6f2887df5b1aede054583d798040f1fa03e2113584c479`  
		Last Modified: Tue, 07 Jun 2022 18:47:45 GMT  
		Size: 21.2 MB (21177045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e75e34fe059e0be78079a5bd13cfd80b8d414fad4f717402e56a2fa8343ed0`  
		Last Modified: Tue, 07 Jun 2022 18:47:41 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:ae822531c5ce930bb49408e170ed0b1fd4efcf86da1777687c90f3471b6f73ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:fba3948c035af5fd3a4cbe953195dcbdab125581f254d44044d87b2e88aef8ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101178830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d39449ad493ed1d71480ba17d4dcd56af4c28605f7f5645a1429f077cd8513`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:23:40 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:23:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:23:46 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:23:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:23:48 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:23:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:23:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:23:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:23:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:23:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:23:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:24:19 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a01eeb4b9660234932fe1a5ed6ee12b88476503688d1af44ef2cf5589db59c5`  
		Last Modified: Tue, 07 Jun 2022 18:25:11 GMT  
		Size: 65.5 MB (65511093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f16477544224c056335320872aa8dd6c2a404df9982484e1f62603e0f1f8e2a`  
		Last Modified: Tue, 07 Jun 2022 18:25:01 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e917105572c19bab12a64c5f1079e8d7b0a3e10899bd0398d1f136d41a4af191`  
		Last Modified: Tue, 07 Jun 2022 18:25:00 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709778230e46fbd5042dc9165462ac00b69b08da200fd164c4b55ee90d71ed6`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94076fc9c77a2ec8cd8737d8ee69c11882eaa16be0e46ea97b42763d6de07213`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0650593e055d90b3f09ecf2e61114a35929437150d1f25d6e9aea5e4d4ef57`  
		Last Modified: Tue, 07 Jun 2022 18:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd116fbfcda7d014c42d3891e0c2d200795c968f665e123ee95a0e6d1e5c934`  
		Last Modified: Tue, 07 Jun 2022 18:26:11 GMT  
		Size: 6.9 MB (6934452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f633c11b5bfc875d87905074a8a032404ce2bfefb7e51f9f6919d36277e77393
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.5 MB (93521092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb6d61e7054c42bfa4ad4e5dca6aee71560f8fddb61b5a6a8101a66320730b1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:44:31 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:44:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:44:36 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:44:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:44:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:44:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:44:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:44:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:44:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:44:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:44:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:44:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:45:32 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208c9164699a390332f26552a4e3372cbba8153d21dd8c579d78b4820727447`  
		Last Modified: Tue, 07 Jun 2022 18:46:58 GMT  
		Size: 60.0 MB (60022171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd660eb6acfde977fdcc2e06e1f8b820b994c605f8d7c2a43c8043fee47a59`  
		Last Modified: Tue, 07 Jun 2022 18:46:49 GMT  
		Size: 13.1 MB (13097908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed4b77ab26353356aa5e47399b195759c104e1949f2c8552ed99141fcd5a8e6`  
		Last Modified: Tue, 07 Jun 2022 18:46:48 GMT  
		Size: 8.7 MB (8663386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e346f102da723c6d8f8709a20fe5d2b88c6efc5c31da9c1e7fba1007acd0ec1f`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97325db524006b151b2a34f2981b47567785b4362b383f8672aa4ccd00df3bfe`  
		Last Modified: Tue, 07 Jun 2022 18:46:47 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6e016098eef53d87f0df18ffe9c41bda01a822971b75a0d351d1787a4d59fb`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538445497cbaebac26dcea42aaadf26367e96ea7ccf5c022dcfd39bd1da7c882`  
		Last Modified: Tue, 07 Jun 2022 18:48:05 GMT  
		Size: 7.0 MB (7044702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:206fb7d9747e035b5fb0b12840d1117ccce38b7508c5967ddd66bfc1f8abc36a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:d06e6924e1364a690ad454e7b51a75b38f01042cb43df2f9d51098bbbc5b836d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94244378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0208b15ab9702b6bf3b7ac59e6c1d7ebbd679b94bb27367f5763297681a61abc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:23:40 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:23:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:23:46 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:23:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:23:48 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:23:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:23:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:23:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:23:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:23:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:23:52 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a01eeb4b9660234932fe1a5ed6ee12b88476503688d1af44ef2cf5589db59c5`  
		Last Modified: Tue, 07 Jun 2022 18:25:11 GMT  
		Size: 65.5 MB (65511093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f16477544224c056335320872aa8dd6c2a404df9982484e1f62603e0f1f8e2a`  
		Last Modified: Tue, 07 Jun 2022 18:25:01 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e917105572c19bab12a64c5f1079e8d7b0a3e10899bd0398d1f136d41a4af191`  
		Last Modified: Tue, 07 Jun 2022 18:25:00 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709778230e46fbd5042dc9165462ac00b69b08da200fd164c4b55ee90d71ed6`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94076fc9c77a2ec8cd8737d8ee69c11882eaa16be0e46ea97b42763d6de07213`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0650593e055d90b3f09ecf2e61114a35929437150d1f25d6e9aea5e4d4ef57`  
		Last Modified: Tue, 07 Jun 2022 18:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4e95dfecee5f5f5a6ed920904149fdba4cbe725d149df62f88e556f6a64204f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.5 MB (86476390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065f5b92312ea447a580a243adb30727f02719699a6e80d668170755e50bf642`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Jun 2022 18:44:31 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:44:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:44:36 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:44:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:44:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:44:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:44:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:44:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:44:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:44:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:44:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:44:52 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208c9164699a390332f26552a4e3372cbba8153d21dd8c579d78b4820727447`  
		Last Modified: Tue, 07 Jun 2022 18:46:58 GMT  
		Size: 60.0 MB (60022171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd660eb6acfde977fdcc2e06e1f8b820b994c605f8d7c2a43c8043fee47a59`  
		Last Modified: Tue, 07 Jun 2022 18:46:49 GMT  
		Size: 13.1 MB (13097908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed4b77ab26353356aa5e47399b195759c104e1949f2c8552ed99141fcd5a8e6`  
		Last Modified: Tue, 07 Jun 2022 18:46:48 GMT  
		Size: 8.7 MB (8663386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e346f102da723c6d8f8709a20fe5d2b88c6efc5c31da9c1e7fba1007acd0ec1f`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97325db524006b151b2a34f2981b47567785b4362b383f8672aa4ccd00df3bfe`  
		Last Modified: Tue, 07 Jun 2022 18:46:47 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6e016098eef53d87f0df18ffe9c41bda01a822971b75a0d351d1787a4d59fb`  
		Last Modified: Tue, 07 Jun 2022 18:46:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:rc`

```console
$ docker pull docker@sha256:0964ecc3084a4908f49afef17df539e7f355c5336969ad41ec9200182b919cb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:rc` - linux; amd64

```console
$ docker pull docker@sha256:b9614a53230d0a4c4f22f2d004e04362d9f147082898cd507de08736cfe744a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.8 MB (90771523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007fe5047a7c961c196b4479f8e4263e4da34c07677f92e330cf9749228dba4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 19:01:29 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 19:01:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 19:01:35 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 19:01:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 19:01:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 19:01:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 19:01:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 19:01:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:45 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99ba1e24152bfcd6f75ac7d03379a0d722bb011a60e4da292b3234ed0c229c5`  
		Last Modified: Mon, 06 Jun 2022 19:03:02 GMT  
		Size: 62.0 MB (62038242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d073b016bf56120f6f99463e72dfc1669ee2cf81aea28338e191dc3392b76c2`  
		Last Modified: Mon, 06 Jun 2022 19:02:53 GMT  
		Size: 14.5 MB (14454318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae7a7070ea618fa5d597e5c3d9fafb5531a4c0ba8b5f7f12e334175f7424643`  
		Last Modified: Mon, 06 Jun 2022 19:02:52 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b69fd3006304e4afc4226a31c41076934d97c9a0c8d536bc2acda02006dab5`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff67f9f388ec6907bd17f3fa9106924c548d5374d7e483e089076822e8759f9`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77709b39dac35a99fc73e9b30dab31b8e61f7729021558d7647d544c1eaa0f23`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f1168269caf92da50e2c6c8781facff325d5a643079ef6534abf1b293d9cbfa7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.5 MB (83481513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3af4b446c8d50a9581547b8dc9a07922f7666fe639a1ffda87e9842bacadbf5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 18:36:44 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 18:36:50 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 18:36:50 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 18:36:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 18:36:55 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 18:36:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 18:37:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 18:37:02 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 18:37:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 18:37:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:05 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f1c4eb6753c4d8ca8abdc68946eaf136ebf43c3ba68b1e3f168d561a7a40e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:21 GMT  
		Size: 57.0 MB (57027293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8543d611571340a3ade0985e604f8050b3bd7c750ce108d248072285be716e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:13 GMT  
		Size: 13.1 MB (13097906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55bb534319c1b57528e0e77d4e31677b56a064afe3ef44ab80b3dcbb546fba69`  
		Last Modified: Mon, 06 Jun 2022 18:39:12 GMT  
		Size: 8.7 MB (8663389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596ba91569b21aa39db419bf97611342f554933900d729efaea259246e43c6c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8084d414abe81d6b025915fb786b9604e6c92ca873948a0840d95927314986bc`  
		Last Modified: Mon, 06 Jun 2022 18:39:11 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62b19d6f46e3b8b83902e63f8497def66bced996fd9b45792acf2c9d5afe0c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:rc-dind`

```console
$ docker pull docker@sha256:aac3ee54242eb33fddb238884878e0d5c059b2b227f6914086ddb183064f7314
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:rc-dind` - linux; amd64

```console
$ docker pull docker@sha256:ceb6d3f593b1d1a8991d661a78f9f46b35fd0c32f4e5ea95bd70505ab9141d6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.6 MB (97639097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60c88fe5471ef65f8032de6a0e7bf7162da118b90df5747a2b3b598b7d50a455`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 19:01:29 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 19:01:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 19:01:35 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 19:01:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 19:01:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 19:01:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 19:01:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 19:01:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:45 GMT
CMD ["sh"]
# Mon, 06 Jun 2022 19:01:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 06 Jun 2022 19:01:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 06 Jun 2022 19:01:53 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 06 Jun 2022 19:01:54 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 06 Jun 2022 19:01:54 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:54 GMT
VOLUME [/var/lib/docker]
# Mon, 06 Jun 2022 19:01:54 GMT
EXPOSE 2375 2376
# Mon, 06 Jun 2022 19:01:54 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:54 GMT
CMD []
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99ba1e24152bfcd6f75ac7d03379a0d722bb011a60e4da292b3234ed0c229c5`  
		Last Modified: Mon, 06 Jun 2022 19:03:02 GMT  
		Size: 62.0 MB (62038242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d073b016bf56120f6f99463e72dfc1669ee2cf81aea28338e191dc3392b76c2`  
		Last Modified: Mon, 06 Jun 2022 19:02:53 GMT  
		Size: 14.5 MB (14454318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae7a7070ea618fa5d597e5c3d9fafb5531a4c0ba8b5f7f12e334175f7424643`  
		Last Modified: Mon, 06 Jun 2022 19:02:52 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b69fd3006304e4afc4226a31c41076934d97c9a0c8d536bc2acda02006dab5`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff67f9f388ec6907bd17f3fa9106924c548d5374d7e483e089076822e8759f9`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77709b39dac35a99fc73e9b30dab31b8e61f7729021558d7647d544c1eaa0f23`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050708f4cb014b2395c1711989e46137eee788ff144f8a78fb7d27e8f6a54dc2`  
		Last Modified: Mon, 06 Jun 2022 19:03:18 GMT  
		Size: 6.9 MB (6862552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57437c337af006e3910175ac4b9f04054d69be2d790281e168f454cdb4d32301`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9320a07c879e2f8f96b6cb7f5ed2578bb1126537514c17728e6459ba3dbc35c`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f41b868a08905a9d2b14f2212edab168e71b841ca2db546976f5bd25bcd52e`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 2.7 KB (2745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:7c7ec0aed8659021619bc24b0b9a7df51eb46ee8156bff5075a59a3f16c4eeda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90221146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cc869c8ebc6cae1fb3b1baabab00e9d8029967f6c7f60411689d8d53af8a7aa`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 18:36:44 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 18:36:50 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 18:36:50 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 18:36:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 18:36:55 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 18:36:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 18:37:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 18:37:02 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 18:37:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 18:37:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:05 GMT
CMD ["sh"]
# Mon, 06 Jun 2022 18:37:15 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 06 Jun 2022 18:37:16 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 06 Jun 2022 18:37:17 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 06 Jun 2022 18:37:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 06 Jun 2022 18:37:20 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:20 GMT
VOLUME [/var/lib/docker]
# Mon, 06 Jun 2022 18:37:21 GMT
EXPOSE 2375 2376
# Mon, 06 Jun 2022 18:37:22 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:23 GMT
CMD []
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f1c4eb6753c4d8ca8abdc68946eaf136ebf43c3ba68b1e3f168d561a7a40e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:21 GMT  
		Size: 57.0 MB (57027293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8543d611571340a3ade0985e604f8050b3bd7c750ce108d248072285be716e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:13 GMT  
		Size: 13.1 MB (13097906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55bb534319c1b57528e0e77d4e31677b56a064afe3ef44ab80b3dcbb546fba69`  
		Last Modified: Mon, 06 Jun 2022 18:39:12 GMT  
		Size: 8.7 MB (8663389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596ba91569b21aa39db419bf97611342f554933900d729efaea259246e43c6c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8084d414abe81d6b025915fb786b9604e6c92ca873948a0840d95927314986bc`  
		Last Modified: Mon, 06 Jun 2022 18:39:11 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62b19d6f46e3b8b83902e63f8497def66bced996fd9b45792acf2c9d5afe0c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c89092436ecc8615129e3f6851e1aeb6859cef0e5c8a99b5fe161c697d3b66a`  
		Last Modified: Mon, 06 Jun 2022 18:39:40 GMT  
		Size: 6.7 MB (6734638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b59828045492d626ecfdc53018fe98f86abbe1be9bf97a382026766e6680967`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731ca3affcf287405fe70a2a14535aea43776a755f4fa7701b780bd7773319fe`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59501b524a36d2a0f78ce443006bcfb2ce1c35a184836795fe0c527dbef3f02c`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:rc-dind-rootless`

```console
$ docker pull docker@sha256:5268e25e95d2380f29cbd313c117b47368679fb9bd823cb26405f881e0f96849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:rc-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:aa96a6309f6b63e8f5a04cfd9fd4dfca1b832a4464c213c5dcf08e51770b8e60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118791286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f868da0c728f57942c20154333eba26a5778c79a98b138498910d05d7543f0e1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 19:01:29 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 19:01:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 19:01:35 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 19:01:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 19:01:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 19:01:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 19:01:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 19:01:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:45 GMT
CMD ["sh"]
# Mon, 06 Jun 2022 19:01:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 06 Jun 2022 19:01:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 06 Jun 2022 19:01:53 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 06 Jun 2022 19:01:54 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 06 Jun 2022 19:01:54 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:54 GMT
VOLUME [/var/lib/docker]
# Mon, 06 Jun 2022 19:01:54 GMT
EXPOSE 2375 2376
# Mon, 06 Jun 2022 19:01:54 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:54 GMT
CMD []
# Mon, 06 Jun 2022 19:01:58 GMT
RUN apk add --no-cache iproute2
# Mon, 06 Jun 2022 19:01:59 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 06 Jun 2022 19:01:59 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 06 Jun 2022 19:02:02 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-rootless-extras-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 06 Jun 2022 19:02:03 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 06 Jun 2022 19:02:03 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 06 Jun 2022 19:02:03 GMT
USER rootless
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99ba1e24152bfcd6f75ac7d03379a0d722bb011a60e4da292b3234ed0c229c5`  
		Last Modified: Mon, 06 Jun 2022 19:03:02 GMT  
		Size: 62.0 MB (62038242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d073b016bf56120f6f99463e72dfc1669ee2cf81aea28338e191dc3392b76c2`  
		Last Modified: Mon, 06 Jun 2022 19:02:53 GMT  
		Size: 14.5 MB (14454318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae7a7070ea618fa5d597e5c3d9fafb5531a4c0ba8b5f7f12e334175f7424643`  
		Last Modified: Mon, 06 Jun 2022 19:02:52 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b69fd3006304e4afc4226a31c41076934d97c9a0c8d536bc2acda02006dab5`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff67f9f388ec6907bd17f3fa9106924c548d5374d7e483e089076822e8759f9`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77709b39dac35a99fc73e9b30dab31b8e61f7729021558d7647d544c1eaa0f23`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050708f4cb014b2395c1711989e46137eee788ff144f8a78fb7d27e8f6a54dc2`  
		Last Modified: Mon, 06 Jun 2022 19:03:18 GMT  
		Size: 6.9 MB (6862552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57437c337af006e3910175ac4b9f04054d69be2d790281e168f454cdb4d32301`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9320a07c879e2f8f96b6cb7f5ed2578bb1126537514c17728e6459ba3dbc35c`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f41b868a08905a9d2b14f2212edab168e71b841ca2db546976f5bd25bcd52e`  
		Last Modified: Mon, 06 Jun 2022 19:03:17 GMT  
		Size: 2.7 KB (2745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc40b41e848d564c191097f81774cc897146ea1de2e76de308bb9269285f9b45`  
		Last Modified: Mon, 06 Jun 2022 19:03:34 GMT  
		Size: 1.2 MB (1232607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bfe48e653a7dc4eeb5579193ad0b4e6034a2b2586180a962e20bacab33624b`  
		Last Modified: Mon, 06 Jun 2022 19:03:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60e157845c0009309f2947508ada20712260eb7d8802f8ad3bd6025cb5da2eb`  
		Last Modified: Mon, 06 Jun 2022 19:03:34 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1838ba7dfdeda85348a3cf82992a7be7b26f4d9ff4d47609e2ca9e0cd1cf60`  
		Last Modified: Mon, 06 Jun 2022 19:03:37 GMT  
		Size: 19.9 MB (19917868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523494b3db69397e50326566071235673b0f24e5b1fcc42be82486b99fce41ca`  
		Last Modified: Mon, 06 Jun 2022 19:03:34 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:54ee14edc9c35713cdafaced9e7fd525eb23e6b02fbf0d0f9b133b74b3a070ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.4 MB (113356240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f7b08a2a6cb290aa2d68a8d07cf52d8ed14e8e72121e6ce90fbeaf924d862ab`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 18:36:44 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 18:36:50 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 18:36:50 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 18:36:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 18:36:55 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 18:36:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 18:37:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 18:37:02 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 18:37:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 18:37:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:05 GMT
CMD ["sh"]
# Mon, 06 Jun 2022 18:37:15 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 06 Jun 2022 18:37:16 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 06 Jun 2022 18:37:17 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 06 Jun 2022 18:37:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 06 Jun 2022 18:37:20 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:20 GMT
VOLUME [/var/lib/docker]
# Mon, 06 Jun 2022 18:37:21 GMT
EXPOSE 2375 2376
# Mon, 06 Jun 2022 18:37:22 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:23 GMT
CMD []
# Mon, 06 Jun 2022 18:37:31 GMT
RUN apk add --no-cache iproute2
# Mon, 06 Jun 2022 18:37:32 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 06 Jun 2022 18:37:33 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 06 Jun 2022 18:37:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-rootless-extras-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 06 Jun 2022 18:37:37 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 06 Jun 2022 18:37:38 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 06 Jun 2022 18:37:39 GMT
USER rootless
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f1c4eb6753c4d8ca8abdc68946eaf136ebf43c3ba68b1e3f168d561a7a40e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:21 GMT  
		Size: 57.0 MB (57027293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8543d611571340a3ade0985e604f8050b3bd7c750ce108d248072285be716e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:13 GMT  
		Size: 13.1 MB (13097906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55bb534319c1b57528e0e77d4e31677b56a064afe3ef44ab80b3dcbb546fba69`  
		Last Modified: Mon, 06 Jun 2022 18:39:12 GMT  
		Size: 8.7 MB (8663389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596ba91569b21aa39db419bf97611342f554933900d729efaea259246e43c6c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8084d414abe81d6b025915fb786b9604e6c92ca873948a0840d95927314986bc`  
		Last Modified: Mon, 06 Jun 2022 18:39:11 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62b19d6f46e3b8b83902e63f8497def66bced996fd9b45792acf2c9d5afe0c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c89092436ecc8615129e3f6851e1aeb6859cef0e5c8a99b5fe161c697d3b66a`  
		Last Modified: Mon, 06 Jun 2022 18:39:40 GMT  
		Size: 6.7 MB (6734638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b59828045492d626ecfdc53018fe98f86abbe1be9bf97a382026766e6680967`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731ca3affcf287405fe70a2a14535aea43776a755f4fa7701b780bd7773319fe`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59501b524a36d2a0f78ce443006bcfb2ce1c35a184836795fe0c527dbef3f02c`  
		Last Modified: Mon, 06 Jun 2022 18:39:39 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1349775e36852c48e984ab260b7262a05f902263a5488a8c3310a9e7ce84d612`  
		Last Modified: Mon, 06 Jun 2022 18:39:58 GMT  
		Size: 1.2 MB (1246071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ef4534bef24c4f8122f7275ee5a49000cbbeafeac66ecaa0c9e0d35c413eb5`  
		Last Modified: Mon, 06 Jun 2022 18:39:57 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4d33e0ed79838456d16cfbfcd8378818231b3cd82ee5630d58ac5e48a671fc`  
		Last Modified: Mon, 06 Jun 2022 18:39:58 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3433ce83674bad06b4dac071ea1995bdd1eb1014e83c23135e06971a450618dc`  
		Last Modified: Mon, 06 Jun 2022 18:40:01 GMT  
		Size: 21.9 MB (21887400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf27541a67b4884567ee908beefa5866a7295afe5d3eaa5ce8a04070fab57b6e`  
		Last Modified: Mon, 06 Jun 2022 18:39:58 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:rc-git`

```console
$ docker pull docker@sha256:79316cbde1069c03adef776435eb3624c5ae9866dd1df6a399b020146bec8a82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:rc-git` - linux; amd64

```console
$ docker pull docker@sha256:50d2107405e49b19cf4d72e886153f0679eb3abf48e2d3b3de4669d56d49f9eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.7 MB (97705984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcf6afb24ceadac365d6f10e98b0588eec5290ea19c9d8e76923ac45d134e3b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 19:01:29 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 19:01:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 19:01:35 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 19:01:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 19:01:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 19:01:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 19:01:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 19:01:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 19:01:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 19:01:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 19:01:45 GMT
CMD ["sh"]
# Mon, 06 Jun 2022 19:02:08 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99ba1e24152bfcd6f75ac7d03379a0d722bb011a60e4da292b3234ed0c229c5`  
		Last Modified: Mon, 06 Jun 2022 19:03:02 GMT  
		Size: 62.0 MB (62038242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d073b016bf56120f6f99463e72dfc1669ee2cf81aea28338e191dc3392b76c2`  
		Last Modified: Mon, 06 Jun 2022 19:02:53 GMT  
		Size: 14.5 MB (14454318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae7a7070ea618fa5d597e5c3d9fafb5531a4c0ba8b5f7f12e334175f7424643`  
		Last Modified: Mon, 06 Jun 2022 19:02:52 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b69fd3006304e4afc4226a31c41076934d97c9a0c8d536bc2acda02006dab5`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff67f9f388ec6907bd17f3fa9106924c548d5374d7e483e089076822e8759f9`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77709b39dac35a99fc73e9b30dab31b8e61f7729021558d7647d544c1eaa0f23`  
		Last Modified: Mon, 06 Jun 2022 19:02:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4029b623e7cf6a5b9070d256c16adf13d0c929453290286bba377419aae00e`  
		Last Modified: Mon, 06 Jun 2022 19:04:05 GMT  
		Size: 6.9 MB (6934461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f06691ad72c9fd7d3baaae7926667a6ea2e421dbcc613687d533ecdbdd0facae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.5 MB (90526228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb3d44d014348c6a18353b4dc9d6ef164e61a59e2dc8dc968e8ec25928b3a259`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 18:36:44 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Mon, 06 Jun 2022 18:36:50 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 06 Jun 2022 18:36:50 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Mon, 06 Jun 2022 18:36:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 06 Jun 2022 18:36:55 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Mon, 06 Jun 2022 18:36:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 06 Jun 2022 18:37:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 06 Jun 2022 18:37:02 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 06 Jun 2022 18:37:02 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 06 Jun 2022 18:37:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 06 Jun 2022 18:37:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 18:37:05 GMT
CMD ["sh"]
# Mon, 06 Jun 2022 18:37:46 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f1c4eb6753c4d8ca8abdc68946eaf136ebf43c3ba68b1e3f168d561a7a40e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:21 GMT  
		Size: 57.0 MB (57027293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8543d611571340a3ade0985e604f8050b3bd7c750ce108d248072285be716e4`  
		Last Modified: Mon, 06 Jun 2022 18:39:13 GMT  
		Size: 13.1 MB (13097906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55bb534319c1b57528e0e77d4e31677b56a064afe3ef44ab80b3dcbb546fba69`  
		Last Modified: Mon, 06 Jun 2022 18:39:12 GMT  
		Size: 8.7 MB (8663389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596ba91569b21aa39db419bf97611342f554933900d729efaea259246e43c6c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8084d414abe81d6b025915fb786b9604e6c92ca873948a0840d95927314986bc`  
		Last Modified: Mon, 06 Jun 2022 18:39:11 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62b19d6f46e3b8b83902e63f8497def66bced996fd9b45792acf2c9d5afe0c`  
		Last Modified: Mon, 06 Jun 2022 18:39:10 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6266696465611c20778351065a15881b4a1edf1c9b4564e4d0779e0b7a3b6565`  
		Last Modified: Mon, 06 Jun 2022 18:40:33 GMT  
		Size: 7.0 MB (7044715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:rc-windowsservercore`

```console
$ docker pull docker@sha256:a34a08901b0c5a62d5638ae79160ad5cf955957f1ccf74b33c1863d15a9c2715
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.768; amd64
	-	windows version 10.0.17763.3046; amd64

### `docker:rc-windowsservercore` - windows version 10.0.20348.768; amd64

```console
$ docker pull docker@sha256:31b40cdc8e6e34d3869c35721212713e9d854c740003a20a1ca54262b4c6feab
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2288871549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6184a51f1d672575333cf01827c8883557519edbfbb7c8de596fd7b52760b768`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 09 Jun 2022 04:32:50 GMT
RUN Install update 10.0.20348.768
# Wed, 15 Jun 2022 12:13:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:46:14 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:46:15 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Wed, 15 Jun 2022 22:46:16 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/test/x86_64/docker-22.06.0-beta.0.zip
# Wed, 15 Jun 2022 22:46:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c71967ff41928927e4c407171e4ffbac3c9ab4221eb64f5ca5a34ff4c230567`  
		Size: 841.6 MB (841600427 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dec0338feaf01f35eb916b7fd9ecc08b719354163254885d5215e513c1a3eb2e`  
		Last Modified: Wed, 15 Jun 2022 12:49:26 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a162967ebe5da992f6dc4e9ebdd4ec9f402a84f6974c0c562cff1ed6f17dd39`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 630.9 KB (630886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7902af8cf06c7ef3cc0300bbdcd16b3d7610d4fb13025ded6e6d713b521b96`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b543c7ed7d518ed7e28b7429fa7638f623013abfb287c5e3de9ac6feadbcc964`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3eebb13fc88926962ee253a6b493aa8ac1b4eb3b24ac973a2443f8f50b5af00`  
		Last Modified: Wed, 15 Jun 2022 22:52:35 GMT  
		Size: 9.8 MB (9772337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-windowsservercore` - windows version 10.0.17763.3046; amd64

```console
$ docker pull docker@sha256:493c7d58e2a74e217d0260db9fe2990755ad5d67b47d02c688277170415a1ceb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2673168277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97f8ec54ab6b0001e01fe57fce6bd7049a77d0b53f2a991dd90a46616ed565cf`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:48:09 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:48:10 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Wed, 15 Jun 2022 22:48:11 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/test/x86_64/docker-22.06.0-beta.0.zip
# Wed, 15 Jun 2022 22:49:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4c7110da70e07b37a00b3b05b18361572412287fee26eba04fcf23dcb75639`  
		Last Modified: Wed, 15 Jun 2022 22:52:48 GMT  
		Size: 352.2 KB (352228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c60272810a69a46255c487510637a80961c5d5bca4668b996bf20aa9d73896`  
		Last Modified: Wed, 15 Jun 2022 22:52:47 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3c712e062b5fcb69c4b6081c9c1d833fa38bb3e369b44b6b9347e43e1d58a5`  
		Last Modified: Wed, 15 Jun 2022 22:52:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766d5b06428cea8b3c37d65a9fb8d92a424c2dd2d36fb91835cc37ffda944128`  
		Last Modified: Wed, 15 Jun 2022 22:52:50 GMT  
		Size: 9.5 MB (9532028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:rc-windowsservercore-1809`

```console
$ docker pull docker@sha256:7688c18170e798ada2435ab1829e86c7a1256fdf29f4245cbf88d7a8efa21dcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3046; amd64

### `docker:rc-windowsservercore-1809` - windows version 10.0.17763.3046; amd64

```console
$ docker pull docker@sha256:493c7d58e2a74e217d0260db9fe2990755ad5d67b47d02c688277170415a1ceb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2673168277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97f8ec54ab6b0001e01fe57fce6bd7049a77d0b53f2a991dd90a46616ed565cf`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:48:09 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:48:10 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Wed, 15 Jun 2022 22:48:11 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/test/x86_64/docker-22.06.0-beta.0.zip
# Wed, 15 Jun 2022 22:49:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4c7110da70e07b37a00b3b05b18361572412287fee26eba04fcf23dcb75639`  
		Last Modified: Wed, 15 Jun 2022 22:52:48 GMT  
		Size: 352.2 KB (352228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c60272810a69a46255c487510637a80961c5d5bca4668b996bf20aa9d73896`  
		Last Modified: Wed, 15 Jun 2022 22:52:47 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3c712e062b5fcb69c4b6081c9c1d833fa38bb3e369b44b6b9347e43e1d58a5`  
		Last Modified: Wed, 15 Jun 2022 22:52:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766d5b06428cea8b3c37d65a9fb8d92a424c2dd2d36fb91835cc37ffda944128`  
		Last Modified: Wed, 15 Jun 2022 22:52:50 GMT  
		Size: 9.5 MB (9532028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:rc-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:1b711c5b73ae6926b7f7a1a6538af7de3e1c103ec4ee93ef127a952b50e9a52b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.768; amd64

### `docker:rc-windowsservercore-ltsc2022` - windows version 10.0.20348.768; amd64

```console
$ docker pull docker@sha256:31b40cdc8e6e34d3869c35721212713e9d854c740003a20a1ca54262b4c6feab
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2288871549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6184a51f1d672575333cf01827c8883557519edbfbb7c8de596fd7b52760b768`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 09 Jun 2022 04:32:50 GMT
RUN Install update 10.0.20348.768
# Wed, 15 Jun 2022 12:13:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:46:14 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:46:15 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Wed, 15 Jun 2022 22:46:16 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/test/x86_64/docker-22.06.0-beta.0.zip
# Wed, 15 Jun 2022 22:46:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c71967ff41928927e4c407171e4ffbac3c9ab4221eb64f5ca5a34ff4c230567`  
		Size: 841.6 MB (841600427 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dec0338feaf01f35eb916b7fd9ecc08b719354163254885d5215e513c1a3eb2e`  
		Last Modified: Wed, 15 Jun 2022 12:49:26 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a162967ebe5da992f6dc4e9ebdd4ec9f402a84f6974c0c562cff1ed6f17dd39`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 630.9 KB (630886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7902af8cf06c7ef3cc0300bbdcd16b3d7610d4fb13025ded6e6d713b521b96`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b543c7ed7d518ed7e28b7429fa7638f623013abfb287c5e3de9ac6feadbcc964`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3eebb13fc88926962ee253a6b493aa8ac1b4eb3b24ac973a2443f8f50b5af00`  
		Last Modified: Wed, 15 Jun 2022 22:52:35 GMT  
		Size: 9.8 MB (9772337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore`

```console
$ docker pull docker@sha256:c46b51f81569a8528faf11ab678e415a9846ac53246ec6c2b11fc5a81e61674b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.768; amd64
	-	windows version 10.0.17763.3046; amd64

### `docker:windowsservercore` - windows version 10.0.20348.768; amd64

```console
$ docker pull docker@sha256:c92dc04a8ccb9c898c42318e134d11b4fe5e825349a870ec0af4d00a8aa32f30
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2331628569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbf9b630697f8843ffb9923fb2b24ec28ca80c582e396f4bc8ae9db8517438c8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 09 Jun 2022 04:32:50 GMT
RUN Install update 10.0.20348.768
# Wed, 15 Jun 2022 12:13:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:46:14 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:49:43 GMT
ENV DOCKER_VERSION=20.10.17
# Wed, 15 Jun 2022 22:49:44 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.17.zip
# Wed, 15 Jun 2022 22:50:20 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c71967ff41928927e4c407171e4ffbac3c9ab4221eb64f5ca5a34ff4c230567`  
		Size: 841.6 MB (841600427 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dec0338feaf01f35eb916b7fd9ecc08b719354163254885d5215e513c1a3eb2e`  
		Last Modified: Wed, 15 Jun 2022 12:49:26 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a162967ebe5da992f6dc4e9ebdd4ec9f402a84f6974c0c562cff1ed6f17dd39`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 630.9 KB (630886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6900080f685d53c251ad925dfa2391f7ea21ee77b7d5aa31e56e0d7a30666adc`  
		Last Modified: Wed, 15 Jun 2022 22:53:02 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79983762d3966bbf5de5e5397ea8b7173f7fa121d7ab01e2136817be07ae4e0f`  
		Last Modified: Wed, 15 Jun 2022 22:53:02 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7398906a7954731da34c295d4f50bdd50edb96f50ad88006b29eaa94662ccd2`  
		Last Modified: Wed, 15 Jun 2022 22:53:14 GMT  
		Size: 52.5 MB (52529382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:windowsservercore` - windows version 10.0.17763.3046; amd64

```console
$ docker pull docker@sha256:92b9efc4d05fc727177fa4d4f20e8ca35969778a932858c93dde72a69cafa065
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2715917945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:208e7e03e3e360a634a05b786e8043476d165cf2930fc4237e9c34c390385228`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:48:09 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:50:28 GMT
ENV DOCKER_VERSION=20.10.17
# Wed, 15 Jun 2022 22:50:29 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.17.zip
# Wed, 15 Jun 2022 22:51:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4c7110da70e07b37a00b3b05b18361572412287fee26eba04fcf23dcb75639`  
		Last Modified: Wed, 15 Jun 2022 22:52:48 GMT  
		Size: 352.2 KB (352228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a3fc52e3c402b1be6f7512b16405aaaba3edd6037ede2a7885b367bec19efd`  
		Last Modified: Wed, 15 Jun 2022 22:53:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92deca7aa7a34f968926e81414d0102042c2a2e85968fa9423cb1ceed71a9393`  
		Last Modified: Wed, 15 Jun 2022 22:53:28 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f346f796df4e8cb918a2d6f83dcf31d1544d3af9b283727e9757400a160423ab`  
		Last Modified: Wed, 15 Jun 2022 22:53:39 GMT  
		Size: 52.3 MB (52281684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:f8c99a477afebef2e0a504c1a2d40be47010d4e93cb99febe638d0eb20505199
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3046; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.3046; amd64

```console
$ docker pull docker@sha256:92b9efc4d05fc727177fa4d4f20e8ca35969778a932858c93dde72a69cafa065
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2715917945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:208e7e03e3e360a634a05b786e8043476d165cf2930fc4237e9c34c390385228`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:48:09 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:50:28 GMT
ENV DOCKER_VERSION=20.10.17
# Wed, 15 Jun 2022 22:50:29 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.17.zip
# Wed, 15 Jun 2022 22:51:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4c7110da70e07b37a00b3b05b18361572412287fee26eba04fcf23dcb75639`  
		Last Modified: Wed, 15 Jun 2022 22:52:48 GMT  
		Size: 352.2 KB (352228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a3fc52e3c402b1be6f7512b16405aaaba3edd6037ede2a7885b367bec19efd`  
		Last Modified: Wed, 15 Jun 2022 22:53:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92deca7aa7a34f968926e81414d0102042c2a2e85968fa9423cb1ceed71a9393`  
		Last Modified: Wed, 15 Jun 2022 22:53:28 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f346f796df4e8cb918a2d6f83dcf31d1544d3af9b283727e9757400a160423ab`  
		Last Modified: Wed, 15 Jun 2022 22:53:39 GMT  
		Size: 52.3 MB (52281684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:cd3d27ef331e6abf4963d0f01313133f0ff610644838be15865103605feccd95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.768; amd64

### `docker:windowsservercore-ltsc2022` - windows version 10.0.20348.768; amd64

```console
$ docker pull docker@sha256:c92dc04a8ccb9c898c42318e134d11b4fe5e825349a870ec0af4d00a8aa32f30
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2331628569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbf9b630697f8843ffb9923fb2b24ec28ca80c582e396f4bc8ae9db8517438c8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 09 Jun 2022 04:32:50 GMT
RUN Install update 10.0.20348.768
# Wed, 15 Jun 2022 12:13:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:46:14 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:49:43 GMT
ENV DOCKER_VERSION=20.10.17
# Wed, 15 Jun 2022 22:49:44 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.17.zip
# Wed, 15 Jun 2022 22:50:20 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c71967ff41928927e4c407171e4ffbac3c9ab4221eb64f5ca5a34ff4c230567`  
		Size: 841.6 MB (841600427 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dec0338feaf01f35eb916b7fd9ecc08b719354163254885d5215e513c1a3eb2e`  
		Last Modified: Wed, 15 Jun 2022 12:49:26 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a162967ebe5da992f6dc4e9ebdd4ec9f402a84f6974c0c562cff1ed6f17dd39`  
		Last Modified: Wed, 15 Jun 2022 22:52:25 GMT  
		Size: 630.9 KB (630886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6900080f685d53c251ad925dfa2391f7ea21ee77b7d5aa31e56e0d7a30666adc`  
		Last Modified: Wed, 15 Jun 2022 22:53:02 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79983762d3966bbf5de5e5397ea8b7173f7fa121d7ab01e2136817be07ae4e0f`  
		Last Modified: Wed, 15 Jun 2022 22:53:02 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7398906a7954731da34c295d4f50bdd50edb96f50ad88006b29eaa94662ccd2`  
		Last Modified: Wed, 15 Jun 2022 22:53:14 GMT  
		Size: 52.5 MB (52529382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
