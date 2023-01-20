## `docker:rc-cli`

```console
$ docker pull docker@sha256:6426d1318cfc1e1ee9267c0f0cf49f2a51c0cf96697214a2a4a5d6d31ab53fa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:rc-cli` - linux; amd64

```console
$ docker pull docker@sha256:fc9b0c995ae416dca172378847dfad626557517f993585e91d89fd900db0304a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52126707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca1d8f5cf2e925ccf820e506e847b076ac104b86f9803dc657f96d0487bb4a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Fri, 20 Jan 2023 01:19:25 GMT
ENV DOCKER_VERSION=23.0.0-rc.2
# Fri, 20 Jan 2023 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-23.0.0-rc.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-23.0.0-rc.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-23.0.0-rc.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-23.0.0-rc.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 20 Jan 2023 01:19:31 GMT
ENV DOCKER_BUILDX_VERSION=0.10.0
# Fri, 20 Jan 2023 01:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-amd64'; 			sha256='f76047e43cd2526a870b9cf385effc7c9642c1a17d144559c43545525415867d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-arm-v6'; 			sha256='dc037b64e14388cbf5441d3b23a3f1ccd9a56a47007555ce681d89b70d411d31'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-arm-v7'; 			sha256='19b82ba259d83cc75b12bddb1cdc0712dd276f8763d0a65ded2048193973260b'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-arm64'; 			sha256='abf375431775d46139312591aa9471cdf6909d8a4e8392b73940ca136c34eb4d'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-ppc64le'; 			sha256='9850f6ad445d1014a156c33ac7f9074fffd3358db304ef5b4e4509355a4d9fb9'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-riscv64'; 			sha256='07529564e5b2f1f6e33fbf947700f9118a727dde2d8486c3e2115bc4fb42d86a'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-s390x'; 			sha256='871b4a746765334a1a0b56700525d5ef7f83adcafbb193734e238c8ac102eccc'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 20 Jan 2023 01:19:34 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Fri, 20 Jan 2023 01:19:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 20 Jan 2023 01:19:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 20 Jan 2023 01:19:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 20 Jan 2023 01:19:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 20 Jan 2023 01:19:37 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 20 Jan 2023 01:19:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Jan 2023 01:19:37 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5645e17e8e772f0f5e8fb51320c291e57e60777930f33fb5ec288a7aafafebf`  
		Last Modified: Fri, 20 Jan 2023 01:21:23 GMT  
		Size: 16.2 MB (16210492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786cbea4ef3a6d7445da857bb0179da13092d722ad3bc1d1cfc9fba5643c3c84`  
		Last Modified: Fri, 20 Jan 2023 01:21:22 GMT  
		Size: 16.0 MB (15988681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f87cdbce7976e9b98233450652b68ef8593367ab2aeebc6f8dc3647c9b4a3f3`  
		Last Modified: Fri, 20 Jan 2023 01:21:22 GMT  
		Size: 14.5 MB (14490924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec84e687e49dbe093639faf81ca33b8662f366d37e9b103602202fe7abcf3f2c`  
		Last Modified: Fri, 20 Jan 2023 01:21:19 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b270ffbe8b5bc2423e115882f87b26ef4c75aba7e80668927aead08227029e`  
		Last Modified: Fri, 20 Jan 2023 01:21:19 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803439012a9eb382b563b9f840079fe0b9d292fd874edab986b7cbde6671dfb8`  
		Last Modified: Fri, 20 Jan 2023 01:21:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f64792fa39e19a2c165413f773d4b04132bf081bc7ce6c402cc77aa628bd19b5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48095522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2bce7f84e52c13d124e604c439faf99b0d153d8ccac8da82a2049c56ff7dbe0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Fri, 20 Jan 2023 00:39:23 GMT
ENV DOCKER_VERSION=23.0.0-rc.2
# Fri, 20 Jan 2023 00:39:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-23.0.0-rc.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-23.0.0-rc.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-23.0.0-rc.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-23.0.0-rc.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 20 Jan 2023 00:39:27 GMT
ENV DOCKER_BUILDX_VERSION=0.10.0
# Fri, 20 Jan 2023 00:39:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-amd64'; 			sha256='f76047e43cd2526a870b9cf385effc7c9642c1a17d144559c43545525415867d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-arm-v6'; 			sha256='dc037b64e14388cbf5441d3b23a3f1ccd9a56a47007555ce681d89b70d411d31'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-arm-v7'; 			sha256='19b82ba259d83cc75b12bddb1cdc0712dd276f8763d0a65ded2048193973260b'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-arm64'; 			sha256='abf375431775d46139312591aa9471cdf6909d8a4e8392b73940ca136c34eb4d'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-ppc64le'; 			sha256='9850f6ad445d1014a156c33ac7f9074fffd3358db304ef5b4e4509355a4d9fb9'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-riscv64'; 			sha256='07529564e5b2f1f6e33fbf947700f9118a727dde2d8486c3e2115bc4fb42d86a'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-s390x'; 			sha256='871b4a746765334a1a0b56700525d5ef7f83adcafbb193734e238c8ac102eccc'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 20 Jan 2023 00:39:34 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Fri, 20 Jan 2023 00:39:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 20 Jan 2023 00:39:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 20 Jan 2023 00:39:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 20 Jan 2023 00:39:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 20 Jan 2023 00:39:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 20 Jan 2023 00:39:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Jan 2023 00:39:38 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04448b5ab866ce58e9045d830cb22adf7a6c9df14a32becf446504b2d08771b`  
		Last Modified: Fri, 20 Jan 2023 00:41:21 GMT  
		Size: 15.3 MB (15286237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58febb98d86a1f75bb161b40593029154b51a95f04498668a9302916e4cb8b0b`  
		Last Modified: Fri, 20 Jan 2023 00:41:20 GMT  
		Size: 14.4 MB (14430978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849c5d6785d0ecaa4727a5add37695e51832be46b4c225d70414e286c4cb9493`  
		Last Modified: Fri, 20 Jan 2023 00:41:20 GMT  
		Size: 13.1 MB (13080438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc652dd57da3d14699c3eecc24dc127767b41edd435e6bc6747d1234839d8c5a`  
		Last Modified: Fri, 20 Jan 2023 00:41:19 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a858be319c6c1582f5b54f5e0921db2c4b5161065531f18e273131445c24fb66`  
		Last Modified: Fri, 20 Jan 2023 00:41:18 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d880c535d51decbb91e1f37749562e75643b62c3a60e6161c725b64def51fd8`  
		Last Modified: Fri, 20 Jan 2023 00:41:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
