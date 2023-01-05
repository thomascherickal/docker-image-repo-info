## `docker:rc-cli`

```console
$ docker pull docker@sha256:2500fbb9aa01295d95a1a7dec9f107cd497334ca11b8e85fefdda145bf09f205
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:rc-cli` - linux; amd64

```console
$ docker pull docker@sha256:5b556300f87a0996f6eb22bab17716015708b2627fdf3b489fa9d7af8e81f105
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51333022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b66283ac35adbdf67e3d23859280d3ad99abdb56b06207f2e6b26bf226613f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Tue, 29 Nov 2022 01:27:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 29 Nov 2022 01:27:02 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Thu, 29 Dec 2022 17:20:55 GMT
ENV DOCKER_VERSION=23.0.0-rc.1
# Thu, 29 Dec 2022 17:20:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-23.0.0-rc.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-23.0.0-rc.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-23.0.0-rc.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-23.0.0-rc.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Thu, 29 Dec 2022 17:20:59 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Thu, 29 Dec 2022 17:21:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Thu, 05 Jan 2023 21:21:21 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.0
# Thu, 05 Jan 2023 21:21:24 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-x86_64'; 			sha256='ba481d45be2b137a2a185abd05f61d6d7766dbedfa038f16e4705760767a206e'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-armv6'; 			sha256='0f46aea568f35decc22e1db6af76decaf1c36b9bb374610bc08c3b3618170f8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-armv7'; 			sha256='343b552c61d74446fc8e8ce7695f878cb2ad49f7fae98deb7fb76a37f24c251e'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-aarch64'; 			sha256='634e397090ca0e857a898d853ab08d7e2f226328b305026c143c68d6ce0686de'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-ppc64le'; 			sha256='236831ebb63ad30fe716bf22946c91e21b1277bff2785a8538e616168a0d93f1'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-riscv64'; 			sha256='365d9bf34ae7a2ad0dc028d13363c8c427db1300b1335834a4e06b7e4fa412af'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-s390x'; 			sha256='8072776b50f34d135f90c8118da60749435b2474afee3df96bbd9c95755f7a2f'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Thu, 05 Jan 2023 21:21:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 05 Jan 2023 21:21:24 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 05 Jan 2023 21:21:24 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 05 Jan 2023 21:21:25 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 05 Jan 2023 21:21:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 05 Jan 2023 21:21:25 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:c158987b05517b6f2c5913f3acef1f2182a32345a304fe357e3ace5fadcad715`  
		Last Modified: Tue, 22 Nov 2022 22:19:52 GMT  
		Size: 3.4 MB (3370706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93eea1d5d8e5eb7f3c01c44eb6652605d4b5ad66cf819d1e3b6053733f2f13cf`  
		Last Modified: Tue, 29 Nov 2022 01:28:59 GMT  
		Size: 2.1 MB (2064254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eac26b9fd140bd6a8e7a448eb1e2a6f2b0c34a2f85980151d5ee6845f4b1370`  
		Last Modified: Thu, 29 Dec 2022 17:22:20 GMT  
		Size: 16.2 MB (16214837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24215b171d2c93b81105b4dad5d13c041ac51f8e59f4df9fd70bc315fcda7254`  
		Last Modified: Thu, 29 Dec 2022 17:22:19 GMT  
		Size: 15.2 MB (15204070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cde0144e52d9b3d34cf584982ad193f538dded6a45f5f97ae89258f3da84de0`  
		Last Modified: Thu, 05 Jan 2023 21:23:07 GMT  
		Size: 14.5 MB (14477432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628a6a9fb1eedbb2f6a638b7d8b06999087a65a076fbc787628f5c5aea3e8bc1`  
		Last Modified: Thu, 05 Jan 2023 21:23:03 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cade76e6c506a25ef3fc5d3b1a9b4ca447080266822f98a12f76a8a9a40d82f`  
		Last Modified: Thu, 05 Jan 2023 21:23:03 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef20597d48482d9230a5c9ccf93c9efbb7adb1916aaf046ba0cd564aa38d97a5`  
		Last Modified: Thu, 05 Jan 2023 21:23:03 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:d1e90105a41f196dff708305a40e9348e0ff8a4387cb809883e5018fee300635
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47423220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e39e18c624c6f2f40d1581f9877f9c53d56d640c09dd0969bc7219e02bb2b5fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 22 Nov 2022 22:39:21 GMT
ADD file:685b5edadf1d5bf0aeb2aec35f810d83876e6d2ea0903b213f75a9c5f0dc5901 in / 
# Tue, 22 Nov 2022 22:39:21 GMT
CMD ["/bin/sh"]
# Tue, 29 Nov 2022 01:42:08 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 29 Nov 2022 01:42:08 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Thu, 29 Dec 2022 16:39:22 GMT
ENV DOCKER_VERSION=23.0.0-rc.1
# Thu, 29 Dec 2022 16:39:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-23.0.0-rc.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-23.0.0-rc.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-23.0.0-rc.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-23.0.0-rc.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Thu, 29 Dec 2022 16:39:25 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Thu, 29 Dec 2022 16:39:27 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Thu, 05 Jan 2023 21:41:05 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.0
# Thu, 05 Jan 2023 21:41:09 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-x86_64'; 			sha256='ba481d45be2b137a2a185abd05f61d6d7766dbedfa038f16e4705760767a206e'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-armv6'; 			sha256='0f46aea568f35decc22e1db6af76decaf1c36b9bb374610bc08c3b3618170f8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-armv7'; 			sha256='343b552c61d74446fc8e8ce7695f878cb2ad49f7fae98deb7fb76a37f24c251e'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-aarch64'; 			sha256='634e397090ca0e857a898d853ab08d7e2f226328b305026c143c68d6ce0686de'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-ppc64le'; 			sha256='236831ebb63ad30fe716bf22946c91e21b1277bff2785a8538e616168a0d93f1'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-riscv64'; 			sha256='365d9bf34ae7a2ad0dc028d13363c8c427db1300b1335834a4e06b7e4fa412af'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-s390x'; 			sha256='8072776b50f34d135f90c8118da60749435b2474afee3df96bbd9c95755f7a2f'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Thu, 05 Jan 2023 21:41:09 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 05 Jan 2023 21:41:09 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 05 Jan 2023 21:41:09 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 05 Jan 2023 21:41:09 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 05 Jan 2023 21:41:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 05 Jan 2023 21:41:10 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:261da4162673b93e5c0e7700a3718d40bcc086dbf24b1ec9b54bca0b82300626`  
		Last Modified: Tue, 22 Nov 2022 22:39:45 GMT  
		Size: 3.3 MB (3259190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb5dec0c1f562bd55dc773ccc0c77fbfd42b92083262478523c19bcc0f397af`  
		Last Modified: Tue, 29 Nov 2022 01:44:14 GMT  
		Size: 2.0 MB (2036851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8cadd162baf4e6baf87c3b8cabea5aa1ca9ad5925c0fbc7686eb9c9d61c48c`  
		Last Modified: Thu, 29 Dec 2022 16:40:46 GMT  
		Size: 15.3 MB (15291665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948bd5e25ebbb11921d23a9ebf978a835132271c6e170c575db9e771a16e039b`  
		Last Modified: Thu, 29 Dec 2022 16:40:44 GMT  
		Size: 13.8 MB (13764578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60350b3397e754975564da12028736623d15d1930f3ae30066408df9bcfff64f`  
		Last Modified: Thu, 05 Jan 2023 21:42:42 GMT  
		Size: 13.1 MB (13069210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70ada440488da36a5c9c42cd0d7d88bfb618f324386e21c1d670b97d58dbc25`  
		Last Modified: Thu, 05 Jan 2023 21:42:40 GMT  
		Size: 552.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84335785d0540534084cae1abc7c1532ccde4343ec55252a9c59e716716d198c`  
		Last Modified: Thu, 05 Jan 2023 21:42:44 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fe1255cf41918a61740994f2b82129df427175bdeb6740a128cb43e6871555`  
		Last Modified: Thu, 05 Jan 2023 21:42:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
