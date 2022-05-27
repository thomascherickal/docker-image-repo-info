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
-	[`docker:20.10.16`](#docker201016)
-	[`docker:20.10.16-alpine3.16`](#docker201016-alpine316)
-	[`docker:20.10.16-dind`](#docker201016-dind)
-	[`docker:20.10.16-dind-alpine3.16`](#docker201016-dind-alpine316)
-	[`docker:20.10.16-dind-rootless`](#docker201016-dind-rootless)
-	[`docker:20.10.16-git`](#docker201016-git)
-	[`docker:20.10.16-windowsservercore`](#docker201016-windowsservercore)
-	[`docker:20.10.16-windowsservercore-1809`](#docker201016-windowsservercore-1809)
-	[`docker:20.10.16-windowsservercore-ltsc2022`](#docker201016-windowsservercore-ltsc2022)
-	[`docker:dind`](#dockerdind)
-	[`docker:dind-rootless`](#dockerdind-rootless)
-	[`docker:git`](#dockergit)
-	[`docker:latest`](#dockerlatest)
-	[`docker:windowsservercore`](#dockerwindowsservercore)
-	[`docker:windowsservercore-1809`](#dockerwindowsservercore-1809)
-	[`docker:windowsservercore-ltsc2022`](#dockerwindowsservercore-ltsc2022)

## `docker:20`

```console
$ docker pull docker@sha256:101f87347f4f6e14857f00f216d838399cc879791a6c6c15e00cc374c1ff55b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20` - linux; amd64

```console
$ docker pull docker@sha256:cfcf85506ccc62251c2ebcbf4ef5fb8c0ece78329fb9426f0826e351d2b03f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.9 MB (93898239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3abfaf032fb961ae8ecbf18f6ed4bafb356a6440347e37fa62ddffe33fa7093`
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
# Fri, 27 May 2022 00:21:48 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:21:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:21:53 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:21:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:21:57 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:21:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:21:59 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:21:59 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:21:59 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:22:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:22:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:22:00 GMT
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
	-	`sha256:dcb5a3015bf80b070d4bce71ac156c87dcd4ad72ab2502fa2013d4c1e0fead92`  
		Last Modified: Fri, 27 May 2022 00:22:56 GMT  
		Size: 65.5 MB (65503686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb264a375f3f406fba9d11740f35f04686da753ae8292563677e4584f454446`  
		Last Modified: Fri, 27 May 2022 00:22:46 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876fc70e377523e5d67c000461b90ff46dd456a86fd5379ac9f9f05b6c189ae`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 9.1 MB (9117854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35692714eac874f7dfa2f3f5852a1aa74925a3d784cf192ce3d0b46d1678586b`  
		Last Modified: Fri, 27 May 2022 00:22:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a26a2b9a8d6e83a98d288dfc248e212240aaedadc7936d52ff1e0ea19d1b74`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ac0db0aa74acad5e77f1e5a2ea63bc5dd868214f278e2014bfe1c2661b31b3`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:845a928c6d12de92122717b99036c83d4f54a12f37df68dabcb9d521ca3fa948
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.2 MB (86153553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:030ce6ca0ddb3dcb6420440df8768c4ebe8da7d7bc347b4426c2fdfd120c53b8`
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
# Fri, 27 May 2022 00:42:05 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:42:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:42:11 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:42:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:42:17 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:42:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:42:22 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:42:23 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:23 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:42:24 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:42:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:42:26 GMT
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
	-	`sha256:e849ad00357eb1e6cf62ee3ac11c3ec8a62fdadc0a1b8b017e6803664b057dce`  
		Last Modified: Fri, 27 May 2022 00:44:14 GMT  
		Size: 60.0 MB (60009152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b449558387c3b597b0d43943c6910ae3acd2f931fbb1cfecc2009974571fe19`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 13.1 MB (13097915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105e790fe5537054c20571150d07a30426b417446317d2eb23f5fcd8fdd29f2e`  
		Last Modified: Fri, 27 May 2022 00:44:04 GMT  
		Size: 8.4 MB (8353560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df5eb0cdcaa2b1d1aacd73e495a3a2d5fbeab14e0184e64c5d784a17d88e2c`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f31900af33baaaaf98240d811b048972ca06fd30e5abbee1b11196f9e5a6f2f`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb4a49c216fc10a4ed3eec13da338f2d2822c9e6931107b055499f91a96cc2a`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind`

```console
$ docker pull docker@sha256:88bc41871a4f89d258042f8e7ae1d34de7fd2604eaeedc9fd955121eedfe1cf6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind` - linux; amd64

```console
$ docker pull docker@sha256:c542e54b86bf06c4103be0e74c8997b6785ade74293c3f3c4c7e4ca7252e4aad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100765792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6210acbc0c935934cc1a313e810c0e3879352e7c8656a6815b5560fc1ea4386`
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
# Fri, 27 May 2022 00:21:48 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:21:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:21:53 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:21:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:21:57 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:21:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:21:59 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:21:59 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:21:59 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:22:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:22:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:22:00 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:22:06 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 27 May 2022 00:22:06 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 27 May 2022 00:22:06 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 27 May 2022 00:22:07 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 27 May 2022 00:22:07 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 27 May 2022 00:22:08 GMT
VOLUME [/var/lib/docker]
# Fri, 27 May 2022 00:22:08 GMT
EXPOSE 2375 2376
# Fri, 27 May 2022 00:22:08 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 27 May 2022 00:22:08 GMT
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
	-	`sha256:dcb5a3015bf80b070d4bce71ac156c87dcd4ad72ab2502fa2013d4c1e0fead92`  
		Last Modified: Fri, 27 May 2022 00:22:56 GMT  
		Size: 65.5 MB (65503686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb264a375f3f406fba9d11740f35f04686da753ae8292563677e4584f454446`  
		Last Modified: Fri, 27 May 2022 00:22:46 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876fc70e377523e5d67c000461b90ff46dd456a86fd5379ac9f9f05b6c189ae`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 9.1 MB (9117854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35692714eac874f7dfa2f3f5852a1aa74925a3d784cf192ce3d0b46d1678586b`  
		Last Modified: Fri, 27 May 2022 00:22:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a26a2b9a8d6e83a98d288dfc248e212240aaedadc7936d52ff1e0ea19d1b74`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ac0db0aa74acad5e77f1e5a2ea63bc5dd868214f278e2014bfe1c2661b31b3`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb97e2fc13847c2288fee362362a68f3e1750fb67e60156361e428163b9653e3`  
		Last Modified: Fri, 27 May 2022 00:23:16 GMT  
		Size: 6.9 MB (6862530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51792a691c46c085ecbc9b75494bbd23516e59058fbeefa37627c6d3248e8a7f`  
		Last Modified: Fri, 27 May 2022 00:23:15 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58737fcae94616365add2803d1cd0ca8754d8dbff9e3eb4a0f2d168bfdfa1f9c`  
		Last Modified: Fri, 27 May 2022 00:23:15 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6630fb96e45bcadce94c9988242047ef59663c8cdbe8077274dab4b551962b5c`  
		Last Modified: Fri, 27 May 2022 00:23:14 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:c53c87edc37e5a30061f8216a8a440bb439fc62c98656135ba12fcd7627b602f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.9 MB (92893230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70dc37f3a8211eac7fe1e613595aba9f8ef90f05bd9301ed1f418306230dfff5`
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
# Fri, 27 May 2022 00:42:05 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:42:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:42:11 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:42:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:42:17 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:42:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:42:22 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:42:23 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:23 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:42:24 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:42:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:42:26 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:42:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 27 May 2022 00:42:51 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 27 May 2022 00:42:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 27 May 2022 00:42:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 27 May 2022 00:42:55 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:55 GMT
VOLUME [/var/lib/docker]
# Fri, 27 May 2022 00:42:56 GMT
EXPOSE 2375 2376
# Fri, 27 May 2022 00:42:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 27 May 2022 00:42:58 GMT
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
	-	`sha256:e849ad00357eb1e6cf62ee3ac11c3ec8a62fdadc0a1b8b017e6803664b057dce`  
		Last Modified: Fri, 27 May 2022 00:44:14 GMT  
		Size: 60.0 MB (60009152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b449558387c3b597b0d43943c6910ae3acd2f931fbb1cfecc2009974571fe19`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 13.1 MB (13097915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105e790fe5537054c20571150d07a30426b417446317d2eb23f5fcd8fdd29f2e`  
		Last Modified: Fri, 27 May 2022 00:44:04 GMT  
		Size: 8.4 MB (8353560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df5eb0cdcaa2b1d1aacd73e495a3a2d5fbeab14e0184e64c5d784a17d88e2c`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f31900af33baaaaf98240d811b048972ca06fd30e5abbee1b11196f9e5a6f2f`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb4a49c216fc10a4ed3eec13da338f2d2822c9e6931107b055499f91a96cc2a`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc8bc612f13481c682a75514272cabc48500f40e6b7b178513f45f84a7b8097`  
		Last Modified: Fri, 27 May 2022 00:44:37 GMT  
		Size: 6.7 MB (6734679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12472ed0ca80a6b3179412c9b656bd8f69f7ad7ba3a914fddaf89842151be5ea`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e0b7e5284d6585418802069bda475001882015f00ac767b1f92a7fa8ab444c`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562b2ea3a3e1433190d26fc31f21312899dee67731cc5e3822c8839cc107ef04`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:1a9b2529b54ed941240088bc13649a3eaa9e39b5ac8db043ab85448e65847043
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:ade653e2ca542612d015c8cf24d603064cf9a98be20dc1c6da79e57853f13f81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121343090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79877124f322a2362cbde15709de0a73e5eb1c451c7200b77e982aa04a6c4b88`
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
# Fri, 27 May 2022 00:21:48 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:21:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:21:53 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:21:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:21:57 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:21:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:21:59 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:21:59 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:21:59 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:22:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:22:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:22:00 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:22:06 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 27 May 2022 00:22:06 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 27 May 2022 00:22:06 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 27 May 2022 00:22:07 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 27 May 2022 00:22:07 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 27 May 2022 00:22:08 GMT
VOLUME [/var/lib/docker]
# Fri, 27 May 2022 00:22:08 GMT
EXPOSE 2375 2376
# Fri, 27 May 2022 00:22:08 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 27 May 2022 00:22:08 GMT
CMD []
# Fri, 27 May 2022 00:22:13 GMT
RUN apk add --no-cache iproute2
# Fri, 27 May 2022 00:22:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 27 May 2022 00:22:14 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 27 May 2022 00:22:16 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 27 May 2022 00:22:17 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 27 May 2022 00:22:17 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 27 May 2022 00:22:17 GMT
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
	-	`sha256:dcb5a3015bf80b070d4bce71ac156c87dcd4ad72ab2502fa2013d4c1e0fead92`  
		Last Modified: Fri, 27 May 2022 00:22:56 GMT  
		Size: 65.5 MB (65503686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb264a375f3f406fba9d11740f35f04686da753ae8292563677e4584f454446`  
		Last Modified: Fri, 27 May 2022 00:22:46 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876fc70e377523e5d67c000461b90ff46dd456a86fd5379ac9f9f05b6c189ae`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 9.1 MB (9117854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35692714eac874f7dfa2f3f5852a1aa74925a3d784cf192ce3d0b46d1678586b`  
		Last Modified: Fri, 27 May 2022 00:22:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a26a2b9a8d6e83a98d288dfc248e212240aaedadc7936d52ff1e0ea19d1b74`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ac0db0aa74acad5e77f1e5a2ea63bc5dd868214f278e2014bfe1c2661b31b3`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb97e2fc13847c2288fee362362a68f3e1750fb67e60156361e428163b9653e3`  
		Last Modified: Fri, 27 May 2022 00:23:16 GMT  
		Size: 6.9 MB (6862530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51792a691c46c085ecbc9b75494bbd23516e59058fbeefa37627c6d3248e8a7f`  
		Last Modified: Fri, 27 May 2022 00:23:15 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58737fcae94616365add2803d1cd0ca8754d8dbff9e3eb4a0f2d168bfdfa1f9c`  
		Last Modified: Fri, 27 May 2022 00:23:15 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6630fb96e45bcadce94c9988242047ef59663c8cdbe8077274dab4b551962b5c`  
		Last Modified: Fri, 27 May 2022 00:23:14 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59114d0545a377c31caa148842a2e77a84b3b707bbd234fa1515685107ee1ffa`  
		Last Modified: Fri, 27 May 2022 00:23:35 GMT  
		Size: 1.2 MB (1232605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057f5909ebccb06d1cc78ff31f0302f9cc86bb9b688d1ae29d5950dc0bc192e0`  
		Last Modified: Fri, 27 May 2022 00:23:35 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9409457daaddbdd54b345270c658c286d7a73a2e706c9d9957f28684910b45`  
		Last Modified: Fri, 27 May 2022 00:23:34 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf7506206a4dd8b1b33e2d339e3fb78793adc46bffd8de5b4139cbac62f7a1b`  
		Last Modified: Fri, 27 May 2022 00:23:38 GMT  
		Size: 19.3 MB (19342975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db6939ad7211d86906d92007629e8d040d602b841d729609e4730c1fb41e673`  
		Last Modified: Fri, 27 May 2022 00:23:35 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8806e12170ee5801cf6f5d4f004aeb5d8738492172b979c636cda98c0ab59d05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.3 MB (115317650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9be99b5fd31080774c4a52dc9205ec101fc3ea15af893ac908f06000cc5fb95a`
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
# Fri, 27 May 2022 00:42:05 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:42:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:42:11 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:42:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:42:17 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:42:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:42:22 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:42:23 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:23 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:42:24 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:42:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:42:26 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:42:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 27 May 2022 00:42:51 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 27 May 2022 00:42:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 27 May 2022 00:42:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 27 May 2022 00:42:55 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:55 GMT
VOLUME [/var/lib/docker]
# Fri, 27 May 2022 00:42:56 GMT
EXPOSE 2375 2376
# Fri, 27 May 2022 00:42:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 27 May 2022 00:42:58 GMT
CMD []
# Fri, 27 May 2022 00:43:06 GMT
RUN apk add --no-cache iproute2
# Fri, 27 May 2022 00:43:07 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 27 May 2022 00:43:08 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 27 May 2022 00:43:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 27 May 2022 00:43:12 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 27 May 2022 00:43:13 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 27 May 2022 00:43:14 GMT
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
	-	`sha256:e849ad00357eb1e6cf62ee3ac11c3ec8a62fdadc0a1b8b017e6803664b057dce`  
		Last Modified: Fri, 27 May 2022 00:44:14 GMT  
		Size: 60.0 MB (60009152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b449558387c3b597b0d43943c6910ae3acd2f931fbb1cfecc2009974571fe19`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 13.1 MB (13097915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105e790fe5537054c20571150d07a30426b417446317d2eb23f5fcd8fdd29f2e`  
		Last Modified: Fri, 27 May 2022 00:44:04 GMT  
		Size: 8.4 MB (8353560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df5eb0cdcaa2b1d1aacd73e495a3a2d5fbeab14e0184e64c5d784a17d88e2c`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f31900af33baaaaf98240d811b048972ca06fd30e5abbee1b11196f9e5a6f2f`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb4a49c216fc10a4ed3eec13da338f2d2822c9e6931107b055499f91a96cc2a`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc8bc612f13481c682a75514272cabc48500f40e6b7b178513f45f84a7b8097`  
		Last Modified: Fri, 27 May 2022 00:44:37 GMT  
		Size: 6.7 MB (6734679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12472ed0ca80a6b3179412c9b656bd8f69f7ad7ba3a914fddaf89842151be5ea`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e0b7e5284d6585418802069bda475001882015f00ac767b1f92a7fa8ab444c`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562b2ea3a3e1433190d26fc31f21312899dee67731cc5e3822c8839cc107ef04`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84ea62a2d866227887d328650cd3352453fa40035f01e71a2ef72cbda5bad85`  
		Last Modified: Fri, 27 May 2022 00:45:00 GMT  
		Size: 1.2 MB (1246087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c402e8d2ef20bcdb200bff22e2a705e4f37a156cb2fbd008c9c31c8d4e535e18`  
		Last Modified: Fri, 27 May 2022 00:44:59 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3253d6f987b941766d86e8658f90665d58705a37a4aabc77c6ff070efdff63b`  
		Last Modified: Fri, 27 May 2022 00:44:59 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e460dc3e668f8f987b686d55f79d622cd56ef67a608e98385fe4f7a0460513ee`  
		Last Modified: Fri, 27 May 2022 00:45:04 GMT  
		Size: 21.2 MB (21176712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9e7958c64f130d0afd5d797162869b2c1dde1ad7e23e635f2ed4d5de4e4ded`  
		Last Modified: Fri, 27 May 2022 00:45:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-git`

```console
$ docker pull docker@sha256:9e2600ee34888dd84232d70acfec3d54270eba720fcc399715171da9cc0ba14e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-git` - linux; amd64

```console
$ docker pull docker@sha256:cc35e039f1db7e1561d72b6e6e9ba75c55bf782aeb0494a196fb462051f20a4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100832681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9a3f525a65dc0874c079b8e4fe32921f0c568575c7c3bb5822586e0f2ab90a4`
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
# Fri, 27 May 2022 00:21:48 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:21:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:21:53 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:21:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:21:57 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:21:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:21:59 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:21:59 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:21:59 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:22:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:22:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:22:00 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:22:21 GMT
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
	-	`sha256:dcb5a3015bf80b070d4bce71ac156c87dcd4ad72ab2502fa2013d4c1e0fead92`  
		Last Modified: Fri, 27 May 2022 00:22:56 GMT  
		Size: 65.5 MB (65503686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb264a375f3f406fba9d11740f35f04686da753ae8292563677e4584f454446`  
		Last Modified: Fri, 27 May 2022 00:22:46 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876fc70e377523e5d67c000461b90ff46dd456a86fd5379ac9f9f05b6c189ae`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 9.1 MB (9117854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35692714eac874f7dfa2f3f5852a1aa74925a3d784cf192ce3d0b46d1678586b`  
		Last Modified: Fri, 27 May 2022 00:22:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a26a2b9a8d6e83a98d288dfc248e212240aaedadc7936d52ff1e0ea19d1b74`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ac0db0aa74acad5e77f1e5a2ea63bc5dd868214f278e2014bfe1c2661b31b3`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78a7dd97d955f6d65ff0c9a7ce5f5a908ecc450a7c31b0d300e04a62e93b6fe`  
		Last Modified: Fri, 27 May 2022 00:23:56 GMT  
		Size: 6.9 MB (6934442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:235e1252cb61b2324b5bf8db5cdc08920d70984b6236b5e3ba6ea960bc78f2d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93198228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0235a5284db830fc45c62a3ca16389b3d6c16ccce2f0482956fbffc854155d4`
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
# Fri, 27 May 2022 00:42:05 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:42:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:42:11 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:42:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:42:17 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:42:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:42:22 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:42:23 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:23 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:42:24 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:42:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:42:26 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:43:22 GMT
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
	-	`sha256:e849ad00357eb1e6cf62ee3ac11c3ec8a62fdadc0a1b8b017e6803664b057dce`  
		Last Modified: Fri, 27 May 2022 00:44:14 GMT  
		Size: 60.0 MB (60009152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b449558387c3b597b0d43943c6910ae3acd2f931fbb1cfecc2009974571fe19`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 13.1 MB (13097915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105e790fe5537054c20571150d07a30426b417446317d2eb23f5fcd8fdd29f2e`  
		Last Modified: Fri, 27 May 2022 00:44:04 GMT  
		Size: 8.4 MB (8353560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df5eb0cdcaa2b1d1aacd73e495a3a2d5fbeab14e0184e64c5d784a17d88e2c`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f31900af33baaaaf98240d811b048972ca06fd30e5abbee1b11196f9e5a6f2f`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb4a49c216fc10a4ed3eec13da338f2d2822c9e6931107b055499f91a96cc2a`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162afa0690e82d48da0a96e8705fb05cfb176624e95a40f0f045dce4190b389f`  
		Last Modified: Fri, 27 May 2022 00:45:25 GMT  
		Size: 7.0 MB (7044675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore`

```console
$ docker pull docker@sha256:44251ae4b6e381ac726b35292cd0cedc2c9273e3b83991b56eca7290f59ee4ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.707; amd64
	-	windows version 10.0.17763.2928; amd64

### `docker:20-windowsservercore` - windows version 10.0.20348.707; amd64

```console
$ docker pull docker@sha256:d63c51f65add3dd63c6d57455a72eda503f74a3d8b382c7b847942f75efdc12c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2290667395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba95e6fc2818e4a6b2961fbf12c81c442c94666e05812a63248a527d57d0605c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 01:15:12 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 May 2022 19:16:00 GMT
ENV DOCKER_VERSION=20.10.16
# Thu, 12 May 2022 19:16:01 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.16.zip
# Thu, 12 May 2022 19:16:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cc0e7671236328b80eb96b578eb47d9bb8c85841986a699074c0abb105d7a6`  
		Last Modified: Wed, 11 May 2022 01:18:49 GMT  
		Size: 604.5 KB (604476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9698df5d87653df3e05322abc936eba7b08b4ac1e1531d300326f852acb560d`  
		Last Modified: Thu, 12 May 2022 19:18:42 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea315f146ff5d08a865f8afe9f6b3abbc0fbe3254d7c658afd18f2c6a6916c3`  
		Last Modified: Thu, 12 May 2022 19:18:42 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c801fe2ce56a50e273ce72ad681cab5b3aff867063f17ed4a285d1d11f33e6`  
		Last Modified: Thu, 12 May 2022 19:19:40 GMT  
		Size: 52.5 MB (52523408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-windowsservercore` - windows version 10.0.17763.2928; amd64

```console
$ docker pull docker@sha256:d91fe2d69d9526fb466c37afa1a7c5c14b3449caa82ead5ae8d88f081a98b8e7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2556871108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7963abf2508f0bb0b3f5da00f2a354a0c74d867eaabd99877b24cc991a6c99be`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 01:17:07 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 May 2022 19:16:53 GMT
ENV DOCKER_VERSION=20.10.16
# Thu, 12 May 2022 19:16:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.16.zip
# Thu, 12 May 2022 19:18:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b919bb58ec3ed41b7e2e67e75497f0619d0f5ffa4ed0bf076d25d167186aed5`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 486.0 KB (486016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17963b29ee9a8eb140f806106b868925eef0ec9b9b9b7530399e44aa39644831`  
		Last Modified: Thu, 12 May 2022 19:19:54 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81794437e928236733907f6be03a38e33807049ff42b8df4f81f2585ce98a5cd`  
		Last Modified: Thu, 12 May 2022 19:19:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fec92946e098247270b24628d39d2599af778a0f46841732c2d6180065fc43`  
		Last Modified: Thu, 12 May 2022 19:20:52 GMT  
		Size: 52.3 MB (52324957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-1809`

```console
$ docker pull docker@sha256:4298f49bbd424c400dc5d6e9f78f9710dc2abdde78924e61ec48bf4d10b649f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `docker:20-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull docker@sha256:d91fe2d69d9526fb466c37afa1a7c5c14b3449caa82ead5ae8d88f081a98b8e7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2556871108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7963abf2508f0bb0b3f5da00f2a354a0c74d867eaabd99877b24cc991a6c99be`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 01:17:07 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 May 2022 19:16:53 GMT
ENV DOCKER_VERSION=20.10.16
# Thu, 12 May 2022 19:16:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.16.zip
# Thu, 12 May 2022 19:18:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b919bb58ec3ed41b7e2e67e75497f0619d0f5ffa4ed0bf076d25d167186aed5`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 486.0 KB (486016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17963b29ee9a8eb140f806106b868925eef0ec9b9b9b7530399e44aa39644831`  
		Last Modified: Thu, 12 May 2022 19:19:54 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81794437e928236733907f6be03a38e33807049ff42b8df4f81f2585ce98a5cd`  
		Last Modified: Thu, 12 May 2022 19:19:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fec92946e098247270b24628d39d2599af778a0f46841732c2d6180065fc43`  
		Last Modified: Thu, 12 May 2022 19:20:52 GMT  
		Size: 52.3 MB (52324957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:025608dd7c48461a51e36543342256af22b1bc5933f311d3774503c2eaacd05e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `docker:20-windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull docker@sha256:d63c51f65add3dd63c6d57455a72eda503f74a3d8b382c7b847942f75efdc12c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2290667395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba95e6fc2818e4a6b2961fbf12c81c442c94666e05812a63248a527d57d0605c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 01:15:12 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 May 2022 19:16:00 GMT
ENV DOCKER_VERSION=20.10.16
# Thu, 12 May 2022 19:16:01 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.16.zip
# Thu, 12 May 2022 19:16:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cc0e7671236328b80eb96b578eb47d9bb8c85841986a699074c0abb105d7a6`  
		Last Modified: Wed, 11 May 2022 01:18:49 GMT  
		Size: 604.5 KB (604476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9698df5d87653df3e05322abc936eba7b08b4ac1e1531d300326f852acb560d`  
		Last Modified: Thu, 12 May 2022 19:18:42 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea315f146ff5d08a865f8afe9f6b3abbc0fbe3254d7c658afd18f2c6a6916c3`  
		Last Modified: Thu, 12 May 2022 19:18:42 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c801fe2ce56a50e273ce72ad681cab5b3aff867063f17ed4a285d1d11f33e6`  
		Last Modified: Thu, 12 May 2022 19:19:40 GMT  
		Size: 52.5 MB (52523408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10`

```console
$ docker pull docker@sha256:101f87347f4f6e14857f00f216d838399cc879791a6c6c15e00cc374c1ff55b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10` - linux; amd64

```console
$ docker pull docker@sha256:cfcf85506ccc62251c2ebcbf4ef5fb8c0ece78329fb9426f0826e351d2b03f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.9 MB (93898239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3abfaf032fb961ae8ecbf18f6ed4bafb356a6440347e37fa62ddffe33fa7093`
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
# Fri, 27 May 2022 00:21:48 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:21:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:21:53 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:21:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:21:57 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:21:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:21:59 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:21:59 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:21:59 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:22:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:22:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:22:00 GMT
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
	-	`sha256:dcb5a3015bf80b070d4bce71ac156c87dcd4ad72ab2502fa2013d4c1e0fead92`  
		Last Modified: Fri, 27 May 2022 00:22:56 GMT  
		Size: 65.5 MB (65503686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb264a375f3f406fba9d11740f35f04686da753ae8292563677e4584f454446`  
		Last Modified: Fri, 27 May 2022 00:22:46 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876fc70e377523e5d67c000461b90ff46dd456a86fd5379ac9f9f05b6c189ae`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 9.1 MB (9117854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35692714eac874f7dfa2f3f5852a1aa74925a3d784cf192ce3d0b46d1678586b`  
		Last Modified: Fri, 27 May 2022 00:22:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a26a2b9a8d6e83a98d288dfc248e212240aaedadc7936d52ff1e0ea19d1b74`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ac0db0aa74acad5e77f1e5a2ea63bc5dd868214f278e2014bfe1c2661b31b3`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:845a928c6d12de92122717b99036c83d4f54a12f37df68dabcb9d521ca3fa948
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.2 MB (86153553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:030ce6ca0ddb3dcb6420440df8768c4ebe8da7d7bc347b4426c2fdfd120c53b8`
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
# Fri, 27 May 2022 00:42:05 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:42:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:42:11 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:42:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:42:17 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:42:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:42:22 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:42:23 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:23 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:42:24 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:42:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:42:26 GMT
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
	-	`sha256:e849ad00357eb1e6cf62ee3ac11c3ec8a62fdadc0a1b8b017e6803664b057dce`  
		Last Modified: Fri, 27 May 2022 00:44:14 GMT  
		Size: 60.0 MB (60009152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b449558387c3b597b0d43943c6910ae3acd2f931fbb1cfecc2009974571fe19`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 13.1 MB (13097915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105e790fe5537054c20571150d07a30426b417446317d2eb23f5fcd8fdd29f2e`  
		Last Modified: Fri, 27 May 2022 00:44:04 GMT  
		Size: 8.4 MB (8353560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df5eb0cdcaa2b1d1aacd73e495a3a2d5fbeab14e0184e64c5d784a17d88e2c`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f31900af33baaaaf98240d811b048972ca06fd30e5abbee1b11196f9e5a6f2f`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb4a49c216fc10a4ed3eec13da338f2d2822c9e6931107b055499f91a96cc2a`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind`

```console
$ docker pull docker@sha256:88bc41871a4f89d258042f8e7ae1d34de7fd2604eaeedc9fd955121eedfe1cf6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind` - linux; amd64

```console
$ docker pull docker@sha256:c542e54b86bf06c4103be0e74c8997b6785ade74293c3f3c4c7e4ca7252e4aad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100765792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6210acbc0c935934cc1a313e810c0e3879352e7c8656a6815b5560fc1ea4386`
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
# Fri, 27 May 2022 00:21:48 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:21:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:21:53 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:21:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:21:57 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:21:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:21:59 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:21:59 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:21:59 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:22:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:22:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:22:00 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:22:06 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 27 May 2022 00:22:06 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 27 May 2022 00:22:06 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 27 May 2022 00:22:07 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 27 May 2022 00:22:07 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 27 May 2022 00:22:08 GMT
VOLUME [/var/lib/docker]
# Fri, 27 May 2022 00:22:08 GMT
EXPOSE 2375 2376
# Fri, 27 May 2022 00:22:08 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 27 May 2022 00:22:08 GMT
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
	-	`sha256:dcb5a3015bf80b070d4bce71ac156c87dcd4ad72ab2502fa2013d4c1e0fead92`  
		Last Modified: Fri, 27 May 2022 00:22:56 GMT  
		Size: 65.5 MB (65503686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb264a375f3f406fba9d11740f35f04686da753ae8292563677e4584f454446`  
		Last Modified: Fri, 27 May 2022 00:22:46 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876fc70e377523e5d67c000461b90ff46dd456a86fd5379ac9f9f05b6c189ae`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 9.1 MB (9117854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35692714eac874f7dfa2f3f5852a1aa74925a3d784cf192ce3d0b46d1678586b`  
		Last Modified: Fri, 27 May 2022 00:22:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a26a2b9a8d6e83a98d288dfc248e212240aaedadc7936d52ff1e0ea19d1b74`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ac0db0aa74acad5e77f1e5a2ea63bc5dd868214f278e2014bfe1c2661b31b3`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb97e2fc13847c2288fee362362a68f3e1750fb67e60156361e428163b9653e3`  
		Last Modified: Fri, 27 May 2022 00:23:16 GMT  
		Size: 6.9 MB (6862530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51792a691c46c085ecbc9b75494bbd23516e59058fbeefa37627c6d3248e8a7f`  
		Last Modified: Fri, 27 May 2022 00:23:15 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58737fcae94616365add2803d1cd0ca8754d8dbff9e3eb4a0f2d168bfdfa1f9c`  
		Last Modified: Fri, 27 May 2022 00:23:15 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6630fb96e45bcadce94c9988242047ef59663c8cdbe8077274dab4b551962b5c`  
		Last Modified: Fri, 27 May 2022 00:23:14 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:c53c87edc37e5a30061f8216a8a440bb439fc62c98656135ba12fcd7627b602f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.9 MB (92893230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70dc37f3a8211eac7fe1e613595aba9f8ef90f05bd9301ed1f418306230dfff5`
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
# Fri, 27 May 2022 00:42:05 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:42:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:42:11 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:42:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:42:17 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:42:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:42:22 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:42:23 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:23 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:42:24 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:42:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:42:26 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:42:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 27 May 2022 00:42:51 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 27 May 2022 00:42:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 27 May 2022 00:42:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 27 May 2022 00:42:55 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:55 GMT
VOLUME [/var/lib/docker]
# Fri, 27 May 2022 00:42:56 GMT
EXPOSE 2375 2376
# Fri, 27 May 2022 00:42:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 27 May 2022 00:42:58 GMT
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
	-	`sha256:e849ad00357eb1e6cf62ee3ac11c3ec8a62fdadc0a1b8b017e6803664b057dce`  
		Last Modified: Fri, 27 May 2022 00:44:14 GMT  
		Size: 60.0 MB (60009152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b449558387c3b597b0d43943c6910ae3acd2f931fbb1cfecc2009974571fe19`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 13.1 MB (13097915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105e790fe5537054c20571150d07a30426b417446317d2eb23f5fcd8fdd29f2e`  
		Last Modified: Fri, 27 May 2022 00:44:04 GMT  
		Size: 8.4 MB (8353560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df5eb0cdcaa2b1d1aacd73e495a3a2d5fbeab14e0184e64c5d784a17d88e2c`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f31900af33baaaaf98240d811b048972ca06fd30e5abbee1b11196f9e5a6f2f`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb4a49c216fc10a4ed3eec13da338f2d2822c9e6931107b055499f91a96cc2a`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc8bc612f13481c682a75514272cabc48500f40e6b7b178513f45f84a7b8097`  
		Last Modified: Fri, 27 May 2022 00:44:37 GMT  
		Size: 6.7 MB (6734679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12472ed0ca80a6b3179412c9b656bd8f69f7ad7ba3a914fddaf89842151be5ea`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e0b7e5284d6585418802069bda475001882015f00ac767b1f92a7fa8ab444c`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562b2ea3a3e1433190d26fc31f21312899dee67731cc5e3822c8839cc107ef04`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind-rootless`

```console
$ docker pull docker@sha256:1a9b2529b54ed941240088bc13649a3eaa9e39b5ac8db043ab85448e65847043
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:ade653e2ca542612d015c8cf24d603064cf9a98be20dc1c6da79e57853f13f81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121343090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79877124f322a2362cbde15709de0a73e5eb1c451c7200b77e982aa04a6c4b88`
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
# Fri, 27 May 2022 00:21:48 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:21:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:21:53 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:21:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:21:57 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:21:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:21:59 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:21:59 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:21:59 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:22:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:22:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:22:00 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:22:06 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 27 May 2022 00:22:06 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 27 May 2022 00:22:06 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 27 May 2022 00:22:07 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 27 May 2022 00:22:07 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 27 May 2022 00:22:08 GMT
VOLUME [/var/lib/docker]
# Fri, 27 May 2022 00:22:08 GMT
EXPOSE 2375 2376
# Fri, 27 May 2022 00:22:08 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 27 May 2022 00:22:08 GMT
CMD []
# Fri, 27 May 2022 00:22:13 GMT
RUN apk add --no-cache iproute2
# Fri, 27 May 2022 00:22:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 27 May 2022 00:22:14 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 27 May 2022 00:22:16 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 27 May 2022 00:22:17 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 27 May 2022 00:22:17 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 27 May 2022 00:22:17 GMT
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
	-	`sha256:dcb5a3015bf80b070d4bce71ac156c87dcd4ad72ab2502fa2013d4c1e0fead92`  
		Last Modified: Fri, 27 May 2022 00:22:56 GMT  
		Size: 65.5 MB (65503686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb264a375f3f406fba9d11740f35f04686da753ae8292563677e4584f454446`  
		Last Modified: Fri, 27 May 2022 00:22:46 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876fc70e377523e5d67c000461b90ff46dd456a86fd5379ac9f9f05b6c189ae`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 9.1 MB (9117854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35692714eac874f7dfa2f3f5852a1aa74925a3d784cf192ce3d0b46d1678586b`  
		Last Modified: Fri, 27 May 2022 00:22:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a26a2b9a8d6e83a98d288dfc248e212240aaedadc7936d52ff1e0ea19d1b74`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ac0db0aa74acad5e77f1e5a2ea63bc5dd868214f278e2014bfe1c2661b31b3`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb97e2fc13847c2288fee362362a68f3e1750fb67e60156361e428163b9653e3`  
		Last Modified: Fri, 27 May 2022 00:23:16 GMT  
		Size: 6.9 MB (6862530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51792a691c46c085ecbc9b75494bbd23516e59058fbeefa37627c6d3248e8a7f`  
		Last Modified: Fri, 27 May 2022 00:23:15 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58737fcae94616365add2803d1cd0ca8754d8dbff9e3eb4a0f2d168bfdfa1f9c`  
		Last Modified: Fri, 27 May 2022 00:23:15 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6630fb96e45bcadce94c9988242047ef59663c8cdbe8077274dab4b551962b5c`  
		Last Modified: Fri, 27 May 2022 00:23:14 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59114d0545a377c31caa148842a2e77a84b3b707bbd234fa1515685107ee1ffa`  
		Last Modified: Fri, 27 May 2022 00:23:35 GMT  
		Size: 1.2 MB (1232605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057f5909ebccb06d1cc78ff31f0302f9cc86bb9b688d1ae29d5950dc0bc192e0`  
		Last Modified: Fri, 27 May 2022 00:23:35 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9409457daaddbdd54b345270c658c286d7a73a2e706c9d9957f28684910b45`  
		Last Modified: Fri, 27 May 2022 00:23:34 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf7506206a4dd8b1b33e2d339e3fb78793adc46bffd8de5b4139cbac62f7a1b`  
		Last Modified: Fri, 27 May 2022 00:23:38 GMT  
		Size: 19.3 MB (19342975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db6939ad7211d86906d92007629e8d040d602b841d729609e4730c1fb41e673`  
		Last Modified: Fri, 27 May 2022 00:23:35 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8806e12170ee5801cf6f5d4f004aeb5d8738492172b979c636cda98c0ab59d05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.3 MB (115317650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9be99b5fd31080774c4a52dc9205ec101fc3ea15af893ac908f06000cc5fb95a`
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
# Fri, 27 May 2022 00:42:05 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:42:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:42:11 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:42:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:42:17 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:42:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:42:22 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:42:23 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:23 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:42:24 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:42:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:42:26 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:42:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 27 May 2022 00:42:51 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 27 May 2022 00:42:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 27 May 2022 00:42:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 27 May 2022 00:42:55 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:55 GMT
VOLUME [/var/lib/docker]
# Fri, 27 May 2022 00:42:56 GMT
EXPOSE 2375 2376
# Fri, 27 May 2022 00:42:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 27 May 2022 00:42:58 GMT
CMD []
# Fri, 27 May 2022 00:43:06 GMT
RUN apk add --no-cache iproute2
# Fri, 27 May 2022 00:43:07 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 27 May 2022 00:43:08 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 27 May 2022 00:43:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 27 May 2022 00:43:12 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 27 May 2022 00:43:13 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 27 May 2022 00:43:14 GMT
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
	-	`sha256:e849ad00357eb1e6cf62ee3ac11c3ec8a62fdadc0a1b8b017e6803664b057dce`  
		Last Modified: Fri, 27 May 2022 00:44:14 GMT  
		Size: 60.0 MB (60009152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b449558387c3b597b0d43943c6910ae3acd2f931fbb1cfecc2009974571fe19`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 13.1 MB (13097915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105e790fe5537054c20571150d07a30426b417446317d2eb23f5fcd8fdd29f2e`  
		Last Modified: Fri, 27 May 2022 00:44:04 GMT  
		Size: 8.4 MB (8353560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df5eb0cdcaa2b1d1aacd73e495a3a2d5fbeab14e0184e64c5d784a17d88e2c`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f31900af33baaaaf98240d811b048972ca06fd30e5abbee1b11196f9e5a6f2f`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb4a49c216fc10a4ed3eec13da338f2d2822c9e6931107b055499f91a96cc2a`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc8bc612f13481c682a75514272cabc48500f40e6b7b178513f45f84a7b8097`  
		Last Modified: Fri, 27 May 2022 00:44:37 GMT  
		Size: 6.7 MB (6734679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12472ed0ca80a6b3179412c9b656bd8f69f7ad7ba3a914fddaf89842151be5ea`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e0b7e5284d6585418802069bda475001882015f00ac767b1f92a7fa8ab444c`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562b2ea3a3e1433190d26fc31f21312899dee67731cc5e3822c8839cc107ef04`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84ea62a2d866227887d328650cd3352453fa40035f01e71a2ef72cbda5bad85`  
		Last Modified: Fri, 27 May 2022 00:45:00 GMT  
		Size: 1.2 MB (1246087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c402e8d2ef20bcdb200bff22e2a705e4f37a156cb2fbd008c9c31c8d4e535e18`  
		Last Modified: Fri, 27 May 2022 00:44:59 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3253d6f987b941766d86e8658f90665d58705a37a4aabc77c6ff070efdff63b`  
		Last Modified: Fri, 27 May 2022 00:44:59 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e460dc3e668f8f987b686d55f79d622cd56ef67a608e98385fe4f7a0460513ee`  
		Last Modified: Fri, 27 May 2022 00:45:04 GMT  
		Size: 21.2 MB (21176712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9e7958c64f130d0afd5d797162869b2c1dde1ad7e23e635f2ed4d5de4e4ded`  
		Last Modified: Fri, 27 May 2022 00:45:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-git`

```console
$ docker pull docker@sha256:9e2600ee34888dd84232d70acfec3d54270eba720fcc399715171da9cc0ba14e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-git` - linux; amd64

```console
$ docker pull docker@sha256:cc35e039f1db7e1561d72b6e6e9ba75c55bf782aeb0494a196fb462051f20a4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100832681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9a3f525a65dc0874c079b8e4fe32921f0c568575c7c3bb5822586e0f2ab90a4`
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
# Fri, 27 May 2022 00:21:48 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:21:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:21:53 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:21:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:21:57 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:21:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:21:59 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:21:59 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:21:59 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:22:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:22:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:22:00 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:22:21 GMT
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
	-	`sha256:dcb5a3015bf80b070d4bce71ac156c87dcd4ad72ab2502fa2013d4c1e0fead92`  
		Last Modified: Fri, 27 May 2022 00:22:56 GMT  
		Size: 65.5 MB (65503686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb264a375f3f406fba9d11740f35f04686da753ae8292563677e4584f454446`  
		Last Modified: Fri, 27 May 2022 00:22:46 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876fc70e377523e5d67c000461b90ff46dd456a86fd5379ac9f9f05b6c189ae`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 9.1 MB (9117854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35692714eac874f7dfa2f3f5852a1aa74925a3d784cf192ce3d0b46d1678586b`  
		Last Modified: Fri, 27 May 2022 00:22:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a26a2b9a8d6e83a98d288dfc248e212240aaedadc7936d52ff1e0ea19d1b74`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ac0db0aa74acad5e77f1e5a2ea63bc5dd868214f278e2014bfe1c2661b31b3`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78a7dd97d955f6d65ff0c9a7ce5f5a908ecc450a7c31b0d300e04a62e93b6fe`  
		Last Modified: Fri, 27 May 2022 00:23:56 GMT  
		Size: 6.9 MB (6934442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:235e1252cb61b2324b5bf8db5cdc08920d70984b6236b5e3ba6ea960bc78f2d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93198228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0235a5284db830fc45c62a3ca16389b3d6c16ccce2f0482956fbffc854155d4`
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
# Fri, 27 May 2022 00:42:05 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:42:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:42:11 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:42:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:42:17 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:42:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:42:22 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:42:23 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:23 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:42:24 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:42:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:42:26 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:43:22 GMT
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
	-	`sha256:e849ad00357eb1e6cf62ee3ac11c3ec8a62fdadc0a1b8b017e6803664b057dce`  
		Last Modified: Fri, 27 May 2022 00:44:14 GMT  
		Size: 60.0 MB (60009152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b449558387c3b597b0d43943c6910ae3acd2f931fbb1cfecc2009974571fe19`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 13.1 MB (13097915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105e790fe5537054c20571150d07a30426b417446317d2eb23f5fcd8fdd29f2e`  
		Last Modified: Fri, 27 May 2022 00:44:04 GMT  
		Size: 8.4 MB (8353560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df5eb0cdcaa2b1d1aacd73e495a3a2d5fbeab14e0184e64c5d784a17d88e2c`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f31900af33baaaaf98240d811b048972ca06fd30e5abbee1b11196f9e5a6f2f`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb4a49c216fc10a4ed3eec13da338f2d2822c9e6931107b055499f91a96cc2a`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162afa0690e82d48da0a96e8705fb05cfb176624e95a40f0f045dce4190b389f`  
		Last Modified: Fri, 27 May 2022 00:45:25 GMT  
		Size: 7.0 MB (7044675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore`

```console
$ docker pull docker@sha256:44251ae4b6e381ac726b35292cd0cedc2c9273e3b83991b56eca7290f59ee4ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.707; amd64
	-	windows version 10.0.17763.2928; amd64

### `docker:20.10-windowsservercore` - windows version 10.0.20348.707; amd64

```console
$ docker pull docker@sha256:d63c51f65add3dd63c6d57455a72eda503f74a3d8b382c7b847942f75efdc12c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2290667395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba95e6fc2818e4a6b2961fbf12c81c442c94666e05812a63248a527d57d0605c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 01:15:12 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 May 2022 19:16:00 GMT
ENV DOCKER_VERSION=20.10.16
# Thu, 12 May 2022 19:16:01 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.16.zip
# Thu, 12 May 2022 19:16:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cc0e7671236328b80eb96b578eb47d9bb8c85841986a699074c0abb105d7a6`  
		Last Modified: Wed, 11 May 2022 01:18:49 GMT  
		Size: 604.5 KB (604476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9698df5d87653df3e05322abc936eba7b08b4ac1e1531d300326f852acb560d`  
		Last Modified: Thu, 12 May 2022 19:18:42 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea315f146ff5d08a865f8afe9f6b3abbc0fbe3254d7c658afd18f2c6a6916c3`  
		Last Modified: Thu, 12 May 2022 19:18:42 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c801fe2ce56a50e273ce72ad681cab5b3aff867063f17ed4a285d1d11f33e6`  
		Last Modified: Thu, 12 May 2022 19:19:40 GMT  
		Size: 52.5 MB (52523408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-windowsservercore` - windows version 10.0.17763.2928; amd64

```console
$ docker pull docker@sha256:d91fe2d69d9526fb466c37afa1a7c5c14b3449caa82ead5ae8d88f081a98b8e7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2556871108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7963abf2508f0bb0b3f5da00f2a354a0c74d867eaabd99877b24cc991a6c99be`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 01:17:07 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 May 2022 19:16:53 GMT
ENV DOCKER_VERSION=20.10.16
# Thu, 12 May 2022 19:16:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.16.zip
# Thu, 12 May 2022 19:18:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b919bb58ec3ed41b7e2e67e75497f0619d0f5ffa4ed0bf076d25d167186aed5`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 486.0 KB (486016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17963b29ee9a8eb140f806106b868925eef0ec9b9b9b7530399e44aa39644831`  
		Last Modified: Thu, 12 May 2022 19:19:54 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81794437e928236733907f6be03a38e33807049ff42b8df4f81f2585ce98a5cd`  
		Last Modified: Thu, 12 May 2022 19:19:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fec92946e098247270b24628d39d2599af778a0f46841732c2d6180065fc43`  
		Last Modified: Thu, 12 May 2022 19:20:52 GMT  
		Size: 52.3 MB (52324957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-1809`

```console
$ docker pull docker@sha256:4298f49bbd424c400dc5d6e9f78f9710dc2abdde78924e61ec48bf4d10b649f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `docker:20.10-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull docker@sha256:d91fe2d69d9526fb466c37afa1a7c5c14b3449caa82ead5ae8d88f081a98b8e7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2556871108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7963abf2508f0bb0b3f5da00f2a354a0c74d867eaabd99877b24cc991a6c99be`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 01:17:07 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 May 2022 19:16:53 GMT
ENV DOCKER_VERSION=20.10.16
# Thu, 12 May 2022 19:16:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.16.zip
# Thu, 12 May 2022 19:18:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b919bb58ec3ed41b7e2e67e75497f0619d0f5ffa4ed0bf076d25d167186aed5`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 486.0 KB (486016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17963b29ee9a8eb140f806106b868925eef0ec9b9b9b7530399e44aa39644831`  
		Last Modified: Thu, 12 May 2022 19:19:54 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81794437e928236733907f6be03a38e33807049ff42b8df4f81f2585ce98a5cd`  
		Last Modified: Thu, 12 May 2022 19:19:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fec92946e098247270b24628d39d2599af778a0f46841732c2d6180065fc43`  
		Last Modified: Thu, 12 May 2022 19:20:52 GMT  
		Size: 52.3 MB (52324957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:025608dd7c48461a51e36543342256af22b1bc5933f311d3774503c2eaacd05e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `docker:20.10-windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull docker@sha256:d63c51f65add3dd63c6d57455a72eda503f74a3d8b382c7b847942f75efdc12c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2290667395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba95e6fc2818e4a6b2961fbf12c81c442c94666e05812a63248a527d57d0605c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 01:15:12 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 May 2022 19:16:00 GMT
ENV DOCKER_VERSION=20.10.16
# Thu, 12 May 2022 19:16:01 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.16.zip
# Thu, 12 May 2022 19:16:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cc0e7671236328b80eb96b578eb47d9bb8c85841986a699074c0abb105d7a6`  
		Last Modified: Wed, 11 May 2022 01:18:49 GMT  
		Size: 604.5 KB (604476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9698df5d87653df3e05322abc936eba7b08b4ac1e1531d300326f852acb560d`  
		Last Modified: Thu, 12 May 2022 19:18:42 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea315f146ff5d08a865f8afe9f6b3abbc0fbe3254d7c658afd18f2c6a6916c3`  
		Last Modified: Thu, 12 May 2022 19:18:42 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c801fe2ce56a50e273ce72ad681cab5b3aff867063f17ed4a285d1d11f33e6`  
		Last Modified: Thu, 12 May 2022 19:19:40 GMT  
		Size: 52.5 MB (52523408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.16`

```console
$ docker pull docker@sha256:101f87347f4f6e14857f00f216d838399cc879791a6c6c15e00cc374c1ff55b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.16` - linux; amd64

```console
$ docker pull docker@sha256:cfcf85506ccc62251c2ebcbf4ef5fb8c0ece78329fb9426f0826e351d2b03f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.9 MB (93898239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3abfaf032fb961ae8ecbf18f6ed4bafb356a6440347e37fa62ddffe33fa7093`
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
# Fri, 27 May 2022 00:21:48 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:21:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:21:53 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:21:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:21:57 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:21:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:21:59 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:21:59 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:21:59 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:22:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:22:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:22:00 GMT
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
	-	`sha256:dcb5a3015bf80b070d4bce71ac156c87dcd4ad72ab2502fa2013d4c1e0fead92`  
		Last Modified: Fri, 27 May 2022 00:22:56 GMT  
		Size: 65.5 MB (65503686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb264a375f3f406fba9d11740f35f04686da753ae8292563677e4584f454446`  
		Last Modified: Fri, 27 May 2022 00:22:46 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876fc70e377523e5d67c000461b90ff46dd456a86fd5379ac9f9f05b6c189ae`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 9.1 MB (9117854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35692714eac874f7dfa2f3f5852a1aa74925a3d784cf192ce3d0b46d1678586b`  
		Last Modified: Fri, 27 May 2022 00:22:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a26a2b9a8d6e83a98d288dfc248e212240aaedadc7936d52ff1e0ea19d1b74`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ac0db0aa74acad5e77f1e5a2ea63bc5dd868214f278e2014bfe1c2661b31b3`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.16` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:845a928c6d12de92122717b99036c83d4f54a12f37df68dabcb9d521ca3fa948
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.2 MB (86153553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:030ce6ca0ddb3dcb6420440df8768c4ebe8da7d7bc347b4426c2fdfd120c53b8`
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
# Fri, 27 May 2022 00:42:05 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:42:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:42:11 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:42:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:42:17 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:42:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:42:22 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:42:23 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:23 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:42:24 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:42:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:42:26 GMT
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
	-	`sha256:e849ad00357eb1e6cf62ee3ac11c3ec8a62fdadc0a1b8b017e6803664b057dce`  
		Last Modified: Fri, 27 May 2022 00:44:14 GMT  
		Size: 60.0 MB (60009152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b449558387c3b597b0d43943c6910ae3acd2f931fbb1cfecc2009974571fe19`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 13.1 MB (13097915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105e790fe5537054c20571150d07a30426b417446317d2eb23f5fcd8fdd29f2e`  
		Last Modified: Fri, 27 May 2022 00:44:04 GMT  
		Size: 8.4 MB (8353560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df5eb0cdcaa2b1d1aacd73e495a3a2d5fbeab14e0184e64c5d784a17d88e2c`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f31900af33baaaaf98240d811b048972ca06fd30e5abbee1b11196f9e5a6f2f`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb4a49c216fc10a4ed3eec13da338f2d2822c9e6931107b055499f91a96cc2a`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.16-alpine3.16`

```console
$ docker pull docker@sha256:101f87347f4f6e14857f00f216d838399cc879791a6c6c15e00cc374c1ff55b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.16-alpine3.16` - linux; amd64

```console
$ docker pull docker@sha256:cfcf85506ccc62251c2ebcbf4ef5fb8c0ece78329fb9426f0826e351d2b03f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.9 MB (93898239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3abfaf032fb961ae8ecbf18f6ed4bafb356a6440347e37fa62ddffe33fa7093`
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
# Fri, 27 May 2022 00:21:48 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:21:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:21:53 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:21:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:21:57 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:21:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:21:59 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:21:59 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:21:59 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:22:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:22:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:22:00 GMT
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
	-	`sha256:dcb5a3015bf80b070d4bce71ac156c87dcd4ad72ab2502fa2013d4c1e0fead92`  
		Last Modified: Fri, 27 May 2022 00:22:56 GMT  
		Size: 65.5 MB (65503686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb264a375f3f406fba9d11740f35f04686da753ae8292563677e4584f454446`  
		Last Modified: Fri, 27 May 2022 00:22:46 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876fc70e377523e5d67c000461b90ff46dd456a86fd5379ac9f9f05b6c189ae`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 9.1 MB (9117854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35692714eac874f7dfa2f3f5852a1aa74925a3d784cf192ce3d0b46d1678586b`  
		Last Modified: Fri, 27 May 2022 00:22:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a26a2b9a8d6e83a98d288dfc248e212240aaedadc7936d52ff1e0ea19d1b74`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ac0db0aa74acad5e77f1e5a2ea63bc5dd868214f278e2014bfe1c2661b31b3`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.16-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:845a928c6d12de92122717b99036c83d4f54a12f37df68dabcb9d521ca3fa948
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.2 MB (86153553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:030ce6ca0ddb3dcb6420440df8768c4ebe8da7d7bc347b4426c2fdfd120c53b8`
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
# Fri, 27 May 2022 00:42:05 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:42:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:42:11 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:42:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:42:17 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:42:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:42:22 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:42:23 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:23 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:42:24 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:42:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:42:26 GMT
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
	-	`sha256:e849ad00357eb1e6cf62ee3ac11c3ec8a62fdadc0a1b8b017e6803664b057dce`  
		Last Modified: Fri, 27 May 2022 00:44:14 GMT  
		Size: 60.0 MB (60009152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b449558387c3b597b0d43943c6910ae3acd2f931fbb1cfecc2009974571fe19`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 13.1 MB (13097915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105e790fe5537054c20571150d07a30426b417446317d2eb23f5fcd8fdd29f2e`  
		Last Modified: Fri, 27 May 2022 00:44:04 GMT  
		Size: 8.4 MB (8353560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df5eb0cdcaa2b1d1aacd73e495a3a2d5fbeab14e0184e64c5d784a17d88e2c`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f31900af33baaaaf98240d811b048972ca06fd30e5abbee1b11196f9e5a6f2f`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb4a49c216fc10a4ed3eec13da338f2d2822c9e6931107b055499f91a96cc2a`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.16-dind`

```console
$ docker pull docker@sha256:88bc41871a4f89d258042f8e7ae1d34de7fd2604eaeedc9fd955121eedfe1cf6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.16-dind` - linux; amd64

```console
$ docker pull docker@sha256:c542e54b86bf06c4103be0e74c8997b6785ade74293c3f3c4c7e4ca7252e4aad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100765792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6210acbc0c935934cc1a313e810c0e3879352e7c8656a6815b5560fc1ea4386`
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
# Fri, 27 May 2022 00:21:48 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:21:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:21:53 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:21:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:21:57 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:21:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:21:59 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:21:59 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:21:59 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:22:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:22:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:22:00 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:22:06 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 27 May 2022 00:22:06 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 27 May 2022 00:22:06 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 27 May 2022 00:22:07 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 27 May 2022 00:22:07 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 27 May 2022 00:22:08 GMT
VOLUME [/var/lib/docker]
# Fri, 27 May 2022 00:22:08 GMT
EXPOSE 2375 2376
# Fri, 27 May 2022 00:22:08 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 27 May 2022 00:22:08 GMT
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
	-	`sha256:dcb5a3015bf80b070d4bce71ac156c87dcd4ad72ab2502fa2013d4c1e0fead92`  
		Last Modified: Fri, 27 May 2022 00:22:56 GMT  
		Size: 65.5 MB (65503686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb264a375f3f406fba9d11740f35f04686da753ae8292563677e4584f454446`  
		Last Modified: Fri, 27 May 2022 00:22:46 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876fc70e377523e5d67c000461b90ff46dd456a86fd5379ac9f9f05b6c189ae`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 9.1 MB (9117854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35692714eac874f7dfa2f3f5852a1aa74925a3d784cf192ce3d0b46d1678586b`  
		Last Modified: Fri, 27 May 2022 00:22:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a26a2b9a8d6e83a98d288dfc248e212240aaedadc7936d52ff1e0ea19d1b74`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ac0db0aa74acad5e77f1e5a2ea63bc5dd868214f278e2014bfe1c2661b31b3`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb97e2fc13847c2288fee362362a68f3e1750fb67e60156361e428163b9653e3`  
		Last Modified: Fri, 27 May 2022 00:23:16 GMT  
		Size: 6.9 MB (6862530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51792a691c46c085ecbc9b75494bbd23516e59058fbeefa37627c6d3248e8a7f`  
		Last Modified: Fri, 27 May 2022 00:23:15 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58737fcae94616365add2803d1cd0ca8754d8dbff9e3eb4a0f2d168bfdfa1f9c`  
		Last Modified: Fri, 27 May 2022 00:23:15 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6630fb96e45bcadce94c9988242047ef59663c8cdbe8077274dab4b551962b5c`  
		Last Modified: Fri, 27 May 2022 00:23:14 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.16-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:c53c87edc37e5a30061f8216a8a440bb439fc62c98656135ba12fcd7627b602f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.9 MB (92893230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70dc37f3a8211eac7fe1e613595aba9f8ef90f05bd9301ed1f418306230dfff5`
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
# Fri, 27 May 2022 00:42:05 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:42:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:42:11 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:42:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:42:17 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:42:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:42:22 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:42:23 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:23 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:42:24 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:42:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:42:26 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:42:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 27 May 2022 00:42:51 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 27 May 2022 00:42:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 27 May 2022 00:42:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 27 May 2022 00:42:55 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:55 GMT
VOLUME [/var/lib/docker]
# Fri, 27 May 2022 00:42:56 GMT
EXPOSE 2375 2376
# Fri, 27 May 2022 00:42:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 27 May 2022 00:42:58 GMT
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
	-	`sha256:e849ad00357eb1e6cf62ee3ac11c3ec8a62fdadc0a1b8b017e6803664b057dce`  
		Last Modified: Fri, 27 May 2022 00:44:14 GMT  
		Size: 60.0 MB (60009152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b449558387c3b597b0d43943c6910ae3acd2f931fbb1cfecc2009974571fe19`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 13.1 MB (13097915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105e790fe5537054c20571150d07a30426b417446317d2eb23f5fcd8fdd29f2e`  
		Last Modified: Fri, 27 May 2022 00:44:04 GMT  
		Size: 8.4 MB (8353560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df5eb0cdcaa2b1d1aacd73e495a3a2d5fbeab14e0184e64c5d784a17d88e2c`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f31900af33baaaaf98240d811b048972ca06fd30e5abbee1b11196f9e5a6f2f`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb4a49c216fc10a4ed3eec13da338f2d2822c9e6931107b055499f91a96cc2a`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc8bc612f13481c682a75514272cabc48500f40e6b7b178513f45f84a7b8097`  
		Last Modified: Fri, 27 May 2022 00:44:37 GMT  
		Size: 6.7 MB (6734679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12472ed0ca80a6b3179412c9b656bd8f69f7ad7ba3a914fddaf89842151be5ea`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e0b7e5284d6585418802069bda475001882015f00ac767b1f92a7fa8ab444c`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562b2ea3a3e1433190d26fc31f21312899dee67731cc5e3822c8839cc107ef04`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.16-dind-alpine3.16`

```console
$ docker pull docker@sha256:88bc41871a4f89d258042f8e7ae1d34de7fd2604eaeedc9fd955121eedfe1cf6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.16-dind-alpine3.16` - linux; amd64

```console
$ docker pull docker@sha256:c542e54b86bf06c4103be0e74c8997b6785ade74293c3f3c4c7e4ca7252e4aad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100765792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6210acbc0c935934cc1a313e810c0e3879352e7c8656a6815b5560fc1ea4386`
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
# Fri, 27 May 2022 00:21:48 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:21:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:21:53 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:21:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:21:57 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:21:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:21:59 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:21:59 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:21:59 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:22:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:22:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:22:00 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:22:06 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 27 May 2022 00:22:06 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 27 May 2022 00:22:06 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 27 May 2022 00:22:07 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 27 May 2022 00:22:07 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 27 May 2022 00:22:08 GMT
VOLUME [/var/lib/docker]
# Fri, 27 May 2022 00:22:08 GMT
EXPOSE 2375 2376
# Fri, 27 May 2022 00:22:08 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 27 May 2022 00:22:08 GMT
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
	-	`sha256:dcb5a3015bf80b070d4bce71ac156c87dcd4ad72ab2502fa2013d4c1e0fead92`  
		Last Modified: Fri, 27 May 2022 00:22:56 GMT  
		Size: 65.5 MB (65503686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb264a375f3f406fba9d11740f35f04686da753ae8292563677e4584f454446`  
		Last Modified: Fri, 27 May 2022 00:22:46 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876fc70e377523e5d67c000461b90ff46dd456a86fd5379ac9f9f05b6c189ae`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 9.1 MB (9117854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35692714eac874f7dfa2f3f5852a1aa74925a3d784cf192ce3d0b46d1678586b`  
		Last Modified: Fri, 27 May 2022 00:22:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a26a2b9a8d6e83a98d288dfc248e212240aaedadc7936d52ff1e0ea19d1b74`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ac0db0aa74acad5e77f1e5a2ea63bc5dd868214f278e2014bfe1c2661b31b3`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb97e2fc13847c2288fee362362a68f3e1750fb67e60156361e428163b9653e3`  
		Last Modified: Fri, 27 May 2022 00:23:16 GMT  
		Size: 6.9 MB (6862530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51792a691c46c085ecbc9b75494bbd23516e59058fbeefa37627c6d3248e8a7f`  
		Last Modified: Fri, 27 May 2022 00:23:15 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58737fcae94616365add2803d1cd0ca8754d8dbff9e3eb4a0f2d168bfdfa1f9c`  
		Last Modified: Fri, 27 May 2022 00:23:15 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6630fb96e45bcadce94c9988242047ef59663c8cdbe8077274dab4b551962b5c`  
		Last Modified: Fri, 27 May 2022 00:23:14 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.16-dind-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:c53c87edc37e5a30061f8216a8a440bb439fc62c98656135ba12fcd7627b602f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.9 MB (92893230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70dc37f3a8211eac7fe1e613595aba9f8ef90f05bd9301ed1f418306230dfff5`
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
# Fri, 27 May 2022 00:42:05 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:42:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:42:11 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:42:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:42:17 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:42:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:42:22 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:42:23 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:23 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:42:24 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:42:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:42:26 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:42:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 27 May 2022 00:42:51 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 27 May 2022 00:42:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 27 May 2022 00:42:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 27 May 2022 00:42:55 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:55 GMT
VOLUME [/var/lib/docker]
# Fri, 27 May 2022 00:42:56 GMT
EXPOSE 2375 2376
# Fri, 27 May 2022 00:42:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 27 May 2022 00:42:58 GMT
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
	-	`sha256:e849ad00357eb1e6cf62ee3ac11c3ec8a62fdadc0a1b8b017e6803664b057dce`  
		Last Modified: Fri, 27 May 2022 00:44:14 GMT  
		Size: 60.0 MB (60009152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b449558387c3b597b0d43943c6910ae3acd2f931fbb1cfecc2009974571fe19`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 13.1 MB (13097915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105e790fe5537054c20571150d07a30426b417446317d2eb23f5fcd8fdd29f2e`  
		Last Modified: Fri, 27 May 2022 00:44:04 GMT  
		Size: 8.4 MB (8353560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df5eb0cdcaa2b1d1aacd73e495a3a2d5fbeab14e0184e64c5d784a17d88e2c`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f31900af33baaaaf98240d811b048972ca06fd30e5abbee1b11196f9e5a6f2f`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb4a49c216fc10a4ed3eec13da338f2d2822c9e6931107b055499f91a96cc2a`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc8bc612f13481c682a75514272cabc48500f40e6b7b178513f45f84a7b8097`  
		Last Modified: Fri, 27 May 2022 00:44:37 GMT  
		Size: 6.7 MB (6734679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12472ed0ca80a6b3179412c9b656bd8f69f7ad7ba3a914fddaf89842151be5ea`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e0b7e5284d6585418802069bda475001882015f00ac767b1f92a7fa8ab444c`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562b2ea3a3e1433190d26fc31f21312899dee67731cc5e3822c8839cc107ef04`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.16-dind-rootless`

```console
$ docker pull docker@sha256:1a9b2529b54ed941240088bc13649a3eaa9e39b5ac8db043ab85448e65847043
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.16-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:ade653e2ca542612d015c8cf24d603064cf9a98be20dc1c6da79e57853f13f81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121343090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79877124f322a2362cbde15709de0a73e5eb1c451c7200b77e982aa04a6c4b88`
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
# Fri, 27 May 2022 00:21:48 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:21:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:21:53 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:21:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:21:57 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:21:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:21:59 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:21:59 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:21:59 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:22:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:22:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:22:00 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:22:06 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 27 May 2022 00:22:06 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 27 May 2022 00:22:06 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 27 May 2022 00:22:07 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 27 May 2022 00:22:07 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 27 May 2022 00:22:08 GMT
VOLUME [/var/lib/docker]
# Fri, 27 May 2022 00:22:08 GMT
EXPOSE 2375 2376
# Fri, 27 May 2022 00:22:08 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 27 May 2022 00:22:08 GMT
CMD []
# Fri, 27 May 2022 00:22:13 GMT
RUN apk add --no-cache iproute2
# Fri, 27 May 2022 00:22:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 27 May 2022 00:22:14 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 27 May 2022 00:22:16 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 27 May 2022 00:22:17 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 27 May 2022 00:22:17 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 27 May 2022 00:22:17 GMT
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
	-	`sha256:dcb5a3015bf80b070d4bce71ac156c87dcd4ad72ab2502fa2013d4c1e0fead92`  
		Last Modified: Fri, 27 May 2022 00:22:56 GMT  
		Size: 65.5 MB (65503686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb264a375f3f406fba9d11740f35f04686da753ae8292563677e4584f454446`  
		Last Modified: Fri, 27 May 2022 00:22:46 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876fc70e377523e5d67c000461b90ff46dd456a86fd5379ac9f9f05b6c189ae`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 9.1 MB (9117854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35692714eac874f7dfa2f3f5852a1aa74925a3d784cf192ce3d0b46d1678586b`  
		Last Modified: Fri, 27 May 2022 00:22:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a26a2b9a8d6e83a98d288dfc248e212240aaedadc7936d52ff1e0ea19d1b74`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ac0db0aa74acad5e77f1e5a2ea63bc5dd868214f278e2014bfe1c2661b31b3`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb97e2fc13847c2288fee362362a68f3e1750fb67e60156361e428163b9653e3`  
		Last Modified: Fri, 27 May 2022 00:23:16 GMT  
		Size: 6.9 MB (6862530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51792a691c46c085ecbc9b75494bbd23516e59058fbeefa37627c6d3248e8a7f`  
		Last Modified: Fri, 27 May 2022 00:23:15 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58737fcae94616365add2803d1cd0ca8754d8dbff9e3eb4a0f2d168bfdfa1f9c`  
		Last Modified: Fri, 27 May 2022 00:23:15 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6630fb96e45bcadce94c9988242047ef59663c8cdbe8077274dab4b551962b5c`  
		Last Modified: Fri, 27 May 2022 00:23:14 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59114d0545a377c31caa148842a2e77a84b3b707bbd234fa1515685107ee1ffa`  
		Last Modified: Fri, 27 May 2022 00:23:35 GMT  
		Size: 1.2 MB (1232605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057f5909ebccb06d1cc78ff31f0302f9cc86bb9b688d1ae29d5950dc0bc192e0`  
		Last Modified: Fri, 27 May 2022 00:23:35 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9409457daaddbdd54b345270c658c286d7a73a2e706c9d9957f28684910b45`  
		Last Modified: Fri, 27 May 2022 00:23:34 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf7506206a4dd8b1b33e2d339e3fb78793adc46bffd8de5b4139cbac62f7a1b`  
		Last Modified: Fri, 27 May 2022 00:23:38 GMT  
		Size: 19.3 MB (19342975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db6939ad7211d86906d92007629e8d040d602b841d729609e4730c1fb41e673`  
		Last Modified: Fri, 27 May 2022 00:23:35 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.16-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8806e12170ee5801cf6f5d4f004aeb5d8738492172b979c636cda98c0ab59d05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.3 MB (115317650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9be99b5fd31080774c4a52dc9205ec101fc3ea15af893ac908f06000cc5fb95a`
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
# Fri, 27 May 2022 00:42:05 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:42:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:42:11 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:42:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:42:17 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:42:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:42:22 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:42:23 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:23 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:42:24 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:42:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:42:26 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:42:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 27 May 2022 00:42:51 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 27 May 2022 00:42:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 27 May 2022 00:42:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 27 May 2022 00:42:55 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:55 GMT
VOLUME [/var/lib/docker]
# Fri, 27 May 2022 00:42:56 GMT
EXPOSE 2375 2376
# Fri, 27 May 2022 00:42:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 27 May 2022 00:42:58 GMT
CMD []
# Fri, 27 May 2022 00:43:06 GMT
RUN apk add --no-cache iproute2
# Fri, 27 May 2022 00:43:07 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 27 May 2022 00:43:08 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 27 May 2022 00:43:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 27 May 2022 00:43:12 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 27 May 2022 00:43:13 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 27 May 2022 00:43:14 GMT
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
	-	`sha256:e849ad00357eb1e6cf62ee3ac11c3ec8a62fdadc0a1b8b017e6803664b057dce`  
		Last Modified: Fri, 27 May 2022 00:44:14 GMT  
		Size: 60.0 MB (60009152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b449558387c3b597b0d43943c6910ae3acd2f931fbb1cfecc2009974571fe19`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 13.1 MB (13097915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105e790fe5537054c20571150d07a30426b417446317d2eb23f5fcd8fdd29f2e`  
		Last Modified: Fri, 27 May 2022 00:44:04 GMT  
		Size: 8.4 MB (8353560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df5eb0cdcaa2b1d1aacd73e495a3a2d5fbeab14e0184e64c5d784a17d88e2c`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f31900af33baaaaf98240d811b048972ca06fd30e5abbee1b11196f9e5a6f2f`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb4a49c216fc10a4ed3eec13da338f2d2822c9e6931107b055499f91a96cc2a`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc8bc612f13481c682a75514272cabc48500f40e6b7b178513f45f84a7b8097`  
		Last Modified: Fri, 27 May 2022 00:44:37 GMT  
		Size: 6.7 MB (6734679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12472ed0ca80a6b3179412c9b656bd8f69f7ad7ba3a914fddaf89842151be5ea`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e0b7e5284d6585418802069bda475001882015f00ac767b1f92a7fa8ab444c`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562b2ea3a3e1433190d26fc31f21312899dee67731cc5e3822c8839cc107ef04`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84ea62a2d866227887d328650cd3352453fa40035f01e71a2ef72cbda5bad85`  
		Last Modified: Fri, 27 May 2022 00:45:00 GMT  
		Size: 1.2 MB (1246087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c402e8d2ef20bcdb200bff22e2a705e4f37a156cb2fbd008c9c31c8d4e535e18`  
		Last Modified: Fri, 27 May 2022 00:44:59 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3253d6f987b941766d86e8658f90665d58705a37a4aabc77c6ff070efdff63b`  
		Last Modified: Fri, 27 May 2022 00:44:59 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e460dc3e668f8f987b686d55f79d622cd56ef67a608e98385fe4f7a0460513ee`  
		Last Modified: Fri, 27 May 2022 00:45:04 GMT  
		Size: 21.2 MB (21176712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9e7958c64f130d0afd5d797162869b2c1dde1ad7e23e635f2ed4d5de4e4ded`  
		Last Modified: Fri, 27 May 2022 00:45:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.16-git`

```console
$ docker pull docker@sha256:9e2600ee34888dd84232d70acfec3d54270eba720fcc399715171da9cc0ba14e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.16-git` - linux; amd64

```console
$ docker pull docker@sha256:cc35e039f1db7e1561d72b6e6e9ba75c55bf782aeb0494a196fb462051f20a4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100832681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9a3f525a65dc0874c079b8e4fe32921f0c568575c7c3bb5822586e0f2ab90a4`
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
# Fri, 27 May 2022 00:21:48 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:21:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:21:53 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:21:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:21:57 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:21:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:21:59 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:21:59 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:21:59 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:22:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:22:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:22:00 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:22:21 GMT
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
	-	`sha256:dcb5a3015bf80b070d4bce71ac156c87dcd4ad72ab2502fa2013d4c1e0fead92`  
		Last Modified: Fri, 27 May 2022 00:22:56 GMT  
		Size: 65.5 MB (65503686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb264a375f3f406fba9d11740f35f04686da753ae8292563677e4584f454446`  
		Last Modified: Fri, 27 May 2022 00:22:46 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876fc70e377523e5d67c000461b90ff46dd456a86fd5379ac9f9f05b6c189ae`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 9.1 MB (9117854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35692714eac874f7dfa2f3f5852a1aa74925a3d784cf192ce3d0b46d1678586b`  
		Last Modified: Fri, 27 May 2022 00:22:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a26a2b9a8d6e83a98d288dfc248e212240aaedadc7936d52ff1e0ea19d1b74`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ac0db0aa74acad5e77f1e5a2ea63bc5dd868214f278e2014bfe1c2661b31b3`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78a7dd97d955f6d65ff0c9a7ce5f5a908ecc450a7c31b0d300e04a62e93b6fe`  
		Last Modified: Fri, 27 May 2022 00:23:56 GMT  
		Size: 6.9 MB (6934442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.16-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:235e1252cb61b2324b5bf8db5cdc08920d70984b6236b5e3ba6ea960bc78f2d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93198228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0235a5284db830fc45c62a3ca16389b3d6c16ccce2f0482956fbffc854155d4`
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
# Fri, 27 May 2022 00:42:05 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:42:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:42:11 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:42:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:42:17 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:42:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:42:22 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:42:23 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:23 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:42:24 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:42:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:42:26 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:43:22 GMT
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
	-	`sha256:e849ad00357eb1e6cf62ee3ac11c3ec8a62fdadc0a1b8b017e6803664b057dce`  
		Last Modified: Fri, 27 May 2022 00:44:14 GMT  
		Size: 60.0 MB (60009152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b449558387c3b597b0d43943c6910ae3acd2f931fbb1cfecc2009974571fe19`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 13.1 MB (13097915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105e790fe5537054c20571150d07a30426b417446317d2eb23f5fcd8fdd29f2e`  
		Last Modified: Fri, 27 May 2022 00:44:04 GMT  
		Size: 8.4 MB (8353560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df5eb0cdcaa2b1d1aacd73e495a3a2d5fbeab14e0184e64c5d784a17d88e2c`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f31900af33baaaaf98240d811b048972ca06fd30e5abbee1b11196f9e5a6f2f`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb4a49c216fc10a4ed3eec13da338f2d2822c9e6931107b055499f91a96cc2a`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162afa0690e82d48da0a96e8705fb05cfb176624e95a40f0f045dce4190b389f`  
		Last Modified: Fri, 27 May 2022 00:45:25 GMT  
		Size: 7.0 MB (7044675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.16-windowsservercore`

```console
$ docker pull docker@sha256:44251ae4b6e381ac726b35292cd0cedc2c9273e3b83991b56eca7290f59ee4ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.707; amd64
	-	windows version 10.0.17763.2928; amd64

### `docker:20.10.16-windowsservercore` - windows version 10.0.20348.707; amd64

```console
$ docker pull docker@sha256:d63c51f65add3dd63c6d57455a72eda503f74a3d8b382c7b847942f75efdc12c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2290667395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba95e6fc2818e4a6b2961fbf12c81c442c94666e05812a63248a527d57d0605c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 01:15:12 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 May 2022 19:16:00 GMT
ENV DOCKER_VERSION=20.10.16
# Thu, 12 May 2022 19:16:01 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.16.zip
# Thu, 12 May 2022 19:16:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cc0e7671236328b80eb96b578eb47d9bb8c85841986a699074c0abb105d7a6`  
		Last Modified: Wed, 11 May 2022 01:18:49 GMT  
		Size: 604.5 KB (604476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9698df5d87653df3e05322abc936eba7b08b4ac1e1531d300326f852acb560d`  
		Last Modified: Thu, 12 May 2022 19:18:42 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea315f146ff5d08a865f8afe9f6b3abbc0fbe3254d7c658afd18f2c6a6916c3`  
		Last Modified: Thu, 12 May 2022 19:18:42 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c801fe2ce56a50e273ce72ad681cab5b3aff867063f17ed4a285d1d11f33e6`  
		Last Modified: Thu, 12 May 2022 19:19:40 GMT  
		Size: 52.5 MB (52523408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.16-windowsservercore` - windows version 10.0.17763.2928; amd64

```console
$ docker pull docker@sha256:d91fe2d69d9526fb466c37afa1a7c5c14b3449caa82ead5ae8d88f081a98b8e7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2556871108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7963abf2508f0bb0b3f5da00f2a354a0c74d867eaabd99877b24cc991a6c99be`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 01:17:07 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 May 2022 19:16:53 GMT
ENV DOCKER_VERSION=20.10.16
# Thu, 12 May 2022 19:16:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.16.zip
# Thu, 12 May 2022 19:18:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b919bb58ec3ed41b7e2e67e75497f0619d0f5ffa4ed0bf076d25d167186aed5`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 486.0 KB (486016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17963b29ee9a8eb140f806106b868925eef0ec9b9b9b7530399e44aa39644831`  
		Last Modified: Thu, 12 May 2022 19:19:54 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81794437e928236733907f6be03a38e33807049ff42b8df4f81f2585ce98a5cd`  
		Last Modified: Thu, 12 May 2022 19:19:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fec92946e098247270b24628d39d2599af778a0f46841732c2d6180065fc43`  
		Last Modified: Thu, 12 May 2022 19:20:52 GMT  
		Size: 52.3 MB (52324957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.16-windowsservercore-1809`

```console
$ docker pull docker@sha256:4298f49bbd424c400dc5d6e9f78f9710dc2abdde78924e61ec48bf4d10b649f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `docker:20.10.16-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull docker@sha256:d91fe2d69d9526fb466c37afa1a7c5c14b3449caa82ead5ae8d88f081a98b8e7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2556871108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7963abf2508f0bb0b3f5da00f2a354a0c74d867eaabd99877b24cc991a6c99be`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 01:17:07 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 May 2022 19:16:53 GMT
ENV DOCKER_VERSION=20.10.16
# Thu, 12 May 2022 19:16:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.16.zip
# Thu, 12 May 2022 19:18:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b919bb58ec3ed41b7e2e67e75497f0619d0f5ffa4ed0bf076d25d167186aed5`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 486.0 KB (486016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17963b29ee9a8eb140f806106b868925eef0ec9b9b9b7530399e44aa39644831`  
		Last Modified: Thu, 12 May 2022 19:19:54 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81794437e928236733907f6be03a38e33807049ff42b8df4f81f2585ce98a5cd`  
		Last Modified: Thu, 12 May 2022 19:19:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fec92946e098247270b24628d39d2599af778a0f46841732c2d6180065fc43`  
		Last Modified: Thu, 12 May 2022 19:20:52 GMT  
		Size: 52.3 MB (52324957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.16-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:025608dd7c48461a51e36543342256af22b1bc5933f311d3774503c2eaacd05e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `docker:20.10.16-windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull docker@sha256:d63c51f65add3dd63c6d57455a72eda503f74a3d8b382c7b847942f75efdc12c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2290667395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba95e6fc2818e4a6b2961fbf12c81c442c94666e05812a63248a527d57d0605c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 01:15:12 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 May 2022 19:16:00 GMT
ENV DOCKER_VERSION=20.10.16
# Thu, 12 May 2022 19:16:01 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.16.zip
# Thu, 12 May 2022 19:16:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cc0e7671236328b80eb96b578eb47d9bb8c85841986a699074c0abb105d7a6`  
		Last Modified: Wed, 11 May 2022 01:18:49 GMT  
		Size: 604.5 KB (604476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9698df5d87653df3e05322abc936eba7b08b4ac1e1531d300326f852acb560d`  
		Last Modified: Thu, 12 May 2022 19:18:42 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea315f146ff5d08a865f8afe9f6b3abbc0fbe3254d7c658afd18f2c6a6916c3`  
		Last Modified: Thu, 12 May 2022 19:18:42 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c801fe2ce56a50e273ce72ad681cab5b3aff867063f17ed4a285d1d11f33e6`  
		Last Modified: Thu, 12 May 2022 19:19:40 GMT  
		Size: 52.5 MB (52523408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:88bc41871a4f89d258042f8e7ae1d34de7fd2604eaeedc9fd955121eedfe1cf6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:c542e54b86bf06c4103be0e74c8997b6785ade74293c3f3c4c7e4ca7252e4aad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100765792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6210acbc0c935934cc1a313e810c0e3879352e7c8656a6815b5560fc1ea4386`
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
# Fri, 27 May 2022 00:21:48 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:21:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:21:53 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:21:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:21:57 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:21:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:21:59 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:21:59 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:21:59 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:22:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:22:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:22:00 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:22:06 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 27 May 2022 00:22:06 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 27 May 2022 00:22:06 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 27 May 2022 00:22:07 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 27 May 2022 00:22:07 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 27 May 2022 00:22:08 GMT
VOLUME [/var/lib/docker]
# Fri, 27 May 2022 00:22:08 GMT
EXPOSE 2375 2376
# Fri, 27 May 2022 00:22:08 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 27 May 2022 00:22:08 GMT
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
	-	`sha256:dcb5a3015bf80b070d4bce71ac156c87dcd4ad72ab2502fa2013d4c1e0fead92`  
		Last Modified: Fri, 27 May 2022 00:22:56 GMT  
		Size: 65.5 MB (65503686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb264a375f3f406fba9d11740f35f04686da753ae8292563677e4584f454446`  
		Last Modified: Fri, 27 May 2022 00:22:46 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876fc70e377523e5d67c000461b90ff46dd456a86fd5379ac9f9f05b6c189ae`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 9.1 MB (9117854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35692714eac874f7dfa2f3f5852a1aa74925a3d784cf192ce3d0b46d1678586b`  
		Last Modified: Fri, 27 May 2022 00:22:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a26a2b9a8d6e83a98d288dfc248e212240aaedadc7936d52ff1e0ea19d1b74`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ac0db0aa74acad5e77f1e5a2ea63bc5dd868214f278e2014bfe1c2661b31b3`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb97e2fc13847c2288fee362362a68f3e1750fb67e60156361e428163b9653e3`  
		Last Modified: Fri, 27 May 2022 00:23:16 GMT  
		Size: 6.9 MB (6862530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51792a691c46c085ecbc9b75494bbd23516e59058fbeefa37627c6d3248e8a7f`  
		Last Modified: Fri, 27 May 2022 00:23:15 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58737fcae94616365add2803d1cd0ca8754d8dbff9e3eb4a0f2d168bfdfa1f9c`  
		Last Modified: Fri, 27 May 2022 00:23:15 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6630fb96e45bcadce94c9988242047ef59663c8cdbe8077274dab4b551962b5c`  
		Last Modified: Fri, 27 May 2022 00:23:14 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:c53c87edc37e5a30061f8216a8a440bb439fc62c98656135ba12fcd7627b602f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.9 MB (92893230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70dc37f3a8211eac7fe1e613595aba9f8ef90f05bd9301ed1f418306230dfff5`
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
# Fri, 27 May 2022 00:42:05 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:42:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:42:11 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:42:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:42:17 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:42:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:42:22 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:42:23 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:23 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:42:24 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:42:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:42:26 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:42:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 27 May 2022 00:42:51 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 27 May 2022 00:42:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 27 May 2022 00:42:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 27 May 2022 00:42:55 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:55 GMT
VOLUME [/var/lib/docker]
# Fri, 27 May 2022 00:42:56 GMT
EXPOSE 2375 2376
# Fri, 27 May 2022 00:42:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 27 May 2022 00:42:58 GMT
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
	-	`sha256:e849ad00357eb1e6cf62ee3ac11c3ec8a62fdadc0a1b8b017e6803664b057dce`  
		Last Modified: Fri, 27 May 2022 00:44:14 GMT  
		Size: 60.0 MB (60009152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b449558387c3b597b0d43943c6910ae3acd2f931fbb1cfecc2009974571fe19`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 13.1 MB (13097915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105e790fe5537054c20571150d07a30426b417446317d2eb23f5fcd8fdd29f2e`  
		Last Modified: Fri, 27 May 2022 00:44:04 GMT  
		Size: 8.4 MB (8353560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df5eb0cdcaa2b1d1aacd73e495a3a2d5fbeab14e0184e64c5d784a17d88e2c`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f31900af33baaaaf98240d811b048972ca06fd30e5abbee1b11196f9e5a6f2f`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb4a49c216fc10a4ed3eec13da338f2d2822c9e6931107b055499f91a96cc2a`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc8bc612f13481c682a75514272cabc48500f40e6b7b178513f45f84a7b8097`  
		Last Modified: Fri, 27 May 2022 00:44:37 GMT  
		Size: 6.7 MB (6734679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12472ed0ca80a6b3179412c9b656bd8f69f7ad7ba3a914fddaf89842151be5ea`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e0b7e5284d6585418802069bda475001882015f00ac767b1f92a7fa8ab444c`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562b2ea3a3e1433190d26fc31f21312899dee67731cc5e3822c8839cc107ef04`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:1a9b2529b54ed941240088bc13649a3eaa9e39b5ac8db043ab85448e65847043
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:ade653e2ca542612d015c8cf24d603064cf9a98be20dc1c6da79e57853f13f81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121343090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79877124f322a2362cbde15709de0a73e5eb1c451c7200b77e982aa04a6c4b88`
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
# Fri, 27 May 2022 00:21:48 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:21:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:21:53 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:21:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:21:57 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:21:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:21:59 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:21:59 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:21:59 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:22:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:22:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:22:00 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:22:06 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 27 May 2022 00:22:06 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 27 May 2022 00:22:06 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 27 May 2022 00:22:07 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 27 May 2022 00:22:07 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 27 May 2022 00:22:08 GMT
VOLUME [/var/lib/docker]
# Fri, 27 May 2022 00:22:08 GMT
EXPOSE 2375 2376
# Fri, 27 May 2022 00:22:08 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 27 May 2022 00:22:08 GMT
CMD []
# Fri, 27 May 2022 00:22:13 GMT
RUN apk add --no-cache iproute2
# Fri, 27 May 2022 00:22:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 27 May 2022 00:22:14 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 27 May 2022 00:22:16 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 27 May 2022 00:22:17 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 27 May 2022 00:22:17 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 27 May 2022 00:22:17 GMT
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
	-	`sha256:dcb5a3015bf80b070d4bce71ac156c87dcd4ad72ab2502fa2013d4c1e0fead92`  
		Last Modified: Fri, 27 May 2022 00:22:56 GMT  
		Size: 65.5 MB (65503686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb264a375f3f406fba9d11740f35f04686da753ae8292563677e4584f454446`  
		Last Modified: Fri, 27 May 2022 00:22:46 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876fc70e377523e5d67c000461b90ff46dd456a86fd5379ac9f9f05b6c189ae`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 9.1 MB (9117854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35692714eac874f7dfa2f3f5852a1aa74925a3d784cf192ce3d0b46d1678586b`  
		Last Modified: Fri, 27 May 2022 00:22:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a26a2b9a8d6e83a98d288dfc248e212240aaedadc7936d52ff1e0ea19d1b74`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ac0db0aa74acad5e77f1e5a2ea63bc5dd868214f278e2014bfe1c2661b31b3`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb97e2fc13847c2288fee362362a68f3e1750fb67e60156361e428163b9653e3`  
		Last Modified: Fri, 27 May 2022 00:23:16 GMT  
		Size: 6.9 MB (6862530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51792a691c46c085ecbc9b75494bbd23516e59058fbeefa37627c6d3248e8a7f`  
		Last Modified: Fri, 27 May 2022 00:23:15 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58737fcae94616365add2803d1cd0ca8754d8dbff9e3eb4a0f2d168bfdfa1f9c`  
		Last Modified: Fri, 27 May 2022 00:23:15 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6630fb96e45bcadce94c9988242047ef59663c8cdbe8077274dab4b551962b5c`  
		Last Modified: Fri, 27 May 2022 00:23:14 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59114d0545a377c31caa148842a2e77a84b3b707bbd234fa1515685107ee1ffa`  
		Last Modified: Fri, 27 May 2022 00:23:35 GMT  
		Size: 1.2 MB (1232605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057f5909ebccb06d1cc78ff31f0302f9cc86bb9b688d1ae29d5950dc0bc192e0`  
		Last Modified: Fri, 27 May 2022 00:23:35 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9409457daaddbdd54b345270c658c286d7a73a2e706c9d9957f28684910b45`  
		Last Modified: Fri, 27 May 2022 00:23:34 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf7506206a4dd8b1b33e2d339e3fb78793adc46bffd8de5b4139cbac62f7a1b`  
		Last Modified: Fri, 27 May 2022 00:23:38 GMT  
		Size: 19.3 MB (19342975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db6939ad7211d86906d92007629e8d040d602b841d729609e4730c1fb41e673`  
		Last Modified: Fri, 27 May 2022 00:23:35 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8806e12170ee5801cf6f5d4f004aeb5d8738492172b979c636cda98c0ab59d05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.3 MB (115317650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9be99b5fd31080774c4a52dc9205ec101fc3ea15af893ac908f06000cc5fb95a`
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
# Fri, 27 May 2022 00:42:05 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:42:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:42:11 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:42:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:42:17 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:42:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:42:22 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:42:23 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:23 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:42:24 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:42:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:42:26 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:42:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 27 May 2022 00:42:51 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 27 May 2022 00:42:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 27 May 2022 00:42:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 27 May 2022 00:42:55 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:55 GMT
VOLUME [/var/lib/docker]
# Fri, 27 May 2022 00:42:56 GMT
EXPOSE 2375 2376
# Fri, 27 May 2022 00:42:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 27 May 2022 00:42:58 GMT
CMD []
# Fri, 27 May 2022 00:43:06 GMT
RUN apk add --no-cache iproute2
# Fri, 27 May 2022 00:43:07 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 27 May 2022 00:43:08 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 27 May 2022 00:43:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 27 May 2022 00:43:12 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 27 May 2022 00:43:13 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 27 May 2022 00:43:14 GMT
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
	-	`sha256:e849ad00357eb1e6cf62ee3ac11c3ec8a62fdadc0a1b8b017e6803664b057dce`  
		Last Modified: Fri, 27 May 2022 00:44:14 GMT  
		Size: 60.0 MB (60009152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b449558387c3b597b0d43943c6910ae3acd2f931fbb1cfecc2009974571fe19`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 13.1 MB (13097915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105e790fe5537054c20571150d07a30426b417446317d2eb23f5fcd8fdd29f2e`  
		Last Modified: Fri, 27 May 2022 00:44:04 GMT  
		Size: 8.4 MB (8353560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df5eb0cdcaa2b1d1aacd73e495a3a2d5fbeab14e0184e64c5d784a17d88e2c`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f31900af33baaaaf98240d811b048972ca06fd30e5abbee1b11196f9e5a6f2f`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb4a49c216fc10a4ed3eec13da338f2d2822c9e6931107b055499f91a96cc2a`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc8bc612f13481c682a75514272cabc48500f40e6b7b178513f45f84a7b8097`  
		Last Modified: Fri, 27 May 2022 00:44:37 GMT  
		Size: 6.7 MB (6734679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12472ed0ca80a6b3179412c9b656bd8f69f7ad7ba3a914fddaf89842151be5ea`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e0b7e5284d6585418802069bda475001882015f00ac767b1f92a7fa8ab444c`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562b2ea3a3e1433190d26fc31f21312899dee67731cc5e3822c8839cc107ef04`  
		Last Modified: Fri, 27 May 2022 00:44:36 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84ea62a2d866227887d328650cd3352453fa40035f01e71a2ef72cbda5bad85`  
		Last Modified: Fri, 27 May 2022 00:45:00 GMT  
		Size: 1.2 MB (1246087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c402e8d2ef20bcdb200bff22e2a705e4f37a156cb2fbd008c9c31c8d4e535e18`  
		Last Modified: Fri, 27 May 2022 00:44:59 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3253d6f987b941766d86e8658f90665d58705a37a4aabc77c6ff070efdff63b`  
		Last Modified: Fri, 27 May 2022 00:44:59 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e460dc3e668f8f987b686d55f79d622cd56ef67a608e98385fe4f7a0460513ee`  
		Last Modified: Fri, 27 May 2022 00:45:04 GMT  
		Size: 21.2 MB (21176712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9e7958c64f130d0afd5d797162869b2c1dde1ad7e23e635f2ed4d5de4e4ded`  
		Last Modified: Fri, 27 May 2022 00:45:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:9e2600ee34888dd84232d70acfec3d54270eba720fcc399715171da9cc0ba14e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:cc35e039f1db7e1561d72b6e6e9ba75c55bf782aeb0494a196fb462051f20a4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100832681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9a3f525a65dc0874c079b8e4fe32921f0c568575c7c3bb5822586e0f2ab90a4`
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
# Fri, 27 May 2022 00:21:48 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:21:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:21:53 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:21:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:21:57 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:21:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:21:59 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:21:59 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:21:59 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:22:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:22:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:22:00 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:22:21 GMT
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
	-	`sha256:dcb5a3015bf80b070d4bce71ac156c87dcd4ad72ab2502fa2013d4c1e0fead92`  
		Last Modified: Fri, 27 May 2022 00:22:56 GMT  
		Size: 65.5 MB (65503686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb264a375f3f406fba9d11740f35f04686da753ae8292563677e4584f454446`  
		Last Modified: Fri, 27 May 2022 00:22:46 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876fc70e377523e5d67c000461b90ff46dd456a86fd5379ac9f9f05b6c189ae`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 9.1 MB (9117854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35692714eac874f7dfa2f3f5852a1aa74925a3d784cf192ce3d0b46d1678586b`  
		Last Modified: Fri, 27 May 2022 00:22:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a26a2b9a8d6e83a98d288dfc248e212240aaedadc7936d52ff1e0ea19d1b74`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ac0db0aa74acad5e77f1e5a2ea63bc5dd868214f278e2014bfe1c2661b31b3`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78a7dd97d955f6d65ff0c9a7ce5f5a908ecc450a7c31b0d300e04a62e93b6fe`  
		Last Modified: Fri, 27 May 2022 00:23:56 GMT  
		Size: 6.9 MB (6934442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:235e1252cb61b2324b5bf8db5cdc08920d70984b6236b5e3ba6ea960bc78f2d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93198228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0235a5284db830fc45c62a3ca16389b3d6c16ccce2f0482956fbffc854155d4`
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
# Fri, 27 May 2022 00:42:05 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:42:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:42:11 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:42:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:42:17 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:42:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:42:22 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:42:23 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:23 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:42:24 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:42:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:42:26 GMT
CMD ["sh"]
# Fri, 27 May 2022 00:43:22 GMT
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
	-	`sha256:e849ad00357eb1e6cf62ee3ac11c3ec8a62fdadc0a1b8b017e6803664b057dce`  
		Last Modified: Fri, 27 May 2022 00:44:14 GMT  
		Size: 60.0 MB (60009152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b449558387c3b597b0d43943c6910ae3acd2f931fbb1cfecc2009974571fe19`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 13.1 MB (13097915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105e790fe5537054c20571150d07a30426b417446317d2eb23f5fcd8fdd29f2e`  
		Last Modified: Fri, 27 May 2022 00:44:04 GMT  
		Size: 8.4 MB (8353560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df5eb0cdcaa2b1d1aacd73e495a3a2d5fbeab14e0184e64c5d784a17d88e2c`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f31900af33baaaaf98240d811b048972ca06fd30e5abbee1b11196f9e5a6f2f`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb4a49c216fc10a4ed3eec13da338f2d2822c9e6931107b055499f91a96cc2a`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162afa0690e82d48da0a96e8705fb05cfb176624e95a40f0f045dce4190b389f`  
		Last Modified: Fri, 27 May 2022 00:45:25 GMT  
		Size: 7.0 MB (7044675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:101f87347f4f6e14857f00f216d838399cc879791a6c6c15e00cc374c1ff55b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:cfcf85506ccc62251c2ebcbf4ef5fb8c0ece78329fb9426f0826e351d2b03f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.9 MB (93898239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3abfaf032fb961ae8ecbf18f6ed4bafb356a6440347e37fa62ddffe33fa7093`
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
# Fri, 27 May 2022 00:21:48 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:21:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:21:53 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:21:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:21:57 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:21:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:21:59 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:21:59 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:21:59 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:22:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:22:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:22:00 GMT
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
	-	`sha256:dcb5a3015bf80b070d4bce71ac156c87dcd4ad72ab2502fa2013d4c1e0fead92`  
		Last Modified: Fri, 27 May 2022 00:22:56 GMT  
		Size: 65.5 MB (65503686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb264a375f3f406fba9d11740f35f04686da753ae8292563677e4584f454446`  
		Last Modified: Fri, 27 May 2022 00:22:46 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876fc70e377523e5d67c000461b90ff46dd456a86fd5379ac9f9f05b6c189ae`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 9.1 MB (9117854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35692714eac874f7dfa2f3f5852a1aa74925a3d784cf192ce3d0b46d1678586b`  
		Last Modified: Fri, 27 May 2022 00:22:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a26a2b9a8d6e83a98d288dfc248e212240aaedadc7936d52ff1e0ea19d1b74`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ac0db0aa74acad5e77f1e5a2ea63bc5dd868214f278e2014bfe1c2661b31b3`  
		Last Modified: Fri, 27 May 2022 00:22:43 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:845a928c6d12de92122717b99036c83d4f54a12f37df68dabcb9d521ca3fa948
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.2 MB (86153553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:030ce6ca0ddb3dcb6420440df8768c4ebe8da7d7bc347b4426c2fdfd120c53b8`
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
# Fri, 27 May 2022 00:42:05 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:42:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:42:11 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:42:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Fri, 27 May 2022 00:42:17 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.1
# Fri, 27 May 2022 00:42:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-x86_64'; 			sha256='d99de1ea7616f2a4c7914d37674f0650660a5e832be555805a71c0fc377233c9'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv6'; 			sha256='86f2eafdb2ff1f3885758854dd5e1c5ea9d81aa292623829fd3babe9d3fc6f9a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-armv7'; 			sha256='f5a15fa6ef16f3c79cf8c2e965d7426d1f3968c273eb588c76d1f2851b1bf90f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-aarch64'; 			sha256='002662ed18a22d9d65d3d2c0358008c7c6a3db7dacb8983488130b3954d00e63'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-ppc64le'; 			sha256='83612098d39d3485945ee0d49f1ede02e0de96fbb7658202770aec6ae0834853'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.1/docker-compose-linux-s390x'; 			sha256='68b9487106fd27e0f8c7defcf80fee2ab4f178f3ccc1d827fa0d2e82f80fa38b'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 27 May 2022 00:42:22 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 27 May 2022 00:42:23 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 27 May 2022 00:42:23 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 27 May 2022 00:42:24 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 27 May 2022 00:42:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:42:26 GMT
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
	-	`sha256:e849ad00357eb1e6cf62ee3ac11c3ec8a62fdadc0a1b8b017e6803664b057dce`  
		Last Modified: Fri, 27 May 2022 00:44:14 GMT  
		Size: 60.0 MB (60009152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b449558387c3b597b0d43943c6910ae3acd2f931fbb1cfecc2009974571fe19`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 13.1 MB (13097915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105e790fe5537054c20571150d07a30426b417446317d2eb23f5fcd8fdd29f2e`  
		Last Modified: Fri, 27 May 2022 00:44:04 GMT  
		Size: 8.4 MB (8353560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df5eb0cdcaa2b1d1aacd73e495a3a2d5fbeab14e0184e64c5d784a17d88e2c`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f31900af33baaaaf98240d811b048972ca06fd30e5abbee1b11196f9e5a6f2f`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb4a49c216fc10a4ed3eec13da338f2d2822c9e6931107b055499f91a96cc2a`  
		Last Modified: Fri, 27 May 2022 00:44:03 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore`

```console
$ docker pull docker@sha256:44251ae4b6e381ac726b35292cd0cedc2c9273e3b83991b56eca7290f59ee4ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.707; amd64
	-	windows version 10.0.17763.2928; amd64

### `docker:windowsservercore` - windows version 10.0.20348.707; amd64

```console
$ docker pull docker@sha256:d63c51f65add3dd63c6d57455a72eda503f74a3d8b382c7b847942f75efdc12c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2290667395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba95e6fc2818e4a6b2961fbf12c81c442c94666e05812a63248a527d57d0605c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 01:15:12 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 May 2022 19:16:00 GMT
ENV DOCKER_VERSION=20.10.16
# Thu, 12 May 2022 19:16:01 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.16.zip
# Thu, 12 May 2022 19:16:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cc0e7671236328b80eb96b578eb47d9bb8c85841986a699074c0abb105d7a6`  
		Last Modified: Wed, 11 May 2022 01:18:49 GMT  
		Size: 604.5 KB (604476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9698df5d87653df3e05322abc936eba7b08b4ac1e1531d300326f852acb560d`  
		Last Modified: Thu, 12 May 2022 19:18:42 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea315f146ff5d08a865f8afe9f6b3abbc0fbe3254d7c658afd18f2c6a6916c3`  
		Last Modified: Thu, 12 May 2022 19:18:42 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c801fe2ce56a50e273ce72ad681cab5b3aff867063f17ed4a285d1d11f33e6`  
		Last Modified: Thu, 12 May 2022 19:19:40 GMT  
		Size: 52.5 MB (52523408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:windowsservercore` - windows version 10.0.17763.2928; amd64

```console
$ docker pull docker@sha256:d91fe2d69d9526fb466c37afa1a7c5c14b3449caa82ead5ae8d88f081a98b8e7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2556871108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7963abf2508f0bb0b3f5da00f2a354a0c74d867eaabd99877b24cc991a6c99be`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 01:17:07 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 May 2022 19:16:53 GMT
ENV DOCKER_VERSION=20.10.16
# Thu, 12 May 2022 19:16:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.16.zip
# Thu, 12 May 2022 19:18:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b919bb58ec3ed41b7e2e67e75497f0619d0f5ffa4ed0bf076d25d167186aed5`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 486.0 KB (486016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17963b29ee9a8eb140f806106b868925eef0ec9b9b9b7530399e44aa39644831`  
		Last Modified: Thu, 12 May 2022 19:19:54 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81794437e928236733907f6be03a38e33807049ff42b8df4f81f2585ce98a5cd`  
		Last Modified: Thu, 12 May 2022 19:19:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fec92946e098247270b24628d39d2599af778a0f46841732c2d6180065fc43`  
		Last Modified: Thu, 12 May 2022 19:20:52 GMT  
		Size: 52.3 MB (52324957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:4298f49bbd424c400dc5d6e9f78f9710dc2abdde78924e61ec48bf4d10b649f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull docker@sha256:d91fe2d69d9526fb466c37afa1a7c5c14b3449caa82ead5ae8d88f081a98b8e7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2556871108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7963abf2508f0bb0b3f5da00f2a354a0c74d867eaabd99877b24cc991a6c99be`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 01:17:07 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 May 2022 19:16:53 GMT
ENV DOCKER_VERSION=20.10.16
# Thu, 12 May 2022 19:16:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.16.zip
# Thu, 12 May 2022 19:18:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b919bb58ec3ed41b7e2e67e75497f0619d0f5ffa4ed0bf076d25d167186aed5`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 486.0 KB (486016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17963b29ee9a8eb140f806106b868925eef0ec9b9b9b7530399e44aa39644831`  
		Last Modified: Thu, 12 May 2022 19:19:54 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81794437e928236733907f6be03a38e33807049ff42b8df4f81f2585ce98a5cd`  
		Last Modified: Thu, 12 May 2022 19:19:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fec92946e098247270b24628d39d2599af778a0f46841732c2d6180065fc43`  
		Last Modified: Thu, 12 May 2022 19:20:52 GMT  
		Size: 52.3 MB (52324957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:025608dd7c48461a51e36543342256af22b1bc5933f311d3774503c2eaacd05e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `docker:windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull docker@sha256:d63c51f65add3dd63c6d57455a72eda503f74a3d8b382c7b847942f75efdc12c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2290667395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba95e6fc2818e4a6b2961fbf12c81c442c94666e05812a63248a527d57d0605c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 01:15:12 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 May 2022 19:16:00 GMT
ENV DOCKER_VERSION=20.10.16
# Thu, 12 May 2022 19:16:01 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.16.zip
# Thu, 12 May 2022 19:16:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cc0e7671236328b80eb96b578eb47d9bb8c85841986a699074c0abb105d7a6`  
		Last Modified: Wed, 11 May 2022 01:18:49 GMT  
		Size: 604.5 KB (604476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9698df5d87653df3e05322abc936eba7b08b4ac1e1531d300326f852acb560d`  
		Last Modified: Thu, 12 May 2022 19:18:42 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea315f146ff5d08a865f8afe9f6b3abbc0fbe3254d7c658afd18f2c6a6916c3`  
		Last Modified: Thu, 12 May 2022 19:18:42 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c801fe2ce56a50e273ce72ad681cab5b3aff867063f17ed4a285d1d11f33e6`  
		Last Modified: Thu, 12 May 2022 19:19:40 GMT  
		Size: 52.5 MB (52523408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
